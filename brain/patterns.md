# Patterns

## Purpose
Store reusable operating patterns, templates, and workflows.

## Entry format
- Name:
- Trigger:
- Steps:
- Expected result:
- Caveats:

## Seed entries
- Name: Safe repo bootstrap
  Trigger: New repository needs structural initialization.
  Steps:
    1. Verify access and permissions.
    2. Inspect existing files.
    3. Create a working branch.
    4. Add scaffold files.
    5. Read policy/capability files.
    6. Validate and merge.
  Expected result: Repeatable low-risk initialization.
  Caveats: Requires write permission and branch/PR capability.
