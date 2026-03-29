# WP-04 — Backups & Restore Testing

## Metadata
- Workpaper ID: WP-04
- Control(s): BK-01, BK-02, BK-03, BK-04
- Period: Last 30 days (fictional) + latest quarterly restore test

## Control objective
Ensure backups are performed, monitored, protected, and recovery is validated.

## Population
- Daily backup jobs: 30 (per system)
- Backup failures: 3
- Restore tests: 1 quarterly test

## Sampling
- 10 daily backup jobs
- All failures (3)
- Restore test (1)

## Test steps
1. Inspect backup schedule configuration (BK-01)
2. Inspect backup success/failure reports (BK-02)
3. For failures: verify alerts/tickets and resolution evidence (BK-02)
4. Inspect restore test evidence and sign-off (BK-03)
5. Inspect backup access permissions (BK-04)

## Results
- Schedule configured and consistent
- Failures: 2/3 resolved with evidence, 1 missing follow-up ticket
- Restore test performed but documentation incomplete

## Conclusion
Operating effectiveness: **Partially effective** (improve restore documentation and failure ticketing).
