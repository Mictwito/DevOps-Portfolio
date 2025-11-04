# Jenkins – Auto Deploy Job

## Overview
Pipeline that builds and deploys a static web/app to target servers over SSH.

## Steps
1. Create credentials in Jenkins (SSH/key or username+password).
2. Configure job (pipeline from SCM or Jenkinsfile).
3. Trigger on push (webhook) or manual run.

## Key Files
- `Jenkinsfile` – stages: checkout → build → deploy.
- `deploy.sh` (optional) – rsync/scp + service restart.

## Security
- Use Jenkins Credentials Binding; never hardcode secrets.

## Interview Q&A
**Q:** How do you secure secrets in Jenkins?
**A:** Credentials store + masking + least privilege on jobs.
