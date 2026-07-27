---
name: Create and send a Nitro Sign envelope
description: Build a signature envelope, add a document, add a signer, place a signature field, and send it for signing using the Nitro Sign API.
api: openapi/gonitro-sign-openapi.json
operations: [getTokenRfc6749, createEnvelope, createDocument, createParticipant, createField, sendForSigning, getEnvelope]
generated: '2026-07-19'
method: generated
---

# Create and send a Nitro Sign envelope

Use the Nitro Sign API (`https://api.gonitro.dev`) to collect a legally binding
eSignature. All requests use an OAuth 2.0 client-credentials JWT bearer token.

## Steps

1. **Get an access token** — `POST /oauth/token` (`getTokenRfc6749`) with
   `{ "clientID": "...", "clientSecret": "..." }`. Use the returned
   `access_token` as `Authorization: Bearer <token>` on every call.
2. **Create the envelope** — `POST /sign/envelopes` (`createEnvelope`) with a
   name and notification settings. Capture the returned `envelopeID`.
3. **Add a document** — `POST /sign/envelopes/{envelopeID}/documents`
   (`createDocument`). Capture the returned `documentID`.
4. **Add a participant** — `POST /sign/envelopes/{envelopeID}/participants`
   (`createParticipant`) with the signer's name and email and role `SIGNER`.
   Capture the `participantID`.
5. **Place a signature field** — `POST /sign/envelopes/{envelopeID}/documents/{documentID}/fields`
   (`createField`) with a signature field bound to the participant and a
   bounding box (page index + x/y/width/height in PDF points).
6. **Send for signing** — `POST /sign/envelopes/{envelopeID}:send-for-signing`
   (`sendForSigning`). The envelope moves to `SENT`.
7. **Track status** — `GET /sign/envelopes/{envelopeID}` (`getEnvelope`), or
   subscribe to Sign webhooks (`EnvelopeSentForSignature`, `SignatureRequestSigned`,
   `EnvelopeSigningCompleted`, `EnvelopeSealed`).

## Rules

- Only envelopes in `SENT` status expose signer signing URLs and can be
  cancelled; draft envelopes cannot be cancelled.
- Errors are RFC 9457 `application/problem+json`; a `409` means the envelope is
  in an invalid state for the operation. See `errors/gonitro-problem-types.yml`.
- No idempotency-key header exists — create the envelope once and reuse its ID
  (see `conventions/gonitro-conventions.yml`).
