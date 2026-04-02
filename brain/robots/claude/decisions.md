# Décisions — claude

## 2026-04-02 — Appels API via backend seulement
Ne jamais appeler une API externe depuis le frontend browser.
→ Toujours passer par le backend Express.
**Raison :** CORS bloque les appels directs. La clé serait exposée dans le JS.

## 2026-04-02 — Clés API dans .env uniquement
→ Toujours utiliser `process.env.NOM_VARIABLE` et stocker dans `.env`.
**Raison :** Clé Gemini hardcodée détectée par GitHub et révoquée automatiquement.

## 2026-04-02 — Gemini comme moteur IA principal
Le projet depanneurIA utilise Gemini 2.5 Flash. La variable s'appelle `ANTHROPIC_API_KEY` pour des raisons historiques.

## 2026-04-02 — Mémoire persistante dans MonCerveauGPT
Maintenir un cerveau dans ce repo ET en local pour le contexte disponible partout.
