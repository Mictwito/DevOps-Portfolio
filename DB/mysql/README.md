# MySQL on Kubernetes (PVC + Secret)

## Overview
Persistent MySQL using PVC and a Secret for credentials.

## YAML (snippet)
apiVersion: v1
kind: Secret
metadata:
  name: mysql-secret
type: Opaque
stringData:
  MYSQL_ROOT_PASSWORD: change-me
---
apiVersion: v1
kind: PersistentVolumeClaim
metadata:
  name: mysql-pvc
spec:
  accessModes: ["ReadWriteOnce"]
  resources:
    requests:
      storage: 10Gi
---
apiVersion: apps/v1
kind: Deployment
metadata:
  name: mysql
spec:
  selector: { matchLabels: { app: mysql } }
  template:
    metadata: { labels: { app: mysql } }
    spec:
      containers:
      - name: mysql
        image: mysql:8
        envFrom:
        - secretRef: { name: mysql-secret }
        volumeMounts:
        - name: data
          mountPath: /var/lib/mysql
      volumes:
      - name: data
        persistentVolumeClaim: { claimName: mysql-pvc }

## Security
- Do not commit Secrets to Git.
- Use environment variables or Vault integration.
