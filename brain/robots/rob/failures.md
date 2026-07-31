# Échecs — Rob

## 2026-03-22
- **Échec :** installation personnelle commencée mais incomplète lors du premier passage.
- **Cause :** exécution interrompue avant la création de toute la structure et des 33 hamsters.
- **Détection :** plusieurs fichiers requis étaient absents et l’utilisateur a relancé l’achèvement.
- **Correction :** reprendre depuis le contexte reconstruit et terminer l’espace complet sur la même branche.
- **Prévention :** valider systématiquement la checklist complète avant d’annoncer la fin d’une installation.

## 2026-03-22
- **Échec :** ambiguïté sur `third-eye.jsonl` car seul `third-eye.txt` existait.
- **Cause :** l’espace collectif n’avait pas encore de journal JSONL opérationnel.
- **Détection :** lecture du brain collectif.
- **Correction :** créer le journal attendu sans altérer les autres éléments collectifs.
- **Prévention :** vérifier les fichiers de coordination avant d’appliquer les règles de traçabilité.

## 2026-07-31
- **Échec :** impossible de conserver le mode d’emploi des 100 étapes dans `Topbrutus/robotic-arm-companion`.
- **Cause :** le dépôt n’est pas visible dans la connexion GitHub active; `get_repo` et `create_file` ont retourné HTTP 404, et la pagination complète des dépôts accessibles ne contient pas ce dépôt.
- **Détection :** résolution directe du dépôt, recherche exacte, recherche par propriétaire et tentative d’écriture sur `main`.
- **Correction requise :** reconnecter ou autoriser `Topbrutus/robotic-arm-companion`, ou créer le dépôt s’il n’existe pas encore, puis écrire `docs/communication/MODE-EMPLOI-100-ETAPES-COLONIE-V1.md` intégralement et le relire sur GitHub.
- **Prévention :** vérifier la visibilité réelle du dépôt live avant toute opération documentaire obligatoire et ne jamais substituer un autre dépôt.

## 2026-07-31 — Linuxia Première
- **Échec :** impossible d’inscrire le pré-mode d’emploi fondateur dans le nouveau dépôt nommé `Linuxia Première`.
- **Cause :** aucun dépôt correspondant n’est visible dans la connexion GitHub active; les recherches par nom et les résolutions directes de `Topbrutus/Linuxia-Premiere`, `Topbrutus/LinuxiaPremiere` et `Topbrutus/linuxia-premiere` retournent une absence ou HTTP 404.
- **Détection :** recherche des dépôts installés, recherche dans l’organisation Topbrutus et résolution directe des variantes usuelles du nom.
- **Correction requise :** créer ou connecter le dépôt officiel, puis écrire intégralement `docs/communication/LINUXIA-PREMIERE-PRE-MODE-EMPLOI-FONDATEUR.md` sur `main` et le relire sur GitHub.
- **Prévention :** obtenir le nom canonique GitHub du nouveau dépôt avant de déplacer la source officielle du projet et ne jamais substituer `Topbrutus/LinuxIA` sans instruction explicite.

Signé : **Rob**
