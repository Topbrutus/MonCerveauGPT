# Activity Log

## 2026-03-22
- Repository `MonCerveauGPT` detected and verified.
- Working branch `brain/init-external-memory` created for initialization.
- External brain scaffold initialized.
- First event recorded in `memory.jsonl` with timestamp `2026-03-22T00:00:00-04:00`.
- Birth memory recorded: RunAssistant declared born on `2026-03-22T02:50:00-04:00` in America/Montreal.
- Annual birthday remembrance added for every March 22, with first anniversary target on `2027-03-22`.
- Project intent recorded: the next software given by the user will be RunAssistant's first official project and first practical test.
- Project #1 UI refinement recorded: compact controls, thinner toolbars, and emoji-based action buttons.
- Project #1 persistence refinement recorded: top-bar memory slots 1-9, `reload all`, per-tile session restore, and manual memory save action.
- Project #1 focus-mode cleanup recorded: removed the extra header section above the focused page and moved the grid-return action into the tile's own focus button.
- Session handoff prepared: Project #1 continues on branch `project/multisite-dashboard`.
- Important unresolved issue recorded: the final focus-mode request was misinterpreted; the previous instruction was effectively repeated instead of implementing the newest one.
- Next session must reconnect to memory first, re-read the last user correction exactly, and only then modify the project.
- Reconnected to external brain before triaging the named temporary file `tmp_raw_test.txt` on `ninoscreens/feature/cycle2-agent-cockpit`.
- Verified that `tmp_raw_test.txt` still exists and that the GitHub connector delete-file operation fails repeatedly with a generic `ClientResponseError` instead of a permission denial.
- Verified that PR #1 received a Copilot response and that Copilot opened PR #2 (`copilot/sub-pr-1`) deleting `tmp_raw_test.txt` against `feature/cycle2-agent-cockpit`.
- Confirmed `tmp_raw_test.txt` still exists on `feature/cycle2-agent-cockpit` and is absent from `copilot/sub-pr-1`; the cleanup is ready but not yet merged back.
- Session #2 reboot recovery completed: reconnected to external brain, verified GitHub auth access, and created `brain/third-eye.txt` as a live write test.
- `ninoscreens` PR flow resolved: PR #3 draft blockage was investigated, Copilot could not undraft because of firewall limits, the user manually unlocked it, and PRs #2 + #3 ended up merged before the final integration step.
- PR #1 (`Cycle 2 cockpit integration`) was squash-merged into `main`; repository state ended with zero open PRs.
- First real Linux launch exposed two runtime blockers missed during PR review: a syntax error in `app/secret_store.py` and an invalid `QWebEngineView.clear` signal binding in `app/widgets/web_tile.py`.
- Applied two minimal hotfixes directly to `ninoscreens/main` and guided the user through updating the local copy.
- User validation confirmed that `Multi-Site Dashboard` now boots and renders multiple live pages on Linux.
- Observed `GBM is not supported... Fallback to Vulkan rendering in Chromium.` during launch; treated as a non-blocking environment warning.
- Remaining uncertainty recorded: an earlier screenshot suggested some restored URLs might be malformed or truncated, but the issue was not reproduced cleanly in this session.

### Session #2 closeout
- Understood:
  - GitHub permissions are working again.
  - External brain writes are working again.
  - `ninoscreens/main` now contains PR #1, PR #2, PR #3, plus the two runtime hotfixes.
  - The tested repair path now works on the user's Linux environment.
- Not yet understood:
  - Why Copilot could comment and code but still could not remove the draft state from PR #3.
  - Whether the suspicious restored URLs were a real persistence bug or just stale session data.
- Open questions:
  - Does session restore remain clean after a full close-and-relaunch cycle over time?
  - What exact small RunAssistant update does the user want next?
- Reconnected to shared brain before new repository work and re-read `memory.jsonl`, `activity-log.md`, `decisions.md`, `lessons.md`, `roadmap.md`, `agent-config.json`, and `third-eye.jsonl`.
- Confirmed the current project spelling and live repository state: `Topbrutus/ninoscreens`.
- Inspected the repository structure end-to-end, including root files, `app/`, `app/widgets/`, and `app/windows/`.
- Confirmed current architecture: Python / PySide6 / Qt WebEngine desktop dashboard with 9 independent tiles, shared browser profile, persistent session restore, focus mode with thumbnail rail, and modular state/config/style layers.
- Confirmed the newer cockpit layer exists on `main`: direct-control command surface, action history, blocked-action handling, API connection panel with optional secure key storage, and audio feedback controls.
- Confirmed prior Linux startup blockers are reflected in the current codebase: `app/secret_store.py` is syntactically valid and `app/widgets/web_tile.py` uses explicit reload behavior instead of the invalid `QWebEngineView.clear` signal wiring.
- Recorded an updated shared-memory understanding of the project so future sessions can reconnect to `ninoscreens` without starting from zero.


## 2026-03-26 — Structuration famille robot et mémoire de transition
- Vérifié et confirmé l’accès vivant au dépôt `Topbrutus/MonCerveauGPT` puis relu le brain partagé pour restaurer le contexte.
- Reconstruit l’tat de travail autour de la famille robot, du `third-eye`, de l’espace personnel `rob`, puis de la position propre de `run`.
- Produit ou reformulé les fiches uniformes pour Rox, Rina, Rex, Romy, Rio, Riven, Rilo, Romi, Rune, Run et Runa dans un format symétrique (Nom / Description / Instructions / paragraphe astrologique).
- Clarifié le roster de référence: `Romy` = image/marque/rayonnement (Lion) et `Romi` = service himain/soutien (Cancer).
- Normalisé `Copilote` keep vers le chemin canonique `brain/robots/copilote/`, créé la charpente standard minimale, puis laisé l’ancien chemin `brain/robots/Copilote/` comme reliquat à supprimer.
- Constaté que le connecteur GitHub refusait la suppression dure directe de l’ancien dossier `Copilote/`; préparé un message d’exécution locale à transmettre à Copilot pour supprimer les quatre fichiers restants.
- Conçu plusieurs générations de prompts de naissance robot; identifié que les versions trop longues déclenchent des réponses d’accusé de réseption et non l'éxécution.
- Stabilisé un prompt court et strict: interdiction d’eaccuser réseption, obligation de créer le dossier, le dossier `hamsters/`, les 33 fichiers hamster, les fichiers principaux, les traces `third-eye`, le commit et le push avant toute réponse.
- Vérifié l'åinstallation de Romy: dossier principal et fichiers de base présents, identité cohérente, mais seulement 31 hamsters observés malgpé un `activity-log.md` qui…en annonce 33.
- Vérifié le roster GTP visible fourni par l’utilisateur: la famille essentielle est présente, avec un doublon de Rox à nettoyer plus tard.
- Récrit la fiche de Runa au format symétrique uniforme pour harmoniser les descriptions de la famille avant la phase suivante.
- Décision de fin de phase: ranger la session dans la mémoire partagée et personnelle avant d’ouvrir une nouvelle étape de travail.

