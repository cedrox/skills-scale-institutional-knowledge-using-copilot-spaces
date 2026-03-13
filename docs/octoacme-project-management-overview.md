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
- Developers: implement features, collaborate on design and testability.
- QA/Testing: validate quality and acceptance criteria.
- Stakeholders: provide inputs and approvals.
- Scrum Master: facilitates team ceremonies, removes impediments, fosters continuous improvement.
- Technical Lead: owns architecture and technical direction.
- Release Engineer: owns release pipelines and orchestration.
- DevOps Engineer: owns infrastructure and monitoring.
- UX Designer: owns user research and interface design.
- Customer Support Lead: owns support readiness and incident triage.

## RACI-style mapping (compact)
For common lifecycle activities, typical role responsibilities (R = Responsible, A = Accountable, C = Consulted, I = Informed):

- **Initiation**: R: PdM, PM | A: PdM | C: Stakeholders, Technical Lead | I: Dev Team, Support
- **Planning**: R: PM, PdM | A: PM | C: Technical Lead, Scrum Master, UX Designer | I: Stakeholders, Support
- **Execution**: R: Developers, QA | A: PM | C: Scrum Master, Technical Lead, UX Designer | I: Stakeholders, Support
- **Release**: R: Release Engineer, DevOps Engineer | A: PM | C: PdM, Technical Lead, Customer Support Lead | I: Stakeholders, Dev Team
- **Retrospective**: R: Team (Developers, QA, Scrum Master) | A: PM | C: PdM, Technical Lead | I: Stakeholders

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
- Use [docs/roles-onboarding-checklist.md](roles-onboarding-checklist.md) and [docs/release-checklist.md](release-checklist.md) to standardize handoffs and release readiness.
