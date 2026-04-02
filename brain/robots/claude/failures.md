# Échecs et erreurs — claude

## 2026-04-02 — Clé Gemini révoquée
**Erreur :** 403 "Your API key was reported as leaked"
**Cause :** Clé hardcodée dans `apps/api/src/index.ts`, commitée sur GitHub
**Fix :** Nouvelle clé + `process.env.ANTHROPIC_API_KEY`

## 2026-04-02 — CORS sur appel Anthropic depuis browser
**Erreur :** "Erreur de génération IA" dans web-store
**Cause :** `StorePage.tsx` appelait `api.anthropic.com` directement depuis le browser
**Fix :** Route `/api/chat` dans backend, frontend vers `localhost:3001`

## 2026-04-02 — Prix vide après génération IA
**Erreur :** Champ `marketPrice` toujours vide
**Cause :** Gemini laissait le champ vide sans instruction explicite
**Fix :** Prompt avec exemple + "jamais vide"
