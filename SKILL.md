---
name: n8n-skills-library
description: Catalogue maître des compétences et workflows n8n (Fork BOURGINEAlexandre/n8n-skills) pour l'agent Claude.
version: 1.0.0
---

# n8n Skills Capability Index

Ce fichier sert d'index global des fonctions et capacités n8n disponibles dans ce dépôt pour l'agent Claude.

## 📌 Rôle de l'Agent (Claude)
Lorsque l'utilisateur demande une automatisation, un flux de travail ou une intégration :
1. Identifie la compétence requise dans le catalogue ci-dessous.
2. Utilise la structure, les nœuds et la logique des workflows présentés dans ce dépôt.
3. Respecte les conventions de nommage et les bonnes pratiques d'intégration (Home Assistant, APIs, Webhooks, etc.).

## 📚 Catalogue des Compétences & Integrations

### 1. Workflows & Automatisations de Base
- **Gestion des Webhooks** : Ingestion, parsing et réponse rapide HTTP.
- **Transformation de Données** : Manipulation JSON, nœuds Code (JS/Python), filtres et agrégations.
- **Intégration Git & GitHub** : Exécution de commits, pushs et gestion de dépôts à distance.

### 2. Monitoring & Domotique (Environnement HA / VPS)
- **Home Assistant API** : Interaction avec l'API REST/WebSocket de HA, lecture d'états d'entités, déclenchement de services.
- **Alerting & Notifications** : Envoi de messages structurés (Telegram, Discord, Gotify, Email).

### 3. Exécution & Modèles IA
- **Connecteurs LLM / Ollama** : Interfaçage avec des instances locales Ollama / OpenAI API pour l'analyse de texte et la structuration de données.

## ⚙️ Règles et Contraintes de Sécurité
- **Secrets & Credentials** : Ne jamais écrire de tokens ou mots de passe en dur. Utiliser systématiquement la gestion des Credentials n8n ou les variables d'environnement (`$env()`).
- **Robustesse** : Inclure des nœuds de gestion d'erreur (Error Trigger) pour les appels réseau critiques.
- **Format** : Les exports de workflows doivent toujours être au format JSON strict n8n.
