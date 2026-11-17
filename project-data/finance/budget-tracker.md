# Budget Tracker (currency: GBP, thousands)

> **DUMMY DATA** (Project Gateway Switch). Position as at 2026-11-14.
> EAC = Actuals to date + Commitments + Forecast to complete. Variance = Budget − EAC (positive = underspend, negative = overspend).

| Cost line | Budget | Actuals to date | Commitments | Forecast to complete | EAC | Variance | Comment |
|---|---|---|---|---|---|---|---|
| Programme management | 300 | 190 | 20 | 100 | 310 | -10 | Extended PM cover for the 3-week sandbox slip (I-001). |
| Engineering & integration | 900 | 520 | 80 | 340 | 940 | -40 | Second integration squad added to mitigate R-001. Main overspend driver. |
| Testing & PCI DSS | 350 | 110 | 60 | 190 | 360 | -10 | QSA fees not yet confirmed (DEP-001); estimate may change. |
| Data migration | 200 | 70 | 10 | 110 | 190 | 10 | Three rehearsals planned (R-002). Small underspend forecast. |
| Operations change & training | 150 | 25 | 0 | 120 | 145 | 5 | Spend is back-loaded to Jan–Mar 2027. |
| Vendor onboarding & licences | 300 | 180 | 40 | 70 | 290 | 10 | NovaPay setup and first-year licence at agreed rates. |
| Contingency (held) | 200 | 0 | 0 | 0 | 0 | 200 | Unallocated. Recommend holding against R-001, R-002, R-003. |
| **Total** | **2,400** | **1,095** | **210** | **930** | **2,235** | **165** | Delivery lines alone: budget 2,200, EAC 2,235, overspend 35 (1.6%). Within ±5% tolerance. |

## Notes
- Overspend of £35k on delivery lines is within the £120k tolerance and can be absorbed by contingency if needed.
- Risk exposure not in the forecast: R-001 (slip cost estimate about £80–120k) and R-004 (PayLink early-exit penalty, value to be confirmed by Legal).
- Open question: the PayLink run-cost saving from decommissioning is not in this budget (see benefits register B-001).

## Review 2026-11-17 (finance health check)
> Position data remains as at 2026-11-14. **No actuals later than 2026-11-14 exist**, so the figures above are unchanged. The review below is a risk-adjusted view only.

**Arithmetic check:** every row (Actuals + Commitments + FTC = EAC; Budget − EAC = Variance) and every total re-computed and correct. Totals: Budget 2,400; Actuals 1,095; Commitments 210; FTC 930; EAC 2,235; Variance +165.

**Reading the +165:** it is not an underspend of delivery. It is the 200 unspent contingency (EAC held at 0) less the 35 delivery overspend. Delivery lines: budget 2,200, EAC 2,235, 35 over (1.6%).

**Risk-adjusted view (GBP k, unmitigated exposure at full value, not probability-weighted):**

| View | Low | High | Vs budget 2,400 | Contingency used (of 200) | Contingency left |
|---|---|---|---|---|---|
| Current EAC (incl. 200 contingency unspent) | 2,235 | 2,235 | +165 under | n/a | 200 |
| Delivery overspend charged to contingency | 2,200 + 35 | 2,200 + 35 | | 35 (18%) | 165 |
| + R-001 slip cost 80-120 | 2,315 | 2,355 | +85 to +45 under | 115 to 155 (58% to 78%) | 85 to 45 |
| + R-004 penalty | TBC | TBC | not quantifiable | | |
| + QSA fee variance (DEP-001) | TBC | TBC | not quantifiable | | |

- Overspend against delivery budget (2,200): 115 to 155 (5.2% to 7.0%). Against the 120 tolerance this is borderline at the low end and a breach at the high end if tolerance is read on the delivery baseline. Read on the total budget (2,400), EAC stays inside tolerance.
- Contingency remaining (45-85) must also cover R-002 (score 15, unquantified), R-003 (QSA), R-004 and R-005, none of which are costed.
- Possible double count: the 40 second-squad cost (already in EAC) may overlap with the R-001 slip estimate of 80-120. Needs confirming with Engineering Lead.
- The existing note that the 35 "can be absorbed by contingency" is valid only if the 200 contingency line is treated as drawn; the EAC currently shows it as 0 drawn.

**Finance RAG: AMBER.** Headline EAC is inside tolerance, but known unbudgeted exposure would consume most of contingency, leaving little for unquantified risks, and the delivery-line view could breach 120. The 2026-11-14 status report shows Budget Green; recommend moving to Amber.

**Assumptions / gaps:** R-001 estimate 80-120 taken as stated, no source or basis in the data; no cost estimates for R-004 or QSA fees; tolerance basis (total 2,400 vs delivery 2,200) not defined in the charter; PayLink run-cost saving not in budget.

**Actions (proposed):** Legal (Lena Fischer) to confirm R-004 penalty by 2026-12-08; Security (Sam Okafor) to confirm QSA fee with slot by 2026-12-01; Engineering (Dev Patel) to confirm R-001 estimate basis and squad overlap by R-001 review 2026-11-24; Sponsor to confirm tolerance basis and any contingency release rule.
