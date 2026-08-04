# Wondercraft (wondercraft)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Wondercraft is an AI audio creation platform for producing podcasts, audio ads, meditations, and audiobooks. Its public REST API generates audio content from an AI-written or user-supplied script, supports a two-host Convo Mode, lets callers attach platform voices and background music by ID, and exposes asynchronous jobs that are polled for status and a finished MP3 download URL.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/wondercraft/refs/heads/main/apis.yml)

## Tags

- AI
- Audio
- Podcast
- Text to Speech
- Generative Audio

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Wondercraft Audio Generation API

Creates podcasts, audio ads, meditations, and audiobooks from a natural-language prompt using an AI-generated script. Optionally accepts platform voice IDs and a background music spec, and returns an asynchronous job_id.

- **Human URL:** [https://docs.wondercraft.ai/api-reference/introduction](https://docs.wondercraft.ai/api-reference/introduction)
- **Base URL:** `https://api.wondercraft.ai/v1`

#### Tags

- Audio
- Podcast
- Text to Speech
- Jobs

#### Properties

- [Documentation](https://docs.wondercraft.ai/quickstart)
- [API Reference](https://docs.wondercraft.ai/api-reference/endpoint/generate_podcast)
- [OpenAPI](openapi/wondercraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wondercraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wondercraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wondercraft Scripted Audio API

Generates audio from a user-provided script of ordered segments, each pairing text with a Wondercraft voice ID, with an optional background music track spec referencing a platform music ID.

- **Human URL:** [https://docs.wondercraft.ai/api-reference/endpoint/user_scripted](https://docs.wondercraft.ai/api-reference/endpoint/user_scripted)
- **Base URL:** `https://api.wondercraft.ai/v1`

#### Tags

- Audio
- Script
- Voices
- Music

#### Properties

- [Documentation](https://docs.wondercraft.ai/quickstart)
- [API Reference](https://docs.wondercraft.ai/api-reference/endpoint/user_scripted)
- [OpenAPI](openapi/wondercraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wondercraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wondercraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wondercraft Convo Mode API

Generates two-host conversational podcasts from either an AI prompt or a user-provided script, taking exactly two voice IDs plus optional delivery instructions and a background music spec.

- **Human URL:** [https://docs.wondercraft.ai/api-reference/endpoint/convo_mode_ai_scripted](https://docs.wondercraft.ai/api-reference/endpoint/convo_mode_ai_scripted)
- **Base URL:** `https://api.wondercraft.ai/v1`

#### Tags

- Audio
- Podcast
- Two Host
- Conversation

#### Properties

- [API Reference](https://docs.wondercraft.ai/api-reference/endpoint/convo_mode_ai_scripted)
- [API Reference](https://docs.wondercraft.ai/api-reference/endpoint/convo_mode_user_scripted)
- [OpenAPI](openapi/wondercraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wondercraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wondercraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Wondercraft Job Status API

Polls an audio generation job by job_id, returning whether it is finished, the generated script, the MP3 download URL, and any error details. Also lists a user's podcasts and verifies an API key.

- **Human URL:** [https://docs.wondercraft.ai/api-reference/endpoint/get_job_status](https://docs.wondercraft.ai/api-reference/endpoint/get_job_status)
- **Base URL:** `https://api.wondercraft.ai/v1`

#### Tags

- Jobs
- Async
- Status

#### Properties

- [API Reference](https://docs.wondercraft.ai/api-reference/endpoint/get_job_status)
- [OpenAPI](openapi/wondercraft-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/wondercraft.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/wondercraft.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/wondercraftai)
- [Website](https://www.wondercraft.ai)
- [Documentation](https://docs.wondercraft.ai)
- [Plans](plans/wondercraft-plans-pricing.yml)
- [Rate Limits](rate-limits/wondercraft-rate-limits.yml)
- [Fin Ops](finops/wondercraft-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
