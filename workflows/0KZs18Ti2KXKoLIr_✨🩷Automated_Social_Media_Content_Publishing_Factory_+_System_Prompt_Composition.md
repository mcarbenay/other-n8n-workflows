# Workflow Documentation: Automated Social Media Content Publishing Factory + System Prompt Composition

## Description
Ce workflow déclenche une action lorsqu'un message de chat est reçu, pour automatiser la publication de contenu sur les réseaux sociaux et composer des prompts système.

## Détails
- **ID** : 0KZs18Ti2KXKoLIr
- **Nom** : Automated Social Media Content Publishing Factory + System Prompt Composition
- **Type de nœud principal** : Chat Trigger
- **Instance ID** : 31e69f7f4a77bf465b805824e303232f0227212ae922d12133a0f96ffeab4fef
- **Webhook ID** : faddb40a-7048-4398-a0f9-d239a19c32ce

## Fonctionnalité
Ce workflow est conçu pour automatiser la publication de contenu sur les réseaux sociaux et faciliter la composition de prompts système basés sur les messages reçus.

## Nœuds

### 1. When chat message received
- **Type**: `@n8n/n8n-nodes-langchain.chatTrigger`
- **Webhook ID**: `faddb40a-7048-4398-a0f9-d239a19c32ce`
- **Options**: `{}`

### 2. Sticky Note20
- **Type**: `n8n-nodes-base.stickyNote`
- **Content**: `## LLM`
- **Color**: `7`
- **Height**: `240`

### 3. Sticky Note21
- **Type**: `n8n-nodes-base.stickyNote`
- **Content**: `## Chat Memory`
- **Color**: `7`
- **Height**: `240`

## Résumé
Ce workflow est idéal pour les entreprises cherchant à automatiser leurs publications sur les réseaux sociaux tout en intégrant des prompts système basés sur les interactions de chat.
