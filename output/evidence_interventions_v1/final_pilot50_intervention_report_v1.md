# RA-CEDA v3.2 — Pilot-50 Evidence Intervention Results

**Status:** Exploratory pilot; not a confirmatory clinical evaluation.

## Run coverage

- Planned generations: 365 (73 claims × 5 conditions).
- Regeneration: none; original raw generations preserved.
- Recovered candidate rows: 174.
- Recovery status counts: `{"candidate_with_trailing_text": 135, "candidate_with_possible_followup_answer": 39, "not_recovered_object_count_not_one": 183, "not_recovered_invalid_choice": 8}`

## Paired choice changes versus control

| Intervention | Usable matched claims | Changed choices | Change rate |
|---|---:|---:|---:|
| real_deletion | 18 | 2 | 11.1% |
| sham_deletion | 16 | 0 | 0.0% |
| real_masking | 18 | 1 | 5.6% |
| sham_masking | 20 | 2 | 10.0% |

## Matched real-versus-sham comparison

| Intervention family | Matched claims | Matched examples | Real changed | Sham changed |
|---|---:|---:|---:|---:|
| deletion | 14 | 5 | 0 | 0 |
| masking | 18 | 8 | 1 | 2 |

## Interpretation

The observed results describe answer-choice sensitivity among recoverable outputs only. They do not establish clinical correctness, faithfulness, or hallucination reduction. Recovery-related selection bias, small matched samples, and clustering of claims within examples limit interpretation.

## Limitations and next step

- No gold labels are available in this pilot workflow.
- Verifier outputs and retrieval scores are signals, not ground truth.
- Ambiguous or unrecovered generations remain excluded from the initial paired comparison rather than being guessed or regenerated.
- Before confirmatory claims, establish gold key-fact labels, predeclare metrics and analysis, and evaluate on a separate locked test set.

## Source artifacts

- `qwen3_8b_runs/intervention_answers.jsonl`
- `qwen3_8b_runs/recovered_answer_candidates.jsonl`
- `paired_answer_comparison_v1.jsonl`
- `paired_answer_comparison_summary_v1.json`
- `matched_real_vs_sham_summary_v1.json`

The raw generations were not modified by this report-generation step.
