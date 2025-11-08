# OctoAcme — Roles and Personas

Purpose
-------
This document lists the project roles and personas used across OctoAcme project management processes. It defines responsibilities, interactions with existing roles, decision authority (where applicable), and examples of activities. Use this document to clarify accountability, avoid overlaps, and speed onboarding.

Scope
-----
Applies to all OctoAcme projects and supplements the project management process documents (initiation, planning, execution, risks & communication, release & deployment, retrospective). New personas below are intended to complement existing roles (Project Manager, Product Owner, Engineering Lead, QA Lead, Architects, Devs, Ops, and Stakeholders).

Guidelines for use
------------------
- Each project may assign one or more personas depending on size and complexity.
- Where responsibilities overlap, assign a primary owner and a secondary/backfill.
- Document assigned people and contact points in the project charter.

New / Clarified Personas
------------------------

### Release Manager
Summary:
Oversees release planning, orchestration, and delivery; ensures release quality, compliance, and communication.

Responsibilities:
- Maintain and publish release calendar and cutoffs.
- Coordinate cross-team release readiness activities (code freeze, migrations, feature toggles).
- Verify that release criteria (QA signoffs, security scans, configuration, rollback plans) are met.
- Escalate release blockers and facilitate resolution.
- Coordinate deployment windows with Ops and stakeholders.

Interacts with:
- Project Manager: align release timeline with project milestones.
- Development / Engineering Lead: verify release contents and readiness.
- QA Lead: obtain test signoffs and regression results.
- Ops / SRE: coordinate deployment runbooks and rollback procedures.
- Communications Lead: prepare release notices.

Decision Authority:
- Approves (or postpones) release go/no-go based on defined criteria.

Example activities:
- Run release readiness checklist 48 hours before deployment.
- Facilitate go/no-go meeting and publish release notes.

---

### Risk Coordinator
Summary:
Central point for identifying, tracking, and managing project risks and mitigations.

Responsibilities:
- Maintain a project risk register and coordinate regular risk reviews.
- Ensure each risk has an owner, impact, likelihood, and mitigation plan.
- Facilitate cross-functional workshops for risk identification and escalation.
- Track mitigation status and surface unresolved high-impact risks to leadership.

Interacts with:
- Project Manager: ensure risks are reflected in project plan and schedule.
- Architects / Engineering Lead: technical risk assessment and mitigation.
- Product Owner / Stakeholder Liaison: business and stakeholder-related risk identification.
- PMO / Governance: escalate risks that impact portfolio-level decisions.

Decision Authority:
- Nominates risk owners and recommends escalations; escalation decisions follow project governance.

Example activities:
- Weekly risk triage meeting and updates to the project dashboard.
- Produce risk heatmap for steering committee.

---

### Communications Lead
Summary:
Manages internal and external communication strategy and artifacts for the project.

Responsibilities:
- Maintain communication plan, including cadence, channels, and audience mapping.
- Draft and publish status updates, stakeholder briefings, and release communications.
- Ensure messaging consistency across teams and documents.
- Coordinate stakeholder meetings, demos, and town-hall briefings.

Interacts with:
- Project Manager: align messaging with project status and key milestones.
- Stakeholder Liaison: validate stakeholder messaging and expectations.
- Release Manager: coordinate release announcements.
- Marketing / Legal (if applicable): approve external-facing communications.

Decision Authority:
- Approves communication templates and publishing cadence; final signoff for external comms may require stakeholder or legal approval.

Example activities:
- Create and distribute weekly status bulletin.
- Draft customer-facing release notes with Release Manager.

---

### Data Analyst (Project Metrics)
Summary:
Provides quantitative insight into project performance through metrics, dashboards, and trend analysis.

Responsibilities:
- Define and track key project metrics (velocity, cycle time, defect rates, test coverage, deployment frequency).
- Build and maintain dashboards and periodic reports.
- Analyze trends and provide recommendations to improve delivery predictability.
- Validate data used in stakeholder reporting.

Interacts with:
- Project Manager: provide status metrics and forecasts.
- QA Lead: collect quality metrics and defect trend analysis.
- Engineering Lead: share engineering productivity and bottleneck analyses.
- Risk Coordinator: support data-driven risk identification.

Decision Authority:
- Advises on metric definitions and triggers for corrective action; does not unilaterally change project plan.

Example activities:
- Weekly metrics dashboard update and a short interpretation note.
- Run root-cause analysis on growing defect trends.

---

### Stakeholder Liaison
Summary:
Primary contact for stakeholder engagement; translates stakeholder needs to the project team and ensures stakeholder expectations are managed.

Responsibilities:
- Maintain stakeholder register and communication preferences.
- Collect stakeholder feedback and issues; route to appropriate owners.
- Prepare stakeholder-specific briefings and approvals.
- Manage expectation alignment when scope or schedule changes are proposed.

Interacts with:
- Product Owner / Project Manager: translate stakeholder priorities into backlog/plan items.
- Communications Lead: ensure stakeholder messaging is clear and tailored.
- Risk Coordinator: bring stakeholder concerns into risk discussions.

Decision Authority:
- Can request escalations or pause non-critical activities pending stakeholder clarification; final decisions follow governance.

Example activities:
- Run stakeholder feedback sessions after demos.
- Prepare summarized stakeholder feedback for the PM and Product Owner.

---

Clarifying interactions with existing roles
-------------------------------------------
- Project Manager (PM): central integrator. PM coordinates planning, dependencies, and schedules. New personas provide domain-specific execution and information (e.g., Release Manager handles the operational release checklist while PM ensures release fits the plan).
- Product Owner (PO): prioritizes scope and features. Stakeholder Liaison and Communications Lead help align external expectations with the PO.
- Engineering / QA Leads: retain technical and quality ownership. Risk Coordinator and Data Analyst support their decisions with risk assessments and metrics.
- Ops / SRE: own production stability. Release Manager must coordinate deployment mechanics with Ops.

Suggested RACI pattern (example)
--------------------------------
- Release planning: R=Release Manager, A=Project Manager, C=Engineering Lead / QA Lead / Ops, I=Stakeholders
- Risk register maintenance: R=Risk Coordinator, A=Project Manager, C=All team leads, I=Stakeholders
- Stakeholder updates: R=Communications Lead / Stakeholder Liaison, A=Project Manager, C=Product Owner, I=Stakeholders

How these personas improve outcomes
----------------------------------
- Clear ownership reduces handoff delays (Release Manager for releases; Risk Coordinator for risks).
- Better stakeholder alignment reduces rework and late-scope changes (Stakeholder Liaison).
- Data-driven interventions help catch trends early and improve predictability (Data Analyst).
- Consistent messaging reduces confusion and increases trust (Communications Lead).

Acceptance Criteria (for adding these personas to process docs)
---------------------------------------------------------------
- Content aligns with the structure and language of existing process documents.
- Each persona has a clear set of responsibilities and named interactions with existing roles.
- Example activities and decision authorities are included to support implementation.
- Document reviewed by at least one PM and one engineering lead for accuracy.

Next steps & governance
-----------------------
1. Review this draft with the PM and Engineering lead for the project(s) that will adopt these personas.
2. Adjust responsibilities to reflect project size (e.g., in small projects, personas may be combined).
3. Publish under docs/ and reference from octoacme-project-planning.md and octoacme-release-and-deployment.md.
4. Track adoption feedback during the next retrospective and iterate.

Change history
--------------
- 2025-11-08 — Initial draft adding Release Manager, Risk Coordinator, Communications Lead, Data Analyst, and Stakeholder Liaison.