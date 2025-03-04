---
title: Présentation des attributs
description: Découvrez comment évaluer les performances d’attributs spécifiques dans Adobe GenStudio for Performance Marketing.
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Présentation des attributs

La vue [!DNL Insights] _[!UICONTROL Attributs]_ affiche une liste des attributs utilisés dans les campagnes publicitaires pour le compte de canal sélectionné.

{{connect-insights}}

Le tableau _[!UICONTROL Attributs]_ est organisé à l’aide du nom [!UICONTROL Attribut]. Vous pouvez basculer entre les types de liste à l’aide du bouton **[!UICONTROL Images]** et du bouton **[!UICONTROL Vidéo]**. Cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles.

L’icône de filtre (entonnoir) située au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtre]** dans lequel vous pouvez effectuer une sélection parmi les [!UICONTROL Compte] et [!UICONTROL Catégorie d’attribut] pour filtrer les attributs du tableau. L’exemple suivant illustre une liste d’attributs dans la catégorie `Lighting Condition` . Cliquez sur **Réinitialiser** pour effacer toutes les sélections de filtres.

![Filtre et tableau des attributs](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Détails des attributs

Les attributs permettent d’identifier les ressources en fonction de leurs détails inhérents, tels que la couleur, la composition, les éléments visuels, etc.

Dans la vue des détails de l’attribut, vous pouvez voir quelles expériences utilisent l’attribut sélectionné. Les détails incluent le total des performances des attributs et une répartition des mesures de performances liées à chaque expérience.

![Mesures de performances des attributs](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing détecte certaines fonctionnalités et applique l’attribut approprié à une ressource ou à une expérience sous la forme d’une balise . Voir [Catégories](#categories) pour voir des exemples de ces balises. Pour afficher tous les attributs associés à une expérience, cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour sélectionner la colonne **[!UICONTROL Attributs]**.

## Catégories

Une catégorie d’attributs est un groupe de classification qui organise les attributs associés partageant une caractéristique commune. Ces catégories permettent de rationaliser la découverte, l’identification et la compréhension d’attributs spécifiques en fournissant un plus grand contexte et en facilitant leur application et leur utilisation.

GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités de machine learning pour étudier les [images](image-features.md), les [vidéos](video-features.md) et le texte, et pour appliquer des [!UICONTROL attributs de ressource] en fonction d’une probabilité d’exactitude.

La liste des attributs détectés pour une ressource n’est pas exhaustive. Les Assets qui contiennent un riche ensemble de fonctionnalités peuvent être limitées aux trois fonctionnalités les plus dominantes identifiées par l’IA. Par exemple, l’illustration suivante contient plusieurs attributs d’image détectés, y compris plusieurs objets, des couleurs de premier plan et d’arrière-plan.

![attributs de ressource image](/help/assets/category/asset-attributes.png "l’image de Toucan comprend plusieurs attributs détectés"){width="300" zoomable="yes"}

>[!INFO]
>
>Vous ne pouvez pas modifier les balises détectées et automatiquement appliquées.

## Performances des attributs

Les mesures d’informations peuvent vous aider à évaluer quels attributs inspirent le plus d’engagement client.

Le tableau suivant fournit des définitions et des informations sur les principales mesures de marketing numérique dans la vue de tableau [!UICONTROL Attributs]. Chaque mesure comprend une brève définition en ce qui concerne une ressource, la manière dont la mesure est calculée et un ou plusieurs insights pour aider à comprendre son importance et son impact sur une campagne publicitaire.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribut]** | Nom de l’attribut. | Triez le tableau en cliquant sur l’en-tête de colonne de l’une des mesures clés. |
| **[!UICONTROL Category]** | La [catégorie](#categories) qui représente la qualité inhérente d’un attribut. |  |
| **[!UICONTROL d’images]** | Nombre d’images possédant cet attribut. | Le nombre indiqué dans le tableau Attributs peut être différent du nombre indiqué dans la vue Détails de l’attribut. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilise des calculs de synthèse légèrement différents. |
| **[!UICONTROL de vidéos]** | Nombre de vidéos comportant cet attribut. | Le nombre indiqué dans le tableau Attributs peut être différent du nombre indiqué dans la vue Détails de l’attribut. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilise des calculs de synthèse légèrement différents. |
| **[!UICONTROL Impressions]** | Nombre de fois qu’une image ou des vidéos avec cet attribut sont chargées dans le canal, quelle que soit l’interaction ou l’affichage. | Un nombre d’impressions élevé peut indiquer une visibilité étendue, mais pour obtenir de véritables informations sur les performances, considérez-les par rapport à d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs interagissent avec une image ou une vidéo avec cet attribut. | Un nombre élevé de clics indique un intérêt et un engagement forts envers le contenu, qui peuvent être efficaces et atteindre la bonne audience. |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions ayant généré des clics sur les images ou les vidéos avec cet attribut.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le contenu est très pertinent et motivant pour le public dans la messagerie et la conception, et qu’il cible efficacement les intérêts du public. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût pour chaque millier d’impressions publicitaires d’une image ou d’une vidéo avec cet attribut.<br>**Calcul** : montant total `spent` divisé par la portée, puis multiplié par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu’un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet d’identifier les attributs qui entraînent des actions client importantes. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic sur les images ou les vidéos avec cet attribut.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget en ce qui concerne les attributs sur une période donnée. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |
