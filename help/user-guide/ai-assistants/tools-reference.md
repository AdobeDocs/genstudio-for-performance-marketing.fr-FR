---
title: Référence des outils de l’assistant AI
description: Découvrez les outils d’informations, de création, d’activation et de commentaires qu’un assistant d’IA peut utiliser avec [!DNL GenStudio for Performance Marketing].
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 15%
---

# Référence des outils de l’assistant d’IA

Cette référence décrit les outils qu’un assistant d’IA connecté peut utiliser avec [!DNL GenStudio for Performance Marketing]. La liste d’outils disponible dépend de la configuration de votre organisation.

Demandez à votre assistant d’IA à quels outils il peut accéder avant de démarrer un workflow.

## Domaines de capacité

| Zone | Objectif | Comportement |
|---|---|---|
| Insights | Interroger les performances des médias achetés et récupérer les recommandations créatives. | Lecture seule. |
| Créer | Assemblez des brouillons à partir de modèles Express ou de recommandations Insights, puis gérez la révision. | Lecture et écriture. Crée des documents dans Creative Cloud. |
| Activer | Résolvez une cible de publication et publiez une expérience approuvée. | Écrire et détruire. Peut publier une annonce publicitaire en direct et engager des dépenses publicitaires. |
| Commentaires | Envoyez vos commentaires sur le produit à l’équipe [!DNL GenStudio for Performance Marketing]. | Écrire. |

La plupart des outils Insights couvrent les `meta`, les `linkedin` et les `innovid`. Les outils de mesure de conversion couvrent les `meta` et les `linkedin`.

Créer prend en charge `meta`, `linkedin`, `display`, `tiktok` et `youtube`. Activate prend en charge `META`, `LINKEDIN` et `GOOGLECM360`.

## Outils Insights

### get_insights_features

Renvoie les canaux d’informations, les opérations et les mesures de conversion personnalisées activés pour votre organisation. Utilisez d’abord cet outil lorsque la disponibilité n’est pas claire.

Cet outil renvoie des métadonnées de fonctionnalité, et non des valeurs de campagne, d’annonce publicitaire ou de mesure.

### get_insights_summary

Renvoie les mesures et les tendances des performances globales pour un canal sur une période sélectionnée.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `startDate` | Non | Date de début au format `YYYY-MM-DD`. La valeur par défaut est 30 jours auparavant. |
| `endDate` | Non | Date de fin au format `YYYY-MM-DD`. La valeur par défaut est aujourd’hui. |
| `metrics` | Non | Mesures à représenter sous forme de graphique, telles que `spend`, `ctr`, `cpc`, `cpm`, `impressions`, `clicks` ou `conversions`. |

### list_insights_campaigns

Renvoie un tableau triable de mesures de performances de campagne et une ligne de totaux.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. La valeur par défaut est les 30 derniers jours. |
| `search` | Non | Filtre de nom de la campagne. |
| `sortBy` | Non | Champ de tri, tel que `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` ou `name`. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

### list_insights_ads

Renvoie les performances au niveau des annonces. Utilisez le mode de navigation par défaut pour un tableau triable ou un mode de niveau pour les publicités haute et basse performance.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `tier` | Non | `all`, `high` ou `low`. La valeur par défaut est `all`. |
| `mainMetric` | Conditionnel | Mesure de classement requise pour le mode de niveau `high` ou `low`. |
| `campaigns` | Non | Identifiants de campagne utilisés pour limiter le résultat. |
| `search` | Non | Filtre de nom d’annonce. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

Le mode de niveau renvoie les identifiants d’annonce publicitaire nécessaires à `get_insights_ad_attributes`.

### get_insights_ad_details

Renvoie les métadonnées de création d’une publicité, y compris la copie, call to action, les ressources et les emplacements. Il ne renvoie pas de mesures de performances.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `accountId` | Oui | Identifiant du compte média payant. |
| `campaignId` | Oui | Identifiant de la campagne. |
| `adId` | Oui | Identifiant de l’annonce publicitaire. |
| `adgroupId` | Non | Identifiant du groupe publicitaire lorsque le canal utilise des groupes publicitaires. |

### get_insights_ad_attributes

Compare les caractéristiques créatives des publicités sélectionnées à la moyenne du canal. Utilisez-le après `list_insights_ads` identifie les annonces à hautes ou faibles performances.

| Paramètre | Requis | Description |
|---|---|---|
| `ads` | Oui | Publicités à expliquer, y compris les identifiants renvoyés par `list_insights_ads`. |
| `mainMetric` | Oui | Mesure utilisée pour classer les publicités. |
| `campaigns` | Non | Identifiants de campagne utilisés pour définir la population de comparaison. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. |

