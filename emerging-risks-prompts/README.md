# Emerging Risks Prompt Library

Start with **[emerging_risks.md](emerging_risks.md)** to generate the combined AI and Non-AI workbook with its 16-sheet architecture, entities, formulas, methodology and reference design. Supply the companion [emerging_risks_reference.json](emerging_risks_reference.json) or let the agent read it from this folder. The default reproduces the historical model; explicitly request current research if you want updated assessments.

| File | Purpose |
| --- | --- |
| `emerging_risks.md` | Recommended combined-report generation prompt, reverse-engineered from the completed workbook |
| `emerging_risks_reference.json` | Exact historical cell data, expanded formulas, native table/style/chart definitions and provenance used by the generation prompt |
| `prompt-final.md` | Preserved earlier prompt for byte-for-byte Base64 restoration; it is not the combined-report generation prompt |
| `prompt-monitoring-final.md` | Execute one available monitoring cycle; provide prior run outputs for schedule-based subsequent cycles |
| `monitoring-prompt-explanation.md` | English explanation of monitoring behavior and output files |
| `ai-emerging-risks-original.md` | Preserved earlier AI-only research prompt with the superseded 11-sheet architecture |
| `ai-emerging-risks-original-notes.md` | Original notes for that AI-only prompt |
| `notes.md` | Preserved notes for the earlier restoration/monitoring package |
| `generation-notes.md` | Evidence, decisions, validation and limitations for the new combined-report prompt |

Use the new generation prompt for the combined report. Do not apply the original AI-only prompt's conflicting schemas to it. Keep this folder together when transferring it to another environment. No monitoring cycle or automation was executed while assembling this package.
