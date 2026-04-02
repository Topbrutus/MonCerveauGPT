# Mémoire active — claude

## Contexte Gaby
- Développeur sur Linux, projet principal : depanneurIA
- Utilise Claude Code CLI avec voice dictation activée
- Langue : français québécois

## depanneurIA — état au 2026-04-02
- **API** port 3001 — Express + tsx + SQLite
- **web-client** port 5201 — gestion produits
- **web-store** port 5200 — boutique client + chat IA
- Clé Gemini dans `.env` → `ANTHROPIC_API_KEY`
- Chat IA operationnel via `/api/chat` (backend)
- Génération produit par photo operationnelle via `/api/generate-product`
- Prix toujours estimé par Gemini (prompt forcé)
