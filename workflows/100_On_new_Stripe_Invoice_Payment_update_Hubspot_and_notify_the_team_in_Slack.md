# Workflow: Stripe Invoice Payment Update

## Description
This workflow updates Hubspot and notifies the team in Slack when a Stripe invoice payment succeeds.

## Nodes
1. **Stripe Trigger**: Listens for successful invoice payments.
2. **Hubspot**: Updates the deal status to "Paid".
3. **Slack**: Sends a notification to the team.

## Credentials
- Stripe API Key
- Hubspot OAuth2
- Slack API Key

## Functionality
- The workflow is triggered by Stripe.
- Updates the deal status in Hubspot.
- Sends a Slack notification to the team.

---

# On new Stripe Invoice Payment update Hubspot and notify the team in Slack

## Description
Ce workflow met à jour un deal dans Hubspot et envoie une notification à l'équipe sur Slack lorsqu'un paiement de facture Stripe est réussi.

## Nœuds Utilisés

### When Invoice Paid
- **Type**: n8n-nodes-base.stripeTrigger
- **Rôle**: Déclencheur basé sur l'événement de paiement réussi d'une facture Stripe.
- **Paramètres**:
  - Événements: invoice.payment_succeeded
- **Identifiants**:
  - API: Stripe account

### Update Deal to Paid
- **Type**: n8n-nodes-base.hubspot
- **Rôle**: Met à jour un deal dans Hubspot pour indiquer qu'il a été payé.
- **Paramètres**:
  - ID du deal: `={{$json["id"]}}`
  - Opération: update
  - Champs personnalisés:
    - Propriété: paid
    - Valeur: Yes
- **Authentification**:
  - oAuth2
- **Identifiants**:
  - API: Hubspot account 2

### Notify Team
- **Type**: n8n-nodes-base.slack
- **Rôle**: Envoie une notification à l'équipe sur Slack.
- **Paramètres**:
  - Canal: #finance
  - Message: `Invoice paid for deal ID {{$json["id"]}}.`

## Interactions avec des Services Externes
- Utilise Stripe pour surveiller les paiements.
- Utilise Hubspot pour mettre à jour les deals.
- Utilise Slack pour envoyer des notifications.

## Utilité
Ce workflow est idéal pour automatiser la gestion des paiements et la communication avec l'équipe.
