# Prometheus

> [Docker Compose file](../stacks/monitoring.yaml)

This is the metrics database I use. Together with Prometheus, I use [Grafana](grafana.md) for visualisation of metrics.

I use various exporters:
- Node exporter for system metrics.
- Cadvisor for Docker container metrics.
- Forge Prometheus Exporter by cpburnz for Minecraft Forge server metrics. This is a Forge mod that is very easy to work with.
