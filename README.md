# ACM Grafana Networking Dashboards

Custom Grafana dashboards for Red Hat Advanced Cluster Management Observability.

## Dashboards

- Networking / Infrastructure
- Networking / Ingress
- Networking / Linux Subsystem Stats

## Target environment

- Red Hat Advanced Cluster Management 2.15
- OpenShift Container Platform 4.20
- ACM Observability with Grafana developer instance
- Managed cluster label filtering using ACM variables:
  - datasource
  - acm_label_names
  - value
  - cluster

## Notes

The dashboard PromQL queries use a 10m rate window where applicable to work better with ACM Observability metric forwarding intervals.

Apply one of the dashboard YAML files with:

```bash
oc apply -f <dashboard-yaml>

