---
title: Présentation des médias
description: Découvrez comment évaluer les performances des médias dans Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 44fedfdc3902b4f993d656ae6360a32e27a62520
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# Présentation des médias

La vue [!DNL Insights] _[!UICONTROL Média]_ affiche une liste des médias utilisés dans les annonces et les campagnes publicitaires pour le compte sélectionné. _Média_ représente une image, une vidéo, un texte ou tout autre contenu créatif approuvé pour une utilisation dans vos initiatives marketing.

{{connect-insights}}

Le tableau _[!UICONTROL Media]_ est organisé à l’aide de l’**[!UICONTROL ID de média]**. Vous pouvez basculer entre les vues à l’aide de l’icône de liste de vues (tableau) et de l’icône de vue galerie (grille). Cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles.

![Filtre média et tableau](/help/assets/insights-media-filter.png){zoomable="yes"}

La vue de galerie _[!UICONTROL Média]_ affiche un collage d’aperçus de médias et d’une mesure, telle que le taux de clic publicitaire. Cliquez sur l’icône des paramètres (cog) située au-dessus du côté droit de la galerie pour ouvrir **[!UICONTROL Paramètres de la carte]** et activer l’une des trois mesures visibles :

- Coût par action (CPA)
- Taux de clic publicitaire (CTR)
- CPC (coût par clic)
- Dépenses

{{filter-table}}

## Détails du média

Dans la vue _Détails du média_, vous pouvez voir quelles publicités utilisent le média sélectionné. Les détails incluent les performances totales du média, les publicités utilisant le média, les attributs définis par l’utilisateur et les fonctionnalités détectées par l’IA associées au média.

![Détails du média](/help/assets/insights-media-details.png){zoomable="yes"}

### Attributs de média

{{$include /help/_includes/generated-attributes.md}}

## Performances des médias

Les mesures d’informations peuvent vous aider à évaluer quels médias contribuent au succès d’une campagne et quels attributs de médias sont les plus efficaces.

Le tableau suivant fournit des définitions et des informations sur les principales mesures de marketing numérique dans la vue de tableau [!UICONTROL Médias]. Chaque mesure comprend une brève définition en ce qui concerne les médias, la manière dont la mesure est calculée et un ou plusieurs insights pour aider à comprendre sa signification et son impact.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID du média]** | Nom associé à une image, une vidéo, un texte ou tout autre contenu créatif. | Triez le tableau en cliquant sur l’en-tête de colonne de l’une des mesures clés. |
| **[!UICONTROL Impressions]** | Décompte de chaque chargement du média dans le canal, indépendamment de l’interaction ou de l’affichage. | Un nombre d’impressions élevé peut indiquer une visibilité étendue, mais pour des performances réelles d’insight, considérez-le par rapport à d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs et utilisatrices interagissent avec un élément cliquable, tel qu’un lien, sur le média. | Un nombre élevé de clics indique un intérêt et un engagement forts envers le contenu, qui peuvent être efficaces et atteindre la bonne audience. |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions ayant donné lieu à des clics dans le média d’une publicité.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le média est très pertinent et attrayant pour le public. Cela suggère que le message et la conception captent efficacement l&#39;intérêt du public et l&#39;incitent à agir. En outre, un taux de clics élevé peut signifier que le média est bien ciblé et qu’il correspond à l’audience visée, ce qui se traduit par de meilleures performances globales de la campagne. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût moyen pour mille impressions de média.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;impressions, puis multiplié par 1 000 | Une valeur CPM faible peut indiquer des performances multimédias rentables, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu’un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet d’identifier les médias qui entraînent des actions client importantes. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic sur le média.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget en ce qui concerne les médias individuels sur une période donnée. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |
| **[!UICONTROL Utilisé dans ces publicités]** | Nombre de publicités qui utilisent ce média. | |
| **Attributs** | Liste des fonctionnalités inhérentes présentes dans ce média. | Les attributs permettent d’identifier les éléments créatifs qui interagissent le plus avec votre audience. |
