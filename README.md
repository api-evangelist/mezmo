# Mezmo (mezmo)

Mezmo (formerly LogDNA) is a log management and telemetry pipeline platform. The platform ingests
logs at logs.mezmo.com, exposes a Log Analysis API at api.mezmo.com for views, alerts, archiving,
exclusions, suspension, and usage, and ships a programmatic Pipelines control plane at
api.mezmo.com/v3 for managing sources, processors, destinations, and edge clients across 100+
integrations including OpenTelemetry, Vector, Kafka, S3, Datadog, Splunk, Elastic, Loki, Sumo Logic,
New Relic, and Honeycomb. Mezmo also publishes AURA, an Apache 2.0 Rust framework for composing
agentic AI workflows on top of its telemetry, plus a Terraform provider, CLI, Helm charts, and an
MCP server.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/mezmo/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Observability, Logs, Telemetry, Telemetry Pipeline, Log Management, AI, SRE, OpenTelemetry, DevOps

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Mezmo Log Ingestion API
Ingest log lines into Mezmo at logs.mezmo.com/logs/ingest. Batched JSON with timestamp, app, env,
hostname, level, and free-form meta. Token or service-key auth.

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/log-ingestion-api](https://docs.mezmo.com/log-analysis-api/reference/log-ingestion-api)

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/log-ingestion-api)
- [OpenAPI](openapi/mezmo-log-ingestion-api-openapi.yml)
- [Naftiko Capability - Logs](capabilities/log-ingestion-logs.yaml)

