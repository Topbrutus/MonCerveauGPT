# Architecture personnelle de Rune

## Position

- centre partagé : `/brain/`
- espace personnel : `/brain/robots/rune/`
- coordination collective : `/brain/third-eye.jsonl`
- essaim local : `/brain/robots/rune/hamsters/`

## Principe

Rune agit comme un intégrateur silencieux entre :
- la mémoire partagée
- la mémoire personnelle
- les journaux d’activité
- les décisions
- les patterns
- les flux entre fichiers

## Savoirs initiaux repris du centre

Les savoirs utiles du centre ont été recopiés sous forme de synthèse locale :

- la mémoire collective est séparée en fichiers à fonction claire
- la coordination passe par `third-eye.jsonl`
- la traçabilité repose sur des journaux, des décisions, des leçons et une mémoire structurée
- chaque espace robot doit rester identifiable, cohérent et limité à son propre périmètre
- l’append est préférable à l’écrasement aveugle
- la validation doit précéder la clôture

## Organisation

- `moi.md` : identité, rôle, posture
- `agent-config.json` : configuration active
- `activity-log.md` : actions réalisées
- `memory.jsonl` et `memory.md` : faits, états, synthèse
- `decisions.md` : choix et raisons
- `lessons.md` : apprentissages
- `patterns.md` : solutions réutilisables
- `repo-policy.md` : règles de dépôt
- `roadmap.md` : prochaines étapes
- `hamsters/` : sous-agents de perception, de contrôle et de protection
