# Journal d'activités — claude

## 2026-04-02 — Session initiale avec Gaby

### Accompli
- Diagnostiqué erreur chat IA web-store (CORS + clé manquante)
- Créé route `/api/chat` dans backend Express (Gemini côté serveur)
- Migré `StorePage.tsx` vers `localhost:3001/api/chat`
- Corrigé clé Gemini révoquée → `process.env.ANTHROPIC_API_KEY`
- Forcé estimation de prix dans prompt Gemini
- Créé mémoire persistante locale
- Créé cerveau complet dans `brain/robots/claude/`

### État final
Tous les bugs de génération IA résolus. Serveur opérationnel port 3001.
