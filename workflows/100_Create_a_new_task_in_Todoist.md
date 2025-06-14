# Workflow: Create a New Task in Todoist

## Description
This workflow creates a new task in Todoist when manually triggered.

## Nodes
1. **Manual Trigger**: Initiates the workflow.
2. **Todoist**: Creates a new task in Todoist.

## Credentials
- Todoist API Key

## Functionality
- The workflow is manually triggered.
- It creates a new task in Todoist with specified content.

## Detailed Documentation

# Create a new task in Todoist

## Description
Ce workflow permet de créer une nouvelle tâche dans Todoist.

## Nœuds Utilisés

### On clicking 'execute'
- **Type**: n8n-nodes-base.manualTrigger
- **Rôle**: Déclencheur manuel pour exécuter le workflow.

### Todoist
- **Type**: n8n-nodes-base.todoist
- **Rôle**: Crée une nouvelle tâche dans Todoist.
- **Paramètres**:
  - Contenu: (vide)
  - Options: {}
- **Identifiants**:
  - API: (vide)

## Interactions avec des Services Externes
- Utilise l'API Todoist pour créer une tâche.

## Utilité
Ce workflow est idéal pour automatiser la création de tâches dans Todoist.

---
