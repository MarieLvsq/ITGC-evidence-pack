# ITGC Control Matrix (25 Controls)

Columns:
- Control ID
- Domain
- Control Statement
- Frequency
- Evidence Examples
- Test Approach (high level)

| Control ID | Domain | Control Statement | Frequency | Evidence Examples | Test Approach |
|---|---|---|---|---|---|
| AC-01 | Access (JML) | Joiner access is provisioned only upon approved request and role definition. | Per event | Ticket + approval + IAM record | Sample joiners; verify approval precedes provisioning. |
| AC-02 | Access (JML) | Mover access changes are processed within defined SLA with approval. | Per event | HR change + ticket + IAM delta | Sample movers; verify timely update and approval. |
| AC-03 | Access (JML) | Leaver access is disabled within SLA upon termination notice. | Per event | HR termination + disable logs | Sample leavers; verify disable timestamp within SLA. |
| AC-04 | Access Review | Periodic user access review is performed and signed off; exceptions remediated. | Quarterly | Review sign-off + remediation tickets | Inspect review; sample exceptions; verify remediation. |
| AC-05 | Authentication | MFA/password policy enforced for key systems. | Continuous | Config screenshot + policy | Inspect settings; verify compliance with policy baseline. |
| PA-01 | Privileged | Privileged accounts are inventoried and owners assigned. | Monthly | Admin account list + owner mapping | Inspect inventory; verify completeness and ownership. |
| PA-02 | Privileged | Privileged access requires ticket + approval before activation. | Per event | PAM request + approval | Sample privileged sessions; verify approval and scope. |
| PA-03 | Privileged | Privileged activity is logged and reviewed. | Monthly | PAM logs + review sign-off | Inspect logs and review evidence; sample review notes. |
| PA-04 | Privileged | Break-glass access is time-bound and reviewed post-use. | Per event | Break-glass ticket + post-review | Sample break-glass events; verify time-bound + review. |
| CH-01 | Change | All production changes are logged via a change record. | Per event | Change tickets + release notes | Sample changes; verify presence of change record. |
| CH-02 | Change | Changes require approval prior to implementation (CAB/owner). | Per event | Approval field + approver identity | Sample changes; verify approvals exist pre-deploy. |
| CH-03 | Change | Segregation of duties enforced for dev/approve/deploy where applicable. | Continuous | Role matrix + pipeline permissions | Inspect role model; sample changes for SoD evidence. |
| CH-04 | Change | Testing evidence (QA/UAT) is attached before deployment. | Per event | Test results + UAT sign-off | Sample changes; verify testing evidence exists. |
| CH-05 | Change | Release traceability links ticket → commit/tag → deployment. | Per event | Git tag + pipeline logs | Sample changes; verify end-to-end traceability. |
| BK-01 | Backup | Backup schedules are configured per policy (systems in scope). | Continuous | Backup config + schedule report | Inspect schedules; verify coverage. |
| BK-02 | Backup | Backup job failures are alerted and remediated timely. | Daily | Failure alerts + incident/ticket | Sample failures; verify follow-up and resolution. |
| BK-03 | Recovery | Restore tests are performed and documented. | Quarterly | Restore report + sign-off | Inspect latest restore test evidence. |
| BK-04 | Backup | Backup access restricted to authorized roles. | Continuous | Access list + role permissions | Inspect access lists; verify least privilege. |
| LM-01 | Logging | Key systems forward logs to centralized logging/SIEM. | Continuous | Logging config screenshot | Inspect forwarding settings; verify coverage. |
| LM-02 | Logging | Log retention meets policy requirements. | Continuous | Retention settings + policy | Inspect retention configs vs policy. |
| LM-03 | Monitoring | Alerts are triaged and tracked through tickets. | Continuous | Alert → ticket link | Sample alerts; verify triage + closure evidence. |
| LM-04 | Monitoring | Periodic review of monitoring dashboards is evidenced. | Monthly | Review sign-off + notes | Inspect review documentation and follow-ups. |
| IM-01 | Incident | Incidents are recorded, classified, and assigned owners. | Per event | Incident tickets | Sample incidents; verify severity, owner, timestamps. |
| IM-02 | Incident | Major incidents have RCA and corrective actions. | Per event | RCA document + action items | Inspect major incident; verify RCA + actions. |
| IM-03 | Incident | Lessons learned tracked to closure and communicated. | Per event | Post-mortem + closure evidence | Inspect completion evidence for actions. |
