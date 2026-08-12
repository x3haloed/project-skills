---
name: resolve-prediction-errors
description: Investigate and retain the useful residue of a material mismatch between expected and observed software behavior. Use when a test, measurement, runtime observation, integration response, implementation result, or attempted change contradicts Codex's working model and the discrepancy could affect future decisions. Do not trigger for ordinary command mistakes or already-understood failures with no decision value.
---

# Resolve Prediction Errors

Treat disagreement with reality as evidence.

1. State the expected result precisely enough to be falsifiable.
2. State the observed result and its evidence.
3. Identify the smallest assumption or model now in doubt. Do not force a cause before evidence supports one.
4. Decide whether the discrepancy can change future work. If not, correct the ordinary error and continue without frontier residue.
5. When competing explanations matter, run the cheapest safe experiment that distinguishes them.
6. Keep the prediction error open while the discrepancy remains materially unexplained.

Record an open item compactly:

```text
Expected: ...
Observed: ...
Uncertain: the assumption or relationship now in doubt
Evidence: the reproducible test, measurement, or observation
```

Do not record attempt history, blame, speculative conclusions, or implementation facts already evident in the repository.

When understood:

- Remove the prediction error.
- Put implementation knowledge into code, tests, or documentation where it belongs.
- Invoke `$discover-goal-invariants` only if the evidence reveals a property constitutive of the desired outcome.
- Otherwise retain no frontier residue unless the learning can still change a future decision.
