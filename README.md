# Ray (ray)

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
