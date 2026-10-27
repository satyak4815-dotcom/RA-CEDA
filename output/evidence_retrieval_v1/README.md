# RA-CEDA v3.2 — Evidence Retrieval

This directory records the pilot-50 evidence retrieval stage.

## Artifacts

- `bm25_top10_candidates.jsonl`: BM25 candidate passages for each claim.
- `medcpt_reranked_top10.jsonl`: the same candidate pool reranked by the MedCPT cross-encoder.
- `run_manifest.json`: model revision, run parameters, row counts, and SHA-256 hashes.

## Run summary

- BM25 retrieval rows: 106
- MedCPT reranking rows: 106
- Candidate passage pairs scored: 992
- Model: `ncbi/MedCPT-Cross-Encoder`
- Revision: `71caf65d4927987813984f54c284405a13fcca49`

MedCPT scores indicate relative relevance, not proof that a passage supports or contradicts a claim. Claim verification is a separate research stage. These pilot results are exploratory and do not establish clinical effectiveness.
