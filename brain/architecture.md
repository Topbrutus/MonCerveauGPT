# Architecture

## Purpose
Describe the external memory system architecture and how artifacts relate.

## Overview
The external brain is stored under `/brain/` and split by function:

- `memory.md`: stable facts
- `lessons.md`: lessons learned
- `failures.md`: failure analysis
- `decisions.md`: decisions and rationale
- `patterns.md`: reusable workflows
- `architecture.md`: system design notes
- `roadmap.md`: next improvements
- `repo-policy.md`: repository operating rules
- `capabilities.md`: agent permissions and operational scope
- `activity-log.md`: chronological activity journal
- `agent-config.json`: runtime configuration
- `memory.jsonl`: append-only event stream

## Operating model
1. Read existing brain state.
2. Reason on current task.
3. Act in repository with verification.
4. Write back durable learning.
