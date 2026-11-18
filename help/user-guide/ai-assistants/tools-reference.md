---
title: Référence des outils de l’assistant AI
description: Découvrez les outils d’informations, de création, de planification, d’activation et de commentaires qu’un assistant AI peut utiliser avec [!DNL GenStudio for Performance Marketing].
role: User
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 244293cf4f83acbc252f1d5f3495db403ed4a9bb
workflow-type: tm+mt
source-wordcount: '2265'
ht-degree: 13%
---

# Référence des outils de l’assistant d’IA

Cette référence décrit les outils qu’un assistant IA connecté peut utiliser avec [!DNL GenStudio for Performance Marketing]. La liste d’outils disponible dépend de la configuration de votre organisation.

Demandez à votre assistant d’IA à quels outils il peut accéder avant de démarrer un workflow.

## Domaines de capacité

| Zone | Objectif | Comportement |
|---|---|---|
| Insights | Interroger les performances des médias achetés et des e-mails et récupérer les recommandations créatives. | Lecture seule. |
| Créer | Recherchez des ressources, assemblez des brouillons à partir de modèles Express ou de recommandations Insights, puis gérez la révision. | Lecture et écriture. Crée des documents dans Creative Cloud. |
| Plan | Extrayez les détails de la campagne d’un résumé et enregistrez-les dans Workfront Planning. | L’extraction est en lecture seule. L’enregistrement crée des enregistrements dans Workfront Planning et ne peut pas être restauré automatiquement. |
| Activer | Résolvez une cible de publication et envoyez une expérience approuvée à la plateforme. | Écrire. Les publicités sont envoyées à la plateforme et publiées dans un état désactivé. Vous les activez séparément. Non réversible grâce à ces outils. |
| Commentaires | Envoyez des commentaires sur le produit à l’équipe [!DNL GenStudio for Performance Marketing]. | Écrire. |

La plupart des outils Insights couvrent `meta`, `linkedin` et `innovid`. Les outils de valeur de mesure couvrent `meta` et `linkedin`. Le rapport de campagne par e-mail couvre Adobe Journey Optimizer (`ajo`) et Adobe Campaign (`acc`).

La création prend en charge `meta`, `linkedin`, `display`, `tiktok` et `youtube`. Activate prend en charge `META`, `LINKEDIN` et `GOOGLECM360`.

## Outils Insights

### get_insights_features

Renvoie les canaux Insights et les opérations de création de rapports activés pour votre organisation. Utilisez d’abord cet outil lorsque la disponibilité n’est pas claire. Les canaux pris en charge sont `meta`, `linkedin`, `innovid`, `ajo` et `acc`.

Cet outil renvoie des métadonnées de fonctionnalité, et non des valeurs de campagne, d’annonce publicitaire ou de mesure. Pour trouver les clés de mesure personnalisées de votre organisation, utilisez `list_connected_channels_and_metrics`.

### list_connector_channels_and_metrics

Renvoie les connexions Meta, LinkedIn et Google Campaign Manager 360 actives de votre organisation, les canaux d’informations et opérations pris en charge, ainsi que les mesures de conversion personnalisées configurées. Utilisez-le pour rechercher des clés de mesure avant d&#39;appeler `get_insights_metric_values`.

Cet outil renvoie des clés de mesure, des libellés et des formats, et non des valeurs de mesure. Une connexion ne garantit pas que les données de rapports historiques sont disponibles.

| Paramètre | Requis | Description |
|---|---|---|
| `limit`, `offset` | Non | Taille de page et décalage de page. Omettez les deux pour renvoyer le catalogue complet. |

### get_insights_summary

Renvoie les mesures et les tendances des performances globales pour un canal sur une période sélectionnée.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `startDate` | Non | Date de début au format `YYYY-MM-DD`. La valeur par défaut est 30 jours auparavant. |
| `endDate` | Non | Date de fin au format `YYYY-MM-DD`. La valeur par défaut est aujourd’hui. |
| `metrics` | Non | Mesures à représenter sous forme de graphique : `spend`, `ctr`, `cpc`, `cpm`, `cpa`, `impressions`, `clicks`, `conversions`, `videoPlays`, `engagement`, `likes`, `comments` ou `shares`. La valeur par défaut est `spend`, `ctr`, `cpc` et `cpm`. |

### list_insights_campaigns

Renvoie un tableau triable de mesures de performances de campagne et une ligne de totaux.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. La valeur par défaut est les 30 derniers jours. |
| `search` | Non | Filtre de nom de la campagne. |
| `sortBy` | Non | Champ de tri : `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` ou `name`. La valeur par défaut est `spend`. Les résultats sont toujours triés par ordre décroissant. |
| `limit`, `offset` | Non | Taille de page et décalage de page. La taille de page par défaut est de 20. |

