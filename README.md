# Langtrace AI (langtrace)

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
