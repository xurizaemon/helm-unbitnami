# 🧭 Awesome Alternatives to Bitnami Helm Charts

> **Context:** Following the **Bitnami Secure Images** transition (Aug 28, 2025), many Bitnami charts will be limited to the `latest` tag and/or moved to `bitnamilegacy`. This table lists **upstream- and vendor‑maintained alternatives** with Artifact Hub links and **stats**.

> 🙌 **Open contributions:** Everyone can propose charts that aren’t listed yet, and any help to reduce reliance on Bitnami’s *"supra‑governance"* is welcome. Add your entries via PR!

---

### Column legend

* **Type**: `Chart` (Helm chart) or `Operator` (operator + CRDs).
* **AH**: Artifact Hub link.
* **Stats (AH)**: `⭐` stars · `✅` Verified Publisher · `🏷️` Official.

> ⚠️ **Note:** Stats are updated automatically. Until the badge is enabled, the column shows `—`.

---

## 📚 Alternatives table

<!-- ah-stats:start -->

| Category          | Bitnami Chart                  | Alternative (name)                        | Publisher            | Type     | AH                                                                                                                                                                         | Stats (AH) | Notes                                                          |
| ----------------- | ------------------------------ | ----------------------------------------- | -------------------- | -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------------- |
| Artifact Registry | `harbor`                       | **Harbor**                                | CNCF Harbor          | Chart    | [https://artifacthub.io/packages/helm/harbor/harbor](https://artifacthub.io/packages/helm/harbor/harbor)                                                                   | —          | Registry + chart repo (OCI/ChartMuseum).                       |
| Certificates/TLS  | `cert-manager`                 | **cert-manager**                          | Jetstack             | Chart    | [https://artifacthub.io/packages/helm/cert-manager/cert-manager](https://artifacthub.io/packages/helm/cert-manager/cert-manager)                                           | —          | Certificates (ACME, Vault, Venafi…).                           |
| Ingress           | `nginx-ingress-controller`     | **ingress-nginx**                         | Kubernetes           | Chart    | [https://artifacthub.io/packages/helm/ingress-nginx/ingress-nginx](https://artifacthub.io/packages/helm/ingress-nginx/ingress-nginx)                                       | —          | Official Kubernetes ingress‑nginx chart.                       |
| Ingress           | `nginx`                        | **NGINX Ingress (F5 NGINX)**              | NGINX                | Chart    | [https://artifacthub.io/packages/helm/nginx/nginx-ingress](https://artifacthub.io/packages/helm/nginx/nginx-ingress)                                                       | —          | Vendor variant (commercial options).                           |
| Kafka             | `kafka`                        | **Strimzi Kafka Operator**                | Strimzi              | Operator | [https://artifacthub.io/packages/helm/strimzi/strimzi-kafka-operator](https://artifacthub.io/packages/helm/strimzi/strimzi-kafka-operator)                                 | —          | CNCF ecosystem project.                                        |
| MySQL             | `mysql`                        | **MySQL Operator**                        | Oracle               | Operator | [https://artifacthub.io/packages/helm/mysql-operator/mysql-operator](https://artifacthub.io/packages/helm/mysql-operator/mysql-operator)                                   | —          | Oracle MySQL InnoDB Cluster operator.                          |
| MySQL             | `mysql`                        | **Percona XtraDB Cluster (PXC) Operator** | Percona              | Operator | [https://artifacthub.io/packages/helm/percona/pxc-operator](https://artifacthub.io/packages/helm/percona/pxc-operator)                                                     | —          | MySQL HA via Galera.                                           |
| NATS              | `nats`                         | **NATS (official chart)**                 | NATS                 | Chart    | [https://artifacthub.io/packages/helm/nats/nats](https://artifacthub.io/packages/helm/nats/nats)                                                                           | —          | JetStream/Controller available.                                |
| Object Storage    | `minio`                        | **MinIO (official chart)**                | MinIO                | Chart    | [https://artifacthub.io/packages/helm/minio/minio](https://artifacthub.io/packages/helm/minio/minio)                                                                       | —          | S3 on‑prem; operator available.                                |
| Observability     | `kube-prometheus`              | **kube-prometheus-stack**                 | prometheus-community | Chart    | [https://artifacthub.io/packages/helm/prometheus-community/kube-prometheus-stack](https://artifacthub.io/packages/helm/prometheus-community/kube-prometheus-stack)         | —          | Prometheus Operator + Grafana.                                 |
| Observability     | `prometheus`                   | **prometheus**                            | prometheus-community | Chart    | [https://artifacthub.io/packages/helm/prometheus-community/prometheus](https://artifacthub.io/packages/helm/prometheus-community/prometheus)                               | —          | Standalone Prometheus.                                         |
| PostgreSQL        | `postgresql`                   | **Percona PG Operator**                   | Percona              | Operator | [https://artifacthub.io/packages/olm/community-operators/percona-postgresql-operator](https://artifacthub.io/packages/olm/community-operators/percona-postgresql-operator) | —          | Percona flavor (operator + CRDs).                              |
| PostgreSQL        | `postgresql`                   | **PGO – Postgres Operator**               | Crunchy Data         | Operator | [https://artifacthub.io/packages/olm/community-operators/postgresql](https://artifacthub.io/packages/olm/community-operators/postgresql)                                   | —          | Crunchy’s PGO operator.                                        |
| PostgreSQL        | `postgresql` / `postgresql-ha` | **CloudNativePG**                         | CloudNativePG        | Operator | [https://artifacthub.io/packages/helm/cloudnative-pg/cloudnative-pg](https://artifacthub.io/packages/helm/cloudnative-pg/cloudnative-pg)                                   | —          | CNPG operator recommended for prod; `cluster` chart available. |
| RabbitMQ          | `rabbitmq`                     | **RabbitMQ Cluster Operator**             | RabbitMQ             | Operator | [https://artifacthub.io/packages/olm/community-operators/rabbitmq-cluster-operator](https://artifacthub.io/packages/olm/community-operators/rabbitmq-cluster-operator)     | —          | Official operator (Broadcom/RabbitMQ).                         |
| Redis             | `redis`                        | **Redis Operator (Spotahome)**            | Spotahome            | Operator | [https://artifacthub.io/packages/helm/redis-operator/redis-operator](https://artifacthub.io/packages/helm/redis-operator/redis-operator)                                   | —          | Popular historical alternative.                                |
| Redis             | `redis` / `redis-cluster`      | **Redis Operator (OT-ContainerKit)**      | OpsTree              | Operator | [https://artifacthub.io/packages/helm/ot-container-kit/redis-operator](https://artifacthub.io/packages/helm/ot-container-kit/redis-operator)                               | —          | Operator + `redis` / `redis-cluster` charts.                   |
| Search            | `elasticsearch`                | **Elasticsearch (Elastic)**               | Elastic              | Chart    | [https://artifacthub.io/packages/helm/elastic/elasticsearch](https://artifacthub.io/packages/helm/elastic/elasticsearch)                                                   | —          | Community‑maintained charts; Elastic recommends ECK.           |
| Search            | `elasticsearch`                | **OpenSearch**                            | OpenSearch           | Chart    | [https://artifacthub.io/packages/helm/opensearch-project-helm-charts/opensearch](https://artifacthub.io/packages/helm/opensearch-project-helm-charts/opensearch)           | —          | OSS alternative to Elasticsearch.                              |
| Storage           | `rook-ceph`                    | **Rook Ceph**                             | Rook                 | Chart    | [https://artifacthub.io/packages/helm/rook/rook-ceph](https://artifacthub.io/packages/helm/rook/rook-ceph)                                                                 | —          | Ceph storage operator (CNCF).                                  |

<!-- ah-stats:end -->

> 💡 **Tip:** When migrating away from Bitnami, prefer **operators** for data and messaging systems (CRDs, Day‑2 ops, upgrades). Keep **charts** for stateless components.

---

## ✅ How to contribute

* Add a row to the table above (keep alphabetical ordering by **Category**).
* Provide an **Artifact Hub** link to the upstream package (official publisher when possible).
* If you propose an **operator**, mention if a helper/cluster chart exists.
* Open a PR with a short **rationale** (why this alternative is compelling post‑Bitnami).

---

## 🛠️ TODO (repo roadmap)

* [ ] **Stats (Artifact Hub):** fetch `stars`, `verified_publisher`, `official` via `GET /api/v1/packages/helm/{repo}/{name}` and update **Stats (AH)** between `<!-- ah-stats:start -->` / `<!-- ah-stats:end -->`.
* [ ] **Submission validation**
* [ ] **GitHub templates:**

  * [ ] `ISSUE_TEMPLATE/new-alternative.yml` (new chart), `ISSUE_TEMPLATE/update.yml` (update), `ISSUE_TEMPLATE/migration-guide.yml` (guide request).
  * [ ] `PULL_REQUEST_TEMPLATE.md` (checklist: schema ok, AH link ok, rationale provided).
* [ ] **Migration docs** (hands‑on guides):

  * [ ] *Bitnami PostgreSQL* ➜ **CloudNativePG** (values → `Cluster` CR, backups, `wal-archive`, probes, PDB, affinities, TLS, secrets).
  * [ ] *Bitnami PostgreSQL* ➜ **Crunchy PGO** (`PostgresCluster` CR, backup/restore, replication, controlled upgrades).
  * [ ] *Bitnami Redis* ➜ **OT‑ContainerKit Redis Operator** (standalone/cluster/sentinel modes, data migration).
  * [ ] *Bitnami Kafka* ➜ **Strimzi** (Topic/User CRs, storage, listeners, auth, upgrades).
* [ ] **Auto‑render table** from `catalog/entries.yaml` (script `tools/render_table.py`) to prevent drift.
* [ ] **Security policy** docs (digest pinning, PSS/PSP, NetworkPolicies, signed images, SBOM).
* [ ] **CODEOWNERS** and light **governance** (reviewer rotation by category).
* [ ] **License** (e.g., MIT) + **Code of Conduct** (Contributor Covenant).

---

### 💬 Future ideas

* Custom *shields.io* badges (JSON endpoint produced by CI) for ⭐/✅/🏷️.
* Preflight scripts (CRD lint, k8s version compat, images pinned by digest).
* Kubernetes support matrix (k8s versions validated by each alternative).

> **PS:** If an alternative is missing, open an issue ✍️ we’ll help qualify it and craft a migration guide.
