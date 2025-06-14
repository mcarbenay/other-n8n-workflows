# #️⃣Nostr #damus AI Powered Reporting + Gmail + Telegram

## Description
Ce workflow utilise l'IA pour générer des rapports automatisés et les envoyer via Gmail et Telegram.

## Nœuds Utilisés

### When clicking ‘Test workflow’
- **Type**: n8n-nodes-base.manualTrigger
- **Rôle**: Déclencheur manuel pour tester le workflow.

### Get HTML
- **Type**: n8n-nodes-base.markdown
- **Rôle**: Convertit du texte Markdown en HTML.
- **Paramètres**:
  - Mode: markdownToHtml
  - Markdown: `={{ $json.text }}`

### Gmail Themes
- **Type**: n8n-nodes-base.gmail
- **Rôle**: Envoie des emails via Gmail.
- **Paramètres**:
  - Destinataire: joe@example.com
  - Message: `={{ $json.data }}`
  - Sujet: #damus

## Interactions avec des Services Externes
- Utilise Gmail pour envoyer des emails.

## Utilité
Ce workflow est idéal pour automatiser la génération et l'envoi de rapports basés sur des données Markdown, avec une intégration facile à Gmail et Telegram.
