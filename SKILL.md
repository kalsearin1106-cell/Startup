---
name: company-report-pdf
description: Create evidence-led company analysis reports and PDFs from user-provided photos, documents, and URLs, with review checkpoints for extracted facts and the draft.
---

# Evidence-led company report and PDF

Use this skill when the user wants to turn supplied company materials into an analysis report and a finished PDF. Ask for missing setup details only when they cannot be inferred: company, report purpose/audience, project output folder, and any requested sections or date convention. The report purpose may change by project; do not assume every report is an investment memo or a job portfolio.

## Evidence rules

- Use only files, images, and URLs the user supplied. Open supplied URLs as needed, but do not search for additional sources on your own. If a required fact is missing or a source cannot be read, ask the user for the missing source or leave the point out.
- Never invent facts, amounts, dates, sources, calculations, or company details. Keep each material factual statement traceable to an evidence item and location.
- Separate directly documented facts, company statements, third-party data, and analyst interpretation. An interpretation is allowed only when it follows from cited evidence and is clearly labeled. An unverified cause or missing detail may appear only as a question to investigate, not as a factual explanation.
- For images, inspect the image itself. Record visible units and periods; if text, digits, or context are unclear, mark the item unreadable and ask for a clearer image or source document.
- Do not silently reconcile conflicting figures. Preserve the competing values with their source basis and explain the mismatch. Keep grant/support amounts separate from private investment. Do not infer customer revenue from an MOU or collaboration announcement.
- For financial data, record period, currency/unit, accounting basis (including consolidated/standalone when shown), source, and data date. Do not combine different providers as if they were one audited series. Do not substitute profit for cash flow or calculate runway without suitable cash balance and cash-flow data.
- Do not add a market size, valuation, KPI, patent status, regulatory approval, or forecast unless supplied evidence supports the exact statement and its scope.

## Workflow and user checkpoints

1. Confirm report purpose, audience, output folder, and scope. Use the project folder chosen for this run (for example, `project1`, `project2`, or another path). Keep this skill package separate from project evidence and report outputs.
2. Inventory supplied materials and URLs. Extract candidate facts into a source register and fact ledger using [the evidence workflow](references/evidence-workflow.md). Show the inventory, key extracted facts, ambiguities, and missing materials to the user. **Pause for the user's review before drafting.** Apply corrections and mark unresolved items explicitly.
3. Draft the report for the selected purpose. Create charts only from verified data, retaining the underlying data and source link in the project folder. Include an editable Markdown report, chart files, and a source register alongside the PDF.
4. Present the report draft and generated PDF preview for the second review. Check claim-to-source links, units, date ranges, arithmetic, chart labels, page breaks, font rendering, clipping, and links. Use the available PDF skill's render-and-inspect workflow when present. **Pause for the user's review before treating the report as final.**
5. Save reviewed deliverables beneath the user-selected project folder. A practical default layout is `report.md`, `sources/source-register.csv`, `visuals/`, and `output/pdf/<date>_<company>_<purpose>.pdf`; adapt to the user's existing folder layout. Never overwrite an existing deliverable without explicit instruction. Do not place company source files or finished project reports in this skill's Git repository.

See [the evidence workflow](references/evidence-workflow.md) for the review payload and minimum ledger fields.

