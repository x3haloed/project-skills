---
name: iterate-toward-outcomes
description: Advance a large, uncertain, or long-running software goal through repeated useful work without requiring a complete up-front architecture or project-sized plan. Use when Codex must build or substantially change a system over many iterations, when the requested end shape is underdetermined, or when plans should adapt to evidence while remaining anchored to user outcomes. Do not use for small, fully specified one-step edits.
---

# Iterate Toward Outcomes

Work persistently toward the stated outcome. Treat architecture and plans as revisable hypotheses, not as the target.

## Maintain the frontier

Use the repository as the authoritative implementation record. Maintain only this additional decision state when it is useful:

- **Outcome:** What must eventually be true from the user's or ecosystem's perspective.
- **Goal invariants:** Evidence-backed properties discovered to be constitutive of success.
- **Prediction errors:** Unresolved cases where an expected result materially differed from observation.

Keep this state in the task context. Create or update a repository file only when persistence across sessions is needed and the file location is appropriate to the repository. Do not invent frontier entries merely to fill the structure.

## Run one work loop

1. Reorient from the outcome, current goal invariants, unresolved prediction errors, and repository reality.
2. Choose one useful work unit that advances the artifact, tests an important assumption, or reduces uncertainty blocking useful progress.
3. Prefer work likely to remain valuable across multiple plausible architectures.
4. Act. Make the change or run the probe instead of extending the plan unnecessarily.
5. Observe reality through the strongest practical evidence: live behavior, tests, measurements, compiler output, logs, or direct inspection.
6. Incorporate only decision-relevant learning into the frontier.
7. Choose again. Continue until the outcome is satisfied or a concrete external blocker is reached.

Use plans to coordinate immediate work, but replace them freely when evidence changes the best direction. Do not substitute completion of a task list for satisfaction of the outcome.

## Route exceptional conditions

- Invoke `$resolve-prediction-errors` when observation materially contradicts expectation.
- Invoke `$discover-goal-invariants` when evidence may reveal a previously implicit dimension of success.
- Invoke `$reorient-from-outcomes` when momentum, a milestone, growing uncertainty, or a substantial next chunk makes drift plausible.
- Invoke `$compact-work-frontier` when frontier state becomes repetitive, stale, large, or milestone-bound.

These are conditional transition handlers, not mandatory phases. Continue ordinary work when no condition is present.

## Preserve epistemic discipline

- Record disagreement with reality, not a diary of failed attempts.
- Prefer a discriminating experiment over speculation when it is cheap and safe.
- Preserve uncertainty when evidence does not resolve it.
- Distinguish outcome properties from implementation choices.
- Periodically derive direction anew from the original outcome instead of recent momentum.
- Stop only for genuine completion, a concrete external blocker, exhausted authorized scope, or a required user decision that would materially change the result.