### list_insights_email_campaigns

Renvoie un tableau triable de campagnes par e-mail avec les mesures de diffusion et d’engagement pour Adobe Journey Optimizer et Adobe Campaign. Pour les campagnes publicitaires, utilisez `list_insights_campaigns`.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `ajo` ou `acc`. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. La valeur par défaut est les 30 derniers jours précédant la date de fin. |
| `search` | Non | Filtre de nom de la campagne. |
| `sortBy` | Non | Champ de tri : `campaignName`, `emailsNumber`, `emailsDelivered`, `totalClicks`, `openRate`, `ctr`, `ctor`, `bounceRate`, `unsubscribeRate` ou `spamComplaintRate`. La valeur par défaut est `emailsDelivered`. Les résultats sont toujours triés par ordre décroissant. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

### list_insights_ads

Renvoie les performances au niveau des annonces. Utilisez le mode de navigation par défaut pour un tableau triable ou un mode de niveau pour les publicités haute et basse performance.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `meta`, `linkedin` ou `innovid`. |
| `tier` | Non | `all`, `high` ou `low`. La valeur par défaut est `all`. |
| `mainMetric` | Non | Mesure de classement pour le mode de niveau `high` ou `low` : `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` ou `clicks`. Ignoré en mode de navigation. |
| `metrics` | Non | Mesures supplémentaires à rapporter pour chaque publicité en mode niveau. |
| `campaigns` | Non | Campagnes utilisées pour limiter le résultat, jusqu’à 50. Chaque campagne comprend `channel`, `accountId` et `campaignId`. |
| `search` | Non | Filtre de nom d’annonce. |
| `sortBy` | Non | Champ de tri du mode de navigation : `spend`, `impressions`, `clicks`, `ctr`, `cpc`, `cpm` ou `name`. La valeur par défaut est `spend`. Les résultats sont toujours triés par ordre décroissant. |
| `spendMin`, `spendMax` | Non | Limites de dépenses totales pour chaque publicité. Mode Niveau uniquement. |
| `includeUnsupported` | Non | Inclut des publicités dont le contenu créatif ne peut pas être rendu. La valeur par défaut est `false`. |
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

Compare les caractéristiques créatives des publicités sélectionnées à la moyenne du canal. Utilisez-le après l&#39;identification par `list_insights_ads` des annonces à performances élevées ou faibles.

| Paramètre | Requis | Description |
|---|---|---|
| `ads` | Oui | Une à 200 publicités à expliquer. Chaque publicité comprend `channel`, `accountId`, `campaignId` et `adId`, et éventuellement `adGroupId` et `performanceTier` (`high` ou `low`). Utilisez les identifiants renvoyés par `list_insights_ads` en mode niveau. |
| `mainMetric` | Oui | Mesure utilisée pour classer les publicités : `ctr`, `cpc`, `cpm`, `cpa`, `spend`, `impressions` ou `clicks`. |
| `campaigns` | Non | Campagnes utilisées pour définir la population de comparaison, jusqu’à 50. Chaque campagne comprend `channel`, `accountId` et `campaignId`. |
| `spendMin`, `spendMax` | Non | Limites de dépenses pour la population de comparaison. |
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
| `tagSource` | Non | `ad_tags` ou `campaign_tags`. La valeur par défaut est `ad_tags`. |
| `sortBy` | Non | Champ de tri : `adsCount`, `spend`, `impressions`, `clicks`, `conversionCount`, `ctr`, `cpc`, `cpm` ou `cpa`. La valeur par défaut est `adsCount`. |
| `search` | Non | Filtre de valeur de balise. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

### get_insights_metric_values

Renvoie les valeurs et les tendances des mesures suivies par votre organisation, telles que les prospects, les inscriptions ou le retour sur dépenses publicitaires, pour Meta et LinkedIn.

| Paramètre | Requis | Description |
|---|---|---|
| `channels` | Non | `meta`, `linkedin` ou les deux. |
| `metrics` | Non | Jusqu&#39;à 20 clés de mesure renvoyées par `list_connected_channels_and_metrics`. La valeur par défaut est le jeu visible par défaut de votre organisation. |
| `campaigns` | Non | Campagnes utilisées pour limiter le résultat, jusqu’à 50. Chaque campagne comprend `channel`, `accountId` et `campaignId`. |
| `startDate`, `endDate` | Non | Période au format `YYYY-MM-DD`. La valeur par défaut est les 30 derniers jours. |

