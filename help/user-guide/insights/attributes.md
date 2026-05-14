---
title: Présentation d’Attributs
description: Découvrez comment évaluer les performances d’attributs spécifiques dans Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Content Attributes, Content Performance
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
TQID: https://experienceleague.adobe.com/FW4WpVLALtYYI2mGT3i3IH5KYuYnZ5h2pbnm9gKcrVE
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: b03d2162-d906-40a0-9cbd-001391e22d4a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5520579-b31f-4df7-9281-f0d9f91e2edc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: 4cac970f46ab08bcec2f23fd882c552af088c4ea
workflow-type: tm+mt
source-wordcount: 812
ht-degree: 0%

---

# Présentation des attributs

La vue [!DNL Insights] _[!UICONTROL Attributs]_ affiche une liste des attributs utilisés dans les campagnes publicitaires pour le compte de canal sélectionné.

{{connect-insights}}

Le tableau _[!UICONTROL Attributs]_ est organisé à l’aide du nom [!UICONTROL Attribut]. Vous pouvez basculer entre les types de liste à l’aide du bouton **[!UICONTROL Images]** et du bouton **[!UICONTROL Vidéo]**. Cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles.

![Filtre et tableau des attributs](/help/assets/insights-attributes-filter.png){zoomable="yes"}

{{filter-table}}

## Détails des attributs

Les attributs permettent d’identifier les [annonces](published-experiences.md#ad-details) et [médias](media.md#media-details) en fonction de leurs détails inhérents, tels que la couleur, la composition, les éléments visuels et d’autres propriétés.

Dans la vue des détails de l’attribut, vous pouvez voir quelles publicités utilisent l’attribut sélectionné. Les détails incluent les performances totales des attributs et une répartition des mesures de performances liées à chaque publicité.

![Mesures de performances des attributs](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing détecte certaines fonctionnalités et applique l’attribut approprié au contenu multimédia ou à la publicité sous la forme d’une balise . Voir [Catégories](#categories) pour obtenir des exemples de ces balises. Pour afficher tous les attributs associés à une publicité, cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour sélectionner la colonne **[!UICONTROL Attributs]**.

## Catégories

Un attribut _category_ est un groupe de classification qui organise les attributs associés partageant une caractéristique commune. Ces catégories permettent de rationaliser la découverte, l’identification et la compréhension d’attributs spécifiques en fournissant un plus grand contexte et en facilitant leur application et leur utilisation.

GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités de machine learning pour étudier les [images](image-features.md), [vidéos](video-features.md) et [texte](text-features.md) et appliquer des attributs aux publicités et aux médias en fonction de la probabilité d’exactitude.

La liste des attributs détectés pour les publicités et le contenu multimédia n’est pas exhaustive. Le contenu qui contient un riche ensemble de fonctionnalités peut être limité aux trois fonctionnalités les plus dominantes identifiées par l’IA. Par exemple, l’illustration suivante contient plusieurs attributs d’image détectés, y compris plusieurs objets, des couleurs de premier plan et d’arrière-plan :

![attributs d’image](/help/assets/category/asset-attributes.png "l’image de Toucan comprend plusieurs attributs détectés"){width="300" zoomable="yes"}

>[!INFO]
>
>Vous ne pouvez pas modifier les balises détectées et automatiquement appliquées.

## Performances des attributs

Les mesures d’informations peuvent vous aider à évaluer quels attributs inspirent le plus d’engagement client.

Le tableau suivant fournit des définitions et des informations sur les principales mesures de marketing numérique dans la vue de tableau [!UICONTROL Attributs]. Chaque mesure comprend une brève définition en ce qui concerne les attributs, la manière dont elle est calculée et un ou plusieurs insights pour aider à comprendre son importance et son impact sur une campagne publicitaire.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribut]** | Nom de l’attribut. | Triez le tableau en cliquant sur l’en-tête de colonne de l’une des mesures clés. |
| **[!UICONTROL Category]** | La [catégorie](#categories) qui représente la qualité inhérente d’un attribut. |  |
| **[!UICONTROL d’images]** | Nombre d’images possédant cet attribut. | Le nombre indiqué dans le tableau Attributs peut être différent du nombre indiqué dans la vue Détails de l’attribut. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilisent des calculs de synthèse légèrement différents. |
| **[!UICONTROL de vidéos]** | Nombre de vidéos comportant cet attribut. | Le nombre indiqué dans le tableau Attributs peut être différent du nombre indiqué dans la vue Détails de l’attribut. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilisent des calculs de synthèse légèrement différents. |
| **[!UICONTROL Impressions]** | Nombre de fois qu’une image ou des vidéos avec cet attribut sont chargées dans le canal, quelle que soit l’interaction ou l’affichage. | Un nombre d’impressions élevé peut indiquer une visibilité étendue, mais pour des performances réelles d’insight, considérez-le par rapport à d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs interagissent avec une image ou une vidéo avec cet attribut. | Un nombre élevé de clics indique un intérêt et un engagement forts envers le contenu, qui peuvent être efficaces et atteindre la bonne audience. |
| **[!UICONTROL Taux de clics &#x200B;]**<br>_CTR_ | Pourcentage (%) d’impressions qui ont généré des clics sur les images ou les vidéos avec cet attribut.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le contenu est très pertinent et motivant pour le public dans la messagerie et la conception, et qu’il cible efficacement les intérêts du public. |
| **&#x200B;**<br>_Coût par millier_ | Coût pour chaque millier d’impressions publicitaires d’une image ou d’une vidéo avec cet attribut.<br>**Calcul** : montant total `spent` divisé par la portée, puis multiplié par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût &#x200B;]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu&#39;un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet d’identifier les attributs qui entraînent des actions client importantes. |
| **[!UICONTROL CPC &#x200B;]**<br>_Coût par clic_ | Coût moyen associé à chaque clic sur les images ou les vidéos avec cet attribut.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget en ce qui concerne les attributs sur une période donnée. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |
