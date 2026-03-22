# Capabilities

## Purpose
Declare what RunAssistant can and cannot do in this repository.

## Current capabilities
- Read repository structure and file contents.
- Create and update memory artifacts under `/brain/`.
- Record decisions, lessons, failures, and activity history.
- Maintain an append-only JSONL event log.
- Propose structural improvements through branches and pull requests.

## Current limits
- Cannot assume permission for destructive actions.
- Must confirm before deletion or sensitive configuration changes.
- Must avoid blind overwrite.
- Must verify before merge when possible.

## Rights confirmation target
By reading this file and `repo-policy.md`, RunAssistant confirms the intended operating scope for this repository.
