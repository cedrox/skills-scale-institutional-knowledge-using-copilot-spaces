# Release Checklist

Purpose: Actionable checklist to ensure releases are safe, coordinated, and well-communicated. Covers pre-release, deployment, and post-release steps with explicit role responsibilities.

Reference: [docs/octoacme-release-and-deployment.md](octoacme-release-and-deployment.md)

---

## Pre-Release

### Code & Quality (Developers / QA)
- [ ] All planned PRs merged and acceptance criteria met
- [ ] CI green: tests and security scans passing
- [ ] QA sign-off on feature acceptance

### Release Preparation (Release Engineer)
- [ ] Release branch/tag created and pipeline validated
- [ ] Release notes drafted and reviewed (PM / PdM / Technical Lead)
- [ ] Staging deployment completed and smoke tests passed
- [ ] Rollback plan documented and rehearsed if needed

### Infrastructure & Monitoring (DevOps Engineer)
- [ ] Infrastructure and environment readiness confirmed
- [ ] Monitoring, alerting, and dashboards verified
- [ ] Capacity and scaling checked for expected load

### Support Readiness (Customer Support Lead)
- [ ] Support runbook and FAQs updated for this release
- [ ] Escalation path and on-call contacts confirmed
- [ ] Support team briefed on known issues and notable changes

### Stakeholder Notification (PM)
- [ ] Stakeholders notified of planned release window
- [ ] External communications or announcements prepared (if applicable)

---

## Deployment

- [ ] Backup or snapshot taken (if applicable)
- [ ] Staging smoke tests confirmed passing (Release Engineer)
- [ ] Production deployment triggered by Release Engineer
- [ ] DevOps Engineer monitors health metrics and alerts during rollout
- [ ] Post-deploy smoke and sanity checks completed

> If a critical issue is detected: trigger incident response, notify on-call (DevOps), and initiate rollback if needed. See [docs/octoacme-release-and-deployment.md](octoacme-release-and-deployment.md) for rollback playbook.

---

## Post-Release

- [ ] Rollout success confirmed; release notes updated with outcomes (Release Engineer / PM)
- [ ] Customer Support Lead confirms support readiness and escalation path active
- [ ] Open post-release action items logged and owners assigned (PM / Scrum Master)
- [ ] Documentation and runbooks updated if issues were found
- [ ] Retrospective scheduled for non-trivial releases (PM / Scrum Master)

---

## Role Highlights

| Role | Responsibility |
|---|---|
| Release Engineer | Pipeline, release orchestration, tagging, release notes, rollback |
| DevOps Engineer | Infrastructure, monitoring, rollback mechanisms |
| Customer Support Lead | Support runbook, FAQ, customer communications, escalation |
| QA | Acceptance sign-off, smoke tests |
| PM / PdM | Stakeholder notifications, acceptance of release outcomes |
| Scrum Master | Coordinates post-release retrospective, tracks action items |
