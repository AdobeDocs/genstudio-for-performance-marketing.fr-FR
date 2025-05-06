---
title: Filtrer les vues d’informations
description: Découvrez comment utiliser les fonctionnalités de filtre améliorées avec Insights.
level: Intermediate
feature: Reporting and Insights
source-git-commit: 656395e517fcb334b64865dcdbde09d8d982dc0a
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# Filtrer les vues Insights

Le tableau de bord [!DNL Insights] fournit un ensemble complet de filtres pour une expérience d’exploration des données efficace. Lors de l’analyse des canaux, des publicités, des médias ou d’attributs spécifiques, les options de filtrage vous permettent de personnaliser votre vue et de rationaliser votre workflow. Utilisez des filtres par mot-clé pour un ciblage précis ou explorez des listes prédéfinies afin d’affiner votre recherche et de vous concentrer sur les données les plus importantes.

## Principes de base des filtres

Chaque vue d’[!DNL Insights] propose une liste d’options de filtre. L’icône de filtre (entonnoir) située au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtrer]**. Que vous visionniez le tableau ou la galerie, les filtres appliqués apparaissent dans la liste **[!UICONTROL Filtrer par]** au-dessus du tableau ou de la galerie. Par défaut, un canal et un compte sont sélectionnés.

![Filtrer par](/help/assets/insights-filter-by.png "Filtrer par"){width=600 zoomable="yes"}

Les filtres appliqués persistent dans toutes les vues. Sélectionnez **[!UICONTROL Effacer tout]** au-dessus du tableau ou de la galerie pour supprimer tous les filtres sélectionnés.

### Champ de recherche

Cliquez sur l’icône de recherche (loupe) pour utiliser un terme de recherche afin de localiser des éléments spécifiques dans le tableau ou la galerie. Par exemple, la saisie du terme `pink` dans le tableau [!UICONTROL Publicités] filtre les résultats pour afficher uniquement les publicités utilisant le terme `pink` dans le nom.

![Exemple de champ de recherche](/help/assets/insights-search.png "Rechercher des annonces avec du rose"){width=600 zoomable="yes"}

### Période

Le sélecteur de période est un outil puissant pour aligner les données affichées avec vos objectifs d’analyse. Utilisez le sélecteur de période pour ajuster la période des données affichées dans la vue Tableau ou Galerie. Par défaut, la période est définie sur les 30 derniers jours. Pour inclure plus de données ou se concentrer sur une période spécifique, développez la période.

![Sélecteur de période](/help/assets/insights-date-range.png "Sélectionnez une période"){width=400}

Si aucun élément n’apparaît en mode Tableau ou Galerie, cela peut être dû à la période sélectionnée, à l’exclusion des données pertinentes. Dans ce cas, augmentez la période pour vous assurer que les données souhaitées sont incluses.

### Pages

Certains tableaux peuvent s’étendre sur plusieurs pages, comme indiqué sous le tableau sur le côté droit. Utilisez les options de recherche et de filtrage polyvalentes pour affiner vos résultats. Pour naviguer entre les pages, utilisez les commandes de pagination droite (en avant) et gauche (en arrière). Veillez à appliquer correctement les filtres afin d’inclure toutes les données pertinentes sur les différentes pages.

### Contrôle des diapositives

Certaines options de filtre incluent un contrôle de diapositive, qui vous permet de sélectionner une valeur dans une plage définie. Par exemple, dans _[!UICONTROL Attributs]_, le curseur **[!UICONTROL Nombre de médias]** permet de filtrer les attributs en fonction du nombre d’images ou de vidéos associées. Faites glisser le curseur pour spécifier une plage, en commençant par un minimum de 0 jusqu’à un maximum pouvant dépasser 100.

## Filtrage avancé

Avec les filtres _[!UICONTROL Campagnes]_ et _[!UICONTROL Publicités]_, vous pouvez utiliser des mots-clés précis pour affiner la liste. Les filtres par mots-clés sont particulièrement utiles pour filtrer les campagnes ou les annonces publicitaires qui utilisent une convention de nommage complexe avec plusieurs identifiants uniques. Par exemple, un nom de campagne peut inclure les éléments suivants :

