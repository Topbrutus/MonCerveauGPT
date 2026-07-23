# LinuxIA — jeu canonique d’images de la fourmi

Date : 2026-07-23

## Décision de Brutus

Les images de la fourmi LinuxIA seront générées **une à la fois** et conservées durablement sur GitHub.

- une image maîtresse unique;
- 36 orientations;
- pas de 10° : 000° à 350°;
- même personnage, posture, taille, centre, palette et transparence;
- seul l’angle change;
- chaque nouvelle frame réutilise la même image maîtresse comme référence;
- une image validée n’est jamais écrasée silencieusement;
- une correction crée une nouvelle version (`v2`, `v3`, etc.).

## Emplacement canonique

Dépôt : `Topbrutus/LinuxIA`

Branche stable : `main`

Dossier :

```text
assets/fourmi/rotation-360-test/
```

Contenu initial :

- `README.md`;
- `frame-prompt-template.md`;
- `manifest.json` avec les 36 angles.

Commit de fusion : `c12f7fb9df3ee85b0c745deedfa5d3515419728d`

## Reprise exacte

Prochaine action : créer et valider l’image maîtresse `reference/ant-master-v1.png`, puis générer `frame-000-v1.png` avant toute autre orientation.

Signé : **Rob**
