---
name: github-automation-skill
description: Permet à l'agent d'automatiser la génération de fichiers, les commits et les pushs Git via Docker.
---

## Description
Ce skill définit les capacités et les règles de sécurité permettant à un agent autonome de gérer un dépôt GitHub localisé sur le VPS.

## Context & Environment
- **OS Host :** Debian / Ubuntu VPS
- **Runtime :** Docker (Alpine Git)
- **Authentification :** SSH Mount (`~/.ssh/id_rsa`)
- **Dépôt cible :** BOURGINEAlexandre/n8n-skills

## Guidelines & Rules
- Toujours vérifier le git status avant de commiter.
- Utiliser des messages de commit explicites (feat:, fix:, docs:).
- Ne jamais inclure de clés d'API ou de secrets dans le dépôt.

## Step-by-Step Instructions
1. Génération : Écrire ou mettre à jour le contenu cible dans SKILL.md.
2. Inspection : Détecter s'il y a des modifications non commitées.
3. Commit & Push : Effectuer git add, git commit et git push origin main.