### Mezmo Log Export API
Query and paginate historical log exports via /v1/export (plan-bounded) and /v2/export (paginated).

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/export](https://docs.mezmo.com/log-analysis-api/reference/export)

- [Documentation](https://docs.mezmo.com/log-analysis-api/reference/export)
- [OpenAPI](openapi/mezmo-log-export-api-openapi.yml)
- [Naftiko Capability - Export](capabilities/log-export-export.yaml)

### Mezmo Views API
CRUD saved Views (queries over hosts, apps, levels, tags, free-text). Views are the resource
preset alerts attach to.

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/views](https://docs.mezmo.com/log-analysis-api/reference/views)

- [OpenAPI](openapi/mezmo-views-api-openapi.yml)
- [Naftiko Capability - Views](capabilities/views-views.yaml)

### Mezmo Alerts API
Manage preset alerts and their notification channels (PagerDuty, Slack, webhook, email, OpsGenie,
VictorOps).

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/alerts](https://docs.mezmo.com/log-analysis-api/reference/alerts)

- [OpenAPI](openapi/mezmo-alerts-api-openapi.yml)
- [Naftiko Capability - Preset Alerts](capabilities/alerts-presetalerts.yaml)

### Mezmo Archiving API
Configure cold-storage archiving to AWS S3, GCS, Azure Blob, IBM COS, or DigitalOcean Spaces.

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/archiving](https://docs.mezmo.com/log-analysis-api/reference/archiving)

- [OpenAPI](openapi/mezmo-archiving-api-openapi.yml)
- [Naftiko Capability - Archiving](capabilities/archiving-archiving.yaml)

### Mezmo Ingestion Control API
Manage exclusion rules and ingestion suspension. Two-factor suspend protects against accidental
cutoff.

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/exclusions](https://docs.mezmo.com/log-analysis-api/reference/exclusions)

- [OpenAPI](openapi/mezmo-ingestion-control-api-openapi.yml)
- [Naftiko Capability - Exclusions](capabilities/ingestion-control-exclusions.yaml)
- [Naftiko Capability - Suspension](capabilities/ingestion-control-suspension.yaml)

### Mezmo Usage API
Query usage by app, host, tag and detailed byte-based consumption for chargeback and FinOps.

**Human URL:** [https://docs.mezmo.com/log-analysis-api/reference/usage](https://docs.mezmo.com/log-analysis-api/reference/usage)

- [OpenAPI](openapi/mezmo-usage-api-openapi.yml)
- [Naftiko Capability - Usage](capabilities/usage-usage.yaml)

### Mezmo Pipeline API
Programmatic CRUD over Mezmo Telemetry Pipelines at api.mezmo.com/v3 — pipelines, sources,
processors, destinations, deployments, audit events, health. Backs the Terraform provider, CLI,
and MCP server.

**Human URL:** [https://docs.mezmo.com/pipeline-api](https://docs.mezmo.com/pipeline-api)

- [OpenAPI](openapi/mezmo-pipeline-api-openapi.yml)
- [Naftiko Capability - Pipelines](capabilities/pipeline-pipelines.yaml)
- [Naftiko Capability - Sources](capabilities/pipeline-sources.yaml)
- [Naftiko Capability - Processors](capabilities/pipeline-processors.yaml)
- [Naftiko Capability - Destinations](capabilities/pipeline-destinations.yaml)

### Mezmo Pipeline Classification API
AI-assisted field profiling, parser inference, and regex generation against pipeline samples.

**Human URL:** [https://docs.mezmo.com/pipeline-api/reference/classification](https://docs.mezmo.com/pipeline-api/reference/classification)

- [OpenAPI](openapi/mezmo-pipeline-classification-api-openapi.yml)
- [Naftiko Capability - Classification](capabilities/pipeline-classification-classification.yaml)

### Mezmo Edge API
Edge / local deployment surface — client registration, heartbeats, task delivery, result
collection for self-hosted pipeline instances.

**Human URL:** [https://docs.mezmo.com/pipeline-api/reference/edge](https://docs.mezmo.com/pipeline-api/reference/edge)

- [OpenAPI](openapi/mezmo-edge-api-openapi.yml)
- [Naftiko Capability - Edge Clients](capabilities/edge-clients.yaml)

### Mezmo Agent (logdna-agent-v2)
Open-source Rust log collection agent. Tails files, journald, and Kubernetes pod logs and ships
to Mezmo's ingestion endpoint. MIT-licensed.

**Human URL:** [https://github.com/logdna/logdna-agent-v2](https://github.com/logdna/logdna-agent-v2)

### AURA Agent Framework
Mezmo's open-source agentic orchestration framework. Apache 2.0 Rust framework for composing AI
agents from declarative TOML config, with MCP tool integration, RAG (Qdrant, Bedrock KB), and
an OpenAI-compatible web API. LLM-agnostic (OpenAI, Anthropic, Bedrock, Gemini, Ollama).

**Human URL:** [https://github.com/mezmo/aura](https://github.com/mezmo/aura)

## Common

- [Mezmo](https://www.mezmo.com/) - Portal
- [Mezmo Docs](https://docs.mezmo.com/) - Documentation
- [Log Analysis API Reference](https://docs.mezmo.com/log-analysis-api) - Documentation
- [Pipeline API Reference](https://docs.mezmo.com/pipeline-api) - Documentation
- [Mezmo Status](https://status.mezmo.com/) - StatusPage
- [Mezmo Changelog](https://www.mezmo.com/changelog) - ChangeLog
- [Mezmo Blog](https://www.mezmo.com/blog) - Blog
- [Mezmo GitHub](https://github.com/mezmo) - SourceCode
- [LogDNA GitHub (legacy)](https://github.com/logdna) - SourceCode
- [Mezmo CLI](https://github.com/mezmo/cli) - CLI
- [Terraform Provider for Mezmo](https://registry.terraform.io/providers/mezmo/mezmo/latest) - SDK
- [Mezmo Agent](https://github.com/logdna/logdna-agent-v2) - SDK
- [LogDNA Node.js SDK](https://github.com/logdna/nodejs) - SDK
- [LogDNA Python SDK](https://github.com/logdna/python) - SDK
- [LogDNA Rust SDK](https://github.com/logdna/logdna-rust) - SDK
- [Mezmo MCP Server](https://github.com/mezmo/mezmo-mcp) - MCPServer
- [AURA](https://github.com/mezmo/aura) - SourceCode
- [Mezmo Helm Charts](https://github.com/mezmo/helm-charts) - SDK
- [Mezmo Pricing](https://www.mezmo.com/pricing) - Pricing

## Artifacts

- [Plans (API Commons)](plans/mezmo-plans-pricing.yml)
- [Rate Limits (API Commons)](rate-limits/mezmo-rate-limits.yml)
- [FinOps Surface](finops/mezmo-finops.yml)
- [Vocabulary](vocabulary/mezmo-vocabulary.yml)
- [Spectral Ruleset](rules/mezmo-rules.yml)
- [JSON-LD Context](json-ld/mezmo-context.jsonld)
- [JSON Schema - Log Line](json-schema/mezmo-log-line-schema.json)
- [JSON Schema - Pipeline](json-schema/mezmo-pipeline-schema.json)