- Nom ou code de région spécifique : `NA`, `EMEA`
- Acronymes des types de contenu : `EB`, `CHT` ou `DSP`
- Codes ou acronymes des offres : `OFFER2023`, `PROMO`

Au fil du temps, la liste des campagnes et des publicités s&#39;allonge de façon exponentielle. Envisagez le scénario suivant pour utiliser le filtre _[!UICONTROL Campagnes]_ afin d’affiner le tableau [!UICONTROL Publicités].

**Pour affiner le tableau Publicités à l’aide du filtre Campagnes** :

1. Dans _[!DNL Insights]_, sélectionnez la vue **[!UICONTROL Publicités]**.

   ![Filtre de publicités et vue tableau](/help/assets/insights-ads-filter.png "Publicités avec liste de filtres"){zoomable="yes"}

1. Cliquez sur l’icône de filtre (entonnoir) au-dessus du côté gauche du tableau pour ouvrir le menu **[!UICONTROL Filtre]**.

1. Vérifiez que le canal et le compte `Filter by` appropriés sont sélectionnés.

1. Développez le filtre **[!UICONTROL Campagnes]**, puis cliquez sur **[!UICONTROL Sélectionner]**.

   ![Filtrer les campagnes](/help/assets/insights-filter-campaigns-expand.png "Développer le filtre des campagnes"){width=200}

1. Dans le champ de recherche _[!UICONTROL Sélectionner des campagnes]_ , saisissez des mots-clés séparés par des virgules.

   - Utilisez autant de mots-clés que nécessaire pour affiner la liste. L’exemple suivant recherche des campagnes dont le nom contient `evergreen`, `ROI` et `Meta` :

     ![Recherche par mot-clé](/help/assets/insights-select-campaigns-keywords.png "saisissez des mots-clés pour rechercher les noms de campagne"){width=500}

   - Vous pouvez ajouter un autre ensemble de mots-clés pour élargir votre recherche. L’utilisation de plusieurs ensembles de mots-clés vous permet d’inclure des campagnes qui correspondent au premier ensemble de mots-clés ou au second. Par exemple, vous pouvez rechercher des campagnes intitulées `evergreen` et `web` des campagnes _OU_ intitulées `photoshop` et `roi` :

     ![Rechercher avec plusieurs ensembles de mots-clés](/help/assets/insights-advanced-or.png "Rechercher des noms de campagne à l’aide de plusieurs ensembles de mots-clés"){width=500}

1. Sélectionnez une ou plusieurs campagnes à partir de la recherche résultante et cliquez sur **[!UICONTROL Appliquer]**.

   ![Liste des campagnes](/help/assets/insights-select-campaigns-list.png "Sélectionner les campagnes à inclure")

Les campagnes sélectionnées apparaissent désormais dans la liste _[!UICONTROL Filtrer par]_ au-dessus du tableau ou de la galerie des publicités. Vous pouvez vous concentrer exclusivement sur les annonces liées aux campagnes sélectionnées. Dans cet exemple, les résultats filtrés comprennent 28 annonces, fournissant une vue plus ciblée pour l’analyse.

![Table filtrée par campagnes](/help/assets/insights-filter-by-campaigns.png "Table avec filtre campagnes"){zoomable="yes"}

Vous pouvez filtrer davantage le tableau [!UICONTROL Média] de la même manière pour les noms d’annonces. Développez le filtre **[!UICONTROL Publicités]** et cliquez sur **[!UICONTROL Sélectionner]**. Vous pouvez ensuite exécuter un filtre par mot-clé similaire pour affiner le tableau des médias ou la vue de la galerie.

## Télécharger les résultats du tableau

Vous pouvez télécharger les résultats filtrés à partir de la vue Tableau pour les analyser ou les partager plus en détail. Cliquez sur l’icône de téléchargement (flèche pointant vers le bas) au-dessus du côté droit du tableau pour télécharger un fichier CSV en fonction du tableau visible. Le téléchargement démarre automatiquement et place le fichier CSV à l’emplacement de téléchargement par défaut.

Certains tableaux peuvent comporter plusieurs pages, que vous pouvez voir sous le côté droit du tableau. Le fichier CSV inclut des données provenant de _toutes_ les pages du tableau.
