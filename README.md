# coroot-grafana-dashboards

![License](https://img.shields.io/github/license/kirillyu/coroot-grafana-dashboards)
![Release](https://img.shields.io/github/v/release/kirillyu/coroot-grafana-dashboards?include_prereleases)
![Stars](https://img.shields.io/github/stars/kirillyu/coroot-grafana-dashboards?style=social)

A collection of Grafana dashboards based on Coroot node agents and Prometheus-compatible data sources.  
Focus on observability with simple deployment — no UI, no ClickHouse, only metrics.

---

## How to start

1. Create **VMRule** based on the `VMRule.yaml` (or use as Prometheus recording rules).
2. Import the dashboards into your Grafana.
3. Set up your Prometheus (or VictoriaMetrics) as the data source.
4. Use and enjoy.

👉 [Demo (YouTube)](https://www.youtube.com/watch?v=e5C6f9aSWSM)

---

## Requirements

1. [Coroot Node Agents](https://github.com/coroot/coroot) (no UI, no ClickHouse, only node agents).
2. Prometheus or any compatible system (VictoriaMetrics recommended).
3. Recording rules support ([documentation](https://prometheus.io/docs/prometheus/latest/configuration/recording_rules/)).
4. Grafana.
5. Eyes, hands, and care for observability.
6. Optionally: kube-state-metrics and cAdvisor for extended container metrics.

---

## Current features

- Drilldown: from an overview to namespace/service level.
- TCP metrics and full connection details including FQDN and traffic direction.
- HTTP metrics: errors, latencies, and traffic.
- Postgres and Kafka metrics (beta).
- CPU throttling metrics for better root cause analysis (RCA).
- IN/OUT separation: errors and latencies by traffic direction.

---

## Roadmap

- [x] Add error metrics for TCP connections.
- [x] Redis and other stateful workloads.
- [ ] Instance/node-level dashboards.
- [x] Visual graph support for stateful workloads.
- [ ] Error timeline improvements.
- [ ] PSI (Pressure Stall Information) metrics integration.

---

> Minimalistic setup: only agents and metrics. No ClickHouse. No heavy backend.
