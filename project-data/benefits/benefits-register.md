# Benefits Register

> **DUMMY DATA** (Project Gateway Switch). No benefits are realised before cutover (2027-03-27), so Actual is "—" for now.

| ID | Benefit | Measure | Baseline | Target | Forecast | Actual | Owner | Realisation date | Status |
|---|---|---|---|---|---|---|---|---|---|
| B-001 | Lower payment processing cost | Blended cost per transaction (GBP) | 0.42 | 0.31 | 0.32 | — | Lena Fischer | 2027-06-30 (after PayLink decommission) | At risk (corrected 2026-11-17 from On track: forecast 0.32 is 0.01 short of target 0.31; volume tier assumption AS-004 still open) |
| B-002 | Higher authorisation rate | % of attempted transactions approved | 91.5% | 93.5% | 93.0% | — | Dev Patel | 2027-06-30 | At risk (3DS2 issue I-002 may hold the uplift back) |
| B-003 | Faster settlement | Days from transaction to funds received | T+3 | T+1 | T+1 | — | Omar Haddad | 2027-04-30 | On track |
| B-004 | Better platform availability | Gateway downtime, minutes per year | 480 | 120 | 150 | — | Dev Patel | 2027-12-31 (12 months of data needed; see note 6) | At risk (corrected 2026-11-17 from On track: forecast 150 min is 30 min above target 120; date gives under 12 months of post-cutover data) |
| B-005 | Lower manual reconciliation effort | Finance FTE-days per month | 22 | 8 | 10 | — | Omar Haddad | 2027-06-30 | At risk (reconciliation build behind plan, I-004) |
| B-006 | Annual cost saving (financial) | £k per year, run-rate | 0 | 540 | 480 | — | Priya Raman | 2027-12-31 | At risk (forecast about £60k below target) |

## Notes
- B-006 is stated to be derived from B-001 at an assumed 18m transactions a year. The volume figure is an assumption to validate with Finance. **It does not reconcile (review 2026-11-17):** 18m x (0.42 - 0.31) = GBP 1,980k against a B-006 target of 540k; 18m x (0.42 - 0.32) = GBP 1,800k against a forecast of 480k; the stated gap of 60k compares with 180k implied by 18m x 0.01. Back-solving gives about 4.9m (target) and 4.8m (forecast) transactions, which differ from each other and from 18m. The true volume is not in project-data and is not assumed here. Treat B-006 figures as unvalidated until Finance confirms the volume and whether B-006 is net of other items (for example NovaPay licence/run costs or PayLink run-cost saving, which is not in the budget).
- Benefits are measured against the baseline period Nov 2025–Oct 2026.
- Status rule applied (2026-11-17): a benefit whose forecast misses target is At risk (Amber). No benefit tolerance is defined in the charter, so none is Red.
- Counts after review: On track 1 (B-003), At risk 5 (B-001, B-002, B-004, B-005, B-006), Off track 0. The 2026-11-14 status report says three of six at risk and should be updated.
- Charter traceability: B-001, B-002, B-003 map to objectives 2, 3, 4. B-004, B-005, B-006 have no charter objective (B-006 is the financial expression of B-001); confirm with the sponsor whether to add them. Objectives 1 and 5 are delivery outcomes, not benefits.
- Timing: B-003 (2027-04-30) falls about 5 weeks after cutover 2027-03-27 and relies on settlement data in that window. B-001 and B-006 depend on PayLink decommission (2027-06-30); B-006 is dated 2027-12-31 while B-001 is 2027-06-30, so confirm the run-rate basis. Schedule tolerance on cutover is 2 weeks; a slip moves all dates.
- Note 6: 12 months of data from cutover 2027-03-27 ends about 2028-03-27, so B-004 at 2027-12-31 gives about 9 months. Either re-date or accept a shorter measurement window (owner decision).
