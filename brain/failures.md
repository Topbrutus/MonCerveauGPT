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
