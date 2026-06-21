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

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Additional Personas (proposed additions)

### Delivery Lead
Role Summary:
The Delivery Lead focuses on day-to-day delivery cadence and ensures cross-functional dependencies are coordinated so roadmap milestones are met.

Responsibilities:
- Oversee sprint/iteration delivery cadence and blockers
- Coordinate cross-team dependencies and integration points
- Track progress against milestones and surface risks early
- Escalate unresolved blockers to the Project Manager

Interaction:
Works closely with the Project Manager and PdM to translate priorities into execution plans; coordinates with Developers, QA, and Release Manager to unblock work and ensure readiness for release.

Example Handoff:
When a feature is ready for test, the Delivery Lead confirms test environments, notifies QA, and ensures deployment windows are scheduled with the Release Manager.

---

### Technical Program Manager (TPM)
Role Summary:
The TPM manages large technical initiatives and cross-team technical dependencies to ensure integration points are delivered smoothly.

Responsibilities:
- Identify and track cross-team technical dependencies
- Drive technical milestones and integration plans
- Facilitate design and architecture discussions across teams
- Track risks related to integrations and third-party systems

Interaction:
Partners with Engineering Managers and Developers to surface integration risks, and with PM/PdM for trade-offs and scheduling. Escalates architectural risks that impact the roadmap.

---

### Engineering Manager
Role Summary:
The Engineering Manager owns people management, technical direction, and long-term code quality within their engineering team.

Responsibilities:
- Capacity planning and staffing
- Coaching and performance management of engineers
- Drive technical debt and quality initiatives
- Assist with estimates and technical trade-offs

Interaction:
Coordinates with Project Managers on team commitments, with TPMs on cross-team technical work, and with Developers on execution and code reviews.

---

### Release Manager
Role Summary:
The Release Manager coordinates deployments, rollback plans, and post-deploy verification to ensure releases are predictable and safe.

Responsibilities:
- Maintain release calendar and coordinate deployment windows
- Verify pre-release checks and sign-offs are complete
- Own rollback and mitigation plans for releases
- Coordinate post-deploy verification and communicate release status

Interaction:
Works with Developers, QA, SRE/On-call, and Product to schedule releases, run checks, and lead post-release triage if needed. Uses the release checklist template for pre/post-release verification.

---

### SRE / On-call Engineer
Role Summary:
Responsible for production reliability, monitoring, and incident response.

Responsibilities:
- Define and maintain runbooks for common incidents
- Monitor production and respond to on-call alerts
- Support deployments and post-deploy verification
- Assist in RCA and follow-up action items after incidents

Interaction:
Engages during deployment and incidents, coordinates with Release Manager and Developers to remediate issues, and advises on reliability improvements.

---

### Security Liaison
Role Summary:
Primary point of contact for security reviews, threat modeling, and triage of security scan findings.

Responsibilities:
- Coordinate security reviews and threat modeling sessions
- Triage and prioritize security findings from scans and audits
- Advise on remediation strategies and acceptable risk
- Ensure security sign-off as needed for releases

Interaction:
Works with Developers and QA to remediate findings and with Product/PM to balance risk vs. schedule; escalates critical security items through the incident/escalation paths.

---

### UX Researcher / Designer
Role Summary:
Ensures usability and validates product decisions through research and design.

Responsibilities:
- Conduct user research and usability testing
- Deliver design assets and specs for implementation
- Validate acceptance criteria with user-centric evidence
- Collaborate on accessibility and UX quality

Interaction:
Partners with PdM to inform acceptance criteria and with Developers to implement and validate designs during development and QA.

---

### Data & Measurement Lead
Role Summary:
Defines success metrics and instrumentation to measure impact.

Responsibilities:
- Define KPIs and instrumentation requirements for features
- Ensure telemetry and dashboards are in place for release
- Validate data quality and event collection
- Support experiments and measurement strategies

Interaction:
Works with PdM on success metrics and Developers to implement instrumentation; partners with Project Manager and QA to validate telemetry during releases.

---

## Handoffs and Decision Points (examples)
- Readiness for release: Developer -> QA -> Delivery Lead -> Release Manager -> SRE/On-call
- Security sign-off: Developer -> Security Liaison -> Product/PM
- Metric validation: Developer -> Data & Measurement Lead -> Product/PM

(Consider using the templates in docs/templates/ for concrete checklists used during release and delivery coordination.)
