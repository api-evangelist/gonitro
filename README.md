# GoNitro

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Nitro Software (GoNitro) is a document productivity company providing PDF editing, electronic signatures, redaction, and intelligent document automation for enterprises, small businesses, and professionals. Nitro exposes two public REST APIs on api.gonitro.dev: the Nitro PDF Services API (convert, transform, extract, and generate PDFs — conversions, compression, merge/split, OCR, redaction, PII detection, table and form extraction, and archival PDF/A) and the Nitro Sign API (enterprise eSignature envelope, document, participant, and field workflows with sealed documents and audit trails). Both use machine-to-machine OAuth 2.0 client-credentials, short-lived JWT bearer tokens, RFC 9457 problem+json errors, and asynchronous job processing. Nitro is ISO 27001, SOC 2, and HIPAA compliant and an accredited eIDAS Qualified Trust Service Provider.

**Areas:** Company · Documents · PDF · E-Signature · Document Automation · Document Conversion · Data Extraction · Redaction · OCR · Productivity · Compliance

## GoNitro on APIs.io

Everything profiled for GoNitro is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/gonitro/](https://apis.io/providers/gonitro/)** — or go straight to one of the APIs or properties below.

### APIs (3)

- [GoNitro Authentication API](https://apis.io/apis/gonitro/gonitro-authentication-api/) — The Authentication API from GoNitro — 1 operation(s) for authentication.
- [GoNitro Platform API](https://apis.io/apis/gonitro/gonitro-platform-api/) — The Platform API from GoNitro — 6 operation(s) for platform.
- [GoNitro Sign API](https://apis.io/apis/gonitro/gonitro-sign-api/) — The Sign API from GoNitro — 22 operation(s) for sign.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (1)

Multi-step workflows that chain operations into a business task.

- [Create and send a Nitro Sign envelope](https://apis.io/arazzos/gonitro/gonitro-create-and-send-envelope/)

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Nitro Sign & PDF Services Webhooks](https://apis.io/asyncapis/gonitro/gonitro-sign-asyncapi/)

#### Event channels (2)

Individual events and webhooks the provider emits.

- [{callbackUrl}](https://apis.io/channels/gonitro/callbackurl/)
- [{webhookUrl}](https://apis.io/channels/gonitro/webhookurl/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Nitro PDF Services MCP](https://apis.io/servers/gonitro/nitro-pdf-services-mcp/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Gonitro Agentic Access](https://apis.io/agentic-access/gonitro/gonitro-agentic-access/)

#### Collections (16)

Postman and Open Collection request collections.

- [Nitro PDF Services Public Authentication API](https://apis.io/collections/gonitro/open-gonitro-authentication-api/)
- [Nitro PDF Services Public Authentication Conversions API](https://apis.io/collections/gonitro/open-gonitro-conversions-api/)
- [Nitro PDF Services Public Authentication Extractions API](https://apis.io/collections/gonitro/open-gonitro-extractions-api/)
- [Nitro PDF Services Public Authentication Generations API](https://apis.io/collections/gonitro/open-gonitro-generations-api/)
- [Nitro PDF Services Public Authentication Jobs API](https://apis.io/collections/gonitro/open-gonitro-jobs-api/)
- [Nitro PDF Services Public Authentication Platform API](https://apis.io/collections/gonitro/open-gonitro-platform-api/)
- [Nitro PDF Services Public Authentication Sign API](https://apis.io/collections/gonitro/open-gonitro-sign-api/)
- [Nitro PDF Services Public Authentication Transformations API](https://apis.io/collections/gonitro/open-gonitro-transformations-api/)
- [Nitro PDF Services Public Authentication API](https://apis.io/collections/gonitro/postman-gonitro-authentication-api/)
- [Nitro PDF Services Public Authentication Conversions API](https://apis.io/collections/gonitro/postman-gonitro-conversions-api/)
- [Nitro PDF Services Public Authentication Extractions API](https://apis.io/collections/gonitro/postman-gonitro-extractions-api/)
- [Nitro PDF Services Public Authentication Generations API](https://apis.io/collections/gonitro/postman-gonitro-generations-api/)
- [Nitro PDF Services Public Authentication Jobs API](https://apis.io/collections/gonitro/postman-gonitro-jobs-api/)
- [Nitro PDF Services Public Authentication Platform API](https://apis.io/collections/gonitro/postman-gonitro-platform-api/)
- [Nitro PDF Services Public Authentication Sign API](https://apis.io/collections/gonitro/postman-gonitro-sign-api/)
- [Nitro PDF Services Public Authentication Transformations API](https://apis.io/collections/gonitro/postman-gonitro-transformations-api/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Gonitro Pdf Services Overlay](https://apis.io/overlays/gonitro/gonitro-pdf-services-overlay/)
- [Gonitro Sign Overlay](https://apis.io/overlays/gonitro/gonitro-sign-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Gonitro Authentication](https://apis.io/security/gonitro/gonitro-authentication/)
- [Gonitro Domain Security](https://apis.io/security/gonitro/gonitro-domain-security/)
- [Gonitro Trust Center](https://apis.io/security/gonitro/gonitro-trust-center/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.gonitro.com)
- [Documentation](https://developers.gonitro.com/docs)
- [Getting started](https://developers.gonitro.com/docs/getting-started/basic-setup)
- [API reference](https://developers.gonitro.com/docs/api-reference/changelog)
- [Pricing](https://www.gonitro.com/pricing)
- [Sign up](https://developers.gonitro.com/docs/authentication/credentials)
- [Support](https://www.gonitro.com/support)
- [Blog](https://www.gonitro.com/blog)
- [Compliance](https://www.gonitro.com/trust-center/compliance)
- [Terms of service](https://www.gonitro.com/legal/terms-of-service)
- [Privacy policy](https://www.gonitro.com/legal/privacy-policy)
- [GitHub](https://github.com/Nitro)
- [Status](https://status.gonitro.com)

## API Evangelist rating

**Kin Score 56.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 58.4 |
| Contract governance | 18.2 |
| Operational transparency | 50.0 |
| Developer ergonomics | 63.7 |
| Access clarity | 60.5 |

**Agent readiness 29.7** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | derived (partial credit) |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 29.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/gonitro/](https://apis.io/providers/gonitro/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for GoNitro: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/gonitro/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