### get_insights_recommendations

Retourne les modifications créatives proposées basées sur les données de performances de votre organisation. Une requête ne peut renvoyer aucune recommandation lorsque la portée sélectionnée ne contient aucune annonce publicitaire éligible.

| Paramètre | Requis | Description |
|---|---|---|
| `channels` | Oui | Un ou plusieurs parmi `meta`, `linkedin` ou `innovid`. |
| `campaigns` | Non | Campagnes utilisées pour limiter le résultat, jusqu’à 50. Chaque campagne comprend `channel`, `accountId` et `campaignId`. |
| `search` | Non | Filtre de nom de la campagne. |
| `recommendationId` | Non | Le `adUid` d’une recommandation, utilisé pour la récupérer en détail. |
| `onlyWithPreview` | Non | Exclut les recommandations qui n’ont pas d’exemple d’aperçu créatif. La valeur par défaut est `true`. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

## Création d’outils

Créez des outils pour rechercher des ressources, assembler des brouillons à partir de modèles Adobe Express et gérer la révision avant qu’une expérience ne soit prête à être activée.

### list_express_templates

Répertorie les modèles Express disponibles avec filtrage et nombre de facettes.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Non | `meta`, `display`, `linkedin`, `tiktok`, `youtube` ou `__unspecified__`. |
| `query` | Non | Terme de recherche pour les modèles. |
| `activatableMimeType`, `aspectRatios`, `externalTemplateSource`, `isHTML5Template`, `keywords`, `languages`, `mediaFormat`, `regions`, `timeframes` | Non | Filtres de facettes de modèle. |
| `sortBy` | Non | `modified` ou `created`. La valeur par défaut est `modified`. |
| `order` | Non | `asc` ou `desc`. La valeur par défaut est `desc`. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

### descriptive_express_template

Renvoie les champs de texte modifiables et les emplacements d’images dans un modèle.

| Paramètre | Requis | Description |
|---|---|---|
| `templateId` | Oui | Identifiant du modèle express. |

### list_cta_options

Renvoie les valeurs call-to-action autorisées pour un canal. L’affichage renvoie une liste vide car il accepte le texte sous forme libre.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Oui | `linkedin`, `meta`, `display`, `tiktok` ou `youtube`. |
| `limit`, `offset` | Non | Taille de page et décalage de page. Omettez les deux pour renvoyer chaque option. |

### search_assets

Effectue une recherche dans les images et les vidéos de votre contenu GenStudio. Utilisez-la pour sélectionner des ressources existantes pour un brouillon. Les ressources dérivées, externes et expirées sont exclues. Cet outil ne charge, ne modifie, ne supprime ni ne génère de ressources. Il nécessite en outre des droits sur le contenu GenStudio.

| Paramètre | Requis | Description |
|---|---|---|
| `query` | Non | Recherche par mot-clé ou en langage naturel dans les métadonnées de ressources. |
| `mediaTypes` | Non | `image`, `video` ou les deux. La valeur par défaut inclut les deux. |
| `aspectRatios` | Non | Les proportions, telles que `1:1` ou `16:9`. Si aucun rapport n’est disponible, l’outil renvoie les choix disponibles. |
| `brands`, `campaigns`, `products`, `personas`, `channels` | Non | Filtre par nom. |
| `customMetadata` | Non | Jusqu’à 5 champs de métadonnées, chacun avec une ou plusieurs valeurs. |
| `uploadedBy` | Non | `me` ou une adresse e-mail de téléchargeur. |
| `createdAtFrom`, `createdAtTo` | Non | Limites de temps de création au format ISO 8601. |
| `aiGenerated` | Non | Filtre par statut de génération de l’IA. |
| `contentCredentials` | Non | Filtre par statut de Content Credentials. |
| `limit`, `offset` | Non | Taille de page et décalage de page. |

Le résultat inclut des références de ressources stables pour `create_draft` et des URL signées de courte durée.

### create_draft

Crée un brouillon modifiable à partir d’un modèle Express avec une ou plusieurs expériences. Chaque appel crée un nouveau brouillon.

| Paramètre | Requis | Description |
|---|---|---|
| `templateId` | Oui | Identifiant du modèle express. |
| `prompt` | Oui | Instructions de résumé et de copie Creative stockées avec le brouillon. |
| `experiences` | Oui | Une ou plusieurs expériences. Voir le tableau suivant. |
| `name` | Non | Nom du document. |
| `allowAssetReuse` | Non | Permet de réutiliser une ressource sélectionnée dans plusieurs expériences. La valeur par défaut est `false`. |

