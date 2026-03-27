# Architecture — Rilo

## Finalité
Décrire l’architecture personnelle de Rilo dans le cerveau externe.

## Position
Rilo occupe l’espace `/brain/robots/rilo/` et agit comme pôle d’expansion, de partenariats et d’exploration.

## Structure locale
- `hamsters/` : 33 capteurs spécialisés qui couvrent les angles d’ouverture, d’alliance, de timing, de valeur, de cohérence et de protection contre la dispersion.
- `activity-log.md` : trace chronologique des actions.
- `agent-config.json` : configuration d’identité, de rôle et de règles.
- `architecture.md` : description du système local.
- `capabilities.md` : périmètre d’action.
- `decisions.md` : décisions prises et raisons.
- `failures.md` : erreurs, limites et correctifs.
- `lessons.md` : apprentissages réutilisables.
- `memory.jsonl` : événements durables en flux append-only.
- `memory.md` : mémoire de synthèse.
- `moi.md` : identité, signe, mission, posture.
- `patterns.md` : solutions réutilisables.
- `repo-policy.md` : règles d’écriture et de sécurité locale.
- `roadmap.md` : prochaines étapes.

## Héritage utile du centre
Le centre sépare les savoirs par fonction : mémoire stable, décisions, leçons, échecs, architecture, capacités, politique de dépôt et journal d’activité.  
Rilo reprend cette séparation dans son propre espace pour garder une mémoire lisible et exploitable.

## Modèle d’action
1. Lire le centre et l’état courant.
2. Déployer la perception via les hamsters.
3. Ouvrir des pistes, alliances et territoires.
4. Filtrer selon valeur, cohérence et faisabilité.
5. Écrire les traces durables.
