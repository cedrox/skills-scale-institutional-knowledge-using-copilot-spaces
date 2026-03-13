# OctoAcme Project Management Overview

## Purpose
Provide a concise, shareable introduction to how OctoAcme runs projects so new teammates can quickly understand our approach, roles, and key artifacts.

## Scope
Applies to all cross-functional projects that deliver product features, services, or integrations.

## Principles
- Customer-first: prioritize customer value and usability.
- Iterative delivery: deliver small, testable increments.
- Clear ownership: each project has a named Project Manager (PM) and Product Lead.
- Data-informed decisions: measure impact and iterate based on evidence.
- Psychological safety: encourage feedback and learning.

## Core Roles
- Project Manager (PM): coordinates delivery, schedules, risk, communications.
- Product Manager (PdM): defines outcomes, prioritizes backlog, and measures success.
- Scrum Master: facilitates agile ceremonies, removes impediments, coaches team.
- Developers: implement features, collaborate on design and testability.
- QA/Testing: validate quality and acceptance criteria.
- Technical Lead: drives architecture decisions, sets engineering standards, guides developers.
- UX Designer: translates user needs into designs; conducts research and usability validation.
- Release Engineer: owns CI/CD pipelines, coordinates deployments, prepares release notes.
- DevOps Engineer: manages infrastructure, monitoring, and delivery tooling.
- Customer Support Lead: ensures support readiness, routes feedback, escalates critical issues.
- Stakeholders: provide inputs and approvals.

See [octoacme-roles-and-personas.md](octoacme-roles-and-personas.md) for full role definitions.

### RACI Summary

| Activity | Responsible | Accountable | Consulted | Informed |
|---|---|---|---|---|
| **Initiation** | PM | PM / Sponsor | PdM, Technical Lead, Stakeholders | All roles |
| **Planning** | PM + PdM | PM | Technical Lead, Scrum Master, UX Designer, Developers | Stakeholders, DevOps, Release Eng |
| **Execution** | Developers, QA, UX Designer | PM + Technical Lead | Scrum Master, PdM | Stakeholders, Customer Support Lead |
| **Release** | Release Engineer, DevOps Engineer | PM + Release Engineer | QA, Technical Lead, Customer Support Lead | Stakeholders, All roles |
| **Retrospective** | Scrum Master | PM | All team roles | Stakeholders (summary only) |

> **Key:** R = Responsible (does the work), A = Accountable (owns the outcome), C = Consulted (provides input), I = Informed (kept in the loop).

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- Risk Register
- Retrospective notes and action items

## Lifecycle (high-level)
1. Initiation: problem statement, stakeholders, high-level timeline.
2. Planning: scope, resources, milestones, dependencies.
3. Execution: build, test, review, iterate.
4. Release: deploy, verify, announce.
5. Close & Retrospective: capture learnings and next steps.

## Communication Cadence
- Weekly sync between PM + PdM
- Twice-weekly standups for delivery team (or as agreed)
- Monthly stakeholder updates
- Ad-hoc escalations as needed

## How to use these docs
- Keep the Project Charter updated in the project repo.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context.
