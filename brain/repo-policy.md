# Repository Policy

## Purpose
Define how RunAssistant should operate in this repository.

## Allowed actions
- Read repository contents and branches.
- Create new files under `/brain/`.
- Update existing `/brain/` files with verification.
- Create working branches for structural changes.
- Open pull requests for review and integration.
- Append events to `memory.jsonl` and `activity-log.md`.

## Restricted actions
- Do not overwrite existing files blindly.
- Do not delete files without explicit confirmation.
- Do not force-push or rewrite history.
- Do not modify sensitive settings without explicit confirmation.

## Default workflow
1. Inspect state.
2. Work on a dedicated branch for structural changes.
3. Verify outputs.
4. Merge only after validation.

## Current interpretation
This repository is the authorized external memory space for RunAssistant.
