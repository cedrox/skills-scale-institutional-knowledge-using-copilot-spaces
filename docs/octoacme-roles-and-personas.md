# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA / Testing

### Role Summary
QA Engineers validate that features meet acceptance criteria and quality standards before release. They design and execute test plans, identify defects, and safeguard the stability of each release.

### Responsibilities
- Design and execute test plans (unit, integration, end-to-end)
- Identify, document, and track defects to resolution
- Validate acceptance criteria before features move to done
- Maintain automated test suites and smoke test packs
- Provide sign-off on release readiness

### Goals
- Ensure high product quality and low production defect rates
- Increase confidence in each release through repeatable test coverage
- Collaborate with Developers early to prevent defects rather than catch them late

### Typical Communication / Interactions
- Paired with Developers during implementation and bug triage
- Coordinates release sign-off with Release Engineer and PM
- Reports testing status to PM and Technical Lead

---

## Scrum Master

### Role Summary
The Scrum Master facilitates agile ceremonies, protects the team from distractions, and coaches the team on agile best practices. They act as a servant-leader who enables continuous improvement and removes impediments.

### Responsibilities
- Facilitate daily standups, sprint planning, sprint reviews, and retrospectives
- Identify and remove impediments blocking team progress
- Coach the team and stakeholders on agile principles and practices
- Shield the team from unplanned work and scope creep during a sprint
- Track team velocity and flag deviations to the PM
- Maintain the sprint board and ensure it accurately reflects team status

### Goals
- Maintain a predictable, sustainable delivery cadence
- Foster a culture of transparency, trust, and continuous improvement
- Minimize waste and maximize team throughput

### Typical Communication / Interactions
- Daily with Developers and QA to surface and resolve blockers
- Regular sync with PM to align on sprint health and escalation needs
- Works with PdM to ensure backlog is refined and sprint-ready
- Facilitates cross-team coordination when dependencies arise

---

## UX Designer

### Role Summary
UX Designers translate user needs into intuitive, accessible product experiences. They conduct research, create wireframes and prototypes, and validate designs with real users before development begins.

### Responsibilities
- Conduct user research, interviews, and usability tests
- Create wireframes, prototypes, and high-fidelity designs
- Define user flows and interaction patterns
- Collaborate with PdM to translate business goals into user-centered solutions
- Partner with Developers to ensure design intent is implemented accurately
- Maintain a shared design system and component library

### Goals
- Deliver experiences that are intuitive, accessible, and delightful
- Reduce rework by validating designs before development starts
- Ensure consistency across all product surfaces

### Typical Communication / Interactions
- Collaborates closely with PdM on requirements and user stories
- Pairs with Developers during implementation to clarify design intent
- Works with QA to verify UI/UX acceptance criteria
- Presents research findings and design proposals to Stakeholders

---

## Technical Lead

### Role Summary
The Technical Lead drives architectural decisions, sets engineering standards, and guides the team through complex technical challenges. They bridge the gap between product goals and technical implementation.

### Responsibilities
- Architect solutions and evaluate technology trade-offs
- Establish and enforce coding standards, patterns, and best practices
- Lead technical design reviews and spike investigations
- Mentor and upskill Developers on the team
- Identify technical risks and propose mitigations early
- Coordinate with DevOps and Release Engineers on infrastructure and delivery requirements

### Goals
- Deliver a scalable, maintainable, and secure codebase
- Minimize technical debt while enabling rapid feature delivery
- Ensure all technical decisions align with product and business goals

### Typical Communication / Interactions
- Works daily with Developers to provide guidance and unblock technical issues
- Aligns with PM and PdM on feasibility, effort estimates, and trade-offs
- Partners with DevOps Engineer and Release Engineer on build, deploy, and infrastructure concerns
- Communicates architecture decisions via design docs and PR reviews

---

## Release Engineer

### Role Summary
The Release Engineer owns the release pipeline, coordinates deployments, and ensures that each release is delivered safely, consistently, and with a clear rollback path.

### Responsibilities
- Manage and maintain CI/CD pipelines for build, test, and deploy stages
- Coordinate release schedules and deployment windows with PM and stakeholders
- Prepare and publish release notes for each deployment
- Validate that all pre-release requirements are met before promoting a build
- Define and document rollback procedures and runbooks
- Automate deployment steps to reduce manual risk

### Goals
- Achieve zero-surprise, repeatable releases
- Reduce mean time to deploy and mean time to recover (MTTR)
- Ensure release artifacts are traceable and auditable

### Typical Communication / Interactions
- Coordinates closely with Developers and QA for build validation and release sign-off
- Aligns with DevOps Engineer on infrastructure readiness and environment configuration
- Communicates deployment schedules and release notes to PM and Stakeholders
- Works with Customer Support Lead to confirm support readiness before go-live

---

## Customer Support Lead

### Role Summary
The Customer Support Lead ensures the support team is prepared for each release, channels customer feedback into the product process, and escalates critical production issues to the appropriate teams.

### Responsibilities
- Prepare support documentation, FAQs, and runbooks ahead of releases
- Train support staff on new features and known edge cases
- Collect, triage, and route customer feedback and bug reports to PdM and PM
- Escalate high-severity production issues to PM and on-call engineering
- Track support ticket trends and report insights in retrospectives
- Coordinate with Release Engineer to confirm post-deploy support readiness

### Goals
- Minimize customer impact from new releases through proactive readiness
- Close the feedback loop between customers and the product team
- Reduce escalation volume by enabling self-service and clear documentation

### Typical Communication / Interactions
- Coordinates with PM and PdM on release timelines and feature summaries
- Works with Release Engineer to confirm support readiness before go-live
- Provides feedback themes to PdM during planning and retrospectives
- Communicates directly with customers and routes escalations to engineering

---

## DevOps Engineer

### Role Summary
DevOps Engineers design, maintain, and improve the infrastructure and tooling that enables reliable, scalable, and secure software delivery. They bridge development and operations to support continuous delivery practices.

### Responsibilities
- Provision and manage cloud infrastructure (compute, networking, storage, IAM)
- Build and maintain CI/CD tooling, monitoring, and alerting systems
- Implement and enforce security and compliance controls in the pipeline
- Manage environment configuration, secrets, and access controls
- Optimize system reliability, performance, and cost
- Respond to and resolve infrastructure incidents

### Goals
- Ensure high availability and resilience for all production systems
- Enable developers to ship safely and quickly with minimal friction
- Drive automation to reduce manual operations and human error

### Typical Communication / Interactions
- Works closely with Release Engineer on pipeline design, deployment automation, and runbooks
- Engages with Technical Lead on infrastructure requirements and architecture decisions
- Coordinates with Developers and QA on environment needs and access
- Reports infrastructure health and incident summaries to PM and Technical Lead

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [roles-onboarding-checklist.md](roles-onboarding-checklist.md) for a checklist new team members can use to confirm responsibilities and contacts.

