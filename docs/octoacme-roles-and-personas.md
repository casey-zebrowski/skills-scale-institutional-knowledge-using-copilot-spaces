# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

## Roles Defined in This Document

| Role | Section |
|---|---|
| Developer | [Developers](#developers) |
| Product Manager | [Product Managers](#product-managers) |
| Project Manager | [Project Managers](#project-managers) |
| Tech Lead | [Tech Lead](#tech-lead) |
| Release Coordinator | [Release Coordinator](#release-coordinator) |
| QA/Test Lead | [QA/Test Lead](#qatest-lead) |
| Business Analyst | [Business Analyst](#business-analyst) |
| Stakeholder Sponsor | [Stakeholder Sponsor](#stakeholder-sponsor) |
| Agile Coach | [Agile Coach](#agile-coach) |

## Supporting Templates

The following templates help make these roles actionable. Each template references the relevant personas and describes when to use it in the project lifecycle.

| Template | Owner | Lifecycle Phase |
|---|---|---|
| [Release Readiness Checklist](templates/release-readiness-checklist.md) | Release Coordinator | Release |
| [Test Strategy Checklist](templates/test-strategy-checklist.md) | QA/Test Lead | Planning → Release |
| [Requirements Brief Template](templates/requirements-brief-template.md) | Business Analyst | Initiation → Planning |
| [Stakeholder Update Template](templates/stakeholder-update-template.md) | Project Manager / Stakeholder Sponsor | Execution → Close |
| [Agile Ceremonies Checklist](templates/agile-ceremonies-checklist.md) | Agile Coach | Execution (every sprint) |

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

## Tech Lead

### Role Summary
Tech Leads provide technical oversight, guide architectural decisions, and mentor developers. They bridge engineering and project management concerns to keep delivery on track.

### Responsibilities
- Own architectural decisions and technical direction
- Review and approve critical pull requests
- Identify and mitigate technical risks early
- Mentor developers and support skill development
- Coordinate with the Project Manager on capacity and technical blockers

### Goals
- Ensure technical quality, scalability, and maintainability
- Reduce architectural debt and unplanned rework
- Enable developers to work with speed and confidence

### Typical Communication
- Architecture decision records (ADRs)
- Code review feedback and design docs
- Daily standups and sprint planning sessions

### Key Interactions
- **Project Manager**: shares technical risks and timeline impacts
- **Developers**: provides guidance, reviews code, unblocks issues
- **QA/Test Lead**: aligns on testability requirements and acceptance criteria
- **Release Coordinator**: confirms code readiness before release

---

## Release Coordinator

### Role Summary
The Release Coordinator oversees release planning and execution, ensures all readiness criteria are met before deployment, and coordinates across QA, Development, and Stakeholders to deliver smooth, low-risk releases.

### Responsibilities
- Maintain the release calendar and communicate deployment windows
- Verify all pre-release criteria are satisfied (code freeze, CI green, release notes)
- Coordinate with QA/Test Lead on smoke-test sign-off
- Communicate go/no-go decisions to the team and stakeholders
- Own the rollback plan and incident escalation path for each release
- Publish post-release announcements and close release tickets

### Goals
- Reduce release-related incidents and unplanned downtime
- Provide predictable, repeatable release cadence
- Ensure full visibility into release status across all stakeholders

### Typical Communication
- Release readiness reports and go/no-go emails
- Deployment-window notifications to stakeholders
- Post-release announcements

### Key Interactions
- **Project Manager**: aligns release dates with project milestones
- **Tech Lead**: confirms technical readiness and sign-off
- **QA/Test Lead**: receives test sign-off before go/no-go decision
- **Stakeholder Sponsor**: communicates high-level release status and risks
- **Developers**: collects merge status and resolves last-minute blockers

### Artifacts Owned
- Release calendar
- Go/no-go decision record
- Post-release announcement

### RACI Notes
| Activity | Release Coordinator |
|---|---|
| Define release schedule | **Accountable** |
| Go/no-go decision | **Accountable** |
| Deploy to production | Responsible (coordinates) |
| Smoke-test sign-off | Consulted |
| Stakeholder notification | Responsible |

> **Supporting template:** [Release Readiness Checklist](templates/release-readiness-checklist.md)

---

## QA/Test Lead

### Role Summary
The QA/Test Lead owns the testing strategy, ensures sufficient test coverage across all release candidates, tracks defects, and communicates quality outcomes to the team.

### Responsibilities
- Define and maintain the overall test strategy and test plan
- Design, review, and maintain test cases (functional, regression, integration)
- Coordinate defect triage and track bugs to resolution
- Provide test-coverage reports and quality metrics to the team
- Approve or block releases based on quality thresholds
- Champion test automation adoption and continuous quality improvement

### Goals
- Prevent critical defects from reaching production
- Improve defect detection rate early in the development cycle
- Increase automation coverage to reduce manual test effort over time

### Typical Communication
- Test plans and test execution reports
- Defect reports and triage meeting notes
- Quality metrics dashboards or summaries shared at sprint review

### Key Interactions
- **Release Coordinator**: provides test sign-off as a prerequisite for go/no-go
- **Tech Lead**: aligns on testability and coverage requirements
- **Developers**: clarifies acceptance criteria; collaborates on automated tests
- **Project Manager**: reports quality status and escalates blocking defects
- **Business Analyst**: validates that test cases cover all stated requirements

### Artifacts Owned
- Test strategy document
- Test plan and test cases
- Defect log
- Test execution summary report

### RACI Notes
| Activity | QA/Test Lead |
|---|---|
| Test strategy | **Accountable** |
| Test-case authoring | Responsible |
| Defect triage | **Accountable** |
| Release quality sign-off | **Accountable** |
| Automation roadmap | Responsible |

> **Supporting template:** [Test Strategy Checklist](templates/test-strategy-checklist.md)

---

## Business Analyst

### Role Summary
The Business Analyst captures, clarifies, and documents requirements. They serve as the primary bridge between stakeholders and the technical team, ensuring shared understanding of what needs to be built and why.

### Responsibilities
- Elicit, analyze, and document business requirements
- Translate stakeholder needs into clear user stories and acceptance criteria
- Facilitate requirements workshops and clarification sessions
- Maintain the requirements backlog and ensure traceability
- Document current-state and future-state process flows
- Identify scope gaps, contradictions, or ambiguities early

### Goals
- Eliminate ambiguity in requirements before development begins
- Ensure solutions address the stated business problem
- Reduce rework caused by misunderstood or missing requirements

### Typical Communication
- Requirements brief and user stories
- Process-flow diagrams (current state / future state)
- Meeting notes from stakeholder workshops

### Key Interactions
- **Product Manager**: aligns requirements to product vision and roadmap
- **Project Manager**: surfaces scope changes and timeline impacts
- **Stakeholder Sponsor**: validates business intent and prioritization
- **Developers**: answers clarification questions during implementation
- **QA/Test Lead**: ensures test cases fully cover documented requirements

### Artifacts Owned
- Requirements brief / specification
- User story backlog entries with acceptance criteria
- Process-flow diagrams
- Requirements traceability matrix

### RACI Notes
| Activity | Business Analyst |
|---|---|
| Requirements elicitation | **Accountable** |
| User-story authoring | Responsible |
| Acceptance criteria | Responsible |
| Process-flow documentation | **Accountable** |
| Scope-change assessment | Consulted |

> **Supporting template:** [Requirements Brief Template](templates/requirements-brief-template.md)

---

## Stakeholder Sponsor

### Role Summary
The Stakeholder Sponsor provides executive or senior-leadership direction for the project, ensures adequate resource allocation, and unblocks issues that cannot be resolved at the project team level.

### Responsibilities
- Champion the project at the leadership level and secure funding/resources
- Set strategic priorities and provide high-level direction
- Review and approve major scope changes or budget adjustments
- Receive and act on escalations from the Project Manager
- Ensure alignment between the project and organizational goals
- Participate in key milestone reviews (kickoff, mid-point, release sign-off)

### Goals
- Protect strategic investment and ensure business value is delivered
- Remove organizational blockers quickly to keep the project on track
- Maintain trust and confidence of senior leadership in the project

### Typical Communication
- Monthly executive stakeholder update (written brief)
- Milestone review presentations
- Escalation responses (ad hoc)

### Key Interactions
- **Project Manager**: primary day-to-day liaison; escalation path for blockers
- **Product Manager**: aligns on roadmap priority and business outcomes
- **Business Analyst**: validates that business requirements reflect organizational intent
- **Release Coordinator**: approves high-risk or high-visibility release decisions

### Artifacts Owned
- Project charter approval
- Budget/resource approval records
- Escalation decision log

### RACI Notes
| Activity | Stakeholder Sponsor |
|---|---|
| Budget/resource approval | **Accountable** |
| Strategic direction | **Accountable** |
| Scope-change approval | **Accountable** |
| Escalation resolution | **Accountable** |
| Milestone review sign-off | Responsible |

> **Supporting template:** [Stakeholder Update Template](templates/stakeholder-update-template.md)

---

## Agile Coach

### Role Summary
The Agile Coach facilitates agile ceremonies, mentors the team on agile best practices, and continuously identifies process improvement opportunities to increase team effectiveness and delivery flow.

### Responsibilities
- Facilitate retrospectives, sprint planning, daily standups, and sprint reviews
- Coach team members and leadership on agile principles and practices
- Identify and remove process impediments and inefficiencies
- Guide adoption of agile metrics (velocity, cycle time, lead time)
- Protect the team from scope creep and unplanned interruptions
- Support formation of high-performing, self-organizing teams

### Goals
- Increase team velocity, predictability, and morale
- Embed continuous improvement as a team habit
- Reduce waste and non-value-adding activities in the delivery process

### Typical Communication
- Retrospective notes and action items
- Process improvement proposals and experiment reports
- Agile health-check assessments

### Key Interactions
- **Project Manager**: partners to improve planning and delivery cadence
- **Tech Lead**: addresses technical process friction (e.g., long PR review cycles)
- **Developers**: fosters a culture of collaboration and continuous learning
- **Product Manager**: ensures backlog health and supports refined prioritization
- **Stakeholder Sponsor**: educates on agile principles and sets expectations

### Artifacts Owned
- Retrospective action log
- Agile health-check results
- Team working agreements

### RACI Notes
| Activity | Agile Coach |
|---|---|
| Ceremony facilitation | **Accountable** |
| Process improvement proposals | Responsible |
| Agile coaching sessions | **Accountable** |
| Team working agreements | Responsible |
| Velocity/metrics review | Consulted |

> **Supporting template:** [Agile Ceremonies Checklist](templates/agile-ceremonies-checklist.md)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

