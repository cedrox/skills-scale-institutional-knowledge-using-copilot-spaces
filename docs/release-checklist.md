# Release Checklist

Use this checklist for every production release. Work through each section in order, obtaining sign-off where indicated. Roles are called out explicitly so owners are clear.

See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for full role definitions and [octoacme-release-and-deployment.md](octoacme-release-and-deployment.md) for release type guidance.

---

## 1. Pre-Release Readiness (PM + Release Engineer + QA)

- [ ] Release scope finalized and communicated to all stakeholders (PM)
- [ ] All feature PRs merged to the release branch (Developers)
- [ ] All acceptance criteria met and verified (QA)
- [ ] All automated tests passing in CI — no open critical failures (Release Engineer)
- [ ] Security scans completed with no unresolved high/critical findings (DevOps Engineer)
- [ ] Release notes drafted and reviewed (Release Engineer + PM)
- [ ] Rollback plan documented and accessible to on-call team (Release Engineer + DevOps Engineer)
- [ ] Runbooks updated to reflect any new operational steps (DevOps Engineer)

## 2. Pipeline Validation (Release Engineer + DevOps Engineer)

- [ ] CI/CD pipeline configuration reviewed for this release (Release Engineer)
- [ ] Feature flags and environment variables verified for staging and production (DevOps Engineer)
- [ ] Staging environment matches production configuration (DevOps Engineer)
- [ ] Build artifact integrity verified (checksums or equivalent) (Release Engineer)
- [ ] Infrastructure capacity and scaling reviewed for expected traffic (DevOps Engineer)
- [ ] Monitoring and alerting thresholds reviewed and active (DevOps Engineer)

## 3. Staging Deployment & Smoke Tests (Release Engineer + QA)

- [ ] Deployed to staging environment without errors (Release Engineer)
- [ ] Smoke tests executed against staging (QA)
- [ ] Critical user flows validated manually where automation does not cover (QA)
- [ ] Performance baseline checked — no significant regressions (DevOps Engineer)
- [ ] Staging sign-off obtained from QA Lead
- [ ] Staging sign-off obtained from Technical Lead

## 4. Support Readiness (Customer Support Lead + PM)

- [ ] Customer Support Lead briefed on new features, known issues, and edge cases (PM + Release Engineer)
- [ ] Support documentation and FAQs updated (Customer Support Lead)
- [ ] Support team trained on new functionality (Customer Support Lead)
- [ ] Escalation path from Support to engineering confirmed (Customer Support Lead + PM)
- [ ] Support tooling (ticketing, alerts) configured for post-release monitoring (Customer Support Lead + DevOps Engineer)

## 5. Production Deployment (Release Engineer + DevOps Engineer)

- [ ] Deployment window scheduled and communicated (PM + Release Engineer)
- [ ] Change management / change advisory board (CAB) approval obtained if required (PM)
- [ ] Database migrations or schema changes executed and verified (Developers + DevOps Engineer)
- [ ] Deployment executed via automated pipeline (Release Engineer)
- [ ] Deployment logs reviewed for errors immediately post-deploy (Release Engineer)
- [ ] Rollback triggered immediately if critical errors detected (Release Engineer)

## 6. Post-Deploy Verification (DevOps Engineer + QA + Release Engineer)

- [ ] Health checks and readiness probes passing in production (DevOps Engineer)
- [ ] Key metrics within baseline range (error rate, latency, throughput) (DevOps Engineer)
- [ ] Smoke tests executed against production (QA)
- [ ] Logs and traces reviewed for anomalies (DevOps Engineer)
- [ ] On-call engineer confirmed and monitoring dashboards active (DevOps Engineer)

## 7. Stakeholder & Support Notification (PM + Release Engineer)

- [ ] Release announced to stakeholders (PM)
- [ ] Release notes published to appropriate channel (Release Engineer)
- [ ] Customer Support Lead notified of go-live and provided final release summary (PM + Release Engineer)
- [ ] Internal teams (sales, success, marketing) notified as agreed (PM)

## 8. Post-Release Handoff

- [ ] Release retrospective or brief review scheduled (PM + Scrum Master)
- [ ] Any production incidents from deploy documented and triaged (PM + DevOps Engineer)
- [ ] Follow-on tickets created for known issues or deferred work (PM + Developers)
- [ ] Release checklist archived in project repo

---

## Sign-off

| Role | Name | Sign-off | Date |
|------|------|----------|------|
| Release Engineer | | | |
| DevOps Engineer | | | |
| QA Lead | | | |
| Customer Support Lead | | | |
| Project Manager | | | |

> All sign-offs are required before a production deployment proceeds. In urgent hotfix scenarios, PM may approve with partial sign-off and document the exception.
