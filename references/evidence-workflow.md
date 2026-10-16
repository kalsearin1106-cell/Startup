# Evidence inventory and review workflow

## Stage 1: inventory and extraction

Create a stable source ID for every supplied item (`S01`, `S02`, ...). Keep original filenames and user-provided URLs intact. For a web page, record its title or publisher and the URL actually reviewed. For a screenshot or scan, record the filename and the visible page/table/section when identifiable.

For every candidate claim or value, capture:

| Field | What to record |
|---|---|
| Fact ID | Stable ID such as `F001` |
| Proposed claim/value | Plain statement, with exact amount and unit where applicable |
| Evidence class | Documented fact, company statement, third-party data, or analyst interpretation |
| Source ID and locator | Source ID plus URL, page, heading, table, or image region |
| Period and basis | Reporting period, currency/unit, and accounting basis if shown |
| Limits/conflicts | Missing date, unclear OCR, conflicting source, or scope caveat |
| Status | Readable, needs confirmation, conflicting, or excluded |

Before drafting, present the user with:

- The source inventory and what each item appears to contain.
- The key extracted facts, including their source IDs and locators.
- Any ambiguous readings, conflicting values, inaccessible pages, and facts needed for the requested report but not supplied.
- Specific requests for additional material where needed. Do not fill gaps with assumptions. Search public sources only when the user authorized public research; prioritize primary records and record every page actually checked. Do not use private, paid, or account-gated sources without explicit access permission.

If the user selected staged review, wait for corrections or confirmation before drafting; a missing response is not confirmation. If the user explicitly selected direct drafting, proceed after inventory and carry unresolved items into the report as limits or questions.

## Stage 2: report and PDF draft

Keep source IDs next to claims during drafting so the source register can map each material number and assertion to evidence. In the reader-facing report, use links or concise source notes close to the related claim, plus a source list with title, publisher, URL/file, reviewed date, and data period when available.

Clearly label the following at the point they appear in the report, not only in the source appendix:

- Company descriptions and performance claims as company statements.
- Data supplied by third-party information services as third-party data, including provider and period.
- Interpretations as analysis, with the supporting facts visible nearby.
- Missing explanations as verification questions, such as “Was the 2025 revenue decline caused by contract timing or service mix? What project-level sales data would confirm this?” Do not present a possible cause as an established explanation.
- Company announcements and plans separately from outcomes independently confirmed in filings, public registries, regulator records, trial registries, or patent records. A company announcement remains a company statement even when carried by a newswire.

For an investment or strategic conclusion framed as conditional observation, map the conditions to evidence that could change the view. State what evidence would strengthen, weaken, or leave the view unresolved, and why. Do not invent thresholds, probabilities, or forecasts. Where valuation, fully diluted ownership/dilution, recent cash flows, financing needs, or development budgets are unavailable, limit any conclusion about attractiveness or runway and identify which data would make it assessable.

For cash flow, separate operating, investing, and financing flows. Do not interpret financing-driven cash increases as operating cash generation. Use audited cashflow statements when present in the reviewed filing; label the period and basis, and do not project future runway from a single annual period without an appropriate forecast/budget basis.

For each chart, keep a table of the plotted values and source IDs. Include title, axes, period, units, source basis, and caveats. If the data has too few points for a trend, use a comparison chart or a table; do not imply a forecast.

Before the second checkpoint, complete internal editorial and evidence QA: reconcile every claim to its locator; recalculate subtotals and derived figures; compare repeated values across prose, tables, charts, and ledgers; edit typos, duplication, unnecessary caveats, and workflow meta text; inspect source-note legibility, page breaks, clipping, and sparse orphan pages.

At the second checkpoint, show the editable report and a rendered PDF preview. Confirm that edits are reflected in the latest PDF, references are readable, calculations can be reproduced from the ledger, and every material number is consistent across prose, tables, and charts. Record requested corrections before producing the reviewed final. Ask the user for substantive judgments, not for checks that can be performed from available evidence.

## Suggested project files

Adapt these to the user's destination folder; do not create empty placeholders:

- `report.md` — editable report source.
- `sources/source-register.csv` — source inventory and fact-to-source mapping.
- `visuals/` — charts included in the report, plus their verified input data if not already in the source register.
- `output/pdf/` — reviewed PDF deliverable.

Keep private source documents in the user-selected project area. The skill's own repository contains instructions and generic templates only, never company-specific source material or report outputs.
