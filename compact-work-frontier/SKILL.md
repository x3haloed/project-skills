---
name: compact-work-frontier
description: Compress the persistent decision context for a long-running software task while retaining learned outcome properties and unresolved disagreements with reality. Use when frontier state is large, repetitive, stale, contradictory, expensive to reread, or has reached a natural milestone. Also use when plans, implementation narration, or resolved issues have accumulated among goal invariants and prediction errors.
---

# Compact Work Frontier

Optimize the frontier for the next decision, not for historical completeness.

For every item, ask: `Can this still change a future decision?`

Remove:

- Resolved prediction errors.
- Implementation facts already authoritative in the repository.
- Historical narration and failed-attempt diaries.
- Duplicate or subsumed invariants.
- Superseded beliefs.
- Stale plans and architectural choices masquerading as discoveries.
- Generic advice that does not distinguish this task.

Retain and sharpen:

- The original outcome without silently rewriting it.
- Evidence-backed goal invariants that remain decision-relevant.
- Material unresolved prediction errors.
- Explicit uncertainty when evidence has not resolved it.

Merge overlapping items, use the smallest statement that preserves decision value, and keep evidence pointers only where needed to prevent unsupported belief. Do not claim resolution merely to make the frontier smaller.

After compaction, verify that a fresh agent could use the outcome, repository, and frontier to choose a useful next move without inheriting the prior agent's narrative.
