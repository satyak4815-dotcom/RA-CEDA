# Claim verifier fusion — v1

Aligns GatorTron and PubMedBERT NLI outputs for the same claims and evidence
passages.

## Method
- Align by claim identity and candidate passage key.
- Preserve each verifier's predicted label and available class scores.
- Record per-passage agreement or disagreement.
- Do not average probabilities or assign a final support threshold.

## Interpretation
Agreement between two models is not ground truth. Their scores are model
signals and may share errors or biases. This artifact is an intermediate
research output, not a clinical decision tool or evidence of effectiveness.

## Files
- `fused_verifier_signals.jsonl`: aligned predictions per claim and passage.
- `run_manifest.json`: counts, method, and SHA-256 checksum.
