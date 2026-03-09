---
title: Présentation des médias
description: Découvrez comment évaluer les performances des médias dans Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Media Performance, Content Attributes
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
TQID: https://experienceleague.adobe.com/fSBgN1uvr39dd7AV3Kvr3D5UnSDY2-dE1aX1g2Q7fTc
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
subfeature_v2: id: a29f532b-105a-4aec-8a5d-e7e725214866id: a98e0185-3180-4e8c-8f31-f72af4cc21a2id: dd48f9df-f2e2-49fe-a918-332a8e240ffeid: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 647
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
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions ayant généré des clics sur le média dans une annonce publicitaire.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le média est très pertinent et attrayant pour le public. Cela suggère que le message et la conception captent efficacement l&#39;intérêt du public et l&#39;incitent à agir. En outre, un taux de clics élevé peut signifier que le média est bien ciblé et qu’il correspond à l’audience visée, ce qui se traduit par de meilleures performances globales de la campagne. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût moyen pour mille impressions de média.<br>**Calcul** : montant total `spent` divisé par le nombre d’impressions, puis multiplié par 1 000 | Une valeur CPM faible peut indiquer des performances multimédias rentables, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu&#39;un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet d’identifier les médias qui entraînent des actions client importantes. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic sur le média.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget en ce qui concerne les médias individuels sur une période donnée. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |
| **[!UICONTROL Utilisé dans ces publicités]** | Nombre de publicités qui utilisent ce média. | |
| **Attributs** | Liste des fonctionnalités inhérentes présentes dans ce média. | Les attributs permettent d’identifier les éléments créatifs qui interagissent le plus avec votre audience. |
