# NinoScreen Handoff — 2026-03-28

## Stable baseline to resume from
- Focus works.
- Split works.
- Selecting a tile from the right-side selector now replaces pane 2 instead of replacing pane 1.
- Top-bar icons work.
- Split pairs are visible in the 36-button bar.
- Per-tile split memory works during the session.
- Split size memory works during the session.

## Good moves from this session
- Fix one behavior at a time instead of refactoring everything at once.
- Work from the user's local working copy when the repo and local state drift apart.
- Keep backups before touching `main_window.py`, `focus_view.py`, `page_matrix.py`, and other fragile files.
- Use immediate syntax checks after each risky patch.
- Stop once the user confirms the core behavior works.

## Bad moves / traps observed
- Mixing old `FocusView` API and newer `main_window.py` logic caused breakage.
- Pushing toward persistence or extra polish before stabilizing split behavior created regressions.
- Restoring too many heavy pages at startup makes the app appear frozen.
- Treating split as a global temporary state instead of per-tile state caused the "desnap" problem.

## Exact next step
Make session/split persistence durable across full application restart:
- keep page memory across restart
- keep split partner memory across restart
- keep split percentage across restart

## After that
Start the RUN/GPT phase so the GPT can manipulate the software from the stable interface.

## Resume instruction
Continue exactly where this handoff stops. Do not restart from scratch. The stable reference state is:
- split works
- icons work
- overall app is usable
- persistence is the next missing layer
