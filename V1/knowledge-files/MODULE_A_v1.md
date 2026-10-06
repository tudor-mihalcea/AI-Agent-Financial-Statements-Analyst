# MODULE A v1.4 — Block 1: Reformulation and profitability

*Runs with the master prompt in force; every term, formula and label is as defined there.*

---

## 1. Declared inputs [component 2]

**Years:** the three most recent fiscal years N, N−1, N−2.

**Documents:**

- Annual report N: primary statements (income statement, OCI, balance sheet, cash flows, changes in equity) and notes, covering N and N−1 (restated comparatives).
- Annual report N−1: the same for N−2, and to check restatements of N−1.
- The company convention register, if any, and the Sector annex.
- The team workbook and its table map (kept in the register), if any.
- For the Penman ROOA split: a short-term market rate supplied by the team (source, URL, tenor, date), unless short-term interest and short-term financial liabilities are both disclosed.

**Notes required from each report, or "not found":**

- accounting policies; revenue and contract balances;
- operating income and expenses by nature (or cost of sales/SG&A/R&D plus the nature-of-expense disclosure); D&A with impairment; personnel expenses;
- equity-accounted investments; financial result / other financial result;
- income tax: composition, reconciliation, deferred-tax allocation;
- discontinued operations and held-for-sale groups: pre-tax result, tax, assets, liabilities, cash;
- business combinations: step-up gains, transaction costs, contingent consideration;
- intangible assets (indefinite-life split); leases; inventories;
- other assets and other liabilities: financial/non-financial, derivatives, other taxes, pension surplus;
- cash; equity and OCI with tax; pensions; provisions; financial debt;
- financial instruments and hedging (purpose of derivatives); related parties (joint ventures);
- segment reporting; management's adjusted-earnings reconciliation; subsequent events.

**Stop rule:** if an essential input is missing, stop the steps that depend on it and ask; do not proceed on an assumption. Continue only the steps that do not depend on it. Retrieve missing public filings from official sources where possible.

---

## 2. Procedure [component 4]

Each step carries the figure-status label its results receive. Workbook results the team has marked final are WORKBOOK; other existing workbook results are CHECK; results missing from the workbook are AGENT.

1. **VERIFY** [AGENT] year coverage, scope, currency, year-end, framework, restatements, rounding policy.
2. **MAP** [WORKBOOK] register entries, table map, classifications and approved exceptions; list which results exist and their status (final / not final). Propose register additions for consistent, unrecorded workbook conventions.
3. **EXTRACT** [AGENT] each year's reported statements and required notes with page/note references. Workbook input cells: [CHECK] against these sources.
4. **REFORMULATE** [CHECK/AGENT] the income statement for each year; build the unusual-item register.
5. **RECONCILE** [AGENT] each year to comprehensive income and the NCI/parent split with the comprehensive-income bridge.
6. **COST LENSES** [CHECK/AGENT] primary lens first; quantify the other two where supported; otherwise list the gaps and ask before estimating.
7. **BALANCE SHEET** [CHECK/AGENT] managerial balance sheet, structure metrics and the Modigliani–Miller/Penman classification bridge for each year.
8. **ROI** [CHECK/AGENT] gross and net ROI, core return on sales, turnover, operating-liability leverage, ROI support ratios, and any register-approved denominator beside the standard one. The ROIs are to be calculated NOT by using the raw inputs, but by using the information you calculated in the reformulated income statement and the managerial balance sheet.
9. **ROE** [CHECK/AGENT] DuPont (reported, with the net income / earnings before taxes split), Modigliani–Miller stages 1–3, Penman with the ROOA split; check each against comprehensive income / equity or net income / equity; ROE change attribution year on year.
10. **THRESHOLDS** [AGENT] compute every §3 metric for each year; report value, threshold and status.
11. **INTERPRET** [AGENT] three-year changes through margin, turnover, operating and financial leverage, tax and unusual items; common-size and trend analysis (growth rates, CAGR, bridges), classifying each variation as recurring, non-recurring, discretionary or anomalous; separate evidenced causes from inference.
12. **OUTPUT** [AGENT] results, comparison checks, limitations and the draft or updated register; propose workbook corrections separately and never apply them.

---

## 3. Thresholds and decision rules [component 5]

Set by the team and justified below. Report each metric's value beside its threshold; add no thresholds of your own. A breach is a flag that requires an explanation, not a conclusion.

### Analytical triggers

