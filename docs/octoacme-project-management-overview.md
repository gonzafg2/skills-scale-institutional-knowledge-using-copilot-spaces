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
- QA Automation Specialist: builds and maintains automated test suites integrated into CI/CD.
- UX/UI Designer: designs user flows, interfaces, and prototypes.
- DevOps/Infrastructure Engineer: manages CI/CD pipelines, environments, and release operations.
- Stakeholders (Business Owner, End User, SME): provide inputs, approvals, and domain expertise.

See [Roles & Personas](./octoacme-roles-and-personas.md) for full descriptions and interaction maps.

## Key Artifacts
- Project Charter / One-pager
- Roadmap and Release Plan
- Sprint/Iteration Backlog
- Acceptance Criteria & Definition of Done
- [Definition of Ready](./octoacme-definition-of-ready.md)
- Risk Register
- [Decision Log](./octoacme-decision-log.md)
- [RACI Responsibility Matrix](./octoacme-raci-template.md)
- [Dependency Handoff Checklist](./octoacme-dependency-handoff-checklist.md)
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
