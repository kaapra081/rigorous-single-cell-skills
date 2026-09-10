---
name: donor-level-inference
description: Design donor-aware single-cell inference and prevent pseudoreplication.
---

# Donor-level inference

- State the estimand: abundance, expression, distribution, or program score. Cells are nested within donors and are not independent biological replicates.
- Draw nesting and pairing. Count independent donors per group and report imbalance.
- Prefer donor-level summaries or pseudobulk counts with an appropriate model. Use mixed models only when nesting, covariance, convergence, and identifiability are explicit.
- Include paired donor terms and batch only when the design identifies them. Do not claim a disease effect when disease is perfectly confounded with batch.
- Define contrasts and the full multiple-testing family before inspecting significance. Report effect sizes and uncertainty.

Stop if donor IDs are missing, pairing is unverified, or the proposed model cannot distinguish the effect from batch. Return the design table, formula, replicate count, contrast, testing family, effect size, and sensitivities.
