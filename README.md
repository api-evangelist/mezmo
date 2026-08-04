# Mezmo (mezmo)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/apis.yml)

## Scope

- **Access:** 3rd-Party

## Tags

- Observability
- Logs
- Telemetry
- Telemetry Pipeline
- Log Management
- AI
- SRE
- OpenTelemetry
- DevOps

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Mezmo Log Ingestion API

Ingest log lines into Mezmo at logs.mezmo.com/logs/ingest. Accepts batched JSON payloads with timestamp, app, env, hostname, and structured metadata. Token or service-key authentication. The primary inbound surface for Mezmo's log analysis platform (formerly LogDNA).

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/log-ingestion-api](https://docs.mezmo.com/log-analysis-api/reference/log-ingestion-api)

#### Tags

- Logs
- Ingestion
- Observability
- Telemetry

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/log-ingestion-api)
- [OpenAPI](openapi/mezmo-log-ingestion-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-log-ingestion-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-log-ingestion-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Log Export API

Query and export logs from Mezmo via /v1/export and /v2/export. V2 supports pagination for unbounded exports, plan-aware retention windows, and filters by hosts, apps, tags, levels, and query strings.

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/export](https://docs.mezmo.com/log-analysis-api/reference/export)

#### Tags

- Logs
- Export
- Observability
- Search

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/export)
- [OpenAPI](openapi/mezmo-log-export-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-log-export-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-log-export-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Views API

Manage Mezmo log Views via /v1/config/view. Views are saved query definitions over hosts, apps, levels, tags, and free-text filters and are the unit alerts attach to.

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/views](https://docs.mezmo.com/log-analysis-api/reference/views)

#### Tags

- Logs
- Views
- Saved Searches
- Observability

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/views)
- [OpenAPI](openapi/mezmo-views-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-views-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-views-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Alerts API

Manage preset alerts via /v1/config/presetalert. Preset alerts encapsulate presence/absence triggers, frequency, and notification channels (PagerDuty, Slack, webhook, email) that views can attach to.

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/alerts](https://docs.mezmo.com/log-analysis-api/reference/alerts)

#### Tags

- Alerts
- Logs
- Observability
- Notifications

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/alerts)
- [OpenAPI](openapi/mezmo-alerts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-alerts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-alerts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Archiving API

Configure cold-storage archiving via /v1/config/archiving. Supports S3, GCS, Azure Blob, IBM COS, and DigitalOcean Spaces destinations for long-term retention beyond plan limits.

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/archiving](https://docs.mezmo.com/log-analysis-api/reference/archiving)

#### Tags

- Archiving
- Logs
- Storage
- Compliance

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/archiving)
- [OpenAPI](openapi/mezmo-archiving-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-archiving-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-archiving-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Ingestion Control API

Manage exclusion rules (/v1/config/ingestion/exclusions) and ingestion suspend/resume (/v1/config/ingestion/suspend, /resume) to cap costs and stop noisy sources without losing configuration. Two-factor suspension protects against accidental cutoff.

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/exclusions](https://docs.mezmo.com/log-analysis-api/reference/exclusions)

#### Tags

- Ingestion
- Exclusions
- Suspension
- Cost Control

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/exclusions)
- [OpenAPI](openapi/mezmo-ingestion-control-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-ingestion-control-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-ingestion-control-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Usage API

Query log usage by app, host, or tag via /v1/usage/{type} and detailed byte-based consumption via /v2/usage. Used for chargeback, anomaly detection, and capacity planning against ingestion contract volumes.

- **Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/usage](https://docs.mezmo.com/log-analysis-api/reference/usage)

#### Tags

- Usage
- Billing
- Reporting
- FinOps

#### Properties

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/usage)
- [OpenAPI](openapi/mezmo-usage-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-usage-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-usage-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Pipeline API

Programmatic CRUD over Mezmo Telemetry Pipelines at api.mezmo.com/v3. Manage pipelines, sources, processors, destinations, deployments, audit events, and health. Backs Terraform, the Mezmo CLI, and the MCP server. 100+ source and destination integrations including OpenTelemetry, Vector, Kafka, S3, Datadog, Splunk, Elastic, Loki, Sumo Logic, New Relic, and Honeycomb.

- **Human URL:** [https://docs.mezmo.com/pipeline-api](https://docs.mezmo.com/pipeline-api)

#### Tags

- Telemetry Pipeline
- Observability
- Data Pipeline
- OpenTelemetry

#### Properties

- [Documentation](https://docs.mezmo.com/pipeline-api)
- [OpenAPI](openapi/mezmo-pipeline-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-pipeline-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-pipeline-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Pipeline Classification API

AI-assisted data classification, field profiling, parser inference, and regex generation against pipeline samples. Used by Mezmo's in-product authoring workflow to accelerate parser and processor configuration.

- **Human URL:** [https://docs.mezmo.com/pipeline-api/reference/classification](https://docs.mezmo.com/pipeline-api/reference/classification)

#### Tags

- Data Classification
- Profiling
- AI
- Telemetry Pipeline

#### Properties

- [Documentation](https://docs.mezmo.com/pipeline-api/reference/classification)
- [OpenAPI](openapi/mezmo-pipeline-classification-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-pipeline-classification-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-pipeline-classification-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Edge API

Edge / local deployment surface for Mezmo Pipelines. Manage client configuration, heartbeats, task assignments, and result collection for self-hosted pipeline instances running outside the Mezmo control plane.

- **Human URL:** [https://docs.mezmo.com/pipeline-api/reference/edge](https://docs.mezmo.com/pipeline-api/reference/edge)

#### Tags

- Edge
- Local Deployment
- Telemetry Pipeline
- Agents

#### Properties

- [Documentation](https://docs.mezmo.com/pipeline-api/reference/edge)
- [OpenAPI](openapi/mezmo-edge-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/mezmo-edge-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-edge-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Mezmo Agent (logdna-agent-v2)

Open-source Rust log collection agent (logdna-agent-v2). Tails files, journald, and Kubernetes pod logs and ships to Mezmo's ingestion endpoint. MIT-licensed.

- **Human URL:** [https://github.com/logdna/logdna-agent-v2](https://github.com/logdna/logdna-agent-v2)

#### Tags

- Agent
- SDK
- Open Source
- Logs

#### Properties

- [Source Code](https://github.com/logdna/logdna-agent-v2)
- [Documentation](https://docs.mezmo.com/docs/mezmo-agent)
- [Postman Collection](collections/mezmo-alerts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-alerts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-archiving-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-archiving-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-edge-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-edge-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-ingestion-control-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-ingestion-control-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-log-export-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-log-export-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-log-ingestion-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-log-ingestion-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-pipeline-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-pipeline-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-pipeline-classification-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-pipeline-classification-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-usage-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-usage-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-views-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-views-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AURA Agent Framework

Mezmo's open-source agentic orchestration framework. Apache 2.0 Rust framework for composing AI agents from declarative TOML config, with MCP tool integration, RAG pipelines (Qdrant, Bedrock KB), and an OpenAI-compatible web API. LLM-agnostic (OpenAI, Anthropic, Bedrock, Gemini, Ollama). Backs Mezmo's AI SRE and root-cause-analysis workflows.

- **Human URL:** [https://github.com/mezmo/aura](https://github.com/mezmo/aura)

#### Tags

- AI
- Agents
- Open Source
- MCP
- SRE

#### Properties

- [Source Code](https://github.com/mezmo/aura)
- [Documentation](https://www.mezmo.com/)
- [Postman Collection](collections/mezmo-alerts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-alerts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-archiving-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-archiving-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-edge-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-edge-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-ingestion-control-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-ingestion-control-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-log-export-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-log-export-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-log-ingestion-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-log-ingestion-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-pipeline-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-pipeline-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-pipeline-classification-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-pipeline-classification-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-usage-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-usage-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/mezmo-views-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/mezmo-views-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/mezmo)
- [Portal](https://www.mezmo.com/)
- [Documentation](https://docs.mezmo.com/)
- [Documentation](https://docs.mezmo.com/log-analysis-api)
- [Documentation](https://docs.mezmo.com/pipeline-api)
- [Status Page](https://status.mezmo.com/)
- [Changelog](https://www.mezmo.com/changelog)
- [Blog](https://www.mezmo.com/blog)
- [Source Code](https://github.com/mezmo)
- [Source Code](https://github.com/logdna)
- [C L I](https://github.com/mezmo/cli)
- [SDK](https://registry.terraform.io/providers/mezmo/mezmo/latest)
- [SDK](https://github.com/logdna/terraform-provider-logdna)
- [SDK](https://github.com/logdna/logdna-agent-v2)
- [SDK](https://github.com/logdna/nodejs)
- [SDK](https://github.com/logdna/python)
- [SDK](https://github.com/logdna/logdna-rust)
- [M C P Server](https://github.com/mezmo/mezmo-mcp)
- [Source Code](https://github.com/mezmo/aura)
- [SDK](https://github.com/mezmo/helm-charts)
- [Pricing](https://www.mezmo.com/pricing)
- [Plans](plans/mezmo-plans-pricing.yml)
- [Rate Limits](rate-limits/mezmo-rate-limits.yml)
- [Fin Ops](finops/mezmo-finops.yml)
- [Vocabulary](vocabulary/mezmo-vocabulary.yml)
- [Spectral Ruleset](rules/mezmo-rules.yml)
- [JSON-LD](json-ld/mezmo-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
