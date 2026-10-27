# RA-CEDA: Qwen3-8B pilot baseline

Status: **INCOMPLETE — exploratory only**

- Dataset: EHRNoteQA pilot-50
- Model: Qwen/Qwen3-8B
- Completed baseline answer records: 31
- Error records: 19
- This is a partial generation run, not a confirmatory result.
- The supplied dataset file has no gold-answer labels; these files do not
  establish clinical accuracy, faithfulness, or clinical effectiveness.
- The original answer and error files are preserved as produced.
- The recovery attempt did not produce recovery output files.
- Do not treat unresolved cases as correct or silently drop them from analysis.

Files:
- `baseline_answers.jsonl`: completed answer records, including saved prompts
- `baseline_errors.jsonl`: unresolved generation/answer-parse errors
- `baseline_run_manifest.json`: run configuration and status
