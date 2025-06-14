# Typeform Feedback Workflow

## Description
Ce workflow collecte les retours d'expérience des utilisateurs via Typeform et filtre les réponses avant de les enregistrer dans Google Sheets.

## Détails
- **ID** : 1001
- **Nom** : Typeform Feedback Workflow
- **Type de nœud principal** : Typeform Trigger
- **Notes** : Feedback de cours
- **Webhook ID** : 1234567890
- **Formulaire ID** : yxcvbnm

## Fonctionnalité
Ce workflow est conçu pour automatiser la collecte de feedback des utilisateurs via Typeform et faciliter leur traitement dans n8n.

## Nœuds Utilisés

### Typeform Trigger
- **Type**: n8n-nodes-base.typeformTrigger
- **Rôle**: Déclencheur basé sur les réponses d'un formulaire Typeform.
- **Paramètres**:
  - Form ID: yxcvbnm
- **Identifiants**:
  - API: typeform

### IF
- **Type**: n8n-nodes-base.if
- **Rôle**: Filtre les réponses en fonction de leur utilité.
- **Paramètres**:
  - Conditions:
    - Utilité >= 3

### Google Sheets
- **Type**: n8n-nodes-base.googleSheets
- **Rôle**: Enregistre les retours positifs dans une feuille Google Sheets.

## Interactions avec des Services Externes
- Typeform pour collecter les réponses.
- Google Sheets pour enregistrer les données filtrées.

## Utilité
Ce workflow est idéal pour les entreprises cherchant à analyser les retours d'expérience des utilisateurs et à identifier les réponses les plus utiles.
