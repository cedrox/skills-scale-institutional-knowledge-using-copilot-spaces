# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
  - Typical facilitator: Scrum Master (or rotating facilitator)
  - Scrum Master ensures standup stays timeboxed, surfaces impediments, and logs action items
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone
- PM and PdM alignment cadence: weekly or as agreed

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup — Scrum Master facilitates and drives a quick triage; logs action items and tracks resolution
- Level 2: PM escalates to Product Lead and dependent teams when cross-team coordination is required; Scrum Master escalates to PM when the blocker cannot be resolved within the team
- Level 3: Sponsor-level escalation for business-impacting issues — PM owns this escalation

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
- [ ] Roles onboarding checklist applied for new joiners (see [docs/roles-onboarding-checklist.md](roles-onboarding-checklist.md))
