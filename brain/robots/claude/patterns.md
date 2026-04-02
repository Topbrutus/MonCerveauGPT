# Patterns — claude

## Redémarrage serveur depanneurIA
```bash
kill $(ss -tlnp | grep 3001 | grep -oP 'pid=\K[0-9]+') 2>/dev/null
sleep 1
export $(cat /home/gaby/depanneurIA/.env | xargs) && node24 \
  --require .../tsx/.../preflight.cjs \
  --import "file://.../loader.mjs" src/index.ts &
```

## Route backend IA (Gemini)
Recevoir `{system, messages}` → reformater pour Gemini → retourner `{text}`

## Prompt Gemini — forcer les champs
Toujours inclure des exemples de valeurs et "jamais vide" pour chaque champ obligatoire.
