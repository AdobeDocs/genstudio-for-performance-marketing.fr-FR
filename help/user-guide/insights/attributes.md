---
title: Présentation des attributs
description: Découvrez comment évaluer les performances d’attributs spécifiques dans Adobe GenStudio for Performance Marketing.
feature: Insights, Attributes
exl-id: 9d05c128-50d5-415a-ae60-7023c36c06ad
source-git-commit: d6ea1a34a8679ae958fb184e40ad0673abbab0a4
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Présentation des attributs

La vue [!DNL Insights] _[!UICONTROL Attributs]_ affiche une liste des attributs utilisés dans les campagnes publicitaires pour le compte de canal sélectionné.

La table _[!UICONTROL Attributes]_ est organisée à l’aide du nom [!UICONTROL Attribute]. Vous pouvez basculer entre les types de liste à l’aide du bouton **[!UICONTROL Images]** et du bouton **[!UICONTROL Vidéo]** . Cliquez sur l’icône de paramètres (engrenage) située au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles.

L’icône de filtre (entonnoir) au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtre]** où vous pouvez sélectionner les attributs dans le tableau [!UICONTROL Compte] et [!UICONTROL Catégorie d’attributs] pour filtrer les attributs. L’exemple suivant montre une liste d’attributs dans la catégorie `Lighting Condition`.

![Filtre Attributs et table](/help/assets/insights-attributes-filter.png){zoomable="yes"}

## Détails des attributs

Les attributs permettent d’identifier les ressources en fonction de leurs détails inhérents, tels que la couleur, la composition, les éléments visuels et d’autres propriétés.

Dans la vue des détails de l’attribut, vous pouvez voir les expériences qui utilisent l’attribut sélectionné. Les détails incluent les performances totales des attributs et une ventilation des mesures de performances liées à chaque expérience.

![Mesures de performances des attributs](/help/assets/insights-attribute-details.png){zoomable="yes"}

GenStudio for Performance Marketing détecte certaines fonctionnalités et applique l’attribut approprié à une ressource ou à une expérience sous la forme d’une balise . Voir [Catégories](#categories) pour consulter des exemples de ces balises. Pour afficher tous les attributs associés à une expérience, cliquez sur l’icône de paramètres (engrenage) située au-dessus du côté droit du tableau pour sélectionner la colonne **[!UICONTROL Attributs]**.

## Catégories

GenStudio for Performance Marketing reconnaît certaines fonctionnalités d’images, de vidéos et de texte et applique une balise de fonction à la ressource. Une _catégorie_ est un ensemble de fonctionnalités qui partagent une caractéristique spécifique. Par exemple, la catégorie _orientation d’image_ a une valeur `landscape`, `portrait` ou `square`.

Vous ne pouvez pas modifier les balises détectées et appliquées automatiquement.

Voir [Catégories d’attributs](/help/user-guide/insights/attribute-category.md) pour obtenir des listes détaillées des fonctionnalités d’image, de vidéo et de texte.

## Performances des attributs

Les mesures de statistiques peuvent vous aider à évaluer les attributs qui inspirent le plus d’engagement des clients.

Le tableau suivant fournit des définitions et des informations sur les mesures de marketing numérique clés dans la vue de tableau [!UICONTROL Attributs]. Chaque mesure comprend une brève définition en ce qui concerne une ressource, le mode de calcul de la mesure et une ou plusieurs informations permettant de comprendre son importance et son impact sur une campagne publicitaire.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Attribut]** | Nom de l’attribut. | Triez le tableau en cliquant sur l’en-tête de colonne de l’une des mesures clés. |
| **[!UICONTROL Category]** | [category](#categories) qui représente la qualité inhérente d’un attribut. |  |
| **[!UICONTROL # des images]** | Nombre d’images avec cet attribut. |  |
| **[!UICONTROL # de vidéos]** | Nombre de vidéos avec cet attribut. |  |
| **[!UICONTROL Impressions]** | Comptage de chaque chargement d’une image ou de vidéos avec cet attribut dans le canal, indépendamment de l’interaction ou de l’affichage. | Un nombre d’impressions élevé peut indiquer une large visibilité, mais pour obtenir de vraies informations sur les performances, prenez en compte d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs interagissent avec une image ou une vidéo avec cet attribut. | Un nombre de clics élevé indique un fort intérêt et un engagement envers le contenu, ce qui peut être efficace et atteindre la bonne audience. |
| **[!UICONTROL CTR ]**<br>_Taux de clics_ | Pourcentage (%) d&#39;impressions ayant généré des clics sur les images ou les vidéos avec cet attribut.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clics élevé indique que le contenu est très pertinent et motivant pour le public dans la messagerie et la conception, et cible effectivement les intérêts du public. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût pour chaque millier d’impressions publicitaires d’une image ou d’une vidéo avec cet attribut.<br>**Calcul** : somme `spent` divisée par portée, puis multipliée par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clics élevé. |
| **[!UICONTROL CPA ]**<br>_Coût par action_ | Coût moyen dépensé pour réaliser une action client spécifique, comme un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d’actions client terminées | Permet d’identifier les attributs qui génèrent des actions précieuses de la part des clients. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic sur les images ou les vidéos avec cet attribut.<br>**Calcul** : montant total `spent` divisé par `clicks` | Des coûts moyens inférieurs peuvent indiquer des dépenses publicitaires rentables, en particulier par rapport à une augmentation des conversions. |
| **[!UICONTROL Dépenser]** | Montant dépensé dans le budget en ce qui concerne les attributs sur une période donnée. | Un montant élevé de dépenses sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à une diminution rapide des ressources. Effectuez le suivi du montant des dépenses par rapport aux mesures de performances clés pour mieux surveiller le retour sur investissement global. |
