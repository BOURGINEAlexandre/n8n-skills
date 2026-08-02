---
name: n8n-skills-manager
description: Skill d'automatisation et de gestion des workflows n8n, intégration Git et APIs.
---

## Rules & Standards
- Exporter les workflows au format JSON valide dans `/workflows`.
- Ne jamais inclure de tokens, passwords ou clés d'API en dur dans les JSON ou les fichiers .md.
- Utiliser l'API n8n ou le node Git natif pour l'historisation des changements.

## Workflow Execution Steps
1. **Trigger** : Déclenchement via Webhook, Cron ou événement Git.
2. **Process** : Exécution des nodes n8n (Code JS/Python, HTTP Request, Transform).
3. **Commit & Push** : Sauvegarde automatique du repo `n8n-skills` vers GitHub (`origin main`).
