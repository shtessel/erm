# What the Monitoring Prompt Does

Running `prompt-monitoring-final.md` instructs the agent to perform **one monitoring cycle** based on `Emerging_Risks_Report_2026.xlsx` and its Monitoring Framework worksheet.

The agent will:

1. **Read the workbook**, including the risk register, sources, methodology, previous decisions and escalation conditions.
2. **Research current external evidence**, including regulatory developments, incidents, research publications and other signals relevant to the risks. It will use the date you specify or, by default, the execution date.
3. **Review all ten monitoring layers.** The first run covers the full register and establishes a baseline. On subsequent runs, when reliable review history is available, the agent reviews the layers that are due and any events requiring immediate attention. You can also request a narrower cycle.
4. **Compare new evidence with the existing assessments** and propose supported changes to evidence, priorities, risk velocity, relationships, or the addition, merger or retirement of risks.
5. **Check escalation conditions.** If it identifies a confirmed trigger, it will notify you within the task and prepare an escalation brief describing the evidence, proposed action and suggested responsible role. Unconfirmed signals remain pending verification.
6. **Save the results**, including a Markdown report and CSV files covering risk reviews, signal observations, sources, proposed changes, actions, escalations and the next-review schedule.

## When Internal Data Is Required

Some reviews require internal VyStar information, such as fraud metrics, liquidity data, credit portfolio performance, vendor dependencies or recovery testing results. The agent will use this information when it is supplied or available through authorized access.

If required information is unavailable, the agent will identify the missing inputs, explain which conclusions cannot yet be reached and mark the affected work as partial or blocked. It will not treat missing data as evidence that no incident or breach occurred, or claim that public research establishes VyStar's actual exposure or control effectiveness.

## What the Run Produces

Results are saved in a new run folder:

`outputs/monitoring/<YYYY-MM-DD>/<unique-run-id>/`

| File | Contents |
| --- | --- |
| `monitoring-report.md` | Findings, evidence, triggers, proposed changes, limitations and decisions needed |
| `risk-review.csv` | Review status and findings for each risk |
| `signal-observations.csv` | Indicator and trigger observations, comparisons and missing inputs |
| `source-evidence.csv` | Sources, supported claims, dates, locations and access limitations |
| `proposed-changes.csv` | Proposed changes with their rationale and approval status |
| `actions-and-escalations.csv` | Follow-up actions and escalation briefs |
| `review-schedule.csv` | Review cadences, due status and next-review dates |
| `validation.md` | Coverage, consistency checks and unresolved issues |

## Scope of Execution

The original Excel workbook remains unchanged. Proposed changes are documented separately for review; they are not automatically approved or applied.

The agent does not independently send notifications to employees, activate crisis procedures, modify external systems or create recurring monitoring automation. Those actions require a separate instruction. Producing a review schedule does not schedule future runs.

The intended result is a completed evidence-based review of the work that available information supports, together with proposed actions and clearly identified gaps. Full completion depends on access to the necessary sources and internal data, and on any required organizational decisions.

This file explains the companion prompt; it does not replace or modify its execution instructions.