Chaque expérience prend en charge les champs suivants :

| champ | Requis | Description |
|---|---|---|
| `channel` | Oui | `linkedin`, `meta`, `display`, `tiktok` ou `youtube`. |
| `title` | Non | Titre de l’expérience. La valeur par défaut est « Concept *n* ». |
| `headline` | Meta et LinkedIn | Titre du Principal. |
| `body` | Meta, LinkedIn et TikTok | Copie du corps. Pour LinkedIn, il s’agit du texte d’introduction. Pour TikTok, il s’agit du texte principal. |
| `description` | YouTube | Description de l’annonce. Facultatif pour Meta et LinkedIn. |
| `display_url` | Meta et LinkedIn | Afficher l’URL affichée dans la publicité. |
| `destination_url` | Non | URL vers laquelle l’annonce publicitaire renvoie. |
| `cta` | Non | Texte call-to-action de `list_cta_options`. |
| `templateFields` | Non | Remplace les éléments de modèle nommés de `describe_express_template`. Chaque remplacement définit du texte, une URL d’image avec des dimensions ou une URL de vidéo. |
| `assetTemplateFields` | Non | Ressources de contenu de `search_assets` pour les champs image ou vidéo dans le modèle. |

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
| `emails` | Oui | Une à 20 adresses électroniques de collaborateurs. |
| `role` | Oui | `editor` ou `viewer`. |
| `message` | Non | Message d’invitation. |

### request_draft_approval

Envoie un brouillon à une ou plusieurs personnes pour approbation.

| Paramètre | Requis | Description |
|---|---|---|
| `draftId` | Oui | Identifiant de ressource de brouillon. |
| `emails` | Oui | Une à 20 adresses e-mail des réviseurs. |

### list_expériences

Renvoie les expériences approuvées et publiées prêtes à être activées. Les brouillons ne sont pas inclus.

| Paramètre | Requis | Description |
|---|---|---|
| `channel` | Non | `email`, `meta`, `meta_organic`, `display`, `ctv`, `linkedin`, `linkedin_organic`, `tiktok`, `chatgpt` ou `youtube`. |
| `createdByMe` | Non | Limite les résultats aux expériences créées par l’utilisateur actuel. |
| `campaignNames` | Non | Jusqu’à 5 filtres de nom de campagne exacts. |
| `creatorEmail` | Non | Filtre d’e-mail du créateur. |
| `createdAtFrom`, `createdAtTo` | Non | Limites de date de création. |
| `language` | Non | Balise de langue BCP 47. |
| `limit`, `cursor` | Non | Taille de la page (1-50, 20 par défaut) et curseur de pagination. |

## Outils de planification

Les outils de plan transforment un résumé de campagne en un brouillon de campagne révisable et l’enregistrent dans Workfront Planning.

### extract_campaign_from_brief

Extrait un brouillon de campagne révisable d’un brief marketing collé. Cet outil n’enregistre aucun enregistrement. Les faits et les dates manquants ne sont pas déduits.

| Paramètre | Requis | Description |
|---|---|---|
| `briefText` | Oui | Le texte brut complet d’un résumé de campagne, jusqu’à 100 000 caractères. Les fichiers et les liens ne sont pas pris en charge. |

Le résultat comprend un brouillon de campagne, des résultats avec des citations annexes, des audiences suggérées et des avertissements.

### create_workfront_campaign

Crée une campagne Workfront Planning avec des produits et des personnages liés à partir d’un brouillon que vous avez examiné et approuvé. Cet outil n’est pas idempotent et les enregistrements ne peuvent pas être restaurés automatiquement. Inspectez Workfront avant de retenter une écriture qui aurait pu réussir.

| Paramètre | Requis | Description |
|---|---|---|
| `campaignDraft` | Oui | Le brouillon approuvé. Nécessite `name`. Les champs facultatifs sont `description`, `objective`, `keyMessaging`, `startDate`, `endDate` (`YYYY-MM-DD`), `status`, `channels`, `products` et `personas`. |
| `channelSelections` | Non | Choix approuvés pour les noms de canal ambigus. |
| `entitySelections` | Non | Approbation des enregistrements de produits et de personas existants. Utilisez `null` pour demander un nouvel enregistrement. |
| `createMissingEntities` | Non | Crée les produits et les personnages que vous avez sélectionnés comme nouveaux. La valeur par défaut est `false`. |

Si un produit, une personne ou un canal est ambigu, l’outil renvoie des choix à confirmer et n’apporte aucune modification.

## Activer les outils

