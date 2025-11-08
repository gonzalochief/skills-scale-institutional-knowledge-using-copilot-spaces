# OctoAcme — Risk Register Template & Guidance

Purpose
-------
A simple, consistent risk register template and guidance to support identification, tracking, and mitigation of project risks.

Risk Register (table template)
------------------------------
| ID | Description | Owner | Impact (H/M/L) | Likelihood (H/M/L) | Priority | Mitigation / Action | Status | Detection Date | Review Cadence |
|----|-------------|-------|----------------|---------------------|----------|---------------------|--------|----------------|----------------|
| R-001 | Short description of the risk | Name (role) | H | M | High | Steps to mitigate or reduce impact | Open / Mitigated / Closed | YYYY-MM-DD | Weekly / Monthly |

Fields explained
--------------
- ID: Unique risk identifier (R-001, R-002, etc.).
- Description: Concise description of the risk scenario and potential impact.
- Owner: Person/role responsible for tracking and executing mitigation.
- Impact: Severity if the risk materializes (High / Medium / Low).
- Likelihood: Probability of occurrence (High / Medium / Low).
- Priority: Derived from impact & likelihood (High/Medium/Low).
- Mitigation / Action: Specific steps to reduce likelihood or impact; contingency plan.
- Status: Current status (Open, Monitoring, Mitigated, Closed).
- Detection Date: When the risk was first logged.
- Review Cadence: How often the risk will be reviewed (e.g., weekly).

How-to & governance
-------------------
- Maintain one register per project (or per major release for larger programs).
- Hold a weekly risk triage meeting (led by Risk Coordinator or PM) to:
  - Review new risks and assign ownership
  - Update mitigation progress
  - Escalate high-priority items to PMO or steering committee
- Create a risk heatmap for quarterly steering reviews for portfolio-level visibility.

Escalation guidance
-------------------
- Escalate to Project Manager when a risk becomes high priority or mitigation requires schedule/financial trade-offs.
- Escalate to PMO/Governance when risks impact cross-project dependencies or portfolio commitments.

Example entry
-------------
| R-001 | Backend database schema migration may cause downtime | Engineering Lead | H | M | High | Create migration with blue-green approach; pre-run on staging; rollback snapshot | Open | 2025-11-01 | Weekly |