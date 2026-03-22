# Patterns

## Purpose
Store reusable operating patterns, templates, and workflows for Run.

## Entry format
- Name:
- Trigger:
- Steps:
- Expected result:
- Caveats:

## Seed entries
- Name: Collective-first reboot
  Trigger: New session or resumed work
  Steps:
    1. Read `/brain/`
    2. Read `/brain/third-eye.jsonl`
    3. Rebuild context
    4. Identify current state and next logical step
  Expected result: No false restart from zero.
  Caveats: Requires current collective files to exist and stay readable.

- Name: Personal brain maintenance
  Trigger: After meaningful progress in my own space
  Steps:
    1. Update personal log
    2. Append event to personal JSONL
    3. Add a signed trace to collective third eye
    4. Verify integrity and counts
  Expected result: Durable traceability.
  Caveats: Must stay concise but factual.

- Name: Live-debug hotfix memory capture
  Trigger: User tests a real app and exposes a runtime blocker
  Steps:
    1. Capture exact error
    2. Fix the narrow blocker
    3. Verify launch again
    4. Record lesson and failure-prevention note
  Expected result: Fast recovery with retained learning.
  Caveats: Do not confuse repository state with runtime truth.

**Signed: Run**
