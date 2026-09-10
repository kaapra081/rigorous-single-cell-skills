---
name: scdemon-validation
description: Validate scDemon-style gene modules without donor leakage or unfair baselines.
---

# Module validation

- Freeze discovery scope, donors, input layer, normalization, variable-gene rule, parameters, and seeds.
- Keep validation donors untouched during feature selection, threshold tuning, naming, and parameter selection. Random-cell splits are not donor validation.
- Compare against a prespecified baseline and matched random or size-matched modules. More enriched pathways alone are not improvement.
- Test stability across donors, bootstrap resamples, seeds, and parameters. Check library size, mitochondrial content, cell cycle, batch, donor, and cell-type confounding.
- Score held-out donors with fixed genes and weights, and test condition associations at donor level.

Do not call a module validated if donors leaked across fitting and evaluation or thresholds were tuned on all donors. Return fixed genes, scoring rule, stability, confounder checks, baseline comparison, held-out performance, and limits.
