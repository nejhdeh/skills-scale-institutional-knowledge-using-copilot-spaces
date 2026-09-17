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

## QA Engineers

### Role Summary
QA Engineers safeguard product quality by defining the test approach, validating features against acceptance criteria, and surfacing defects before they reach customers.

### Responsibilities
- Draft and maintain the QA approach for each release
- Design, automate, and execute functional and regression tests
- Verify acceptance criteria with Product Managers before sign-off
- Report defects with clear reproduction steps and severity
- Track quality trends and flag recurring failure patterns

### Goals
- Catch defects as early as possible in the delivery cycle
- Keep automated test suites reliable and fast
- Provide a clear, evidence-based quality signal for release decisions

### Typical Communication
- Test plans and QA approach notes during planning
- Defect reports and triage discussions with Developers
- Feature acceptance sign-off to Product and Project Managers

### How this persona interacts with existing roles
- Works with **Developers** on testability, defect triage, and automated coverage
- Confirms acceptance criteria with **Product Managers** before a feature is accepted
- Gives **Project Managers** quality status that feeds risk registers and schedules
- Provides the **Release Manager** with the go/no-go quality evidence for a release

---

## Release Managers

### Role Summary
Release Managers own the path to production. They coordinate release readiness, deployment execution, and rollback decisions so changes ship predictably and safely.

### Responsibilities
- Maintain the release calendar and readiness checklist
- Confirm CI, security scans, and QA sign-off are complete before deploy
- Coordinate deployment windows and communicate release status
- Lead rollback or hotfix decisions when a deployment goes wrong
- Capture release outcomes for retrospectives

### Goals
- Deliver low-risk, repeatable, well-communicated releases
- Reduce time to detect and recover from deployment issues
- Keep release history and decisions auditable

### Typical Communication
- Release readiness checklists and go/no-go decisions
- Deployment and rollback announcements to stakeholders
- Incident and post-release summaries

### How this persona interacts with existing roles
- Depends on **QA Engineers** for acceptance and regression results
- Partners with **Developers** on deployment steps, hotfixes, and rollbacks
- Aligns with **Product Managers** on release scope and customer messaging
- Keeps **Project Managers** informed so timelines and risks stay accurate

---

## UX Designers

### Role Summary
UX Designers shape how customers experience the product. They research user needs, design flows and interfaces, and validate that solutions are usable and accessible.

### Responsibilities
- Conduct user research and share findings with the team
- Produce wireframes, prototypes, and interaction specifications
- Define and uphold accessibility and design system standards
- Validate designs through usability testing and post-launch feedback
- Participate in design reviews and refinement sessions

### Goals
- Ensure solutions solve real user problems
- Deliver consistent, accessible experiences across the product
- Reduce rework by validating designs before implementation

### Typical Communication
- Prototypes and design walkthroughs during planning
- Research summaries and usability findings
- Design review comments alongside acceptance criteria

### How this persona interacts with existing roles
- Partners with **Product Managers** to turn problem statements into validated designs
- Hands off specifications and reviews implementations with **Developers**
- Supplies **QA Engineers** with expected behaviours and accessibility criteria
- Flags research or design dependencies to **Project Managers** for scheduling

---

## Executive Sponsors

### Role Summary
Executive Sponsors provide the mandate, funding, and organizational support for a project. They champion the work, unblock escalations, and hold the team accountable to business outcomes.

### Responsibilities
- Approve project scope, budget, and staffing
- Resolve cross-team blockers and escalated risks
- Review progress against agreed business outcomes
- Champion the project with other leaders and stakeholders
- Endorse major scope or priority changes

### Goals
- Ensure the project delivers measurable business value
- Keep investment aligned with strategy
- Remove organizational obstacles quickly

### Typical Communication
- Milestone and outcome reviews
- Escalation decisions recorded in decision logs
- Executive summaries of status, risk, and impact

### How this persona interacts with existing roles
- Receives status, risks, and escalations from **Project Managers**
- Agrees priority and success metrics with **Product Managers**
- Endorses release timing or delays raised by **Release Managers**
- Rarely engages **Developers**, **QA Engineers**, or **UX Designers** directly; requests flow through Product and Project Managers

---

## Support Representatives

### Role Summary
Support Representatives are the voice of the customer after release. They resolve customer issues, escalate defects, and feed real-world usage insights back into the backlog.

### Responsibilities
- Triage and resolve incoming customer issues
- Escalate reproducible defects and incidents to the delivery team
- Maintain customer-facing help content and known-issue notes
- Summarize recurring themes from customer feedback
- Confirm fixes with affected customers after release

### Goals
- Reduce customer time-to-resolution
- Prevent repeat issues by surfacing root causes
- Keep customers informed during incidents and releases

### Typical Communication
- Escalation tickets with reproduction details and customer impact
- Feedback themes shared during planning and retrospectives
- Customer notifications during incidents and releases

### How this persona interacts with existing roles
- Escalates defects to **QA Engineers** and **Developers** with reproduction details
- Feeds customer pain points to **Product Managers** for prioritization
- Receives release and known-issue notes from **Release Managers**
- Alerts **Project Managers** when support load signals a delivery risk

---

## Role interaction at a glance

| Persona | Primary partners | Main hand-off |
| --- | --- | --- |
| Developers | Product Managers, QA Engineers, UX Designers | Implemented, tested changes ready for review |
| Product Managers | Executive Sponsors, UX Designers, Support Representatives | Prioritized backlog and acceptance criteria |
| Project Managers | All personas | Plans, risks, and status reporting |
| QA Engineers | Developers, Product Managers, Release Managers | Quality sign-off for release decisions |
| Release Managers | QA Engineers, Developers, Support Representatives | Go/no-go decision and deployment outcome |
| UX Designers | Product Managers, Developers, QA Engineers | Validated designs and accessibility criteria |
| Executive Sponsors | Product Managers, Project Managers | Funding, priority, and escalation decisions |
| Support Representatives | Product Managers, QA Engineers, Release Managers | Customer feedback and escalated defects |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

