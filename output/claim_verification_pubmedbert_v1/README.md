# PubMedBERT claim verification — v1

Scores MedCPT-reranked evidence passages against decomposed clinical claims
using `pritamdeka/PubMedBERT-MNLI-MedNLI`.

## Method
- Input: the MedCPT top-10 candidate passages for each claim.
- NLI order: evidence passage as premise, claim as hypothesis.
- Maximum sequence length: 256 tokens.
- Batch size: 8.
- Labels: contradiction, entailment, neutral (model IDs 0, 1, 2 respectively).

## Files
- `pubmedbert_predictions.jsonl`: per-claim rows with per-candidate labels and
  class scores.
- `run_manifest.json`: model configuration, counts, and output checksum.

## Interpretation
These outputs are model-generated verification signals, not clinical ground
truth, calibrated support probabilities, or evidence of clinical effectiveness.
They should be interpreted alongside the independent GatorTron signal and
the underlying passages. Model weights are not included in this backup.
