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

## Release Manager

### Role Summary
Release Managers own and coordinate all release activities, ensure readiness for deployment, and manage post-release communications. They are accountable for the full deployment lifecycle—from scheduling deployment windows to confirming production stability—and serve as the central point of coordination between engineering, QA, and stakeholders during release events.

Adding this role improves outcomes by providing a single accountable owner for release quality gates, reducing the risk of incomplete or uncoordinated deployments, and giving stakeholders a clear contact for release status and timing.

### Responsibilities
- Schedule deployment windows and communicate release timelines to the team and stakeholders
- Verify pre-release and post-release checklists (see [Release & Deployment Guide](octoacme-release-and-deployment.md) and [Release Readiness Checklist](octoacme-release-readiness-checklist.md))
- Coordinate release readiness sign-off from Developers and QA Lead
- Own the rollback plan and coordinate incident response if a deployment fails
- Communicate release status, notes, and outcomes to Product Manager and Stakeholders

### Goals
- Ensure every release meets defined quality gates before promotion to production
- Reduce deployment risk through preparation, validation, and documented rollback plans
- Maintain release discipline, transparency, and stakeholder confidence

### Typical Communication
- Deployment window notices and release announcements
- Pre-release readiness confirmations with Developers and QA Lead
- Post-release status updates to Product Manager and Stakeholders
- Incident and rollback communications (see [Risk Management & Communication](octoacme-risks-and-communication.md))

### Key Interactions

| With | Nature of Interaction |
|---|---|
| Project Manager | Aligns on release timelines, dependencies, and milestone completion |
| Product Manager | Notifies of release status; confirms acceptance criteria met before ship |
| Developers | Verifies all PRs merged, CI passing, and smoke tests ready |
| QA Lead | Confirms test completion and final quality sign-off |
| Stakeholders | Communicates release notes, deployment windows, and post-release outcomes |

> See also: [Release & Deployment Guide](octoacme-release-and-deployment.md) · [Release Readiness Checklist](octoacme-release-readiness-checklist.md)

---

## QA Lead

### Role Summary
QA Leads set the strategy for quality assurance across the project lifecycle. They own test planning, oversee automated and manual testing efforts, and ensure features meet acceptance criteria before release. By establishing clear quality standards, QA Leads reduce defects reaching production and improve overall delivery confidence.

Adding this role improves outcomes by centralizing quality ownership, ensuring testing is planned alongside feature work rather than bolted on at the end, and providing a consistent quality signal to the team for release decisions.

### Responsibilities
- Define and maintain test plans and QA approaches for each sprint and release
- Oversee automation and manual test coverage, including unit, integration, and end-to-end tests
- Validate feature acceptance criteria with the Product Manager before sprint sign-off
- Escalate blocking quality issues to the Project Manager and Product Manager
- Coordinate QA readiness confirmation with the Release Manager before each deployment

### Goals
- Ensure features meet acceptance criteria and the Definition of Done before promotion
- Build reliable automation coverage to reduce manual regression effort
- Provide clear quality signals to the team so releases ship with confidence

### Typical Communication
- Test plans and QA status updates aligned to sprint ceremonies
- Defect and blocker escalation reports to Project Manager
- Acceptance validation sign-off to Product Manager and Release Manager
- QA summaries in sprint reviews and release notes

### Key Interactions

| With | Nature of Interaction |
|---|---|
| Project Manager | Coordinates test scheduling within sprint and release plans |
| Product Manager | Validates acceptance criteria and confirms feature sign-off |
| Developers | Partners on test coverage, automation approach, and bug triage |
| Release Manager | Provides quality sign-off as a release gate |
| Business Analyst | Reviews requirements and acceptance criteria for testability |
| Stakeholders | Communicates QA status and quality metrics at key milestones |

> See also: [Execution & Tracking](octoacme-execution-and-tracking.md) · [Project Planning](octoacme-project-planning.md) · [QA Strategy Template](octoacme-qa-strategy-template.md)

---

## Business Analyst

### Role Summary
Business Analysts bridge business needs and technical execution through structured requirements analysis and documentation. They facilitate stakeholder discovery, translate business goals into clear acceptance criteria, and ensure traceability from requirements to delivered features. This role reduces rework caused by unclear or incomplete requirements and keeps delivery aligned to business outcomes.

Adding this role improves outcomes by introducing formal requirements ownership, improving handoffs from initiation through planning and into development, and providing a shared source of truth for acceptance criteria that QA Leads and Developers can reference throughout execution.

### Responsibilities
- Elicit, clarify, and document requirements from stakeholders and Product Manager
- Map requirements to success metrics, acceptance criteria, and test criteria
- Maintain a requirements traceability matrix to track coverage and handoff status
- Facilitate stakeholder interviews and feedback sessions during initiation and planning (see [Project Initiation Guide](octoacme-project-initiation.md))
- Support QA Lead and Developers with requirements questions during execution

### Goals
- Ensure requirements are clear, complete, and traceable before development begins
- Reduce rework caused by misunderstood or incomplete requirements
- Improve alignment between business stakeholders and the engineering team

### Typical Communication
- Requirements documents and user story refinement notes
- Stakeholder interview summaries and feedback loop outputs
- Traceability matrix and acceptance criteria review sessions
- Requirement clarification responses to Developers and QA Lead during execution

### Key Interactions

| With | Nature of Interaction |
|---|---|
| Product Manager | Refines product goals and success metrics into actionable requirements |
| Project Manager | Supports planning by providing clearly scoped requirements and estimates |
| Developers | Ensures requirements are understood before build begins; resolves clarifying questions |
| QA Lead | Provides acceptance criteria and supports test traceability |
| Stakeholders | Conducts interviews and feedback sessions to surface and validate business needs |

> See also: [Project Initiation Guide](octoacme-project-initiation.md) · [Project Planning](octoacme-project-planning.md) · [Requirements Traceability Checklist](octoacme-requirements-traceability.md)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

