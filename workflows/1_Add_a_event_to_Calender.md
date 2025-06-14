# Add a event to Calender

## Description
Ce workflow ajoute un événement à Google Calendar.

## Nœuds Utilisés

### On clicking 'execute'
- **Type**: n8n-nodes-base.manualTrigger
- **Rôle**: Déclencheur manuel pour exécuter le workflow.

### Google Calendar
- **Type**: n8n-nodes-base.googleCalendar
- **Rôle**: Ajoute un événement à Google Calendar.
- **Paramètres**:
  - Début: 2020-06-25T07:00:00.000Z
  - Fin: 2020-06-27T07:00:00.000Z
  - Calendrier: shaligramshraddha@gmail.com
  - Champs supplémentaires: {}
- **Identifiants**:
  - API: new one

## Interactions avec des Services Externes
- Utilise Google Calendar pour gérer les événements.

## Utilité
Ce workflow est idéal pour automatiser l'ajout d'événements à un calendrier Google.
