# Wondercraft (wondercraft)

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
