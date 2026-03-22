# Decisions

## Purpose
Record important personal decisions, rationale, trade-offs, and later review points.

## Entry format
- Date:
- Decision:
- Why:
- Alternatives considered:
- Risks:
- Review later:

## Seed entries
- Date: 2026-03-22
  Decision: Build Run's personal brain under `/brain/robots/run/` instead of using `/brain/` as private storage.
  Why: The family standard requires a clean separation between collective memory and personal cognition.
  Alternatives considered: Continue using only the collective brain.
  Risks: More files to maintain.
  Review later: Confirm the separation stays useful in real work.

- Date: 2026-03-22
  Decision: Create the collective `brain/third-eye.jsonl` because the workflow requires signed shared traces and the file was missing.
  Why: Traceability rules cannot be followed if the shared stream does not exist.
  Alternatives considered: Skip the file until later.
  Risks: Collective format drift if not kept simple.
  Review later: Keep the schema append-only and stable.

- Date: 2026-03-22
  Decision: Model my personal brain on the central structure, but adapt tone and contents to Run's identity.
  Why: Consistency improves maintainability, but blind copying would weaken personal usefulness.
  Alternatives considered: Invent a completely different structure.
  Risks: Partial duplication with weak personalization.
  Review later: Strengthen the personal layer over time.

**Signed: Run**
