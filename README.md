# coroot-grafana-dashboards
coroot-grafana-dashboards
1. Create VMrule based on .yaml file (or prometheus recording rule)
2. Import dashbords to your grafana and integrate it with your prometheus datasource
3. Use!
![2025-03-0814 32 57-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/74e2b93e-39cd-46a1-91ac-b637757f569c)

# Requirements:
1. Coroot node agents (just it, without UI, Clickhouse, etc.) https://github.com/coroot/coroot
2. Prometheus or analog (VictoriaMetrics in my case) 
3. RecordingRules functionality https://prometheus.io/docs/prometheus/latest/configuration/recording_rules/
4. Grafana
5. Eyes, hands and love to observability.
6. Also I use typical container metrics from kube-state-metrics or cadvisor in my boards, but you can use it without it.

# Current features:
1. Base drilldown from overall view to namespace/service board.
2. All tcp metrics and connections with fqdn and directions
3. HTTP metrics also added
4. Postgres and Kafka in beta testing
5. Also add throttling for better RCA


# Roadmap:
1. Add errors on conntions everywhere
2. Redis and other statefulls
3. Insatnce (Nodes) based graphs
4. Statefuls in graph
5. Error timeline fixes
6. PSI metrics integration
