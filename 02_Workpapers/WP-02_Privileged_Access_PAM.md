# WP-02 — Privileged Access (PAM / Admin)

## Metadata
- Workpaper ID: WP-02
- Control(s): PA-01, PA-02, PA-03, PA-04
- Period: Last full month (fictional)
- Prepared by / Reviewer / Date: <...>

## Control objective
Ensure privileged access is restricted, approved, logged, and reviewed to reduce risk of misuse or unauthorised changes.

## Population
- Privileged sessions (period): 38
- Break-glass events: 2

## Sampling
- Privileged sessions: 10
- Break-glass: 2 (all)

## Test steps
1. Obtain privileged account inventory and owners.
2. For each sampled privileged session:
   - verify ticket exists and approval recorded
   - verify time-bound access where applicable
   - verify session logs exist
3. For monthly review:
   - verify evidence of review/sign-off and follow-up actions
4. For break-glass:
   - verify time-bound use + post-use review documented

## Evidence obtained
- Admin inventory export (placeholder)
- PAM tickets and approvals (placeholder)
- Session logs (placeholder)
- Review sign-off (placeholder)

## Results
- 8/10 privileged sessions pass
- 2/10 missing explicit approval artifact
- Break-glass events: 2/2 pass (post-review present)

## Conclusion
Operating effectiveness: **Partially effective** (approval evidence gaps).

## Reviewer sign-off
<...>
