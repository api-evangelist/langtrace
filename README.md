# Langtrace AI (langtrace)

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

Langtrace is an open-source, OpenTelemetry-based end-to-end observability platform for LLM applications, built by Scale3 Labs. It captures real-time traces, metrics, and evaluations for popular LLMs, agent frameworks, and vector databases. Traces are ingested via an OTLP/HTTP endpoint and a REST API exposes projects, prompt registry, and trace retrieval. Available as a free self-hosted deployment or as Langtrace Cloud.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/langtrace/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Observability
- OpenTelemetry
- Tracing
- Open Source

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Langtrace Trace Ingestion (OTEL)

OpenTelemetry-compatible trace ingestion endpoint (POST /api/trace). Accepts JSON-encoded OTLP/HTTP spans authenticated with a project-level x-api-key header, for both Langtrace Cloud and self-hosted deployments.

- **Human URL:** [https://docs.langtrace.ai/api-reference/traces/POST-trace](https://docs.langtrace.ai/api-reference/traces/POST-trace)
- **Base URL:** `https://app.langtrace.ai/api`

#### Tags

- OpenTelemetry
- Tracing
- Ingestion
- OTLP

#### Properties

- [Documentation](https://docs.langtrace.ai/supported-integrations/otel-support/otel-configuration)
- [API Reference](https://docs.langtrace.ai/api-reference/traces/POST-trace)
- [OpenAPI](openapi/langtrace-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langtrace.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langtrace.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/Scale3-Labs/langtrace)

### Langtrace Projects and API Keys

REST endpoints to create projects (POST /api/project) under a team and to mint project-level API keys (POST /api/api-key), authenticated with an x-api-key header.

- **Human URL:** [https://docs.langtrace.ai/api-reference/project/POST-project](https://docs.langtrace.ai/api-reference/project/POST-project)
- **Base URL:** `https://app.langtrace.ai/api`

#### Tags

- Projects
- API Keys
- Management

#### Properties

- [Documentation](https://docs.langtrace.ai/api-reference/project/POST-project)
- [API Reference](https://docs.langtrace.ai/api-reference/project/POST-project-api-key)
- [OpenAPI](openapi/langtrace-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langtrace.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langtrace.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/Scale3-Labs/langtrace)

### Langtrace Prompt Registry

Fetch versioned prompts from the prompt registry (GET /api/promptset) with optional version selection and dynamic variable substitution, returning the live prompt when no version is specified.

- **Human URL:** [https://docs.langtrace.ai/api-reference/prompt-registry/GET-prompt-registry](https://docs.langtrace.ai/api-reference/prompt-registry/GET-prompt-registry)
- **Base URL:** `https://app.langtrace.ai/api`

#### Tags

- Prompt Registry
- Versioning
- Prompts

#### Properties

- [Documentation](https://docs.langtrace.ai/api-reference/prompt-registry/GET-prompt-registry)
- [API Reference](https://docs.langtrace.ai/api-reference/prompt-registry/GET-prompt-registry)
- [OpenAPI](openapi/langtrace-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langtrace.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langtrace.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/Scale3-Labs/langtrace)

### Langtrace Trace Retrieval and Metrics

Paginated retrieval of stored traces for a project (POST /api/traces), returning span results plus pagination metadata. Underlying spans carry the token, cost, latency, and evaluation metrics surfaced in the Langtrace dashboards.

- **Human URL:** [https://docs.langtrace.ai/api-reference/traces/POST-traces](https://docs.langtrace.ai/api-reference/traces/POST-traces)
- **Base URL:** `https://app.langtrace.ai/api`

#### Tags

- Traces
- Metrics
- Retrieval
- Evaluations

#### Properties

- [Documentation](https://docs.langtrace.ai/api-reference/traces/POST-traces)
- [API Reference](https://docs.langtrace.ai/api-reference/traces/POST-traces)
- [OpenAPI](openapi/langtrace-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/langtrace.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/langtrace.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [GitHub](https://github.com/Scale3-Labs/langtrace)

## Common Properties

- [GitHub Organization](https://github.com/Scale3-Labs)
- [LinkedIn](https://www.linkedin.com/company/langtrace)
- [Website](https://www.langtrace.ai)
- [Documentation](https://docs.langtrace.ai)
- [Plans](plans/langtrace-plans-pricing.yml)
- [Rate Limits](rate-limits/langtrace-rate-limits.yml)
- [Fin Ops](finops/langtrace-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
