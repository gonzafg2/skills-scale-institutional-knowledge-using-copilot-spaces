# OctoAcme Project Management Docs

Welcome to the OctoAcme project management process documentation. This README provides an overview of how OctoAcme runs projects and links out to all the process documents that guide our work.

## Overview

OctoAcme's project management approach follows a lightweight, repeatable lifecycle: **initiation → planning → execution → release → close/retro**. During **initiation**, teams validate the business need and clarify success metrics, stakeholders, timelines, risks, and resource needs via a concise one-pager and an explicit go/no-go decision gate. Once approved, **planning** turns the initiative into an actionable backlog by holding a kickoff, defining acceptance criteria and a Definition of Done, estimating work, mapping milestones and releases, and capturing dependencies and risks in a simple risk register.

Delivery is driven through a consistent **execution and tracking workflow** centered on a project board with clear states (Backlog → Ready → In Progress → In Review → QA → Done). Teams aim for small pull requests, include issue links and acceptance criteria in PR descriptions, and rely on CI (tests, linting, security scans) before requesting review. Progress is monitored via delivery metrics such as velocity and burndown, supported by dashboards for operational signals like errors, latency, and usage.

Roles are explicitly defined to keep ownership unambiguous: a **Project Manager (PM)** coordinates delivery, schedules, risks, and communications; a **Product Manager (PdM)** defines outcomes, prioritizes the backlog, and measures impact; **Developers** implement, write tests, and collaborate on design and reviews; **QA/Testing** validates acceptance criteria and overall quality; and **Stakeholders** provide inputs and approvals. This clarity is reinforced by shared artifacts — charter/one-pager, backlog, DoD, risk register, release notes, and retro action items — so decisions and context remain visible and durable.

Communication and quality practices are baked into the day-to-day cadence. OctoAcme uses daily standups, weekly delivery syncs, periodic demos/reviews, and regular stakeholder updates, with structured escalation paths for blockers and incidents. Quality assurance emphasizes unit and integration testing, end-to-end smoke tests for critical flows, manual QA when needed, and pre-release requirements including passing CI/security scans along with a rollback/mitigation plan and post-deploy verification. After sprints, releases, and incidents, retrospectives convert lessons learned into owned action items with due dates, reinforcing continuous improvement over time.

## Docs Index

- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)
- [RACI Responsibility Mapping Template](./octoacme-raci-template.md)
- [Decision Log Template & Guidance](./octoacme-decision-log.md)
- [Dependency Handoff Checklist](./octoacme-dependency-handoff-checklist.md)
- [Definition of Ready](./octoacme-definition-of-ready.md)
