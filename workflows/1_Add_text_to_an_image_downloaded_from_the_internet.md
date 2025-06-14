# Add text to an image downloaded from the internet

## Description
Ce workflow télécharge une image depuis Internet et y ajoute du texte.

## Nœuds Utilisés

### On clicking 'execute'
- **Type**: n8n-nodes-base.manualTrigger
- **Rôle**: Déclencheur manuel pour exécuter le workflow.

### HTTP Request
- **Type**: n8n-nodes-base.httpRequest
- **Rôle**: Télécharge une image depuis une URL.
- **Paramètres**:
  - URL: https://docs.n8n.io/assets/img/final-workflow.f380b957.png
  - Format de réponse: file

### Edit Image
- **Type**: n8n-nodes-base.editImage
- **Rôle**: Ajoute du texte à l'image téléchargée.
- **Paramètres**:
  - Texte: This is n8n
  - Taille de police: 100
  - Opération: text
  - Position X: 300
  - Position Y: 500

## Interactions avec des Services Externes
- Télécharge une image depuis une URL.

## Utilité
Ce workflow est idéal pour personnaliser des images téléchargées en y ajoutant du texte.
