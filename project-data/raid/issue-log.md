# Issue Log

> **DUMMY DATA** (Project Gateway Switch).

| ID | Description | Severity | Impact | Owner | Raised | Target date | Status | Escalation |
|---|---|---|---|---|---|---|---|---|
| I-001 | NovaPay sandbox was unstable for 9 working days in October (intermittent 503s on the authorisation endpoint). | High | Sandbox integration milestone slipped from 2026-10-31 to 2026-11-21 (3 weeks). Feeds R-001. | Dev Patel | 2026-10-12 | 2026-11-21 | In progress (vendor fix deployed 2026-11-10, retesting) | Raised with NovaPay account director; SteerCo informed |
| I-002 | 3DS2 challenge flow fails for a subset of issuer banks (about 4% of test cards). | High | Could reduce authorisation rate benefit (B-002) if not fixed before pilot. Also relates to DEP-002 (certified 3DS2 configuration). | Dev Patel | 2026-11-03 | 2026-12-04 | In progress | None at present |
| I-003 | Test data refresh from production is blocked pending data-protection sign-off for masked card data. | High (raised from Medium 2026-11-17: blocks a critical-path milestone) | UAT environment cannot be populated; UAT start 2027-01-18 at risk. Peak freeze (2026-11-20 to 2027-01-04) leaves little time to recover. Feeds R-001; depends on DEP-004; test-env availability during freeze relies on AS-002 (unvalidated). | Sam Okafor | 2026-11-06 | 2026-11-27 | Open | Escalate to sponsor if not resolved by 2026-11-27 (sponsor ask already in 2026-11-14 status for SteerCo) |
| I-004 | Finance Systems developer on long-term leave; reconciliation feed build behind plan by about 2 weeks. | Medium | Pressure on R-005, DEP-005 (feed build due 2027-01-29, before pilot 2027-02-08), B-005 and the finance sign-off gate. | Omar Haddad | 2026-11-10 | 2026-12-11 | Open | None at present |
| I-005 | PayLink API rate-limit changes announced for January, affecting the dual-running period. | Low | May throttle migration rehearsals (R-002) and the DEP-003 history export. Exact January date not recorded. | Mei Tanaka | 2026-11-12 | 2026-12-18 | Open | None |
