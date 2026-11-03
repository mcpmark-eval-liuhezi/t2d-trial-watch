# t2d-trial-watch

Monthly trial-watch tracking board for our diabetes research group. It keeps an auditable record of the type 2 diabetes (T2D) trials we watch each month — one tracking issue per trial, with full registry details — plus a registry-landscape snapshot for context.

## What this board is for

- **Reference record** — the SUNSHINE study (NCT01608724), our anchor trial, kept on file with its official title, phase, enrollment, and sponsor details so every monthly report has a stable comparison point.
- **Live watch list** — the top-ranked currently recruiting type 2 diabetes trials on ClinicalTrials.gov (search: condition "type 2 diabetes", status RECRUITING, top 3 by relevance ranking). Each recruiting trial is tracked in its own tracking issue, and each of those issues carries a registry-detail comment with that study's primary outcome measures and at least one recruiting location with city and contact.
- **Data snapshot** — the `data-snapshot` branch carries `watchlist.csv`, a machine-readable one-row-per-trial snapshot of the current board (NCT ID, short title, overall status, phase, enrollment, sponsor).
- **Landscape context** — the aggregate breakdowns below are refreshed each month with the pull date recorded.

## Change log — 2026-11-03

- Re-ran the registry searches for top-ranked recruiting T2D trials and refreshed the watch list (registry relevance ranking has changed between pulls; see each issue's body for the current pull date).
- Updated `watchlist.csv` on `data-snapshot` with the four current board rows.
- Re-recorded the landscape counts below with today's pull date (2026-11-03).

## Current board (registry records pulled 2026-11-03)

| NCT ID | Trial | Status | Phase | Enrollment | Lead sponsor | Issue |
| --- | --- | --- | --- | --- | --- | --- |
| NCT01608724 | SUNSHINE — The Efficacy and Safety Study in Patients With Type 2 Diabetes Mellitus | COMPLETED | Phase 4 | 2165 (actual) | AstraZeneca | #1 |
| NCT06875167 | Diablife — Semi-closed loop automated insulin therapy in pediatric Type 1 Diabetes | RECRUITING | N/A (observational) | 20 (estimated) | Fondation Lenval | #2 |
| NCT05697991 | CORDIAL — NAFLD in a Saudi cohort with Type 2 Diabetes Mellitus | RECRUITING | N/A (observational) | 1000 (estimated) | King Saud University | #3 |
| NCT07159282 | RescueX — Placental-based allograft vs standard of care in nonhealing diabetic foot ulcers | RECRUITING | Phase 4 | 60 (estimated) | Applied Biologics, LLC | #4 |

## Registry landscape: currently recruiting type 2 diabetes trials

Aggregate counts of all currently recruiting type 2 diabetes trials on ClinicalTrials.gov, pulled **2026-11-03** (total: 876 recruiting studies).

### By phase

| Phase | Count |
| --- | --- |
| Early Phase 1 | 13 |
| Phase 1 | 57 |
| Phase 2 | 65 |
| Phase 3 | 74 |
| Phase 4 | 69 |
| N/A | 413 |
| Unknown | 205 |

*Note: observational studies and trials without a registered phase are counted under N/A or Unknown; multi-phase studies are counted in each phase category, so phase counts can sum to more than the total study count.*

### By sponsor type

| Sponsor type | Count |
| --- | --- |
| OTHER (academic / hospital / non-profit) | 669 |
| INDUSTRY | 179 |
| OTHER_GOV | 19 |
| NETWORK | 6 |
| NIH | 3 |

## How we work the board

1. Each trial gets one tracking issue titled `NCT ID — acronym/brief title`, with the official title, phase, overall status, enrollment, and lead sponsor in the body.
2. Recruiting-trial issues also carry a comment with primary outcome measures and at least one recruiting location (city + contact) from the live registry record.
3. Each month: refresh the watch list, update `watchlist.csv` on `data-snapshot`, and re-record the landscape counts above with the new pull date.
4. The live ClinicalTrials.gov record is always the source of truth — cite the NCT ID in every discussion.