Activez les outils pour résoudre une cible de média payant et envoyer une expérience approuvée à la plateforme. Les publicités sont publiées dans un état désactivé (Meta en pause, LinkedIn en version brouillon, Campaign Manager 360 inactif), vous devez donc les activer séparément avant qu’elles ne soient diffusées. L’envoi d’annonces publicitaires à la plateforme n’est pas réversible via ces outils.

### configure_activation_target

résout et valide le compte de média payant, la campagne, la visionneuse d’annonces et la page Facebook, le cas échéant.

| Paramètre | Requis | Description |
|---|---|---|
| `platform` | Oui | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `platformAccountId` | Non | Identifiant du compte média payant. Omettez-le pour découvrir les comptes. |
| `campaignId` | Non | Identifiant de campagne pour Meta ou LinkedIn. Non utilisé pour le gestionnaire de campagne 360. |
| `adsetId` | Non | Visionneuse d’annonces Meta ou identifiant de campagne LinkedIn. Non utilisé pour le gestionnaire de campagne 360. |
| `pageId` | Non | Identifiant de page Facebook pour Meta. |

Pour Campaign Manager 360, seul le compte publicitaire est requis.

### create_activation

Envoie une expérience approuvée à la plateforme sous forme de publicités, à l’aide d’une cible validée. Les publicités sont publiées dans un état désactivé. Meta crée une publicité avec la première image pour chaque format. LinkedIn et Campaign Manager 360 créent une annonce publicitaire pour chaque image résolue.

| Paramètre | Requis | Description |
|---|---|---|
| `platform` | Oui | `META`, `LINKEDIN` ou `GOOGLECM360`. |
| `targetId` | Oui | Cible validée renvoyée par `configure_activation_target`. |
| `experienceId` | Oui | Identifiant d’expérience approuvé renvoyé par `list_experiences`. |
| `name` | Non | Nom d’affichage de l’emplacement publicitaire. La valeur par défaut est le titre de l’annonce publicitaire de l’expérience. |

Le résultat répertorie le nombre d’annonces créées, mises en file d’attente et ignorées, avec le statut initial de chaque annonce et un lien vers celle-ci dans [!DNL GenStudio for Performance Marketing]. Un statut de `PENDING` signifie que le traitement est en file d’attente et non que la publicité est diffusée.

Appeler `create_activation` deux fois crée des annonces supplémentaires au lieu de mettre à jour les premières annonces.

## Outil Commentaires

### submit_mcp_feedback

Envoie des commentaires sur un outil ou un workflow à l&#39;équipe [!DNL GenStudio for Performance Marketing].

| Paramètre | Requis | Description |
|---|---|---|
| `category` | Oui | `bug`, `feature_request` ou `workflow_friction`. |
| `comment` | Oui | Description concise du retour d’informations. |
| `tags` | Non | Balises utilisées pour classer les commentaires. |
| `tool_name` | Non | Outil associé aux commentaires. |

## Workflows courants

Utilisez ces séquences lorsqu’un outil fournit des identifiants ou une configuration pour un autre :

- **Diagnostiquer une annonce publicitaire :** appeler `list_insights_ads` en mode de niveau `high` ou `low`, puis appeler `get_insights_ad_attributes` avec la même mesure de classement.
- **Analysez par balise :** appelez `get_insights_tag_categories`, puis appelez `get_insights_ad_tags` avec une catégorie renvoyée.
- **Vérifier les mesures suivies :** appeler `list_connected_channels_and_metrics`, puis appeler `get_insights_metric_values` avec les clés de mesure renvoyées.
- **Convertir une recommandation en brouillon :** Appeler `get_insights_recommendations`, puis appeler `create_draft_from_recommendation`.
- **Créer à partir d&#39;un modèle :** appeler `list_express_templates`, `describe_express_template` et `list_cta_options`, puis appeler `create_draft`.
- **Créer à partir de ressources existantes :** appeler `search_assets`, puis transmettre les références de ressource renvoyées à `create_draft` dans `assetTemplateFields`.
- **Enregistrez un brief de campagne dans Workfront :** appelez `extract_campaign_from_brief`, vérifiez le brouillon, puis appelez `create_workfront_campaign`.
- **Envoyer une expérience approuvée à une plateforme :** Appeler `list_experiences`, puis appeler `configure_activation_target` et `create_activation`.

## Fonctionnalités connexes

- [Présentation des assistants d’IA](overview.md)
- [Connecter un assistant d’IA](connect-ai-assistants.md)
- [Utilisation des assistants d’IA](use-ai-assistants.md)
