# BigID (bigid)
BigID is a New York City-headquartered data security platform that combines Data Security Posture Management (DSPM), Data Loss Prevention (DLP), access governance, AI security & governance (AISPM), privacy automation, and a unified Data & AI Catalog. Founded in 2016 by Dimitri Sirota and Nimrod Vax, BigID exposes every action available in its UI through a REST API rooted at `/api/v1` — covering data sources, scans, catalog, cluster analysis, DSPM cases, and DSARs — plus an App Framework for building custom apps, a connector framework (Java and REST) for new data sources, and an MCP surface for AI agents.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

 - Data Security, DSPM, DLP, Privacy, AI Security, Data Catalog, DSAR, Data Discovery, Compliance

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### BigID Authentication API
Authenticate against a BigID deployment using either username/password or a long-lived user token. Exchange a user token for a short-lived system token (JWT) used to authorize subsequent REST API calls.

**Human URL:** [https://developer.bigid.com/api/bigid-api-token-authentication/](https://developer.bigid.com/api/bigid-api-token-authentication/)

- [Documentation — User Authentication](https://developer.bigid.com/api/bigid-api-user-authentication/)
- [Documentation — Token Authentication](https://developer.bigid.com/api/bigid-api-token-authentication/)
- [OpenAPI](openapi/bigid-authentication-api-openapi.yml)
- [Example — Create Session](examples/bigid-create-session-example.json)
- [Naftiko Capability — Sessions](capabilities/authentication-sessions.yaml)

### BigID Data Sources API
Programmatically manage data source connections in BigID. List, create, test, and export data sources, and inspect the catalog of available connector templates (e.g. `rdb-mysql`, `s3-v2`, `snowflake`, `sharepoint-online`).

**Human URL:** [https://developer.bigid.com/api/data-source-connections-api-tutorial/](https://developer.bigid.com/api/data-source-connections-api-tutorial/)

- [Documentation — Data Source Connections](https://developer.bigid.com/api/data-source-connections-api-tutorial/)
- [Documentation — Add A Data Source](https://developer.bigid.com/api/bigid-api-add-data-source-tutorial/)
- [OpenAPI](openapi/bigid-data-sources-api-openapi.yml)
- [JSON Schema — Data Source](json-schema/bigid-data-source-schema.json)
- [Example — List Data Sources](examples/bigid-list-data-sources-example.json)
- [Naftiko Capability — Connections](capabilities/data-sources-connections.yaml)
- [Naftiko Capability — Templates](capabilities/data-sources-templates.yaml)

### BigID Scans API
Configure and execute BigID scans. Create scan profiles to control which data sources are scanned and using which classifier template, then start and monitor scan executions and parent-scan rollups.

**Human URL:** [https://developer.bigid.com/api/scan-profiles-api-tutorial/](https://developer.bigid.com/api/scan-profiles-api-tutorial/)

- [Documentation — Scan Profiles](https://developer.bigid.com/api/scan-profiles-api-tutorial/)
- [Documentation — Scan Insights](https://developer.bigid.com/api/scan-insights-api-tutorial/)
- [OpenAPI](openapi/bigid-scans-api-openapi.yml)
- [Naftiko Capability — Scan Profiles](capabilities/scans-profiles.yaml)
- [Naftiko Capability — Scan Executions](capabilities/scans-executions.yaml)

### BigID Data Catalog API
Query and export BigID's data catalog — the central inventory of objects, columns, and attributes discovered by BigID scans. Includes metadata export, duplicate-detection, and cluster-similar-column lookups.

**Human URL:** [https://developer.bigid.com/api/bigid-api-metadata-export-tutorial/](https://developer.bigid.com/api/bigid-api-metadata-export-tutorial/)

- [Documentation — Metadata Export](https://developer.bigid.com/api/bigid-api-metadata-export-tutorial/)
- [Documentation — Duplicate Data](https://developer.bigid.com/api/bigid-api-duplicate-data-tutorial/)
- [OpenAPI](openapi/bigid-data-catalog-api-openapi.yml)
- [JSON Schema — Catalog Object](json-schema/bigid-catalog-object-schema.json)
- [Naftiko Capability — Objects](capabilities/data-catalog-objects.yaml)

### BigID Cluster Analysis API
Retrieve clusters of similar data identified by BigID's cluster-analysis engine. Clusters group structurally or semantically similar columns and objects across data sources to support deduplication, retention, and minimization workflows.

**Human URL:** [https://developer.bigid.com/api/cluster-analysis-api-tutorial/](https://developer.bigid.com/api/cluster-analysis-api-tutorial/)

- [Documentation](https://developer.bigid.com/api/cluster-analysis-api-tutorial/)
- [OpenAPI](openapi/bigid-cluster-analysis-api-openapi.yml)
- [Naftiko Capability — Clusters](capabilities/cluster-analysis-clusters.yaml)

### BigID Data Posture API
Fetch and remediate Data Security Posture Management (DSPM) findings via BigID's actionable insights API. List open cases, bulk-update them, and resolve individual cases with audit reasons.

**Human URL:** [https://developer.bigid.com/api/data-posture-api-tutorial/](https://developer.bigid.com/api/data-posture-api-tutorial/)

- [Documentation](https://developer.bigid.com/api/data-posture-api-tutorial/)
- [OpenAPI](openapi/bigid-data-posture-api-openapi.yml)
- [JSON Schema — Case](json-schema/bigid-case-schema.json)
- [Example — List Cases](examples/bigid-list-posture-cases-example.json)
- [Naftiko Capability — Cases](capabilities/data-posture-cases.yaml)

### BigID DSAR API
Run Data Subject Access Requests (DSARs) and retrieve the resulting reports. Inspect available DSAR profiles and identifier attributes, submit new DSAR scans, poll status, and download short or full reports in JSON or CSV.

**Human URL:** [https://developer.bigid.com/api/bigid-api-dsar-tutorial/](https://developer.bigid.com/api/bigid-api-dsar-tutorial/)

- [Documentation](https://developer.bigid.com/api/bigid-api-dsar-tutorial/)
- [OpenAPI](openapi/bigid-dsar-api-openapi.yml)
- [Example — Create DSAR Report](examples/bigid-create-dsar-report-example.json)
- [Naftiko Capability — Reports](capabilities/dsar-reports.yaml)

## Common Properties

- [BigID Developer Portal](https://developer.bigid.com/) (DeveloperPortal)
- [BigID Get Started Guide](https://developer.bigid.com/guides/get-started/) (GettingStarted)
- [BigID REST API Reference](https://developer.bigid.com/api/bigid-api/) (APIReference)
- [BigID App Framework](https://developer.bigid.com/apps/building-a-bigid-app/) (Documentation)
- [BigID Connector Framework](https://developer.bigid.com/connectors/what-is-a-bigid-connector/) (Documentation)
- [BigID MCP and LLM Integration](https://developer.bigid.com/llms/llms/) (Documentation)
- [BigExchange GitHub Organization](https://github.com/bigexchange) (GitHubOrganization)
- [BigID JavaScript SDK](https://github.com/bigexchange/sdk-javascript) (SDK)
- [BigID iOS Consent SDK](https://github.com/bigexchange/consent-sdk-ios) (SDK)
- [BigID Simple App Quickstart (TypeScript)](https://github.com/bigexchange/quickstart-simple-ts) (Quickstart)
- [BigID DSPM Quickstart (TypeScript)](https://github.com/bigexchange/quickstart-utility-dspm-ts) (Quickstart)
- [BigID App Framework Hello-World App (Java)](https://github.com/bigexchange/app-framework-helloworld-app) (CodeExamples)
- [BigID External-Service Helm Template](https://github.com/bigexchange/helm-template) (CodeExamples)
- [BigID Azure Key Vault App](https://github.com/bigexchange/bigid-azure-key-vault-app) (Integrations)
- [BigID AWS Control Tower Integration](https://github.com/bigexchange/bigid-aws-control-tower) (Integrations)
- [BigID AWS Security Hub Integration](https://github.com/bigexchange/aws-security-hub) (Integrations)
- [BigID XSOAR Content Pack](https://github.com/bigexchange/content) (Integrations)
- [BigID GTM Consent Template](https://github.com/bigexchange/gtm-consent-template) (Integrations)
- [BigID Website](https://bigid.com/) (Portal)
- [BigID Blog](https://bigid.com/blog/) (Blog)
- [About BigID](https://bigid.com/about/) (Hub)
- [Contact BigID](https://bigid.com/contact/) (Contact)
- [BigID Terms and Conditions](https://bigid.com/terms/) (TermsOfService)
- [BigID Privacy Notice](https://bigid.com/privacy-notice/) (PrivacyPolicy)
- [BigID Cookies Policy](https://bigid.com/cookies/) (Legal)
- [BigID Sub-processors](https://bigid.com/sub-processors/) (Compliance)
- [BigID Certifications and Assessments](https://bigid.com/certifications-and-assessments/) (Compliance)
- [BigID on LinkedIn](https://www.linkedin.com/company/bigid/) (LinkedIn)
- [BigID Spectral Ruleset](rules/bigid-rules.yml) (SpectralRules)
- [BigID Vocabulary](vocabulary/bigid-vocabulary.yml) (Vocabulary)
- [BigID JSON-LD Context](json-ld/bigid-context.jsonld) (JSONLD)
- [BigID Plans and Pricing](plans/bigid-plans-pricing.yml) (Plans)
- [BigID Rate Limits](rate-limits/bigid-rate-limits.yml) (RateLimits)
- [BigID FinOps Profile](finops/bigid-finops.yml) (FinOps)

## Features

- **Data Security Posture Management (DSPM)** — Continuous risk detection across cloud, on-prem, and SaaS data with severity-based remediation workflows.
- **Data Loss Prevention (DLP)** — ML-enhanced DLP with custom labeling by sensitivity, residency, and risk; integrates with MIP and Google labels.
- **Access Governance** — Identify over-privileged access, enable zero-trust controls, and mitigate insider risk.
- **AI Security & Governance (AISPM)** — Shadow AI detection, AI model inventory, prompt and response governance, TRiSM.
- **Privacy Automation** — DSAR fulfillment, retention, deletion, consent, and 190,000+ out-of-the-box retention policies.
- **Data & AI Catalog** — Unified catalog of structured/unstructured data, AI models, prompts, and agents.
- **100+ Data Source Connectors** — Cloud, SaaS, on-prem, and developer-environment connectors plus a custom connector framework.
- **1000+ Pre-Trained Classifiers** — Patented AI classification across 100+ languages.
- **App Framework** — Build custom apps via `/manifest`, `/execute`, and `/ui` HTTP endpoints; deploy on Kubernetes.
- **MCP for Agents** — BigID exposes its data governance and connector surface through the Model Context Protocol.

## Use Cases

- **AI Risk Management and TRiSM** — Discover, govern, and secure AI models, training data, prompts, and agent surfaces.
- **Cloud Data Security** — Find and remediate exposed PII, PHI, PCI in S3, GCS, Azure Storage, Snowflake, Databricks.
- **Data Minimization** — Surface duplicate and stale data to shrink the sensitive-data footprint.
- **Privacy Compliance** — Operationalize HIPAA, GDPR, CCPA, LGPD with DSAR, retention, and consent automation.
- **Insider Risk Detection** — Spot suspicious access to sensitive data based on behavior, role, and policy.
- **Breach Investigation** — Determine what sensitive data was implicated in an incident and notify accordingly.
- **Source Code DLP** — Prevent exfiltration of source code and credentials.

## Integrations

AWS, Snowflake, Databricks, Splunk, Wiz, Salesforce, ServiceNow, Collibra, Alation, Informatica, Atlan, Microsoft Information Protection (MIP), Cortex XSOAR, Google Tag Manager.

## Solutions

- **Data Security Platform** — DSPM + DLP + access governance.
- **Privacy Automation Suite** — DSAR, retention, deletion, consent, regulatory reporting.
- **AI Security & Governance** — Shadow AI, model inventory, prompt/response governance, TRiSM.
- **Data & AI Catalog** — Unified catalog spanning structured, unstructured, and AI assets.

## Maintainers

- **Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com) — [apievangelist.com](https://apievangelist.com)
