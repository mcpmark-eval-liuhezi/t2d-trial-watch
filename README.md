# t2d-trial-watch

Monthly trial-watch tracking board for our diabetes research group. It keeps an auditable record of the type 2 diabetes (T2D) trials we watch each month — one tracking issue per trial, with full registry details — plus a registry-landscape snapshot for context.

## What this board is for

- **Reference record** — the SUNSHINE study (NCT01608724), our anchor trial, kept on file with its official title, phase, enrollment, and sponsor details so every monthly report has a stable comparison point.
- **Live watch list** — the top-ranked currently recruiting type 2 diabetes trials on ClinicalTrials.gov (search: condition "type 2 diabetes", status RECRUITING, top 3 by relevance), each tracked in its own issue. Recruiting-trial issues also carry a comment with the study's primary outcome measures and at least one recruiting location with city and contact.
- **Data snapshot** — the `data-snapshot` branch carries `watchlist.csv`, a machine-readable one-row-per-trial snapshot of the current board (NCT ID, short title, overall status, phase, enrollment, sponsor).
- **Landscape context** — the aggregate breakdowns below are refreshed each month with the pull date recorded.

## Current board (registry records pulled 2026-10-19)

| NCT ID | Trial | Status | Phase | Enrollment | Lead sponsor | Issue |
| --- | --- | --- | --- | --- | --- | --- |
| NCT01608724 | SUNSHINE — The Efficacy and Safety Study in Patients With Type 2 Diabetes Mellitus | COMPLETED | Phase 4 | 2165 (actual) | AstraZeneca | #1 |
| NCT06976619 | The Effect of Glycemic Control and of GLP-1 Receptor Agonism on Islet GLP-1 in People With Type 1 and Type 2 Diabetes | RECRUITING | Phase 2 | 60 (estimated) | Mayo Clinic | #2 |
| NCT07233434 | DIADEG — Screening for Type 2 Diabetes by Oral Glucose Tolerance Test in the Population Groups Not Diagnosed by Fasting Blood Glucose in Guadeloupe | RECRUITING | NA | 120 (estimated) | Centre Hospitalier Universitaire de la Guadeloupe | #3 |
| NCT02861781 | COMET — Study of New Determinants of Type 2 Diabetes in Severe Obesity | RECRUITING | N/A (observational) | 270 (estimated) | University Hospital, Montpellier | #4 |

## Registry landscape: currently recruiting type 2 diabetes trials

Aggregate counts of all currently recruiting type 2 diabetes trials on ClinicalTrials.gov, pulled **2026-10-19** (total: 870 recruiting studies).

### By phase

| Phase | Count |
| --- | --- |
| Phase 1 | 59 |
| Early Phase 1 | 13 |
| Phase 2 | 68 |
| Phase 3 | 73 |
| Phase 4 | 68 |
| N/A | 410 |
| Unknown | 201 |

*Note: multi-phase studies are counted in each phase category, so phase counts can sum to more than the total study count.*

### By sponsor type

| Sponsor type | Count |
| --- | --- |
| OTHER (academic / hospital / non-profit) | 666 |
| INDUSTRY | 178 |
| OTHER_GOV | 18 |
| NETWORK | 6 |
| NIH | 2 |

## How we work the board

1. Each trial gets one tracking issue titled `NCT ID — acronym/brief title`, with the official title, phase, overall status, enrollment, and lead sponsor in the body.
2. Recruiting-trial issues also carry a comment with primary outcome measures and at least one recruiting location (city + contact), taken from the live registry record.
3. Each month: refresh the watch list, update `watchlist.csv` on `data-snapshot`, and re-record the landscape counts above with the new pull date.
4. The live ClinicalTrials.gov record is always the source of truth — cite the NCT ID in every discussion.
