# Assumptions & Dependencies

> **DUMMY DATA** (Project Gateway Switch).

| ID | Type | Description | Owner | Validate / due by | Status |
|---|---|---|---|---|---|
| AS-001 | Assumption | NovaPay supports all current payment methods (cards, Apple Pay, Google Pay, PayPal pass-through) with no custom build. | Dev Patel | 2026-11-30 | Partly validated (PayPal pass-through unconfirmed) |
| AS-002 | Assumption | Peak trading freeze (2026-11-20 to 2027-01-04) applies to production only; test environments stay available. | Hannah Brooks | 2026-11-20 | To validate |
| AS-003 | Assumption | NovaPay can import PayLink tokens without cardholder re-entry (network tokens or PSP-to-PSP transfer). | Mei Tanaka | 2026-12-15 | To validate (see R-002) |
| AS-004 | Assumption | Transaction volumes grow no more than 8% year on year, so the NovaPay volume tier pricing holds. | Lena Fischer | 2027-01-31 | Open |
| AS-005 | Assumption | Existing fraud rules port to NovaPay's rule engine with less than 10% rework. | Sam Okafor | 2026-12-18 | Open |
| DEP-001 | Dependency | QSA (external assessor) availability for PCI DSS re-validation before UAT exit. | Sam Okafor | 2026-12-01 | Slot requested, not confirmed |
| DEP-002 | Dependency | NovaPay delivers production credentials and the certified 3DS2 configuration. | Dev Patel | 2027-01-08 | On track |
| DEP-003 | Dependency | PayLink provides a full token and transaction history export. | Mei Tanaka | 2026-12-18 | Requested |
| DEP-004 | Dependency | Data-protection sign-off for masked production test data (see I-003). | Sam Okafor | 2026-11-27 | At risk (not yet overdue; due 2026-11-27; see I-003) |
| DEP-005 | Dependency | Finance Systems reconciliation feed build complete before the pilot. | Omar Haddad | 2027-01-29 | At risk (see I-004) |

## Data gap: no 2026-11-20 status report (logged 2026-11-23)
No status report exists for 2026-11-20 and no project data has been recorded after 2026-11-14 (no actuals, no outcomes). A report has not been produced because it would require invented data; the conventions do not define a "data not refreshed" stub, so none was created. The following have passed their dates with no recorded outcome. Statuses above are unchanged and should be treated as unconfirmed.

| ID | Open question / action | Owner (as recorded or proposed) | Was due | Status |
|---|---|---|---|---|
| A-001 | Record the outcome of AS-002 (are test environments exempt from the freeze?). The AS-002 row above still reads "To validate". | Hannah Brooks (owner may not be right; see health check inconsistency 9) | 2026-11-20 | Overdue, no outcome recorded |
| A-002 | Record the sandbox retest result and whether sandbox exit happened on the 2026-11-21 forecast (I-001, R-001). Owner TBC; the health check names Dev Patel to confirm the retest result. | Dev Patel (proposed) | 2026-11-21 | No outcome recorded |
| A-003 | Provide refreshed actuals and forecast after 2026-11-14, then issue the next status report. | Delivery lead / Finance (TBC) | 2026-11-20 | Not started. Cannot be done without new data |
| A-004 | Confirm intended reporting dates; 2026-11-14 and 2026-11-21 are Saturdays (health check inconsistency 5). | Delivery lead | TBC | Open |

Upcoming and unconfirmed: I-003 / DEP-004 escalation trigger 2026-11-27; R-001 review and Engineering estimate-basis confirmation 2026-11-24.
