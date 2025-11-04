# Kubernetes – Guestbook App

## Overview
Frontend + backend example deployed with Deployments and Services.

## Manifests
- `deploy-frontend.yaml`
- `deploy-backend.yaml`
- `svc-frontend.yaml` (NodePort/LoadBalancer)
- `svc-backend.yaml` (ClusterIP)

## Notes
- Config via `ConfigMap`, secrets via `Secret`.
- Health checks: `readinessProbe` / `livenessProbe`.
