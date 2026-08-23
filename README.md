# Helm Examples

A gallery of Helm chart examples covering observability (Prometheus, Grafana,
Loki), service mesh (Istio), load balancing (MetalLB), and application stacks
(WordPress, Argo CD).

## What's inside

- `Prometheus` — Prometheus Helm chart setup.
- `Grafana` — Grafana dashboarding with Helm.
- `Loki` — Loki log aggregation with Helm.
- `Istio` — Istio control-plane charts.
- `MetalLB` — MetalLB load-balancer integration.
- `WordPress` — WordPress + Helm values.
- `ArgoCD` — Argo CD via Helm.
- `ASimpleAppWithDependencies` — an app that depends on other charts.
- `START-HERE.txt` — a suggested starting order.

## What you'll learn

- Installing common observability stacks with Helm.
- Managing chart values and overrides.
- Deploying application stacks and their dependencies.

## Tools covered

- Helm 3 (charts, values, templating)
- Prometheus / Grafana / Loki / Istio / MetalLB

## How to use

Start with `START-HERE.txt`, then explore each directory for its chart and values.
A typical install looks like:

```bash
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm install my-prometheus prometheus-community/kube-prometheus-stack \
  --namespace monitoring --create-namespace
```

## Related

- Helm docs: https://helm.sh/docs/
