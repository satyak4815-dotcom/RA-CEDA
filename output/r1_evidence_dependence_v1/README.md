# R1 Evidence-Dependence Features

Exploratory claim-level feature table combining fused GatorTron and PubMedBERT
signals, MedCPT retrieval scores, claim decomposition, and source-summary/chunk
provenance.

- Claims: 106
- Missing MedCPT matches: 0
- Missing claim-decomposition matches: 0
- Claims with verifier disagreement: 99
- Claims with potential same-summary dependence: 106

## Interpretation

These are exploratory risk features, not calibrated decisions or ground truth.
Verifier agreement does not establish truth, and MedCPT relevance is not a
support probability. Multiple chunks from the same summary indicate potential
dependence; they do not prove that all chunks overlap. Distinct source summaries
and actual overlap should be distinguished in the subsequent CECS stage.

The data are from the EHRNoteQA pilot-50 workflow. This artifact is not evidence
of clinical effectiveness.
