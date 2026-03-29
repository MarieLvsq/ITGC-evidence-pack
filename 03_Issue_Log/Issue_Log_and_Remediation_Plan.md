# Issue Log & Remediation Plan (3 Findings)

| Finding ID | Severity | Related Control(s) | Condition (What happened) | Risk | Root Cause | Recommendation | Owner | Target Date | Status | Retest Approach |
|---|---|---|---|---|---|---|---|---|---|---|
| F-01 | High | AC-03 | 2/5 leaver accounts disabled after SLA (24h). | Former users retain access; unauthorized activity risk. | Manual HR→IT handoff; no daily exception report. | Automate termination trigger; add daily exceptions report; weekly KPI review. | IAM Owner | +30 days | Open | Re-test next month leaver sample; verify SLA compliance + evidence. |
| F-02 | Medium | CH-02 / CH-04 | 3/10 prod changes missing explicit approval/testing artifact. | Unauthorized/untested change risk; outages/compliance breaches. | Ticket workflow allows missing fields; pipeline not gated. | Enforce mandatory approval/testing fields; block deploy without artifacts. | Release Manager | +45 days | Open | Re-sample 10 changes; confirm approvals and UAT evidence present. |
| F-03 | Medium | BK-03 | Restore test performed but incomplete documentation/sign-off. | Recovery may fail during incident; inability to prove readiness. | No standard restore test template or sign-off owner. | Implement restore test template + quarterly sign-off + evidence storage. | Ops Lead | +60 days | Open | Inspect next quarterly restore test evidence and sign-off. |
