# New Tweets Workflow

## Description
Ce workflow utilise un déclencheur manuel pour interagir avec Twitter, permettant de récupérer ou publier des tweets.

## Détails
- **ID** : 1003
- **Nom** : New Tweets Workflow
- **Type de nœud principal** : Manual Trigger
- **Nœud Twitter** : Interactions avec Twitter

## Fonctionnalité
Ce workflow est conçu pour automatiser les interactions avec Twitter, facilitant la gestion des tweets directement depuis n8n.

# New tweets

## Description
Ce workflow recherche des tweets contenant le mot-clé "verstappen" et enregistre les informations pertinentes.

## Nœuds Utilisés

### On clicking 'execute'
- **Type**: n8n-nodes-base.manualTrigger
- **Rôle**: Déclencheur manuel pour exécuter le workflow.

### Twitter
- **Type**: n8n-nodes-base.twitter
- **Rôle**: Recherche des tweets contenant le mot-clé "verstappen".
- **Paramètres**:
  - Limite: 100
  - Opération: search
  - Texte de recherche: verstappen
  - Champs supplémentaires:
    - Type de résultat: mixed

### Set_AT_list
- **Type**: n8n-nodes-base.set
- **Rôle**: Définit une liste avec les informations des tweets.
- **Paramètres**:
  - Valeurs:
    - Nombre:
      - Nom: Likes
      - Valeur: `={{$node["Twitter"].json["favorite_count"] ? $node["Twitter"].json["favorite_count"] : 0 }}`
    - Chaîne:
      - Nom: Tweet
      - Valeur: `={{$node["get airtable list"].json["fields"]["Tweet"]}}`

## Interactions avec des Services Externes
- Utilise l'API Twitter pour rechercher des tweets.

## Utilité
Ce workflow est idéal pour surveiller les tweets contenant des mots-clés spécifiques et analyser leur popularité.
