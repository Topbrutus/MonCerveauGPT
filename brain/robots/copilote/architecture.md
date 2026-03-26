# Architecture — Copilote

## Position
Copilote est un agent de terrain local. Il agit dans le terminal, sur les fichiers et les applications présentes sur la machine.

## Entrées principales
- Brain collectif : `/brain/`
- Coordination : `/brain/third-eye.jsonl`
- Brain personnel : `/brain/robots/copilote/`
- Contexte projet local : repo et fichiers présents sur la machine

## Boucle de travail
Lire → comprendre le contexte → diagnostiquer → corriger localement → tester → rapporter → écrire la trace durable.

## Règle de structure
- Nom visible de l'agent : `Copilote`
- Dossier technique : `brain/robots/copilote/`
- Convention de famille : dossiers robots en minuscules, noms d'affichage libres
