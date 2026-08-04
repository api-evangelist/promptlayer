# PromptLayer (promptlayer)

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

PromptLayer is a prompt engineering, prompt management, and LLM observability platform. Its REST API logs and tracks LLM requests, manages a versioned prompt registry with release labels, ingests OpenTelemetry-style spans and traces, and runs evaluations and datasets so teams can monitor, debug, and improve their LLM applications.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/promptlayer/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Prompt Engineering
- Prompt Management
- Observability
- Evaluation

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### PromptLayer Request Logging & Tracking API

Logs and tracks LLM requests independent of provider via log-request, associates prompt templates and input variables with a request (track-prompt), and attaches scores (track-score) and custom metadata (track-metadata) to logged requests for monitoring, debugging, and replay.

- **Human URL:** [https://docs.promptlayer.com/reference/rest-api-reference](https://docs.promptlayer.com/reference/rest-api-reference)
- **Base URL:** `https://api.promptlayer.com`

#### Tags

- Logging
- Tracking
- Requests
- Observability

#### Properties

- [Documentation](https://docs.promptlayer.com/why-promptlayer/how-it-works)
- [API Reference](https://docs.promptlayer.com/reference/log-request)
- [OpenAPI](openapi/promptlayer-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/promptlayer.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/promptlayer.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PromptLayer Prompt Registry & Templates API

Retrieves rendered or raw prompt templates by name or id with version and release-label resolution, publishes new prompt template versions, and manages release labels so prompts can be versioned and deployed without code changes.

- **Human URL:** [https://docs.promptlayer.com/features/prompt-registry](https://docs.promptlayer.com/features/prompt-registry)
- **Base URL:** `https://api.promptlayer.com`

#### Tags

- Prompt Registry
- Templates
- Versioning
- Release Labels

#### Properties

- [Documentation](https://docs.promptlayer.com/features/prompt-registry)
- [API Reference](https://docs.promptlayer.com/reference/get-prompt-template)
- [OpenAPI](openapi/promptlayer-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/promptlayer.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/promptlayer.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PromptLayer Evaluations & Datasets API

Creates, lists, runs, and scores evaluation reports against datasets, and manages evaluation datasets and their rows built from uploaded files or request history, enabling systematic, batch testing of prompt and model changes.

- **Human URL:** [https://docs.promptlayer.com/features/evaluations/overview](https://docs.promptlayer.com/features/evaluations/overview)
- **Base URL:** `https://api.promptlayer.com`

#### Tags

- Evaluations
- Datasets
- Reports
- Scoring

#### Properties

- [Documentation](https://docs.promptlayer.com/features/evaluations/overview)
- [API Reference](https://docs.promptlayer.com/reference/list-evaluations)
- [OpenAPI](openapi/promptlayer-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/promptlayer.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/promptlayer.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PromptLayer Spans & Traces API

Ingests OpenTelemetry-style spans in bulk and via an OTLP traces endpoint, retrieves and closes traces, and scopes all activity to PromptLayer workspaces for end-to-end observability of multi-step LLM and agent workflows.

- **Human URL:** [https://docs.promptlayer.com/features/tracing](https://docs.promptlayer.com/features/tracing)
- **Base URL:** `https://api.promptlayer.com`

#### Tags

- Tracing
- Spans
- OpenTelemetry
- Workspaces

#### Properties

- [Documentation](https://docs.promptlayer.com/features/tracing)
- [API Reference](https://docs.promptlayer.com/reference/spans-bulk)
- [OpenAPI](openapi/promptlayer-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/promptlayer.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/promptlayer.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/MagnivOrg)
- [LinkedIn](https://www.linkedin.com/company/promptlayer)
- [Website](https://www.promptlayer.com)
- [Documentation](https://docs.promptlayer.com)
- [Plans](plans/promptlayer-plans-pricing.yml)
- [Rate Limits](rate-limits/promptlayer-rate-limits.yml)
- [Fin Ops](finops/promptlayer-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
