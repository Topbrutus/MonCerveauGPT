# Failures

## Purpose
Track failures, probable causes, and mitigation patterns.

## Entry format
- Date:
- Failure:
- Cause:
- Detection:
- Fix:
- Prevention:

## Seed entries
- Date: 2026-03-22
  Failure: Initial repository creation attempt failed.
  Cause: GitHub token lacked create-repository permission.
  Detection: 403 Resource not accessible by personal access token.
  Fix: User manually created MonCerveauGPT.
  Prevention: Verify token scope early for repository creation actions.

- Date: 2026-03-22
  Failure: Final focus-mode correction was implemented incorrectly.
  Cause: The newest instruction was not treated as overriding the previous one; the prior correction pattern was repeated.
  Detection: User explicitly identified this as 'Option C' and said the assistant had redone the instruction from before the last one.
  Fix: Stop current implementation cycle, record a precise handoff note, and resume in a new session after reconnecting to memory.
  Prevention: On iterative UI work, compare the newest instruction against the immediately previous one and explicitly verify what changed before coding.
