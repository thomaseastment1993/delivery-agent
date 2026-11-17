# Project Health Check: Project Gateway Switch

> **DUMMY DATA**: fictional project, for testing only.

- **Reporting date:** 2026-11-17 (Tuesday; ad hoc health check between weekly Friday reports, supersedes the 2026-11-14 position)
- **Delivery lead:** Thomas Eastment
- **Sponsor:** Priya Raman
- **Overall RAG:** **AMBER, trending Red** if the sandbox exit (2026-11-21) or the freeze / test-environment decisions fail.
- **Data position:** project-data as re-read on 2026-11-17. Financial position is still as at 2026-11-14; no actuals later than that exist.

## RAG summary
| Dimension | RAG | Change vs 2026-11-14 | Rationale |
|---|---|---|---|
| Schedule | Amber | Unchanged | Sandbox exit forecast 2026-11-21 falls after freeze start 2026-11-20, so there is no float (R-001). Full cutover 2027-03-27 is still held and within the 2-week tolerance. |
| Budget / Finance | Amber | Down from Green | EAC £2,235k vs £2,400k budget, inside tolerance. Delivery lines £35k over (1.6%). Unbudgeted exposure: R-001 slip £80-120k, QSA fees, R-004 penalty. With R-001, delivery overspend is £115-155k, using £115-155k of the £200k contingency. |
| Risks | Amber | Scores raised | R-001 now 20 and R-002 15 (two High). R-005 now 12. Four new risks, R-008 to R-011 (11 open in total). |
| Issues | Amber | Worse | Three High issues: I-001, I-002, and I-003 (raised from Medium). |
| Benefits | Amber | Worse | 5 of 6 benefits at risk (was 3 of 6) after B-001 and B-004 were corrected from On track. Only B-003 is On track. |
| Resources | Amber | Unchanged | I-004 (Finance Systems developer on leave, build about 2 weeks behind). Dev Patel owns many items: R-001, R-006, I-001, I-002, AS-001, DEP-002, B-002, B-004, and is proposed owner of R-008 and R-010. |

## Key messages
1. The sandbox exit (2026-11-21) lands one day after the freeze starts (2026-11-20). Any defect found after that depends on whether test environments stay available (AS-002, due 2026-11-20).
2. Budget is Amber, not Green. The headline +£165k is mostly unspent contingency, not delivery underspend. Known exposure could use 58% to 78% of contingency.
3. Benefits position is worse than reported: five of six at risk, and the B-006 figure does not reconcile to B-001.
4. Three decisions or confirmations fall due this week or next: AS-002 (2026-11-20), the I-003 escalation trigger (2026-11-27), and the reduced test scope decision.

## Changes made today by specialists
- **Risk register:** R-001 P 4 to 5, score 16 to 20. R-005 P 3 to 4, score 9 to 12. R-002, R-003, R-004 and R-006 scores unchanged; text updated. R-001 to R-007 review dates brought forward to 2026-11-24 (previously up to 2027-01-19). Added R-008 (3DS2), R-009 (test data and UAT), R-010 (PayPal pass-through), R-011 (test environments during freeze). Owners TBC.
- **Issue log:** I-003 raised from Medium to High (blocks a critical-path milestone). Escalation wording and cross-links to R-001, DEP-004 and AS-002 added.
- **Assumptions and dependencies:** DEP-004 status reworded to "At risk (not yet overdue; due 2026-11-27)".
- **Budget tracker:** "Review 2026-11-17" section added (arithmetic checked, risk-adjusted view, Amber recommended). Position figures unchanged.
- **Benefits register:** B-001 and B-004 corrected from On track to At risk. B-006 reconciliation note, timing notes and charter traceability notes added.

## Milestones
| Milestone | Baseline | Forecast | RAG |
|---|---|---|---|
| Sandbox integration complete | 2026-10-31 | 2026-11-21 | Amber (after freeze start; no retest result in data since 2026-11-14) |
| Peak trading freeze | 2026-11-20 | 2026-11-20 to 2027-01-04 | Amber (scope of freeze unvalidated, AS-002) |
| UAT start | 2027-01-18 | 2027-01-18 | Amber (R-001, R-009, I-003) |
| Pilot (5% of traffic) | 2027-02-08 | 2027-02-08 | Amber (I-002, DEP-005); was Green on 2026-11-14. This is my assessment, not a recorded forecast change. |
| Full cutover | 2027-03-27 | 2027-03-27 | Amber (within 2-week tolerance) |
| PayLink decommissioned | 2027-06-30 | 2027-06-30 | Green |

## RAID highlights
- **Risks:** 11 open. High: R-001 (20), R-002 (15). Medium: R-003, R-005, R-008, R-009, R-010, R-011 (12 each), R-004 (8). Low: R-006, R-007 (6 each).
- **R-008 to R-011 are new**, owners TBC. R-010 and R-011 scores are provisional.
- **Issues:** High: I-001 (sandbox slip), I-002 (3DS2, fix due 2026-12-04), I-003 (test data sign-off, escalate if unresolved by 2026-11-27). Medium: I-004. Low: I-005.
- **Dependencies at risk:** DEP-004 (due 2026-11-27), DEP-005 (due 2027-01-29). DEP-001 (QSA slot) not confirmed, due 2026-12-01.

## Finance (GBP, thousands, as at 2026-11-14)
| Budget | Actuals | Commitments | Forecast to complete | EAC | Budget minus EAC |
|---|---|---|---|---|---|
| 2,400 | 1,095 | 210 | 930 | 2,235 | +165 (underspend) |

