# ✨🩷Automated Social Media Content Publishing Factory + System Prompt Composition

## Description
Ce workflow automatise la publication de contenu sur les réseaux sociaux en utilisant des prompts système. Il inclut des fonctionnalités de mémoire de chat et de gestion des messages reçus.

## Détails
- **ID** : 0KZs18Ti2KXKoLIr
- **Nom** : Automated Social Media Content Publishing Factory + System Prompt Composition
- **Type de nœud principal** : Chat Trigger
- **Instance ID** : 31e69f7f4a77bf465b805824e303232f0227212ae922d12133a0f96ffeab4fef
- **Webhook ID** : faddb40a-7048-4398-a0f9-d239a19c32ce

## Fonctionnalité
Ce workflow est conçu pour automatiser la publication de contenu sur les réseaux sociaux et faciliter la composition de prompts système basés sur les messages reçus.

## Nœuds Utilisés

### When chat message received
- **Type**: @n8n/n8n-nodes-langchain.chatTrigger
- **Rôle**: Déclencheur basé sur les messages reçus via un chat.
- **Webhook ID**: faddb40a-7048-4398-a0f9-d239a19c32ce

### Sticky Note20
- **Type**: n8n-nodes-base.stickyNote
- **Rôle**: Note collante pour indiquer "LLM".
- **Paramètres**:
  - Couleur: 7
  - Hauteur: 240

### Sticky Note21
- **Type**: n8n-nodes-base.stickyNote
- **Rôle**: Note collante pour indiquer "Chat Memory".
- **Paramètres**:
  - Couleur: 7
  - Hauteur: 240

## Interactions avec des Services Externes
- Utilise un webhook pour recevoir des messages de chat.

## Utilité
Ce workflow est idéal pour les entreprises cherchant à automatiser la gestion et la publication de contenu sur les réseaux sociaux tout en intégrant des fonctionnalités avancées de mémoire et de prompts système.