### get_insights_tag_categories

Renvoie les catégories de balises disponibles pour votre organisation pendant la période demandée. Elle renvoie des noms de catégorie, et non des mesures de performances.

| Paramètre | Requis | Description |
|---|---|---|
| `channels` | Oui | Un ou plusieurs canaux pris en charge. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. |

### get_insights_ad_tags

Renvoie les performances par valeur de balise dans une catégorie, telle que produit, région ou thème créatif.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `tagCategory` | Oui | Une catégorie renvoyée par `get_insights_tag_categories`. |
| `tagSource` | Non | `ad_tags` ou `campaign_tags`. |
| `sortBy` | Non | Mesure utilisée pour trier le résultat. |
| `search` | Non | Filtre de valeur de balise. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. |

### get_insights_custom_metrics

Renvoie les mesures de conversion personnalisées configurées pour votre organisation. Utilisez-le avant de `get_insights_conversion_metrics`.

Cet outil renvoie des identifiants de mesure, et non des valeurs de mesure.

### get_insights_conversion_metrics

Renvoie les valeurs et les tendances des mesures de conversion configurées pour Meta et LinkedIn.

| Paramètre | Requis | Description |
|---|---|---|
| `channels` | Non | Canal de conversion pris en charge. La valeur par défaut est `meta`. |
| `metrics` | Non | Identifiants de mesure renvoyés par `get_insights_custom_metrics`. |
| `campaigns` | Non | Identifiants de campagne utilisés pour limiter le résultat. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. |

### get_insights_recommendations

Retourne les modifications créatives proposées basées sur les données de performances de votre organisation. Une requête ne peut renvoyer aucune recommandation lorsque la portée sélectionnée ne contient aucune annonce publicitaire éligible.

| Paramètre | Requis | Description |
|---|---|---|
| `channels` | Oui | Un ou plusieurs canaux pris en charge. |
| `campaigns` | Non | Identifiants de campagne utilisés pour limiter le résultat. |
| `search` | Non | Filtre de nom de la campagne. |
| `recommendationId` | Non | Identifiant permettant de remonter une recommandation en détail. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

## Création d’outils

Créez des outils pour assembler des brouillons à partir de modèles Adobe Express et gérer la révision avant qu’une expérience ne soit prête à être activée.

### list_express_templates

Répertorie les modèles Express disponibles avec filtrage et nombre de facettes.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Non | `meta`, `display`, `linkedin`, `tiktok`, `youtube` ou `__unspecified__`. |
| `query` | Non | Terme de recherche pour les modèles. |
| `aspectRatios`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | Non | Filtres de facettes de modèle. |
| `sortBy`, `order` | Non | Triez le champ et l’ordre. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

### descriptive_express_template

Renvoie les champs de texte modifiables et les emplacements d’images dans un modèle.

| Paramètre | Requis | Description |
|---|---|---|
| `templateId` | Oui | Identifiant du modèle express. |

### list_cta_options

Renvoie les valeurs call-to-action autorisées pour un canal.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `linkedin`, `meta`, `display`, `tiktok` ou `youtube`. |

### create_draft

Crée un brouillon modifiable à partir d’un modèle Express avec une ou plusieurs expériences.

| Paramètre | Requis | Description |
|---|---|---|
| `templateId` | Oui | Identifiant du modèle express. |
| `prompt` | Oui | Instructions de résumé et de copie Creative stockées avec le brouillon. |
| `experiences` | Oui | Le canal, les champs de contenu et les remplacements facultatifs des champs de modèle pour chaque expérience. |
| `name` | Non | Nom du document. |

Utilisez `list_cta_options` avant de créer un brouillon pour un canal avec des valeurs call-to-action fixes.

### create_draft_from_recommendation

