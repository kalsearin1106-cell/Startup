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
- Specific requests for additional material where it is needed. Do not fill these gaps with web searches or assumptions.

Wait for user corrections or confirmation. A missing response is not confirmation. Do not proceed to a factual report draft until the user has reviewed this checkpoint.

## Stage 2: report and PDF draft

Keep source IDs next to claims during drafting so the source register can map each material number and assertion to evidence. In the reader-facing report, use links or concise source notes close to the related claim, plus a source list with title, publisher, URL/file, reviewed date, and data period when available.

Clearly label the following:

- Company descriptions and performance claims as company statements.
- Data supplied by third-party information services as third-party data, including provider and period.
- Interpretations as analysis, with the supporting facts visible nearby.
- Missing explanations as verification questions, such as “Was the 2025 revenue decline caused by contract timing or service mix? What project-level sales data would confirm this?” Do not present a possible cause as an established explanation.

For each chart, keep a table of the plotted values and source IDs. Include title, axes, period, units, source basis, and caveats. If the data has too few points for a trend, use a comparison chart or a table; do not imply a forecast.

At the second checkpoint, show the editable report and a rendered PDF preview. Confirm that edits are reflected in the latest PDF, references are readable, calculations can be reproduced from the ledger, and every material number is consistent across prose, tables, and charts. Record requested corrections before producing the reviewed final.

## Suggested project files

Adapt these to the user's destination folder; do not create empty placeholders:

- `report.md` — editable report source.
- `sources/source-register.csv` — source inventory and fact-to-source mapping.
- `visuals/` — charts included in the report, plus their verified input data if not already in the source register.
- `output/pdf/` — reviewed PDF deliverable.

Keep private source documents in the user-selected project area. The skill's own repository contains instructions and generic templates only, never company-specific source material or report outputs.

