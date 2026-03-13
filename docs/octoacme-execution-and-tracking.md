# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — **facilitated by Scrum Master** — focus on progress, blockers, and dependencies; each team member answers: what did I do, what will I do, what is blocking me
- Weekly delivery sync — PM leads; Scrum Master surfaces sprint health, velocity trends, and flagged risks
- Sprint Planning — Scrum Master facilitates; PdM presents prioritized backlog; Developers commit to sprint scope
- Sprint Review / Demo — team demonstrates completed work; Scrum Master facilitates; PM and PdM invite stakeholders
- Sprint Retrospective — Scrum Master facilitates; team captures what went well, what to improve, and action items

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
- Level 1: **Scrum Master** surfaces and triages blockers in daily standup; attempts team-level resolution within the sprint day
- Level 2: **Scrum Master** escalates cross-team or prolonged blockers (>1 day) to PM; PM coordinates with dependent teams and Product Lead
- Level 3: **PM** escalates business-impacting or resource blockers to Sponsor level; Scrum Master continues to shield team and update sprint board
- Rule of thumb: Scrum Master owns blockers within the team's control; PM owns blockers that require external decisions or resources

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
