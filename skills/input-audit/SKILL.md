---
name: input-audit
description: Audit single-cell inputs before preprocessing or inference.
---

# Input audit

Use before normalization, clustering, differential testing, integration, or module discovery.

- Identify matrix orientation, value type, feature namespace, reference version, and every layer. Preserve immutable original counts. Never label normalized or log-transformed values as raw counts.
- Check dimensions, duplicate genes and barcodes, missing or negative values, sparsity, library sizes, and memory before densifying.
- Reconcile each cell with sample, donor, condition, tissue, batch, chemistry, and exclusion metadata. Quantify missingness and conflicts.
- Inspect QC by donor and condition. Record exclusions and thresholds without silent deletion.
- Detect reused barcodes, duplicated samples, reused donor IDs, and condition-batch confounding.

Stop if original counts cannot be identified, donor mapping is ambiguous, labels conflict, or a merge changes expected totals. Return an audit table with evidence, severity, action, donor counts, count-layer location, exclusions, and unresolved risks.
