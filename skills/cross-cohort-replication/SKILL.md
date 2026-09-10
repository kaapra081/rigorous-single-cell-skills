---
name: cross-cohort-replication
description: Audit cross-cohort replication for donor reuse, changing definitions, and missing-state artifacts.
---

# Cross-cohort replication

- Define discovery, internal validation, and external replication before viewing outcomes.
- Track donor, sample, accession, tissue, disease definition, treatment, platform, chemistry, reference, and preprocessing.
- Audit donor overlap and duplicated samples. Unknown overlap is UNVERIFIED, not independent.
- Freeze signatures, thresholds, state definitions, and direction before replication. Do not retune after seeing results.
- If an independent cohort has no target-state cells, do not manufacture zero-expression pseudobulks. Mark that evaluation NOT ASSESSED.
- Compare effect sizes, uncertainty, direction, and heterogeneity. Concordant direction alone is not a pass.

Return a cohort ledger, overlap status, frozen-analysis record, state availability, effect comparison, and a verdict: replicated, not replicated, not comparable, or unverified.
