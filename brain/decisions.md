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
