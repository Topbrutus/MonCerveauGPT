# Rob — Module maître Bridge, résumés, réponses et test de 10 threads

## Date

2026-07-17

## Demande de Brutus

Créer un très grand module extrêmement explicatif pour terminer une fois pour toutes les trois fonctions prioritaires :

1. Bridge bidirectionnel Terminal Antmux ↔ Nino ↔ page ChatGPT;
2. résumé automatique de fin de job correctement classé et remis à Jules;
3. boîte de réponses Nino avec réponse corrélée, retour au terminal et archivage.

Brutus demande que tout le monde travaille simultanément et souhaite essayer un test réel de dix voies de travail en même temps.

## Action effectuée

Création et relecture dans `Topbrutus/Antmux`, branche `main`, du document :

```text
docs/communication/MODULE-MAITRE-FINALISER-BRIDGE-RESUMES-REPONSES-TEST-10-THREADS.md
```

Commit Antmux :

```text
37fce468b9ca550251375a20986354a1967e063f
```

Blob vérifié :

```text
c41e43505deae773f1d2bea9e6bd8459743e2a66
```

## Architecture retenue

- Reine-Linuxia demeure l’orchestratrice Codex unique.
- Grok 3 demeure l’orchestrateur Grok unique.
- Dix voies de travail sont définies sans compter les deux orchestrateurs :
  1. JOURNALIER-01 — UI Pages et boîte de réponses;
  2. JOURNALIER-02 — moteur Bridge;
  3. Grok 1 — inventaire;
  4. Grok 2 — DOM et capture de réponse;
  5. Claude 1 — architecture et conditions de course;
  6. Gemini Flash 1 — parcours UI et observabilité;
  7. OSS Local 1 — harness, charge et preuves;
  8. Jules — résumé, livraison et retour;
  9. Hermès — memory pack et Obsidian;
  10. Copilot — baseline et revues.

Le test exige dix identités réelles, une fenêtre commune de `RUNNING` d’au moins soixante secondes, dix heartbeats et des preuves de processus ou de session. Aucun heartbeat simulé ou busy-loop artificielle n’est accepté.

## Garde-fous

- D-only;
- `.venv/` et `data/` intacts;
- checkpoint non destructif avant les worktrees;
- fichiers d’écriture disjoints;
- deux Journaliers Codex seulement;
- aucun push ou merge;
- aucune clé SSH privée;
- aucune donnée Web reçue exécutée comme commande;
- deux reprises automatiques maximum;
- fermeture seulement si Bridge, résumé, réponse, dix threads et non-régression sont tous PASS.

## Reprise exacte

Donner à Reine-Linuxia la section `Prompt central exact à donner à Reine-Linuxia` du module maître. La première preuve attendue est le prévol local, suivi de la liste des dix voies réellement disponibles et de leur réservation avant tout lancement mutateur.

Signé : **Rob**
