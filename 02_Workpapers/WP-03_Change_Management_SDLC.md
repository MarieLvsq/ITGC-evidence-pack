# WP-03 — Change Management (SDLC / Release Controls)

## Metadata
- Workpaper ID: WP-03
- Control(s): CH-01, CH-02, CH-03, CH-04, CH-05
- Period: Last full month (fictional)

## Control objective
Ensure production changes are authorised, tested, traceable, and appropriately segregated to reduce risk of unauthorised or faulty changes.

## Population
- Production deployments in period: 26

## Sampling
- 10 deployments (random)

## Test steps
For each sampled deployment:
1. Verify change ticket exists (CH-01)
2. Verify approval exists and is pre-deployment (CH-02)
3. Verify SoD evidence (CH-03) (roles/permissions or independent approval)
4. Verify testing evidence attached (CH-04)
5. Verify traceability: ticket → commit/tag → pipeline/deploy log (CH-05)

## Evidence obtained
- Ticket screenshots (placeholder)
- Approval fields (placeholder)
- Test reports/UAT sign-off (placeholder)
- Pipeline logs/deployment logs (placeholder)
- Git tag references (placeholder)

## Results
- 7/10 pass
- 3/10 missing explicit approval or testing artefact

## Conclusion
Operating effectiveness: **Needs improvement** (approval/testing evidence enforcement recommended).
