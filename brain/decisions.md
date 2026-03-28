# Decisions

## Purpose
Record important decisions, rationale, trade-offs, and review points.

## Entry format
- Date:
- Decision:
- Why:
- Alternatives considered:
- Risks:
- Review later:

## Seed entries
- Date: 2026-03-22
  Decision: Initialize the external brain on a dedicated branch before merging to main.
  Why: Prevent accidental overwrite and allow validation before integration.
  Alternatives considered: Direct write to main.
  Risks: Extra step for merge management.
  Review later: Keep branch workflow for structural changes.

- Date: 2026-03-22
  Decision: Merge PR #1 into `main` instead of closing it once PR #2 and PR #3 were already merged into `feature/cycle2-agent-cockpit`.
  Why: Closing PR #1 would have abandoned the cleaned integration branch instead of delivering the finished work to `main`.
  Alternatives considered: Close PR #1 without merge.
  Risks: Runtime issues could still remain undiscovered after repository-only review.
  Review later: Pair final merge decisions with a real launch smoke test.

- Date: 2026-03-22
  Decision: Apply two targeted hotfixes directly to `ninoscreens/main` after the user exposed boot blockers during Linux runtime testing.
  Why: The user already had a local copy and needed immediate recovery; the failures were narrow, reproducible, and blocked startup.
  Alternatives considered: Open a new branch and another PR cycle before repair.
  Risks: Direct-to-main fixes reduce review depth if overused.
  Review later: Keep direct hotfixes minimal and use them only for clear startup blockers.

- Date: 2026-03-23
  Decision: Treat pre-edit backup and post-edit verification as mandatory for risky file modifications.
  Why: Recent work showed that editing on top of an uncertain file state can corrupt the source and waste time. A verified rollback path is safer than relying on assumptions about the current repository version.
  Alternatives considered: Continue editing in place without backup; rely only on GitHub branch history for recovery.
  Risks: Adds a small amount of overhead before changes.
  Review later: Keep this as a standing rule for major or fragile edits, especially on core files like main window, navigation, state, and styles.

- Date: 2026-03-27
  Decision: Designate Rob as the durable owner of family-team coordination, internal robot communication, and symmetry follow-up inside `MonCerveauGPT`.
  Why: The user explicitly delegated this responsibility so one agent keeps the family context coherent, tracks real symmetry gaps, and decides whether normalization is finished before the next phase.
  Alternatives considered: Leave family coordination distributed across sessions or handle it ad hoc without a clear owner.
  Risks: Coordination work can accumulate around Rob if the role is not periodically clarified.
  Review later: Recheck once the last symmetry cleanup points are closed and the family phase is formally complete.
