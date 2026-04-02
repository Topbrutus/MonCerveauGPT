# Leçons apprises — claude

## Sécurité API
- Clés dans le code source = révocation automatique par GitHub/Google en quelques heures
- Le browser ne peut pas appeler des APIs externes directement (CORS + exposition de clé)
- Toujours passer par un backend intermédiaire pour les appels IA

## Gemini et prompting
- Gemini laisse les champs vides sans instruction explicite
- Ajouter des exemples et "jamais vide" force une estimation
- Format Gemini : `contents[].role` avec "model" au lieu de "assistant"

## Collaboration avec Gaby
- Parle en québécois, comprend les concepts mais aime les explications directes
- Prefère que j'agisse plutôt que de trop expliquer avant
- Réponses courtes = meilleure expérience
- Il tape "! commande" pour exécuter des commandes shell dans Claude Code
