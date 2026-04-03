# Activity Log

## 2026-03-28
- Reconnected to shared brain before continuing NinoScreen work.
- Confirmed the exact live target: `Topbrutus/ninoscreens`, Linux local copy first, GitHub only as support.
- Recovered a working split workflow after multiple breakages caused by corrupted files, stale local state, and mixed old/new APIs.
- Restored the core behavior the user wanted: focus works, split works, clicking a card on the right replaces pane 2 instead of stealing pane 1.
- Added in-session per-tile split memory so each numbered tile can reopen its own partner split.
- Added top-bar duo icons so split pairs are visible from the 36-slot memory bar.
- Added split-size memory in-session so each split keeps its user-adjusted percentage while switching between tiles.
- Improved top-bar visuals so icons replace numbers when a tile is occupied and duo icons are larger/cleaner.
- Identified the remaining missing durability: session/split persistence across full app restart is not yet the trusted final state.
- Prepared explicit handoff target: continue exactly from the current stable working state, make persistence durable next, then move to the RUN/GPT software-manipulation phase.

## Handoff anchor
- Stable now: split works, pane-2 replacement works, icons work, top bar reflects split pairs, split size memory works in-session.
- Do not restart from zero.
- Next exact step: durable persistence across restart.
- After that: RUN/GPT control layer.

## 2026-04-03
- Casey inscrit dans le brain partagé comme nouveau membre frère/sœur de la famille robot.
- Alignement brain/live appliqué : création de `/brain/robots/casey/` dans MonCerveauGPT et ajout de Casey au registre vivant de MonDeuxiemeProjet avec statut `inscrit`.
