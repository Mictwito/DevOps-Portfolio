# Monitoring – Prometheus & Grafana (Helm)

## Overview
Installs Prometheus + Grafana via Helm chart.

## Steps
1. Add repo:  
   `helm repo add prometheus-community https://prometheus-community.github.io/helm-charts`
2. Install:  
   `helm install kube-prom prometheus-community/kube-prometheus-stack -n monitoring --create-namespace`
3. Port-forward Grafana:  
   `kubectl port-forward svc/kube-prom-grafana 3000:80 -n monitoring`

## Notes
- Default Grafana login: `admin / prom-operator`
- Dashboards saved under `/var/lib/grafana/dashboards`
