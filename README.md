# Qlik Sense

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

Qlik Sense and Qlik Cloud from Qlik Parent, Inc. — a business intelligence, data integration and AI analytics platform. Qlik publishes one of the broadest machine-readable API surfaces in the analytics market: 78 OpenAPI 3.0.0 documents covering 681 REST operations, 29 AsyncAPI 3.0.0 event documents carrying CloudEvents 1.0 payloads, an OpenRPC 1.0.0 document for the QIX Associative Engine WebSocket API, 39 JSON Schemas for Qlik Talend Cloud declarative pipelines, and a proto3 gRPC contract for the engine's Server-Side Extension protocol. It also ships a generally-available remote MCP server at <tenant>/api/ai/mcp and maintains a public Agent Skills hub. Every API is tenant-scoped to https://{tenant}.{region}.qlikcloud.com and authenticated with an API key, an OAuth 2.0 token or a signed JWT.

**Areas:** Agents · Analytics · Artificial Intelligence · Business Intelligence · Cloud · Data Integration · Data Visualization · Embedded Analytics · Enterprise · Machine Learning

## Qlik Sense on APIs.io

Everything profiled for Qlik Sense is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/qliksense/](https://apis.io/providers/qliksense/)** — or go straight to one of the APIs or properties below.

### APIs (135)

- [Qlik Engine API](https://apis.io/apis/qliksense/engine-api/) — JSON-RPC WebSocket API for interacting with the Qlik Associative Engine, creating and manipulating apps, and building visualizations.
- [Qlik Server-Side Extension Protocol](https://apis.io/apis/qliksense/server-side-extension/) — gRPC/protobuf contract for extending the Qlik Associative Engine with external compute. A plugin implements the qlik.sse.Connector service and the engine…
- [Qlik Cloud System Events](https://apis.io/apis/qliksense/system-events/) — The Qlik Cloud tenant event surface: 29 AsyncAPI 3.0.0 documents covering 102 message definitions across apps, reloads, spaces, tenants, users, roles,…
- [Qlik MCP Server](https://apis.io/apis/qliksense/mcp-server/) — Qlik's first-party remote Model Context Protocol server, generally available since 2026-02-10 and included from the Starter plan up. It exposes Qlik Cloud…
- [Qlik Sense Engine API](https://apis.io/apis/qliksense/qlik-sense-engine-api/) — WebSocket-based API for interacting with the Qlik Associative Engine, including data modeling, selections, and visualizations.
- [Qlik Sense Repository API](https://apis.io/apis/qliksense/qlik-sense-repository-api/) — REST API for managing Qlik Sense repository objects including apps, streams, users, and security rules.
- [Qlik Sense Proxy API](https://apis.io/apis/qliksense/qlik-sense-proxy-api/) — REST API for session management and authentication through the Qlik Sense Proxy Service.
- [Qlik Data Integration API](https://apis.io/apis/qliksense/qlik-data-integration-api/) — REST API for managing data integration tasks, connections, and data pipelines.
- [Qlik Embedding API](https://apis.io/apis/qliksense/qlik-embedding-api/) — JavaScript API for embedding Qlik Sense visualizations and mashups into web applications.
- [Qlik Sense alerting actions API](https://apis.io/apis/qliksense/qliksense-alerting-actions-api/) — The alerting actions API from Qlik Sense — 2 operation(s) for alerting actions.
- [Qlik Sense alerting settings API](https://apis.io/apis/qliksense/qliksense-alerting-settings-api/) — The alerting settings API from Qlik Sense — 1 operation(s) for alerting settings.
- [Qlik Sense alerting tasks API](https://apis.io/apis/qliksense/qliksense-alerting-tasks-api/) — The alerting tasks API from Qlik Sense — 4 operation(s) for alerting tasks.
- [Qlik Sense alerting tasks executions API](https://apis.io/apis/qliksense/qliksense-alerting-tasks-executions-api/) — The alerting tasks executions API from Qlik Sense — 4 operation(s) for alerting tasks executions.
- [Qlik Sense Aliases API](https://apis.io/apis/qliksense/qliksense-aliases-api/) — The aliases API from Qlik Sense — 2 operation(s) for aliases.
- [Qlik Sense Analytics API](https://apis.io/apis/qliksense/qliksense-analytics-api/) — The Analytics API from Qlik Sense — 1 operation(s) for analytics.
- [Qlik Sense API Keys API](https://apis.io/apis/qliksense/qliksense-api-keys-api/) — The api-keys API from Qlik Sense — 2 operation(s) for api-keys.
- [Qlik Sense api-keys configurations API](https://apis.io/apis/qliksense/qliksense-api-keys-configurations-api/) — The api-keys configurations API from Qlik Sense — 1 operation(s) for api-keys configurations.
- [Qlik Sense api settings API](https://apis.io/apis/qliksense/qliksense-api-settings-api/) — The api settings API from Qlik Sense — 1 operation(s) for api settings.
- [Qlik Sense Apps API](https://apis.io/apis/qliksense/qliksense-apps-api/) — The Apps API from Qlik Sense — 23 operation(s) for apps.
- [Qlik Sense Assignments API](https://apis.io/apis/qliksense/qliksense-assignments-api/) — The assignments API from Qlik Sense — 2 operation(s) for assignments.
- [Qlik Sense Assistants API](https://apis.io/apis/qliksense/qliksense-assistants-api/) — The assistants API from Qlik Sense — 4 operation(s) for assistants.
- [Qlik Sense async actions API](https://apis.io/apis/qliksense/qliksense-async-actions-api/) — The async actions API from Qlik Sense — 1 operation(s) for async actions.
- [Qlik Sense Audits API](https://apis.io/apis/qliksense/qliksense-audits-api/) — The audits API from Qlik Sense — 7 operation(s) for audits.
- [Qlik Sense Automation Connections API](https://apis.io/apis/qliksense/qliksense-automation-connections-api/) — The automation-connections API from Qlik Sense — 10 operation(s) for automation-connections.
- [Qlik Sense Automation Connectors API](https://apis.io/apis/qliksense/qliksense-automation-connectors-api/) — The automation-connectors API from Qlik Sense — 4 operation(s) for automation-connectors.
- [Qlik Sense Automations API](https://apis.io/apis/qliksense/qliksense-automations-api/) — The automations API from Qlik Sense — 30 operation(s) for automations.
- [Qlik Sense Automl Deployments API](https://apis.io/apis/qliksense/qliksense-automl-deployments-api/) — The automl-deployments API from Qlik Sense — 1 operation(s) for automl-deployments.
- [Qlik Sense Automl Predictions API](https://apis.io/apis/qliksense/qliksense-automl-predictions-api/) — The automl-predictions API from Qlik Sense — 6 operation(s) for automl-predictions.
- [Qlik Sense Banner API](https://apis.io/apis/qliksense/qliksense-banner-api/) — The banner API from Qlik Sense — 2 operation(s) for banner.
- [Qlik Sense Brands API](https://apis.io/apis/qliksense/qliksense-brands-api/) — The brands API from Qlik Sense — 6 operation(s) for brands.
- [Qlik Sense Categories API](https://apis.io/apis/qliksense/qliksense-categories-api/) — The categories API from Qlik Sense — 2 operation(s) for categories.
- [Qlik Sense Change Stores API](https://apis.io/apis/qliksense/qliksense-change-stores-api/) — The change-stores API from Qlik Sense — 2 operation(s) for change-stores.
- [Qlik Sense Changes API](https://apis.io/apis/qliksense/qliksense-changes-api/) — The changes API from Qlik Sense — 2 operation(s) for changes.
- [Qlik Sense Chat API](https://apis.io/apis/qliksense/qliksense-chat-api/) — The chat API from Qlik Sense — 2 operation(s) for chat.
- [Qlik Sense Collections API](https://apis.io/apis/qliksense/qliksense-collections-api/) — The collections API from Qlik Sense — 5 operation(s) for collections.
- [Qlik Sense Computation API](https://apis.io/apis/qliksense/qliksense-computation-api/) — The computation API from Qlik Sense — 5 operation(s) for computation.
- [Qlik Sense condition preview API](https://apis.io/apis/qliksense/qliksense-condition-preview-api/) — The condition preview API from Qlik Sense — 2 operation(s) for condition preview.
- [Qlik Sense Conditions API](https://apis.io/apis/qliksense/qliksense-conditions-api/) — The conditions API from Qlik Sense — 2 operation(s) for conditions.
- [Qlik Sense Consumption API](https://apis.io/apis/qliksense/qliksense-consumption-api/) — The Consumption API from Qlik Sense — 1 operation(s) for consumption.
- [Qlik Sense Csp Origins API](https://apis.io/apis/qliksense/qliksense-csp-origins-api/) — The csp-origins API from Qlik Sense — 3 operation(s) for csp-origins.
- [Qlik Sense Csrf API](https://apis.io/apis/qliksense/qliksense-csrf-api/) — The csrf API from Qlik Sense — 1 operation(s) for csrf.
- [Qlik Sense Data Asset API](https://apis.io/apis/qliksense/qliksense-data-asset-api/) — The data-asset API from Qlik Sense — 2 operation(s) for data-asset.
- [Qlik Sense Data Connections API](https://apis.io/apis/qliksense/qliksense-data-connections-api/) — The data-connections API from Qlik Sense — 5 operation(s) for data-connections.
- [Qlik Sense Data Credentials API](https://apis.io/apis/qliksense/qliksense-data-credentials-api/) — The data-credentials API from Qlik Sense — 2 operation(s) for data-credentials.
- [Qlik Sense Data Product Activation API](https://apis.io/apis/qliksense/qliksense-data-product-activation-api/) — The data-product-activation API from Qlik Sense — 2 operation(s) for data-product-activation.
- [Qlik Sense Data Product API](https://apis.io/apis/qliksense/qliksense-data-product-api/) — The data-product API from Qlik Sense — 4 operation(s) for data-product.
- [Qlik Sense Data Product Changelog API](https://apis.io/apis/qliksense/qliksense-data-product-changelog-api/) — The data-product-changelog API from Qlik Sense — 1 operation(s) for data-product-changelog.
- [Qlik Sense Data Product Data Quality API](https://apis.io/apis/qliksense/qliksense-data-product-data-quality-api/) — The data-product-data-quality API from Qlik Sense — 1 operation(s) for data-product-data-quality.
- [Qlik Sense Data Product Generate Provider URL API](https://apis.io/apis/qliksense/qliksense-data-product-generate-provider-url-api/) — The data-product-generate-provider-url API from Qlik Sense — 1 operation(s) for data-product-generate-provider-url.
- [Qlik Sense data project actions API](https://apis.io/apis/qliksense/qliksense-data-project-actions-api/) — The data project actions API from Qlik Sense — 2 operation(s) for data project actions.
- [Qlik Sense data project API](https://apis.io/apis/qliksense/qliksense-data-project-api/) — The data project API from Qlik Sense — 2 operation(s) for data project.
- [Qlik Sense data project deployment API](https://apis.io/apis/qliksense/qliksense-data-project-deployment-api/) — The data project deployment API from Qlik Sense — 5 operation(s) for data project deployment.
- [Qlik Sense Data Quality API](https://apis.io/apis/qliksense/qliksense-data-quality-api/) — The data-quality API from Qlik Sense — 4 operation(s) for data-quality.
- [Qlik Sense Data Sources API](https://apis.io/apis/qliksense/qliksense-data-sources-api/) — The data-sources API from Qlik Sense — 4 operation(s) for data-sources.
- [Qlik Sense data task actions API](https://apis.io/apis/qliksense/qliksense-data-task-actions-api/) — The data task actions API from Qlik Sense — 4 operation(s) for data task actions.
- [Qlik Sense data task API](https://apis.io/apis/qliksense/qliksense-data-task-api/) — The data task API from Qlik Sense — 2 operation(s) for data task.
- [Qlik Sense data task runtime API](https://apis.io/apis/qliksense/qliksense-data-task-runtime-api/) — The data task runtime API from Qlik Sense — 4 operation(s) for data task runtime.
- [Qlik Sense Datafiles API](https://apis.io/apis/qliksense/qliksense-datafiles-api/) — The datafiles API from Qlik Sense — 9 operation(s) for datafiles.
- [Qlik Sense Deliveries API](https://apis.io/apis/qliksense/qliksense-deliveries-api/) — The deliveries API from Qlik Sense — 3 operation(s) for deliveries.
- [Qlik Sense Deployments API](https://apis.io/apis/qliksense/qliksense-deployments-api/) — The deployments API from Qlik Sense — 6 operation(s) for deployments.
- [Qlik Sense Direct Access Agent Benchmarking API](https://apis.io/apis/qliksense/qliksense-direct-access-agent-benchmarking-api/) — The direct-access-agent-benchmarking API from Qlik Sense — 3 operation(s) for direct-access-agent-benchmarking.
- [Qlik Sense Direct Access Agent Configuration API](https://apis.io/apis/qliksense/qliksense-direct-access-agent-configuration-api/) — The direct-access-agent-configuration API from Qlik Sense — 7 operation(s) for direct-access-agent-configuration.
- [Qlik Sense Editable Columns API](https://apis.io/apis/qliksense/qliksense-editable-columns-api/) — The editable-columns API from Qlik Sense — 1 operation(s) for editable-columns.
- [Qlik Sense Email Config Actions API](https://apis.io/apis/qliksense/qliksense-email-config-actions-api/) — The email-config-actions API from Qlik Sense — 3 operation(s) for email-config-actions.
- [Qlik Sense Email Config API](https://apis.io/apis/qliksense/qliksense-email-config-api/) — The email-config API from Qlik Sense — 1 operation(s) for email-config.
- [Qlik Sense Evaluation API](https://apis.io/apis/qliksense/qliksense-evaluation-api/) — The evaluation API from Qlik Sense — 10 operation(s) for evaluation.
- [Qlik Sense Evaluations API](https://apis.io/apis/qliksense/qliksense-evaluations-api/) — The evaluations API from Qlik Sense — 2 operation(s) for evaluations.
- [Qlik Sense Experiments API](https://apis.io/apis/qliksense/qliksense-experiments-api/) — The experiments API from Qlik Sense — 7 operation(s) for experiments.
- [Qlik Sense Extensions API](https://apis.io/apis/qliksense/qliksense-extensions-api/) — The extensions API from Qlik Sense — 4 operation(s) for extensions.
- [Qlik Sense Filters API](https://apis.io/apis/qliksense/qliksense-filters-api/) — The filters API from Qlik Sense — 3 operation(s) for filters.
- [Qlik Sense Glossaries API](https://apis.io/apis/qliksense/qliksense-glossaries-api/) — The glossaries API from Qlik Sense — 4 operation(s) for glossaries.
- [Qlik Sense Groups API](https://apis.io/apis/qliksense/qliksense-groups-api/) — The groups API from Qlik Sense — 3 operation(s) for groups.
- [Qlik Sense Groups Settings API](https://apis.io/apis/qliksense/qliksense-groups-settings-api/) — The groups-settings API from Qlik Sense — 1 operation(s) for groups-settings.
- [Qlik Sense Iam Resources API](https://apis.io/apis/qliksense/qliksense-iam-resources-api/) — The iam-resources API from Qlik Sense — 3 operation(s) for iam-resources.
- [Qlik Sense Idp API](https://apis.io/apis/qliksense/qliksense-idp-api/) — The idp API from Qlik Sense — 5 operation(s) for idp.
- [Qlik Sense Impact API](https://apis.io/apis/qliksense/qliksense-impact-api/) — The impact API from Qlik Sense — 4 operation(s) for impact.
- [Qlik Sense Insight Analyses API](https://apis.io/apis/qliksense/qliksense-insight-analyses-api/) — The insight-analyses API from Qlik Sense — 3 operation(s) for insight-analyses.
- [Qlik Sense Invite API](https://apis.io/apis/qliksense/qliksense-invite-api/) — The invite API from Qlik Sense — 1 operation(s) for invite.
- [Qlik Sense Items API](https://apis.io/apis/qliksense/qliksense-items-api/) — The items API from Qlik Sense — 4 operation(s) for items.
- [Qlik Sense Items Settings API](https://apis.io/apis/qliksense/qliksense-items-settings-api/) — The items-settings API from Qlik Sense — 1 operation(s) for items-settings.
- [Qlik Sense Jobs API](https://apis.io/apis/qliksense/qliksense-jobs-api/) — The jobs API from Qlik Sense — 1 operation(s) for jobs.
- [Qlik Sense Licenses API](https://apis.io/apis/qliksense/qliksense-licenses-api/) — The licenses API from Qlik Sense — 8 operation(s) for licenses.
- [Qlik Sense Lineage Graphs API](https://apis.io/apis/qliksense/qliksense-lineage-graphs-api/) — The lineage-graphs API from Qlik Sense — 4 operation(s) for lineage-graphs.
- [Qlik Sense Link API](https://apis.io/apis/qliksense/qliksense-link-api/) — The Link API from Qlik Sense — 4 operation(s) for link.
- [Qlik Sense Links API](https://apis.io/apis/qliksense/qliksense-links-api/) — The links API from Qlik Sense — 1 operation(s) for links.
- [Qlik Sense Login API](https://apis.io/apis/qliksense/qliksense-login-api/) — The login API from Qlik Sense — 1 operation(s) for login.
- [Qlik Sense Notifications API](https://apis.io/apis/qliksense/qliksense-notifications-api/) — The notifications API from Qlik Sense — 1 operation(s) for notifications.
- [Qlik Sense OAUTH Clients API](https://apis.io/apis/qliksense/qliksense-oauth-clients-api/) — The oauth-clients API from Qlik Sense — 6 operation(s) for oauth-clients.
- [Qlik Sense OAUTH Tokens API](https://apis.io/apis/qliksense/qliksense-oauth-tokens-api/) — The oauth-tokens API from Qlik Sense — 2 operation(s) for oauth-tokens.
- [Qlik Sense Outputs API](https://apis.io/apis/qliksense/qliksense-outputs-api/) — The outputs API from Qlik Sense — 1 operation(s) for outputs.
- [Qlik Sense Owl API](https://apis.io/apis/qliksense/qliksense-owl-api/) — The owl API from Qlik Sense — 1 operation(s) for owl.
- [Qlik Sense pinned links API](https://apis.io/apis/qliksense/qliksense-pinned-links-api/) — The pinned links API from Qlik Sense — 4 operation(s) for pinned links.
- [Qlik Sense Predictions API](https://apis.io/apis/qliksense/qliksense-predictions-api/) — The predictions API from Qlik Sense — 6 operation(s) for predictions.
- [Qlik Sense Profile API](https://apis.io/apis/qliksense/qliksense-profile-api/) — The profile API from Qlik Sense — 1 operation(s) for profile.
- [Qlik Sense Profile Insights API](https://apis.io/apis/qliksense/qliksense-profile-insights-api/) — The profile-insights API from Qlik Sense — 2 operation(s) for profile-insights.
- [Qlik Sense Questions API](https://apis.io/apis/qliksense/qliksense-questions-api/) — The questions API from Qlik Sense — 2 operation(s) for questions.
- [Qlik Sense Quotas API](https://apis.io/apis/qliksense/qliksense-quotas-api/) — The quotas API from Qlik Sense — 2 operation(s) for quotas.
- [Qlik Sense Reload Tasks API](https://apis.io/apis/qliksense/qliksense-reload-tasks-api/) — The reload-tasks API from Qlik Sense — 2 operation(s) for reload-tasks.
- [Qlik Sense Reloads API](https://apis.io/apis/qliksense/qliksense-reloads-api/) — The reloads API from Qlik Sense — 3 operation(s) for reloads.
- [Qlik Sense Report Templates API](https://apis.io/apis/qliksense/qliksense-report-templates-api/) — The report-templates API from Qlik Sense — 3 operation(s) for report-templates.
- [Qlik Sense Reports API](https://apis.io/apis/qliksense/qliksense-reports-api/) — The reports API from Qlik Sense — 1 operation(s) for reports.
- [Qlik Sense Request API](https://apis.io/apis/qliksense/qliksense-request-api/) — The Request API from Qlik Sense — 6 operation(s) for request.
- [Qlik Sense Roles API](https://apis.io/apis/qliksense/qliksense-roles-api/) — The roles API from Qlik Sense — 2 operation(s) for roles.
- [Qlik Sense Search API](https://apis.io/apis/qliksense/qliksense-search-api/) — The search API from Qlik Sense — 2 operation(s) for search.
- [Qlik Sense Setting API](https://apis.io/apis/qliksense/qliksense-setting-api/) — The setting API from Qlik Sense — 1 operation(s) for setting.
- [Qlik Sense Settings API](https://apis.io/apis/qliksense/qliksense-settings-api/) — The Settings API from Qlik Sense — 2 operation(s) for settings.
- [Qlik Sense Shares API](https://apis.io/apis/qliksense/qliksense-shares-api/) — The shares API from Qlik Sense — 2 operation(s) for shares.
- [Qlik Sense sharing settings API](https://apis.io/apis/qliksense/qliksense-sharing-settings-api/) — The sharing settings API from Qlik Sense — 1 operation(s) for sharing settings.
- [Qlik Sense sharing tasks actions API](https://apis.io/apis/qliksense/qliksense-sharing-tasks-actions-api/) — The sharing tasks actions API from Qlik Sense — 2 operation(s) for sharing tasks actions.
- [Qlik Sense sharing tasks API](https://apis.io/apis/qliksense/qliksense-sharing-tasks-api/) — The sharing tasks API from Qlik Sense — 2 operation(s) for sharing tasks.
- [Qlik Sense sharing tasks executions API](https://apis.io/apis/qliksense/qliksense-sharing-tasks-executions-api/) — The sharing tasks executions API from Qlik Sense — 3 operation(s) for sharing tasks executions.
- [Qlik Sense Spaces API](https://apis.io/apis/qliksense/qliksense-spaces-api/) — The spaces API from Qlik Sense — 3 operation(s) for spaces.
- [Qlik Sense Starters API](https://apis.io/apis/qliksense/qliksense-starters-api/) — The starters API from Qlik Sense — 3 operation(s) for starters.
- [Qlik Sense Status API](https://apis.io/apis/qliksense/qliksense-status-api/) — The status API from Qlik Sense — 1 operation(s) for status.
- [Qlik Sense Task API](https://apis.io/apis/qliksense/qliksense-task-api/) — The task API from Qlik Sense — 14 operation(s) for task.
- [Qlik Sense Task Graph API](https://apis.io/apis/qliksense/qliksense-task-graph-api/) — The task-graph API from Qlik Sense — 5 operation(s) for task-graph.
- [Qlik Sense task run history API](https://apis.io/apis/qliksense/qliksense-task-run-history-api/) — The task run history API from Qlik Sense — 3 operation(s) for task run history.
- [Qlik Sense Temporary contents API](https://apis.io/apis/qliksense/qliksense-temporary-contents-api/) — The Temporary contents API from Qlik Sense — 5 operation(s) for temporary contents.
- [Qlik Sense tenant key migration information API](https://apis.io/apis/qliksense/qliksense-tenant-key-migration-information-api/) — The tenant key migration information API from Qlik Sense — 1 operation(s) for tenant key migration information.
- [Qlik Sense tenant key provider management API](https://apis.io/apis/qliksense/qliksense-tenant-key-provider-management-api/) — The tenant key provider management API from Qlik Sense — 3 operation(s) for tenant key provider management.
- [Qlik Sense tenant key provider operations API](https://apis.io/apis/qliksense/qliksense-tenant-key-provider-operations-api/) — The tenant key provider operations API from Qlik Sense — 3 operation(s) for tenant key provider operations.
- [Qlik Sense Tenant Settings API](https://apis.io/apis/qliksense/qliksense-tenant-settings-api/) — The tenant-settings API from Qlik Sense — 4 operation(s) for tenant-settings.
- [Qlik Sense Tenants API](https://apis.io/apis/qliksense/qliksense-tenants-api/) — The tenants API from Qlik Sense — 5 operation(s) for tenants.
- [Qlik Sense Terms API](https://apis.io/apis/qliksense/qliksense-terms-api/) — The terms API from Qlik Sense — 4 operation(s) for terms.
- [Qlik Sense Themes API](https://apis.io/apis/qliksense/qliksense-themes-api/) — The themes API from Qlik Sense — 4 operation(s) for themes.
- [Qlik Sense Threads API](https://apis.io/apis/qliksense/qliksense-threads-api/) — The threads API from Qlik Sense — 7 operation(s) for threads.
- [Qlik Sense Tokens API](https://apis.io/apis/qliksense/qliksense-tokens-api/) — The tokens API from Qlik Sense — 1 operation(s) for tokens.
- [Qlik Sense Trust Score Result API](https://apis.io/apis/qliksense/qliksense-trust-score-result-api/) — The trust-score-result API from Qlik Sense — 1 operation(s) for trust-score-result.
- [Qlik Sense Users API](https://apis.io/apis/qliksense/qliksense-users-api/) — The users API from Qlik Sense — 5 operation(s) for users.
- [Qlik Sense Web Integrations API](https://apis.io/apis/qliksense/qliksense-web-integrations-api/) — The web-integrations API from Qlik Sense — 2 operation(s) for web-integrations.
- [Qlik Sense Web Notifications API](https://apis.io/apis/qliksense/qliksense-web-notifications-api/) — The web-notifications API from Qlik Sense — 3 operation(s) for web-notifications.
- [Qlik Sense Webhooks API](https://apis.io/apis/qliksense/qliksense-webhooks-api/) — The webhooks API from Qlik Sense — 3 operation(s) for webhooks.
- [Qlik Sense Dataset API](https://apis.io/apis/qliksense/qliksense-dataset-api/) — The Dataset API from Qlik Sense — 2 operation(s) for dataset.
- [Qlik Sense Datastore API](https://apis.io/apis/qliksense/qliksense-datastore-api/) — The Datastore API from Qlik Sense — 4 operation(s) for datastore.
- [Qlik Sense Knowledge Bases API](https://apis.io/apis/qliksense/qliksense-knowledge-bases-api/) — The Knowledge Bases API from Qlik Sense — 11 operation(s) for knowledge bases.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (2)

Event-driven and webhook contracts.

- [Qliksense Asyncapi Index](https://apis.io/asyncapis/qliksense/qliksense-asyncapi-index/)
- [Qliksense Webhooks](https://apis.io/asyncapis/qliksense/qliksense-webhooks/)

#### Event channels (30)

Individual events and webhooks the provider emits.

- [system-events.api-keys](https://apis.io/channels/qliksense/api-keys-configs-system-events-api-keys/)
- [system-events.groups](https://apis.io/channels/qliksense/groups-system-events-groups/)
- [system-events.spaces](https://apis.io/channels/qliksense/spaces-system-events-spaces/)
- [system-events.ai.mcp](https://apis.io/channels/qliksense/system-events-ai-mcp/)
- [system-events.alerting](https://apis.io/channels/qliksense/system-events-alerting/)
- [system-events.api-keys](https://apis.io/channels/qliksense/system-events-api-keys/)
- [system-events.app](https://apis.io/channels/qliksense/system-events-app/)
- [system-events.app-usage](https://apis.io/channels/qliksense/system-events-app-usage/)
- [system-events.automation](https://apis.io/channels/qliksense/system-events-automation/)
- [system-events.di-projects.di-tasks](https://apis.io/channels/qliksense/system-events-di-projects-di-tasks/)
- [system-events.engine.app](https://apis.io/channels/qliksense/system-events-engine-app/)
- [system-events.groups](https://apis.io/channels/qliksense/system-events-groups/)
- [system-events.hub-dashboards](https://apis.io/channels/qliksense/system-events-hub-dashboards/)
- [system-events.ip-policy](https://apis.io/channels/qliksense/system-events-ip-policy/)
- [system-events.licenses](https://apis.io/channels/qliksense/system-events-licenses/)
- [system-events.notification-digest](https://apis.io/channels/qliksense/system-events-notification-digest/)
- [system-events.oauth-clients](https://apis.io/channels/qliksense/system-events-oauth-clients/)
- [system-events.oauth-tokens](https://apis.io/channels/qliksense/system-events-oauth-tokens/)
- [system-events.quota](https://apis.io/channels/qliksense/system-events-quota/)
- [system-events.rate-limit](https://apis.io/channels/qliksense/system-events-rate-limit/)
- [system-events.reload](https://apis.io/channels/qliksense/system-events-reload/)
- [system-events.roles](https://apis.io/channels/qliksense/system-events-roles/)
- [system-events.sharing](https://apis.io/channels/qliksense/system-events-sharing/)
- [system-events.spaces](https://apis.io/channels/qliksense/system-events-spaces/)
- [system-events.task](https://apis.io/channels/qliksense/system-events-task/)
- …and 5 more published on APIs.io

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [Qlik MCP Server](https://apis.io/servers/qliksense/qlik-mcp-server/)

#### JSON Schema (39)

The data models the API reads and writes.

- [New Task Defaults Configuration](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.schema/)
- [Common Task Settings Definitions](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.common.schema/)
- [Defaults for new Datamart Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.datamart.schema/)
- [Defaults for new File Based Knowledge Mart Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.filebasedknowledgemart.schema/)
- [Defaults for new Knowledge Mart Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.knowledgemart.schema/)
- [Defaults for new Lakehouse Storage Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.lakehousestorage.schema/)
- [Defaults for new Lake Landing Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.lakelanding.schema/)
- [Defaults for new Landing Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.landing.schema/)
- [Defaults for new QVD Storage Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.qvdstorage.schema/)
- [Defaults for new Registered Data Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.registereddata.schema/)
- [Defaults for new Replicate Landing Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.replicatelanding.schema/)
- [Defaults for new Storage Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.storage.schema/)
- [Defaults for new Streaming Lake Landing Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.streaminglakelanding.schema/)
- [Defaults for new Streaming Transform Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.streamingtransform.schema/)
- [Defaults for new Transform Task](https://apis.io/schemas/qliksense/qliksense-qtcp-newtaskdefaults.settings.transform.schema/)
- [Project Configuration](https://apis.io/schemas/qliksense/qliksense-qtcp-project.schema/)
- [Task Dataset Configuration](https://apis.io/schemas/qliksense/qliksense-qtcp-task.dataset.schema/)
- [Task Model Configuration](https://apis.io/schemas/qliksense/qliksense-qtcp-task.model.schema/)
- [Task Schedule Configuration](https://apis.io/schemas/qliksense/qliksense-qtcp-task.schedule.schema/)
- [Task Configuration](https://apis.io/schemas/qliksense/qliksense-qtcp-task.schema/)
- [Common Task Settings Definitions](https://apis.io/schemas/qliksense/qliksense-qtcp-task.settings.common.schema/)
- [Datamart Task Settings](https://apis.io/schemas/qliksense/qliksense-qtcp-task.settings.datamart.schema/)
- [File Based Knowledge Mart Task Settings](https://apis.io/schemas/qliksense/qliksense-qtcp-task.settings.filebasedknowledgemart.schema/)
- [Knowledge Mart Task Settings](https://apis.io/schemas/qliksense/qliksense-qtcp-task.settings.knowledgemart.schema/)
- [Lakehouse Mirror Task Settings](https://apis.io/schemas/qliksense/qliksense-qtcp-task.settings.lakehousemirror.schema/)
- …and 14 more published on APIs.io

#### Overlays (204)

OpenAPI overlays, including conversational phrasing for each operation.

- [Qliksense Alerting Actions Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-alerting-actions-api-phrasing-overlay/)
- [Qliksense Alerting Settings Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-alerting-settings-api-phrasing-overlay/)
- [Qliksense Alerting Tasks Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-alerting-tasks-api-phrasing-overlay/)
- [Qliksense Alerting Tasks Executions Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-alerting-tasks-executions-api-phrasing-overlay/)
- [Qliksense Aliases Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-aliases-api-phrasing-overlay/)
- [Qliksense Analytics Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-api-phrasing-overlay/)
- [Qliksense Analytics Apps Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-apps-overlay/)
- [Qliksense Analytics Change Stores Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-change-stores-overlay/)
- [Qliksense Analytics Discovery Agent Adaptive Cards Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-discovery-agent-adaptive-cards-overlay/)
- [Qliksense Analytics Odag Apps Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-odag-apps-overlay/)
- [Qliksense Analytics Odag Links Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-odag-links-overlay/)
- [Qliksense Analytics Odag Requests Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-odag-requests-overlay/)
- [Qliksense Analytics Odag Settings Overlay](https://apis.io/overlays/qliksense/qliksense-analytics-odag-settings-overlay/)
- [Qliksense Api Keys Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-api-keys-api-phrasing-overlay/)
- [Qliksense Api Keys Configurations Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-api-keys-configurations-api-phrasing-overlay/)
- [Qliksense Api Keys Overlay](https://apis.io/overlays/qliksense/qliksense-api-keys-overlay/)
- [Qliksense Api Settings Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-api-settings-api-phrasing-overlay/)
- [Qliksense Apps Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-apps-api-phrasing-overlay/)
- [Qliksense Apps Overlay](https://apis.io/overlays/qliksense/qliksense-apps-overlay/)
- [Qliksense Assignments Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-assignments-api-phrasing-overlay/)
- [Qliksense Assistants Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-assistants-api-phrasing-overlay/)
- [Qliksense Assistants Overlay](https://apis.io/overlays/qliksense/qliksense-assistants-overlay/)
- [Qliksense Async Actions Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-async-actions-api-phrasing-overlay/)
- [Qliksense Audits Api Phrasing Overlay](https://apis.io/overlays/qliksense/qliksense-audits-api-phrasing-overlay/)
- [Qliksense Audits Overlay](https://apis.io/overlays/qliksense/qliksense-audits-overlay/)
- …and 179 more published on APIs.io

#### Security (4)

Authentication, trust centre, and vulnerability disclosure.

- [Qliksense Authentication](https://apis.io/security/qliksense/qliksense-authentication/)
- [Qliksense Domain Security](https://apis.io/security/qliksense/qliksense-domain-security/)
- [Qliksense Trust Center](https://apis.io/security/qliksense/qliksense-trust-center/)
- [Qliksense Vulnerability Disclosure](https://apis.io/security/qliksense/qliksense-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Qliksense Scopes](https://apis.io/scopes/qliksense/qliksense-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Qliksense Plans Pricing](https://apis.io/plans/qliksense/qliksense-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Qliksense Rate Limits](https://apis.io/rate-limits/qliksense/qliksense-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Qliksense Finops](https://apis.io/finops/qliksense/qliksense-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.qlik.com/us/products/qlik-sense)
- [Documentation](https://qlik.dev/apis/)
- [Getting started](https://qlik.dev/manage/get-started-first-api-call/)
- [API reference](https://qlik.dev/apis/rest/)
- [Pricing](https://www.qlik.com/us/pricing)
- [Sign up](https://www.qlik.com/us/trial/qlik-cloud-analytics)
- [Support](https://support.qlik.com/)
- [Changelog](https://qlik.dev/changelog/)
- [Blog](https://www.qlik.com/us/blog)
- [Terms of service](https://www.qlik.com/us/legal/terms-of-use)
- [Privacy policy](https://www.qlik.com/us/privacy)
- [GitHub](https://github.com/qlik-oss)
- [Status](https://status.qlikcloud.com/)

## API Evangelist rating

**Kin Score 71.0** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 58.3 |
| Contract quality | 51.6 |
| Contract governance | 4.5 |
| Operational transparency | 84.2 |
| Developer ergonomics | 78.6 |
| Access clarity | 92.1 |

**Agent readiness 42.9** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | documented (partial credit) |
| MCP Server | templated |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | — |

**Regulatory alignment 41.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/qliksense/](https://apis.io/providers/qliksense/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Qlik Sense: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/qliksense/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