| ID | Metric | Flag when | Justification |
|---|---|---|---|
| T1 | Sum of unusual items excluding OCI / \|income before unusual items and taxes\| | > 10% | Reported earnings depend on non-recurring items (Enron test). |
| T2 | Same unusual category with the same sign | in ≥ 2 of 3 years | Possibly recurring — judgment to confirm. |
| T3 | Any cost line as % of value of production (or sales), year on year | change ≥ 1.0 pp | Unusual change of a usual item; classify it (Abbott example: a 1.2 pp decline in R&D / sales was flagged). |
| T4 | \|OCI\| / \|comprehensive income\| | > 10% | Dirty-surplus effect on ROE; show ROE on net income and on comprehensive income. |
| T5 | \|uniform tax rate − statutory rate\| | > 5 pp | Explain from the tax reconciliation. |
| T6 | \|non-core operating income\| / \|operating income\| | > 10% | Material non-core results; report the non-core return separately. |
| T7 | NFP / EBITDA | > 4.0x | Covenant-type limit. |
| T8 | NFP / equity | > 3.0x | Covenant-type limit. |
| T9 | Operating income / interest expense | < 3.0x | Times interest earned. |
| T10 | CAPEX / D&A | < 1.0x or > 2.0x | Maintenance-only vs growth investment. |
| T11 | NOWC / sales, year on year | change ≥ 5 pp | NOWC should move with sales. |
| T12 | Operating liabilities / gross operating invested capital | > 50% | High operating-liability leverage; report the Penman ROOA split. |
| T13 | Equity − goodwill | < 0 | Negative tangible equity. |
| T14 | NCI / equity | > 10% | Report leverage with NCI as financing. |
| T15 | \|cost of NFO\| or \|return on NFA\| relative to interest expense / financial debt | > 3× | Financing rate not economically meaningful. |
| T16 | Sign of NFP or NFO | changes within the year | Flag financing ratios; keep closing balances. |

### Technical tolerances

- Decomposition vs direct return: > 0.01 pp, unrounded.
- Capital weights: total differs from 100% by > 0.01 pp; also report monetary residuals.
- Denominator sensitivity: \|net operating invested capital\| / gross operating invested capital < 5% where gross operating invested capital > 0.
- Workbook comparison: amounts match within 0.5 units of source precision; ratios within 0.01 pp (multiples 0.0001). Classify every non-match as a method difference (propose a register entry), a workbook defect (propose a correction) or a source conflict.
- Comprehensive-income bridge: unexplained rounding remainder > 2 units of source precision.

Never assume a residual is rounding. Flag zero or negative equity or net operating assets, unsupported adjustments and source conflicts. Do not add covenant, credit-risk or fraud thresholds beyond this table.

---

## 4. Prescribed output [component 7]

Cover all three years; mark any unavailable result and the reason. Interpretation ≤ 1,200 words, excluding tables and quotations. Tables, in this order:

1. **Input status:** Input | Period | Source/version | Available? | Limitation.
2. **Reformulated income statement:** Line | N | N−1 | N−2 | Status (WORKBOOK/CHECK/AGENT) | Source page/note. If possible, every input that needs to be calculated in the income statement (such as, but not limited to: value of production, EBITDA, Added Value, etc.) is to be calculated using the existing input in the income statement, not the raw input. Include the comprehensive income in the reformulated income statement.
3. **Unusual-item register:** Item/year | Signed amount | Original line | Category (a)–(l) | Criterion | Recurrence evidence | Tax basis | Status.
4. **Cost lenses:** Lens/line/ratio | N | N−1 | N−2 | Source/calculation.
5. **Managerial balance sheet and structure metrics:** Category | N | N−1 | N−2 | Source/calculation | Classification. The managerial balance sheet needs to be consistent with the income statement. 
6. **ROI:** Measure | Year | Workbook | Agent | Difference | Status.- The ROIs are to be calculated NOT by using the raw inputs, but by using the information you calculated in the reformulated income statement and the managerial balance sheet.
7. **ROE:** DuPont (with the net income / earnings before taxes split), Modigliani–Miller (choose only 1 stage according to the managerial balance sheet - mandatory to specify exactly which you choose), Penman with the ROOA split — components, direct check and ROE change drivers.
8. **Thresholds:** ID | Metric | Year | Value | Threshold | Status | Explanation. NO FLAG will be green, FLAG will be red.
9. **Interpretation:** Change | Driver | Evidence | Qualification. The interpretation is to be done ONLY for the change in ratios (ROE and ROI).
10. **Self-check:** Issue/assumption | Affected result | Evidence or decision needed | Status.
11. **Workbook issues** (if a workbook is supplied): # | Issue | Location | Effect | Proposed correction | Severity.
12. **Convention register,** draft or updated.

Close with a statement of what could not be verified. Do not write the progress note or Agent Log entries.
