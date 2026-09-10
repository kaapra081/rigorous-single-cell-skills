---
name: target-evidence
description: Audit target claims across expression, specificity, causality, assay endpoints, potency, and modality.
---

# Target evidence

Assess separately: presence, specificity, association, perturbation, and translation. Single-cell expression supports presence or hypothesis generation, not causality, efficacy, or safety.

- Verify detection, dropout, ambient RNA, doublets, dissociation effects, assay specificity, isoform limits, and donor dependence.
- Preserve assay endpoints and bounds. Do not compare IC50 to censored Ki as if they were the same quantity, or manufacture selectivity ratios from incomparable assays.
- Distinguish RNA, protein, activity, perturbation, and functional readouts. A computational association is not experimental validation.
- Check off-target cells, tissues, conditions, delivery, safety, and whether the claimed modality is supported.

Return an evidence matrix with claim, modality, endpoint, dataset, biological replicate, effect or bound, uncertainty, confounders, directness, confidence, and what remains unestablished.
