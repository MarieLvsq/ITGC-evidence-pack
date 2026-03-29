# WP-01 — Access Controls (JML & RBAC)

## Workpaper metadata
- Workpaper ID: WP-01
- Control(s): AC-01, AC-02, AC-03, AC-04
- Period: Last full month (fictional)
- Prepared by: <Your Name>
- Reviewer: <Mock Reviewer>
- Date: <YYYY-MM-DD>

## Control objective
Ensure user access is provisioned, modified, and removed based on authorised requests and within defined SLAs, reducing risk of unauthorised access.

## Population
- Joiners in period: 42
- Movers in period: 18
- Leavers in period: 11
- Access reviews: 1 quarterly review in scope (if applicable)

## Sampling method
- Joiners: 10 random
- Movers: 5 random
- Leavers: 5 random
- Access review: inspect the latest review evidence and sample 3 exceptions (if any)

## Test steps
1. Obtain HR JML report for period.
2. Obtain IAM export of user accounts and status timestamps.
3. For each sampled item:
   - verify approved request exists (manager/system owner)
   - verify role assigned matches request
   - verify timestamps meet SLA (joiner before first day; leaver disable within SLA)
4. For access review:
   - verify review occurred, has approver sign-off
   - verify exceptions have remediation tickets and closure evidence

## Evidence obtained (examples)
- HR JML export (sanitised sample)
- IAM account export (sanitised sample)
- Ticket IDs for JML requests (placeholders)
- Quarterly access review sign-off (placeholder)

## Results
- Joiners: 9/10 pass, 1 exception
- Movers: 5/5 pass
- Leavers: 3/5 pass, 2 exceptions
- Access review: review performed; 1 exception remediated; 1 exception pending

### Exceptions
- EX-01: Leaver disable occurred 48h after termination notice (SLA: 24h).
- EX-02: Leaver disable occurred 72h after termination notice (SLA: 24h).
- EX-03: Joiner request missing explicit manager approval artefact (approval implied, not evidenced).

## Conclusion
Control operating effectiveness: **Needs improvement** (exceptions for timely deprovisioning and approval evidence).

## Reviewer sign-off
- Reviewer: ____________________
- Date: ________________________
