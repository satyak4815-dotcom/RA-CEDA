# GatorTron claim verification — pilot stage

- Scored 106 claim rows and 992 retrieved claim–passage pairs.
- Checkpoint: fine-tuned GatorTron sequence classifier.
- Labels: entailment, neutral, contradiction.
- Input order used: evidence passage first, claim second.
- Maximum sequence length: 128.
- Development accuracy: 0.9018; macro-F1: 0.9021 (n=1,395), from the saved training report.
- The development metrics are not EHRNoteQA pilot performance estimates.
- Pair order should be confirmed against the fine-tuning preprocessing before confirmatory evaluation.
- Model outputs are classifier signals, not ground truth or calibrated clinical truth probabilities.
- No model weights are included.

See `run_manifest.json` for provenance and the predictions file hash.