Sign convention: +165 is Budget minus EAC (underspend). Delivery lines alone (budget 2,200) are 35 over (EAC 2,235).

| Risk-adjusted view | EAC | Contingency used (of 200) | Contingency left |
|---|---|---|---|
| Delivery overspend only | 2,235 | 35 | 165 |
| Plus R-001 slip 80-120 | 2,315 to 2,355 | 115 to 155 (58% to 78%) | 85 to 45 |
| Plus R-004 penalty, QSA fee variance | TBC | not quantifiable | not quantifiable |

Remaining contingency must also cover R-002, R-003, R-004 and R-005, none of which are costed. Figures are unmitigated, at full value, not probability-weighted.

## Benefits
No benefits are realised yet (cutover 2027-03-27). On track: B-003. At risk: B-001 (forecast 0.32 vs 0.31), B-002, B-004 (forecast 150 vs 120 minutes, and the 2027-12-31 date gives about 9 months of data), B-005, B-006 (forecast £480k vs £540k target). B-006 is unvalidated (see inconsistency 2).

## Cross-file inconsistencies found
Checked against the files. Items marked "fixed" were corrected by specialists today; the rest remain open.
1. **2026-11-14 status is stale (open; superseded by this report):** it says 3 of 6 benefits at risk (now 5), Budget Green (now Amber), R-001 score 16 (now 20), two High issues (now three), I-003 Medium (now High), and risk counts and scores are out of date.
2. **B-006 does not reconcile to B-001 (open):** at 18m transactions, 18m x 0.11 = £1,980k vs the £540k target, and 18m x 0.10 = £1,800k vs the £480k forecast. The stated gap is £60k, but 18m x 0.01 implies £180k. Back-solving gives about 4.9m and 4.8m transactions, so 18m is not supported. B-001 cites AS-004 for volume, but AS-004 is about growth of no more than 8% year on year, not volume. The true volume is not in project-data.
3. **Tracker variance and contingency (open):** the +165 is mostly the 200 unspent contingency less 35 delivery overspend. The tracker note says the 35 is "absorbed by contingency", but the contingency line shows 0 drawn. The second squad (about £40k, already in EAC) may overlap with the R-001 estimate of £80-120k, which risks a double count; Engineering to confirm. The tolerance basis is undefined: 5% of 2,400 is 120, while the delivery overspend of 115-155 is measured against 2,200. It is borderline at the low end and a breach at the high end on the delivery basis, but inside tolerance on the total budget.
4. **Sign ambiguity (open):** the 2026-11-14 status shows "+165 (delivery lines -35)". Both are Budget minus EAC but read differently (+ underspend on the total, - overspend on delivery lines). This report states the convention.
5. **Weekday mismatch (open):** 2026-11-14 and 2026-11-21 are Saturdays. Reporting is Friday (the next Friday is 2026-11-20, which is also freeze start and the AS-002 due date). 2026-11-17 is a Tuesday. Confirm the intended dates.
6. **Risk review dates (fixed):** they previously breached the weekly RAID cadence (up to 2027-01-19); now 2026-11-24.
7. **SteerCo cadence (fixed):** R-001 mitigation described SteerCo as weekly-reviewed; the charter says fortnightly. Wording corrected.
8. **DEP-004 wording (fixed):** "Overdue risk" changed to "At risk (not yet overdue)".
9. **AS-002 (open):** the owner (Hannah Brooks, Operations) may not be the right person to validate a freeze scope; confirm. The charter says "code freeze" while AS-002 says "production only"; these differ in effect on test environments. Due 2026-11-20.
10. **"Spend is on plan" (open):** the 2026-11-14 status key message conflicts with the tracker (delivery lines 35 over, second squad about £40k added).

Dropped as not holding: none.

## Escalations and decisions
1. **I-003:** sponsor escalation trigger is 2026-11-27. Pre-warn the sponsor now.
2. **AS-002:** confirm by 2026-11-20 whether test environments and pipelines are exempt from the freeze.
3. **SteerCo decision:** reduced test scope for the freeze period (R-001).
4. **SteerCo ask:** approve a request to NovaPay for a named deputy architect (R-006).
5. **Sponsor:** confirm the tolerance basis (2,400 vs 2,200) and the contingency release rule.
6. **Legal (Lena Fischer):** confirm the R-004 penalty by 2026-12-08.
7. **Security (Sam Okafor):** confirm the QSA slot and fee by 2026-12-01.
8. **Finance:** validate transaction volume and B-006.
9. **Engineering (Dev Patel):** confirm the sandbox retest result (no data since 2026-11-14), the R-001 estimate basis and the squad overlap by 2026-11-24.

## Next steps
- Confirm sandbox exit on 2026-11-21 and the AS-002 outcome on 2026-11-20.
- Confirm owners for R-008 to R-011.
- Obtain written NovaPay confirmation on PayPal pass-through by 2026-11-30 (AS-001, R-010).
- Next RAID review 2026-11-24. Next Friday status report 2026-11-20.

## Assumptions and open questions
- The next SteerCo date is not in the data, so the asks above have no confirmed forum date. The charter says fortnightly.
- No actuals after 2026-11-14. All finance figures are as at that date.
- R-010 and R-011 scores are provisional. Owners for R-008 to R-011 are TBC (proposed only).
- The R-001 estimate (£80-120k) has no stated source or basis. There are no cost estimates for R-004 or QSA fees.
- The pilot RAG change to Amber is my assessment, not recorded in a source file.
- The 18m annual transactions figure is unvalidated and the true volume is not in project-data.
- All data is dummy data.
