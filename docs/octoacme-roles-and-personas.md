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

## Data Steward

### Role Summary
The Data Steward is accountable for the integrity, classification, access control, and documentation of data assets within a project. They act as the bridge between engineering, legal/compliance, and the project team to ensure data is handled responsibly throughout the project lifecycle.

### Responsibilities
- Define and enforce data classification (Public, Internal, Confidential, Restricted)
- Manage access permissions using the least-privilege principle
- Document data sources, schemas, lineage, and quality issues
- Define and monitor data retention and disposal procedures
- Ensure compliance with applicable regulations (e.g., GDPR, CCPA)
- Lead data breach response coordination

### Goals
- Maintain data integrity and prevent unauthorized access
- Reduce compliance risk across the project
- Ensure all data assets are well-documented and discoverable

### Typical Interactions (RACI)

| Activity | Data Steward | Project Manager | Engineering Lead | Legal/Compliance |
|---|---|---|---|---|
| Data classification | **Responsible** | Consulted | Consulted | Accountable |
| Access provisioning | **Responsible** | Informed | Consulted | — |
| Compliance review | **Responsible** | Informed | Informed | Accountable |
| Data documentation | **Accountable** | Informed | Responsible | — |
| Incident response | **Responsible** | Accountable | Consulted | Consulted |

### Key Artifacts
- [Data Stewardship Checklist](templates/data-stewardship-checklist.md)
- Data dictionary / schema docs (maintained in project repo)
- Data retention and disposal policy (linked from project docs)

---

## Onboarding Mentor

### Role Summary
The Onboarding Mentor supports new team members from their first day through their first month, acting as the primary point of contact for questions and helping them become productive contributors quickly. They collaborate with HR, team leads, and the Project Manager to deliver a consistent onboarding experience.

### Responsibilities
- Coordinate pre-arrival setup (accounts, equipment, access)
- Guide new team members through the codebase, conventions, and tooling
- Facilitate introductions to key cross-functional partners
- Assign initial tasks that build confidence and familiarity
- Maintain and improve the onboarding checklist based on experience

### Goals
- Reduce time-to-productivity for new team members
- Ensure no gaps in access, knowledge, or relationships at the end of week one
- Capture and share feedback to continuously improve the onboarding process

### Typical Interactions (RACI)

| Activity | Onboarding Mentor | Project Manager | Engineering Lead | HR |
|---|---|---|---|---|
| Pre-arrival setup | **Responsible** | Informed | Consulted | Accountable |
| Day-1 orientation | **Responsible** | Consulted | Consulted | Informed |
| Technical walkthrough | **Responsible** | — | Accountable | — |
| First task assignment | **Responsible** | Consulted | Accountable | — |
| Onboarding feedback | **Accountable** | Informed | Informed | Informed |

### Key Artifacts
- [Onboarding Checklist](checklists/onboarding-checklist.md)
- New team member first-week schedule
- Questions log (maintained during onboarding period)

---

## Stakeholder Liaison

### Role Summary
The Stakeholder Liaison facilitates communication between the project team and external business stakeholders. They ensure stakeholders are informed, aligned, and have a clear channel for providing feedback and escalating concerns. They report back to the Project Manager and help maintain a unified view of stakeholder priorities.

### Responsibilities
- Build and maintain the stakeholder map for the project
- Define and manage the communication cadence (meetings, updates, channels)
- Collect and relay stakeholder feedback to the project team
- Escalate unresolved needs or conflicts to the Project Manager
- Prepare and distribute regular status updates

### Goals
- Keep stakeholders informed and engaged without overwhelming them
- Prevent surprises by surfacing issues before they become blockers
- Maintain alignment between business expectations and delivery realities

### Typical Interactions (RACI)

| Activity | Stakeholder Liaison | Project Manager | Product Manager | Stakeholders |
|---|---|---|---|---|
| Stakeholder mapping | **Accountable** | Consulted | Consulted | Informed |
| Status updates | **Responsible** | Accountable | Consulted | Informed |
| Feedback collection | **Responsible** | Informed | Consulted | Accountable |
| Escalation | **Responsible** | Accountable | Consulted | Informed |
| Communications plan | **Accountable** | Consulted | Informed | — |

### Key Artifacts
- [Stakeholder Communications Plan](templates/stakeholder-communications-plan.md)
- Stakeholder map (maintained in project repo)
- Weekly status updates (see [Risk Management & Communication](octoacme-risks-and-communication.md))

---

## Deployment Coordinator

### Role Summary
The Deployment Coordinator manages the end-to-end release process, ensuring all prerequisites are met, approvals are obtained, and handoffs between engineering, QA, and product are smooth. They own the deployment readiness checklist and are the single point of accountability for the mechanics of a release.

### Responsibilities
- Schedule deployment windows and coordinate across engineering, QA, and product
- Verify all pre-release requirements are satisfied before deployment proceeds
- Own and execute the deployment readiness checklist
- Document rollback plans and ensure they are tested or reviewed
- Communicate deployment status to stakeholders and the support team

### Goals
- Reduce deployment risk through disciplined pre-flight verification
- Minimize unplanned downtime and rollback incidents
- Ensure all stakeholders are informed before, during, and after every release

### Typical Interactions (RACI)

| Activity | Deployment Coordinator | Engineering Lead | QA | Product Manager | Stakeholder Liaison |
|---|---|---|---|---|---|
| Deployment scheduling | **Accountable** | Consulted | Consulted | Informed | Informed |
| Pre-release checklist | **Responsible** | Consulted | Consulted | Informed | — |
| Approval collection | **Responsible** | Accountable | Accountable | Accountable | — |
| Rollback planning | **Accountable** | Responsible | Consulted | Informed | — |
| Release announcement | **Responsible** | Informed | Informed | Consulted | Accountable |

### Key Artifacts
- [Deployment Readiness Checklist](checklists/deployment-readiness-checklist.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- Release notes (see [Release & Deployment Guide](octoacme-release-and-deployment.md))

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