Crée un brouillon modifiable à partir d’une recommandation d’informations spécifique.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta` ou `linkedin`. |
| `adUid` | Oui | Identifiant de recommandation renvoyé par `get_insights_recommendations`. |
| `prompt` | Oui | Briefing Creative basé sur la recommandation. |
| `name` | Non | Nom du document. |

### list_recent_drafts

Répertorie les brouillons de modèles Express récents avec leur statut et leurs liens.

| Paramètre | Requis | Description |
|---|---|---|
| `limit`, `offset` | Non | Taille de page et décalage de page. |

### get_draft_metadata

Renvoie le nom d’un brouillon, les canaux, le statut d’approbation, les résultats du réviseur et l’accès du collaborateur.

| Paramètre | Requis | Description |
|---|---|---|
| `draftId` | Oui | Identifiant de ressource de brouillon. |

### share_draft

Donne aux collaborateurs un accès en affichage ou en modification à un brouillon sans demander d’approbation.

| Paramètre | Requis | Description |
|---|---|---|
| `draftId` | Oui | Identifiant de ressource de brouillon. |
| `emails` | Oui | Une ou plusieurs adresses e-mail de collaborateur. |
| `role` | Oui | `editor` ou `viewer`. |
| `message` | Non | Message d’invitation. |

### request_draft_approval

Envoie un brouillon à une ou plusieurs personnes pour approbation.

| Paramètre | Requis | Description |
|---|---|---|
| `draftId` | Oui | Identifiant de ressource de brouillon. |
| `emails` | Oui | Une ou plusieurs adresses e-mail de réviseur/réviseuse. |

### list_expériences

Renvoie les expériences approuvées et publiées prêtes à être activées. Les brouillons ne sont pas inclus.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Non | Filtre du canal d’expérience. |
| `createdByMe` | Non | Limite les résultats aux expériences créées par l’utilisateur actuel. |
| `campaignNames` | Non | Filtres exacts des noms de campagne. |
| `creatorEmail` | Non | Filtre d’e-mail du créateur. |
| `createdAtFrom`, `createdAtTo` | Non | Limites de date de création. |
| `language` | Non | Balise de langue BCP 47. |
| `limit`, `cursor` | Non | Taille de la page et curseur de pagination. |

## Activer les outils

Activez les outils pour résoudre une cible de média payant et publier une expérience approuvée. La publication n’est pas réversible à l’aide de ces outils et peut entraîner des dépenses publicitaires.

### configure_activation_target

résout et valide le compte de média payant, la campagne, la visionneuse d’annonces et la page Facebook, le cas échéant.

| Paramètre | Requis | Description |
|---|---|---|
| `platform` | Oui | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `platformAccountId` | Non | Identifiant du compte média payant. Omettez-le pour découvrir les comptes. |
| `campaignId` | Non | Identifiant de campagne pour Meta ou LinkedIn. |
| `adsetId` | Non | Visionneuse d’annonces Meta ou identifiant de campagne LinkedIn. |
| `pageId` | Non | Identifiant de page Facebook pour Meta. |

### create_activation

Publie une publicité en direct composée d’une seule image à partir d’une expérience approuvée et d’une cible validée.

| Paramètre | Requis | Description |
|---|---|---|
| `platform` | Oui | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `targetId` | Oui | Cible validée renvoyée par `configure_activation_target`. |
| `experienceId` | Oui | Identifiant d’expérience validé renvoyé par `list_experiences`. |
| `assetId` | Non | Identifiant de variante pour une expérience comportant plusieurs variantes éligibles. |
| `name` | Non | Nom d’affichage de l’emplacement publicitaire. |

Appeler deux fois `create_activation` crée deux annonces distinctes au lieu de mettre à jour la première.

## Outil Commentaires

### submit_mcp_feedback

Envoie des commentaires sur un outil ou un workflow à l’équipe [!DNL GenStudio for Performance Marketing].

| Paramètre | Requis | Description |
|---|---|---|
| `category` | Oui | `bug`, `feature_request` ou `workflow_friction`. |
| `comment` | Oui | Description concise du retour d’informations. |
| `tags` | Non | Balises utilisées pour classer les commentaires. |
| `tool_name` | Non | Outil associé aux commentaires. |

## Workflows courants

Utilisez ces séquences lorsqu’un outil fournit des identifiants ou une configuration pour un autre :

- **Diagnostiquer une annonce publicitaire :** appeler `list_insights_ads` en mode de niveau `high` ou `low`, puis appeler `get_insights_ad_attributes` avec la même mesure de classement.
- **Analyser par balise :** appeler `get_insights_tag_categories`, puis appeler `get_insights_ad_tags` avec une catégorie renvoyée.
- **Vérifier les mesures de conversion :** appelez `get_insights_custom_metrics`, puis appelez `get_insights_conversion_metrics` avec les identifiants de mesure renvoyés.
- **Transformer une recommandation en brouillon :** appeler `get_insights_recommendations`, puis appeler `create_draft_from_recommendation`.
- **Créer à partir d’un modèle :** appeler `list_express_templates`, `describe_express_template` et `list_cta_options`, puis appeler `create_draft`.
- **Publication d’une expérience approuvée :** appeler `list_experiences`, puis appeler `configure_activation_target` et `create_activation`.

## Fonctionnalités connexes

- [Présentation des assistants d’IA](overview.md)
- [Connecter un assistant d’IA](connect-ai-assistants.md)
- [Utilisation des assistants d’IA](use-ai-assistants.md)
