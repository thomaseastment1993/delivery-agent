# Project Charter

> **DUMMY DATA**: fictional project and vendors, for testing the delivery agents only.

- **Project name:** Project Gateway Switch: migrate card payments from PayLink (legacy) to NovaPay
- **Sponsor:** Priya Raman (Chief Financial Officer)
- **Delivery lead:** Thomas Eastment
- **Objectives:**
  1. Move 100% of online card and wallet transactions from PayLink to NovaPay by 2027-03-27.
  2. Cut blended cost per transaction from £0.42 to £0.31.
  3. Improve authorisation rate from 91.5% to 93.5%.
  4. Reduce settlement time from T+3 to T+1.
  5. Decommission PayLink by 2027-06-30 with no loss of PCI DSS compliance.
- **Scope (in / out):**
  - In: web and mobile checkout integration, tokenised card-vault migration, refunds and chargebacks, reconciliation and finance reporting feeds, PCI DSS re-validation, merchant-ops training, cutover and PayLink decommission.
  - Out: in-store POS terminals, a new fraud engine (existing rules are ported only), and a checkout UX redesign.
- **Key milestones:**
  | Milestone | Date | Status |
  |---|---|---|
  | NovaPay contract signed | 2026-06-30 | Complete |
  | PCI scoping complete | 2026-09-15 | Complete |
  | Sandbox integration complete | 2026-10-31 (re-baselined 2026-11-21) | Late |
  | Peak trading code freeze | 2026-11-20 to 2027-01-04 | Planned |
  | UAT start | 2027-01-18 | Planned |
  | Pilot (5% of traffic) | 2027-02-08 | Planned |
  | Full cutover | 2027-03-27 | Planned |
  | PayLink decommissioned | 2027-06-30 | Planned |
- **Budget & tolerances:**
  - Approved budget £2,400k (including £200k contingency). Currency GBP, figures in thousands.
  - Cost tolerance ±5% (£120k) on EAC before escalation to the sponsor.
  - Schedule tolerance: 2 weeks on the full-cutover date.
- **Governance & reporting cadence:**
  - Weekly status report every Friday to the Steering Committee (SteerCo).
  - Fortnightly SteerCo chaired by the sponsor.
  - RAID reviewed weekly. Finance and benefits reviewed monthly.
