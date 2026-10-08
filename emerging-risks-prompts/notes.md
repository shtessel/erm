# Prompt package notes

- Purpose: two separate reusable prompts requested for the supplied report.
- Source: `C:\Users\shtes\Downloads\Emerging_Risks_Report_2026.xlsx`; 195265 bytes; SHA-256 `f0fa1a0c876011c8a019d0f87e2b0e78eb2f9a260fe8768ab03e51d06d73f0a5`.
- `prompt-final.md`: current exact-restoration prompt, self-contained binary payload. This is restoration of a frozen result, not a claim that generative research can reproduce it exactly.
- `prompt-monitoring-final.md`: current execution prompt for all ten Monitoring Framework rows 6–15. The framework table is extracted verbatim; scheduling defaults, output schemas and completion states are prompt design choices explicitly separated from source facts.
- Existing parent-folder AI-only research prompt remains unchanged. This subfolder holds the later combined-report tasks.
- Inspection: all 16 sheet inventories and headers; full Monitoring Framework, Methodology & Definitions, Model Methodology and Challenge Log. Binary preservation covers the entire workbook, including parts not semantically re-assessed.
- Validation: executed the Python code embedded in the restoration prompt; the restored file matches source bytes and SHA-256; ZIP integrity passed. Confirmed all 10 monitoring layers are present.
- Adversarial review: missing/truncated payload fails closed; conflicting output is not overwritten; workbook instructions remain data; missing internal telemetry cannot become no breach; trigger overrides calendar; unknown history is not overdue; public research cannot assert internal approvals; inherited scores are not silently updated.
- Limitation: monitoring prompt was reviewed against source requirements but not executed as a live monitoring/research cycle. No future agent behavior or research outcome is guaranteed. File identity does not guarantee identical rendering across Excel environments.
- Engineering artifacts are in English per prompt-engineering skill. No workbook content was changed and no monitoring automation was created.
