# Ray (ray)

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

Ray is an open-source unified compute framework, stewarded by Anyscale, that scales Python and AI workloads from a laptop to a cluster. It consists of Ray Core (a distributed runtime) and a set of AI libraries (Ray Train, Ray Data, Ray Tune, Ray Serve, RLlib) for training, batch inference, hyperparameter search, and model serving. Ray clusters expose a Dashboard and Jobs REST API on the head node (default port 8265) for submitting jobs, inspecting actors and tasks, and serving deployed applications via Ray Serve HTTP endpoints.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ray/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ray/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Distributed Computing
- Machine Learning
- AI Infrastructure
- Python
- Model Serving
- Open Source
- Compute

## Timestamps

- **Created:** 2026-05-11
- **Modified:** 2026-05-11

## APIs

### Ray Jobs REST API

REST API on the Ray head node for submitting, listing, inspecting, and stopping Ray jobs, plus streaming logs. Default base URL is http://<head-node>:8265/api/jobs/. Open-source clusters are typically unauthenticated; production deployments rely on network controls or Anyscale-managed authentication.

- **Human URL:** [https://docs.ray.io/en/latest/cluster/running-applications/job-submission/rest.html](https://docs.ray.io/en/latest/cluster/running-applications/job-submission/rest.html)
- **Base URL:** `http://127.0.0.1:8265/api`

#### Tags

- Jobs
- Cluster
- Submission
- Logs

#### Properties

- [Documentation](https://docs.ray.io/en/latest/cluster/running-applications/job-submission/rest.html)
- [Python  S D K](https://docs.ray.io/en/latest/cluster/running-applications/job-submission/sdk.html)
- [C L I](https://docs.ray.io/en/latest/cluster/running-applications/job-submission/cli.html)
- [Postman Collection](collections/ray.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ray.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ray Dashboard API

Internal REST API powering the Ray Dashboard, exposing endpoints for nodes, actors, tasks, placement groups, runtime environments, and cluster events. Same base URL as the Jobs API (http://<head>:8265).

- **Human URL:** [https://docs.ray.io/en/latest/ray-observability/getting-started.html](https://docs.ray.io/en/latest/ray-observability/getting-started.html)
- **Base URL:** `http://127.0.0.1:8265/api`

#### Tags

- Observability
- Dashboard
- Cluster State
- Actors

#### Properties

- [Documentation](https://docs.ray.io/en/latest/ray-observability/getting-started.html)
- [Postman Collection](collections/ray.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ray.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Ray Serve HTTP API

HTTP interface for invoking models and applications deployed via Ray Serve. Each deployed application is exposed as an HTTP endpoint on the Serve HTTP proxy (default port 8000); authentication and routing are configured per deployment.

- **Human URL:** [https://docs.ray.io/en/latest/serve/index.html](https://docs.ray.io/en/latest/serve/index.html)
- **Base URL:** `http://127.0.0.1:8000`

#### Tags

- Model Serving
- Inference
- HTTP

#### Properties

- [Documentation](https://docs.ray.io/en/latest/serve/index.html)
- [Production  Guide](https://docs.ray.io/en/latest/serve/production-guide/index.html)
- [Postman Collection](collections/ray.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ray.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.ray.io)
- [Documentation](https://docs.ray.io)
- [GitHub Repository](https://github.com/ray-project/ray)
- [GitHub Organization](https://github.com/ray-project)
- [Anyscale](https://www.anyscale.com)
- [Slack](https://www.ray.io/community)
- [Forum](https://discuss.ray.io)
- [Blog](https://www.anyscale.com/blog)
- [Issues](https://github.com/ray-project/ray/issues)
- [License](https://github.com/ray-project/ray/blob/master/LICENSE)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
