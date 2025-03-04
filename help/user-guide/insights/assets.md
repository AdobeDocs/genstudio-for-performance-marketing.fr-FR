---
title: Présentation d’Assets
description: Découvrez comment évaluer les performances des ressources dans Adobe GenStudio for Performance Marketing.
feature: Insights, Assets
exl-id: 1e93422b-2645-4e29-a216-fc1008afbfc7
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# Présentation d’Assets

La vue [!DNL Insights] _[!UICONTROL Assets]_ affiche une liste des ressources utilisées dans les expériences et les campagnes publicitaires pour le compte de canal sélectionné.

{{connect-insights}}

Le tableau _[!UICONTROL Assets]_ est organisé à l’aide de [!UICONTROL ID de ressource]. Vous pouvez basculer entre les vues à l’aide de l’icône de liste de vues (tableau) et de l’icône de vue galerie (grille). Cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles. L’icône de filtre (entonnoir) située au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtre]** dans lequel vous pouvez effectuer une sélection à partir de plusieurs listes. Cliquez sur **Réinitialiser** pour effacer toutes les sélections de filtres.

![Filtre et tableau Assets](/help/assets/insights-assets-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

La vue de la galerie _[!UICONTROL Assets]_ affiche un collage d’aperçus de ressources et d’une mesure, telle que le taux de clic publicitaire. Cliquez sur l’icône des paramètres (cog) située au-dessus du côté droit de la galerie pour ouvrir **[!UICONTROL Paramètres de la carte]** et activer l’une des trois mesures visibles :

- Coût par action (CPA)
- Taux de clic publicitaire (CTR)
- CPC (coût par clic)
- Dépenses

## Détails de la ressource

Une _ressource_ est une image, une vidéo, un texte ou tout autre contenu créatif approuvé pour une utilisation dans vos initiatives marketing.

Dans la vue des détails de la ressource, vous pouvez voir quelles expériences utilisent la ressource sélectionnée. Les détails incluent les performances totales de la ressource, les attributs définis par l’utilisateur et les fonctionnalités détectées par l’IA associées à la ressource.

![Détails de la ressource](/help/assets/insights-asset-details.png){zoomable="yes"}

## Performances des ressources

Les mesures d’informations peuvent vous aider à évaluer quelles ressources contribuent au succès d’une campagne et quels attributs de ressource sont les plus efficaces.

Le tableau suivant fournit des définitions et des informations sur les principales mesures de marketing numérique dans la vue du tableau [!UICONTROL Assets]. Chaque mesure comprend une brève définition en ce qui concerne une ressource, la manière dont la mesure est calculée et un ou plusieurs insights pour aider à comprendre son importance et son impact sur une ressource.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL ID de ressource]** | Nom associé à cette ressource. | Triez le tableau en cliquant sur l’en-tête de colonne de l’une des mesures clés. |
| **[!UICONTROL Impressions]** | Nombre de fois où la ressource se charge dans le canal, quelle que soit l’interaction ou l’affichage. | Un nombre d’impressions élevé peut indiquer une visibilité étendue, mais pour obtenir de véritables informations sur les performances, considérez-les par rapport à d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs interagissent avec un élément cliquable, tel qu’un lien, sur la ressource. | Un nombre élevé de clics indique un intérêt et un engagement forts envers le contenu, qui peuvent être efficaces et atteindre la bonne audience. |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions qui ont généré des clics sur les ressources dans une expérience.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le contenu est hautement pertinent et attrayant pour l’audience. Cela suggère que le message et la conception captent efficacement l&#39;intérêt du public et l&#39;incitent à agir. En outre, un taux de clics élevé peut signifier que la ressource est bien ciblée et correspond à l’audience visée, ce qui se traduit par de meilleures performances globales de la campagne. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût pour mille impressions publicitaires pour la ressource.<br>**Calcul** : montant total `spent` divisé par la portée, puis multiplié par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu’un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet d’identifier les ressources qui entraînent des actions client importantes. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic sur une ressource.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget en ce qui concerne les actifs individuels sur une période donnée. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |
| **[!UICONTROL Nombre d’expériences]** | Nombre d’expériences qui utilisent cette ressource. | |
| **[!UICONTROL Attributs]** | Liste des attributs détectés et appliqués à cette ressource. | |
