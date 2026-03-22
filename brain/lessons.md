# Lessons

## Purpose
Capture lessons learned from successes, mistakes, and repeated workflows.

## Entry format
- Date:
- Context:
- Lesson:
- Action to reuse:
- Outcome:

## Seed entries
- Date: 2026-03-22
  Context: Initial setup of external memory repository.
  Lesson: Create a dedicated branch before structural changes to reduce risk.
  Action to reuse: Use a working branch for initialization and structural updates.
  Outcome: safer repository bootstrap

- Date: 2026-03-22
  Context: Iterative UI corrections on Project #1.
  Lesson: The newest user instruction must override earlier nearby instructions; do not reuse the previous fix pattern unless it still matches the latest wording.
  Action to reuse: Before implementing a follow-up correction, restate the delta between the last accepted change and the new request.
  Outcome: Better handoff quality and lower risk of repeating the wrong correction.

- Date: 2026-03-22
  Context: First real Linux launch after merging the `ninoscreens` integration work.
  Lesson: Repository inspection and merged PR status are not enough to declare a desktop app healthy; the first live launch can still reveal syntax and runtime blockers.
  Action to reuse: After major merges, ask for or perform a launch smoke test before calling the work complete.
  Outcome: Two startup blockers were caught quickly and fixed.

- Date: 2026-03-22
  Context: PySide6 `QWebEngineView` toolbar signal wiring.
  Lesson: Do not assume generic widget methods exist on WebEngine widgets; bind reload controls to `reload()` and keep explicit reset logic separate.
  Action to reuse: Check the actual Qt class API before wiring button callbacks on browser components.
  Outcome: Prevented a restore-time crash caused by `QWebEngineView.clear`.

- Date: 2026-03-22
  Context: Live debugging with a user who had already downloaded a stale local copy.
  Lesson: Remote hotfixes do not help until the user re-syncs, re-downloads, or patches the local files.
  Action to reuse: Every GitHub hotfix should be paired with a concrete local recovery command.
  Outcome: Faster user recovery during iterative debugging.
