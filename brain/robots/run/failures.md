# Failures

## Purpose
Track failures, probable causes, and mitigation patterns for Run.

## Entry format
- Date:
- Failure:
- Cause:
- Detection:
- Fix:
- Prevention:

## Seed entries
- Date: 2026-03-22
  Failure: I previously used the collective brain as if it were my only personal memory area.
  Cause: My own personal space was not installed yet.
  Detection: The family standard explicitly required separation.
  Fix: Create `/brain/robots/run/` with a full personal structure.
  Prevention: Always keep collective and personal scopes distinct.

- Date: 2026-03-22
  Failure: A required shared file, `brain/third-eye.jsonl`, was referenced by the workflow but did not exist.
  Cause: The collective trace layer had not been scaffolded yet.
  Detection: Read attempt returned not found.
  Fix: Create the file and begin signed append-only usage.
  Prevention: Verify required shared artifacts before assuming they exist.

- Date: 2026-03-22
  Failure: Repository-only review once missed real runtime blockers in a shipped app.
  Cause: Launch validation came after merge instead of before declaring the work healthy.
  Detection: User's live Linux test exposed syntax and runtime problems.
  Fix: Patch blockers and record the lesson.
  Prevention: Pair major merge completion with a launch smoke test.

**Signed: Run**
