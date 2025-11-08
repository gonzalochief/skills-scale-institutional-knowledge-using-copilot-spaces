# OctoAcme — Release Checklist

Purpose
-------
A practical pre-release checklist to be used by Release Manager and Project Manager to ensure releases are safe, predictable, and well-communicated.

Owner
-----
Primary: Release Manager
Informed: Project Manager, Engineering Lead, QA Lead, Ops

Timing and checkpoints
----------------------
- T-48 hours: Release readiness review (high-level)
- T-24 hours: Detailed pre-release checklist run
- T-1 hour: Final runbook & monitoring check
- Deployment window: Go/No-Go meeting and execution
- Post-deploy (T+1 hour, T+24 hours): Verify monitoring and rollback markers

Pre-release checklist (example)
-------------------------------
- Release calendar entry published and stakeholders informed.
- Release notes drafted and reviewed.
- Feature list validated and release scope confirmed.
- QA signoffs completed (regression, acceptance tests).
- Security scans completed and critical issues resolved or accepted with mitigations.
- Database migrations planned, reviewed, and rollback steps verified.
- Deployment runbook ready and reviewed with Ops/SRE.
- Rollback plan and smoke tests prepared.
- Monitoring/alerting configured for post-release checks.
- Feature flags / toggles reviewed and validated.
- Backups / snapshots created where applicable.
- Approvals captured (as per governance).
- Communications plan for the release drafted (internal & external).

Go / No-Go meeting (example agenda)
----------------------------------
1. Review release scope and critical changes.
2. Confirm QA and security signoffs.
3. Confirm Ops readiness and deployment window.
4. Review rollback plan and monitoring.
5. Final list of known risks / mitigations.
6. Vote/decision (Release Manager recommends, Project Manager approves).

Post-release
------------
- Confirm post-deploy smoke tests pass.
- Monitor metrics for regressions (error rate, latency, key transactions).
- Publish release summary and retrospective notes.
- If issues occur, follow rollback/runbook and conduct incident retrospective.

Customization notes
-------------------
- For small projects, PM may act as Release Manager.
- For high-risk or high-visibility releases, increase cadence of readiness checks and require stakeholder signoff.

Template: Ownership and timing (example)
- T-48h: Release Manager — run readiness; notify stakeholders
- T-24h: Release Manager — confirm QA signoffs; Ops runbook review
- T-1h: Ops/Release Manager — final checks
- Deploy: Release Manager + Ops — execute; Project Manager — communicate