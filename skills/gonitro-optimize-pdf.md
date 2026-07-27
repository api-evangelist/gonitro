---
name: Optimize or transform a PDF with Nitro PDF Services
description: Authenticate, submit a PDF transformation (e.g. optimize/compress/OCR), and retrieve the result synchronously or by polling the async job.
api: openapi/gonitro-pdf-services-openapi.json
operations: [getTokenRfc6749, transformDocument, getJobStatus, getJobResult]
generated: '2026-07-19'
method: generated
---

# Optimize or transform a PDF with Nitro PDF Services

Use the Nitro PDF Services API (`https://api.gonitro.dev`) to process a PDF.
The four processing endpoints are polymorphic — the tool is selected by the
request body.

## Steps

1. **Get an access token** — `POST /oauth/token` (`getTokenRfc6749`) with your
   `clientID`/`clientSecret`; use the `access_token` as a bearer token.
2. **Submit the transformation** — `POST /transformations` (`transformDocument`)
   as multipart with the `file` part and a `params` part selecting the tool
   (e.g. optimize, compress, ocr, redact, watermark, protect, split, merge,
   rotate, flatten, delete, unprotect, set-properties). Set the `Accept` header
   to `application/json` for a file link, or `application/octet-stream` for the
   binary result.
3. **If the response is a job** — poll `GET /jobs/{jobID}/status`
   (`getJobStatus`) until complete, then `GET /jobs/{jobID}` (`getJobResult`) to
   retrieve the output. Alternatively supply a `delivery` callback to receive a
   `{jobID, location}` POST on completion.
4. **Download** the result from the returned pre-signed URL. Output files are
   deleted ~15 minutes after completion, so download promptly.

## Rules

- Limits: max 100 MB per request, max 500 pages per document.
- Extractions always return JSON; conversions/transformations return JSON or
  binary per the `Accept` header.
- Errors follow the documented status catalog (`errors/gonitro-error-codes.yml`);
  `413` = file too large, `415` = unsupported media type, `429` = rate limited
  (respect `retry-after`).
