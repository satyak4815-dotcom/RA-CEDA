# Pilot-50 baseline parsing recovery

These are separate retry artifacts. They do not replace or merge into the
original baseline answer/error files.

## Provenance and limitations

- Model: Qwen/Qwen3-8B, pinned revision `b968826d9c46dd6066d109eabc6255188de91218`
- Recovery used FP16 loading, SDPA attention, greedy decoding, and up to 256 new tokens.
- This differs from the original 4-bit NF4 baseline configuration.
- Retry generations are not the original failed generations.
- `baseline_parse_retry_raw.jsonl` preserves raw retry outputs and prompts.
- `baseline_parse_retry_normalized.jsonl` records a separate normalization.
- `EHRNQ_0088` has an explicitly recovered choice from truncated JSON; other
  response fields remain null and full JSON parsing did not succeed.
- `EHRNQ_0550` remains unresolved due to CUDA out-of-memory.
- Successful parsing does not establish clinical correctness.
- These outputs are exploratory pilot artifacts, not confirmatory results.

## SHA-256

- `baseline_parse_retry_raw.jsonl`: `e356552736f0421f7e8f9aded1ee3e298c64c8fef9672b3a6662c0062ea712d6`
- `baseline_parse_retry_normalized.jsonl`: `5dee2d6e84c11badf3facf9bf173ac5775d9810387a9069ee3f267f259c961fd`
