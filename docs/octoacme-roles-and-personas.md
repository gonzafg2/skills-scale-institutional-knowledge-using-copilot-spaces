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
QA/Testing engineers validate that delivered features meet acceptance criteria, quality standards, and performance expectations before release.

### Responsibilities
- Review acceptance criteria and define test cases
- Perform functional, regression, and exploratory testing
- Log, track, and verify defects to closure
- Participate in sprint reviews and release readiness sign-offs
- Communicate quality risks to the Project Manager and team

### Goals
- Ensure every release meets the Definition of Done
- Reduce defect escape rate to production
- Provide timely quality feedback that unblocks delivery

### Typical Communication
- Bug reports and test summary reports
- Participation in sprint planning and review ceremonies
- Close collaboration with Developers on defect triage

### Interactions with Other Roles
- **Project Manager**: reports release readiness and quality blockers
- **Product Manager**: clarifies acceptance criteria and edge cases
- **Developers**: pairs on bug reproduction and test coverage
- **Stakeholders**: escalates critical quality issues that affect user acceptance

---

## Stakeholders

Stakeholders represent the people and groups most affected by project outcomes. They provide context, approvals, and feedback that shape what gets built and how it is prioritised.

### Business Owner

#### Role Summary
Business Owners are accountable for the business case and return on investment. They authorize resources and have final say on scope and priorities at the portfolio level.

#### Responsibilities
- Approve project charter and business case
- Provide budget and resource authorization
- Resolve escalated scope or priority conflicts
- Review milestone outcomes and approve launch

#### Goals
- Maximize business value and ROI from the investment
- Ensure project outcomes align with organizational strategy

#### Typical Communication
- Monthly or milestone-based executive briefings
- Formal approval at key decision gates (go/no-go)

#### Interactions with Other Roles
- **Project Manager**: receives escalations, budget, and priority decisions
- **Product Manager**: aligns business strategy with product vision
- **Developers / QA**: rarely direct; informed via PM or PdM updates

---

### End User

#### Role Summary
End Users are the people who will directly use the delivered product or service. Their needs and feedback are the primary driver of product quality and usability.

#### Responsibilities
- Participate in user research, usability testing, and beta programs
- Provide feedback on prototypes and early releases
- Raise adoption barriers and usability concerns

#### Goals
- Access a solution that solves real workflow or business problems
- Experience minimal disruption during transitions or releases

#### Typical Communication
- Usability test sessions and surveys
- Beta feedback channels and support tickets
- User acceptance testing (UAT) sessions

#### Interactions with Other Roles
- **Product Manager**: primary channel for capturing user needs
- **UX/UI Designer**: provides feedback on designs and prototypes
- **QA/Testing**: participates in UAT sign-off

---

### Subject Matter Expert (SME)

#### Role Summary
SMEs bring specialized domain knowledge—regulatory, technical, or operational—that the core team relies on to make accurate, compliant, and feasible decisions.

#### Responsibilities
- Answer domain-specific questions and validate assumptions
- Review requirements and designs for accuracy and compliance
- Flag domain risks that the core team may not anticipate

#### Goals
- Ensure the delivered solution is accurate and fit for purpose in the target domain
- Transfer enough domain knowledge to the team for sustainable ownership

#### Typical Communication
- Ad-hoc consultation during discovery and design phases
- Written reviews of specs or requirements documents
- Attendance at key milestone reviews as needed

#### Interactions with Other Roles
- **Product Manager**: validates requirements against domain constraints
- **Developers**: advises on domain logic and data rules
- **Project Manager**: flags compliance or domain risks to the risk register

---

## UX/UI Designer

### Role Summary
UX/UI Designers are responsible for the usability, accessibility, and visual consistency of the product. They translate user needs and product requirements into clear, testable designs.

### Responsibilities
- Conduct user research and translate findings into design requirements
- Create wireframes, prototypes, and high-fidelity designs
- Maintain a design system or style guide for consistency
- Collaborate with developers to ensure faithful implementation
- Validate designs through usability testing and iteration

### Goals
- Deliver intuitive, accessible experiences that meet user needs
- Reduce rework by involving design early in the feature lifecycle
- Keep design and implementation aligned throughout delivery

### Typical Communication
- Design files and annotated prototypes shared in design tools (e.g., Figma)
- Design review sessions with developers and Product Manager
- Usability test readouts and iteration notes

### Interactions with Other Roles
- **Product Manager**: receives feature requirements and aligns on user goals
- **Developers**: provides specs and reviews implementation for fidelity
- **End Users / Stakeholders**: runs research sessions and collects feedback
- **Project Manager**: surfaces design dependencies that affect timeline

---

## DevOps / Infrastructure Engineer

### Role Summary
DevOps/Infrastructure Engineers build and maintain the delivery pipeline, infrastructure, and operational tooling that enable the team to ship reliably and recover quickly from incidents.

### Responsibilities
- Design and maintain CI/CD pipelines and deployment automation
- Manage infrastructure-as-code and environment configuration
- Monitor system health and respond to operational incidents
- Support security scanning, secrets management, and compliance requirements
- Enable and document rollback procedures and disaster recovery processes

### Goals
- Maximize deployment frequency while minimizing change failure rate
- Reduce mean time to recovery (MTTR) for production incidents
- Keep infrastructure costs and toil in check

### Typical Communication
- Runbooks, infrastructure docs, and deployment guides
- Incident postmortems and on-call handoffs
- Participation in release planning and change advisory discussions

### Interactions with Other Roles
- **Developers**: reviews PRs for infrastructure impact; enables local dev environments
- **Project Manager**: communicates pipeline blockers and release dependencies
- **QA/Testing**: provisions test environments and supports test automation infrastructure
- **Stakeholders / Business Owner**: escalated during high-severity incidents affecting users

---

## QA Automation Specialist

### Role Summary
QA Automation Specialists design, build, and maintain automated test suites that provide fast, reliable quality feedback throughout the delivery pipeline.

### Responsibilities
- Develop and maintain automated test frameworks (unit, integration, end-to-end)
- Integrate automated tests into CI/CD pipelines
- Monitor test coverage, flakiness, and suite performance
- Identify testability gaps and work with Developers to close them
- Report on automation coverage and quality trends

### Goals
- Provide rapid, reliable quality feedback at every stage of delivery
- Increase confidence in releases by reducing reliance on manual regression
- Keep test suites maintainable and free of false positives

### Typical Communication
- Test coverage reports and CI quality dashboards
- Automation backlog updates in sprint planning
- Cross-functional pairing sessions with Developers on testability

### Interactions with Other Roles
- **Developers**: pairs on test design, testability improvements, and flaky test resolution
- **QA/Testing**: complements manual testing with automation coverage
- **DevOps/Infrastructure Engineer**: coordinates pipeline integration and environment stability
- **Project Manager**: provides automation status and flags coverage risks before release

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

