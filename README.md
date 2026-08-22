# BigID (bigid)

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

BigID is a New York City-headquartered data security platform that combines Data Security Posture Management (DSPM), Data Loss Prevention (DLP), access governance, AI security & governance (AISPM), privacy automation, and a unified Data & AI Catalog. Founded in 2016 by Dimitri Sirota and Nimrod Vax, BigID exposes every action available in its UI through a REST API rooted at /api/v1 — covering data sources, scans, catalog, cluster analysis, DSPM cases, and DSARs — plus an App Framework for building custom apps, a connector framework (Java and REST) for new data sources, and an MCP surface for AI agents.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/bigid/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Access:** 3rd-Party

## Tags

- Data Security
- DSPM
- DLP
- Privacy
- AI Security
- Data Catalog
- DSAR
- Data Discovery
- Compliance

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### BigID Authentication API

Authenticate against a BigID deployment using either username/password or a long-lived user token. Exchange a user token for a short-lived system token (JWT) used to authorize subsequent REST API calls.

- **Human URL:** [https://developer.bigid.com/api/bigid-api-token-authentication/](https://developer.bigid.com/api/bigid-api-token-authentication/)

#### Tags

- Authentication
- Sessions
- Tokens

#### Properties

- [Documentation](https://developer.bigid.com/api/bigid-api-user-authentication/)
- [Documentation](https://developer.bigid.com/api/bigid-api-token-authentication/)
- [OpenAPI](openapi/bigid-authentication-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-authentication-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-authentication-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/bigid-create-session-example.json)

### BigID Data Sources API

Programmatically manage data source connections in BigID. List, create, test, and export data sources, and inspect the catalog of available connector templates (e.g. rdb-mysql, s3-v2, snowflake, sharepoint-online).

- **Human URL:** [https://developer.bigid.com/api/data-source-connections-api-tutorial/](https://developer.bigid.com/api/data-source-connections-api-tutorial/)

#### Tags

- Data Sources
- Connectors

#### Properties

- [Documentation](https://developer.bigid.com/api/data-source-connections-api-tutorial/)
- [Documentation](https://developer.bigid.com/api/bigid-api-add-data-source-tutorial/)
- [OpenAPI](openapi/bigid-data-sources-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-data-sources-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-data-sources-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bigid-data-source-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/bigid-list-data-sources-example.json)

### BigID Scans API

Configure and execute BigID scans. Create scan profiles to control which data sources are scanned and using which classifier template, then start and monitor scan executions and parent-scan rollups.

- **Human URL:** [https://developer.bigid.com/api/scan-profiles-api-tutorial/](https://developer.bigid.com/api/scan-profiles-api-tutorial/)

#### Tags

- Scans
- Scan Profiles

#### Properties

- [Documentation](https://developer.bigid.com/api/scan-profiles-api-tutorial/)
- [Documentation](https://developer.bigid.com/api/scan-insights-api-tutorial/)
- [OpenAPI](openapi/bigid-scans-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-scans-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-scans-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### BigID Data Catalog API

Query and export BigID's data catalog — the central inventory of objects, columns, and attributes discovered by BigID scans. Includes metadata export, duplicate-detection, and cluster-similar-column lookups.

- **Human URL:** [https://developer.bigid.com/api/bigid-api-metadata-export-tutorial/](https://developer.bigid.com/api/bigid-api-metadata-export-tutorial/)

#### Tags

- Catalog
- Metadata
- Duplicates

#### Properties

- [Documentation](https://developer.bigid.com/api/bigid-api-metadata-export-tutorial/)
- [Documentation](https://developer.bigid.com/api/bigid-api-duplicate-data-tutorial/)
- [OpenAPI](openapi/bigid-data-catalog-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-data-catalog-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-data-catalog-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bigid-catalog-object-schema.json) — [JSON Schema](https://json-schema.org/specification)

### BigID Cluster Analysis API

Retrieve clusters of similar data identified by BigID's cluster-analysis engine. Clusters group structurally or semantically similar columns and objects across data sources to support deduplication, retention, and minimization workflows.

- **Human URL:** [https://developer.bigid.com/api/cluster-analysis-api-tutorial/](https://developer.bigid.com/api/cluster-analysis-api-tutorial/)

#### Tags

- Clusters
- Analytics

#### Properties

- [Documentation](https://developer.bigid.com/api/cluster-analysis-api-tutorial/)
- [OpenAPI](openapi/bigid-cluster-analysis-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-cluster-analysis-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-cluster-analysis-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### BigID Data Posture API

Fetch and remediate Data Security Posture Management (DSPM) findings via BigID's actionable insights API. List open cases, bulk-update them, and resolve individual cases with audit reasons.

- **Human URL:** [https://developer.bigid.com/api/data-posture-api-tutorial/](https://developer.bigid.com/api/data-posture-api-tutorial/)

#### Tags

- DSPM
- Actionable Insights
- Security

#### Properties

- [Documentation](https://developer.bigid.com/api/data-posture-api-tutorial/)
- [OpenAPI](openapi/bigid-data-posture-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-data-posture-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-data-posture-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/bigid-case-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Example](examples/bigid-list-posture-cases-example.json)

### BigID DSAR API

Run Data Subject Access Requests (DSARs) and retrieve the resulting reports. Inspect available DSAR profiles and identifier attributes, submit new DSAR scans, poll status, and download short or full reports in JSON or CSV.

- **Human URL:** [https://developer.bigid.com/api/bigid-api-dsar-tutorial/](https://developer.bigid.com/api/bigid-api-dsar-tutorial/)

#### Tags

- DSAR
- Privacy

#### Properties

- [Documentation](https://developer.bigid.com/api/bigid-api-dsar-tutorial/)
- [OpenAPI](openapi/bigid-dsar-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/bigid-dsar-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/bigid-dsar-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Example](examples/bigid-create-dsar-report-example.json)

## Common Properties

- [Developer Portal](https://developer.bigid.com/)
- [Getting Started](https://developer.bigid.com/guides/get-started/)
- [API Reference](https://developer.bigid.com/api/bigid-api/)
- [Documentation](https://developer.bigid.com/apps/building-a-bigid-app/)
- [Documentation](https://developer.bigid.com/connectors/what-is-a-bigid-connector/)
- [Documentation](https://developer.bigid.com/llms/llms/)
- [GitHub Organization](https://github.com/bigexchange)
- [SDK](https://github.com/bigexchange/sdk-javascript)
- [SDK](https://github.com/bigexchange/consent-sdk-ios)
- [Quickstart](https://github.com/bigexchange/quickstart-simple-ts)
- [Quickstart](https://github.com/bigexchange/quickstart-utility-dspm-ts)
- [Code Examples](https://github.com/bigexchange/app-framework-helloworld-app)
- [Code Examples](https://github.com/bigexchange/helm-template)
- [Integrations](https://github.com/bigexchange/bigid-azure-key-vault-app)
- [Integrations](https://github.com/bigexchange/bigid-aws-control-tower)
- [Integrations](https://github.com/bigexchange/aws-security-hub)
- [Integrations](https://github.com/bigexchange/content)
- [Integrations](https://github.com/bigexchange/gtm-consent-template)
- [Portal](https://bigid.com/)
- [Blog](https://bigid.com/blog/)
- [Hub](https://bigid.com/about/)
- [Contact](https://bigid.com/contact/)
- [Terms of Service](https://bigid.com/terms/)
- [Privacy Policy](https://bigid.com/privacy-notice/)
- [Legal](https://bigid.com/cookies/)
- [Compliance](https://bigid.com/sub-processors/)
- [Compliance](https://bigid.com/certifications-and-assessments/)
- [LinkedIn](https://www.linkedin.com/company/bigid/)
- [Spectral Rules](rules/bigid-rules.yml)
- [Vocabulary](vocabulary/bigid-vocabulary.yml)
- [JSON-LD](json-ld/bigid-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Plans](plans/bigid-plans-pricing.yml)
- [Rate Limits](rate-limits/bigid-rate-limits.yml)
- [Fin Ops](finops/bigid-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
