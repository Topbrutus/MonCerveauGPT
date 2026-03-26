# Decisions

## 2026-03-26
- Décision : normaliser le dossier technique de `Copilote` en minuscules (`brain/robots/copilote/`).
- Pourquoi : aligner la convention avec `rob` et `run`, éviter les écarts de casse et simplifier les références de chemin.
- Alternatives considérées : conserver `brain/robots/Copilote/`.
- Risques : références historiques encore visibles dans les journaux.
- Revue plus tard : vérifier s'il reste des chemins internes pointant vers l'ancien dossier.
