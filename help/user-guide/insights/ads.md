---
title: Publicités et emplacement publicitaire - Aperçu
description: Consultez un aperçu de l’engagement des clients, du budget et des dépenses pour les publicités et les performances de placement publicitaire dans Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Ad Performance, Text Attributes, Reporting and Insights
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# Publicités et emplacement publicitaire - Aperçu

La vue [!DNL Insights] _[!UICONTROL Publicités]_ affiche une liste des publicités pour le compte publicitaire du canal connecté. Une _publicité_ est une ressource promotionnelle qui comprend du contenu visuel et interactif destiné à être distribué à une audience spécifique dans le cadre d’une campagne marketing.

{{connect-insights}}

Le tableau _[!UICONTROL Annonces]_ est organisé à l’aide des [!UICONTROL noms d’annonces]. Cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles.

![Filtre et tableau des publicités](/help/assets/insights-ads-filter.png){zoomable="yes"}

La vue galerie _[!UICONTROL Annonce]_ affiche un collage d’aperçus d’annonce publicitaire et d’une mesure, telle que le taux de clic publicitaire. Cliquez sur l’icône des paramètres (cog) située au-dessus du côté droit de la galerie pour ouvrir **[!UICONTROL Paramètres de la carte]** et activer l’une des trois mesures visibles :

- Coût par action (CPA)
- Taux de clic publicitaire (CTR)
- CPC (coût par clic)
- Dépenses

{{filter-table}}

## Détails de l’annonce

Sélectionnez une publicité et affichez les mesures de performances, les attributs de texte et les emplacements associés à chaque publicité. La _[!UICONTROL page Détails de l’annonce publicitaire]_ comprend des mesures relatives à l’`click-through rate`, à la `cost per action` et à l’`spend` de l’annonce : pourcentage du budget consacré à l’annonce publicitaire. Comme les publicités peuvent avoir plusieurs emplacements, tels qu’un flux ou une bannière, vous pouvez voir une répartition des mêmes mesures pour chaque emplacement publicitaire. Utilisez les flèches gauche et droite sous **[!UICONTROL Performances par emplacement publicitaire]** pour parcourir les mesures d’emplacement.

![Détails de l’annonce avec des mesures et des emplacements publicitaires](/help/assets/insights-ad-details.png){zoomable="yes"}

### Ajouter des attributs

Sous l’aperçu de l’annonce publicitaire se trouve une liste des attributs associés à l’annonce publicitaire.

{{$include /help/_includes/generated-attributes.md}}

### Formats publicitaires

Les formats d’annonces font référence aux différents éléments créatifs et mises en page utilisés pour s’aligner sur les objectifs de votre campagne, faire participer votre audience cible et suivre les mesures de performances.

[!DNL Insights] dans GenStudio for Performance Marketing prend actuellement en charge les formats d’annonce suivants.

| Pris en charge | Non pris en charge |
|----------------------------------|-----------------------------------|
| Dynamic Ads<br>Link Ads<br>Simple Image Ads<br>Simple Video Ads | Boutique Publicités<br>Avantage+ Shopping Publicités<br>Avantage+ Catalogue Publicités<br>Carrousel Publicités<br>Messagerie Publicités<br>Lead Publicités<br>Collection Publicités<br>Appels Publicités<br>Postes de page détenus Publicités<br>Partenariats Publicités<br>Flexibilité Publicités |

### Ajouter des emplacements

Les emplacements publicitaires font référence aux emplacements ou plateformes spécifiques où vos annonces apparaissent dans une campagne. Ces emplacements déterminent comment et où votre audience interagit avec votre contenu. Les emplacements publicitaires élargissent la portée de l’audience, ce qui permet d’optimiser la visibilité, l’engagement et l’efficacité globale de la campagne.

Lorsque vous créez une campagne avec des annonces Meta, vous avez peut-être sélectionné l’emplacement où exécuter vos annonces en fonction de l’objectif [de la campagne](channels.md#objectives).

Voici une liste des emplacements publicitaires pris en charge :

| Audience Network | Facebook/Meta \* | Instagram | Messager |
|--------------------|--------------------|-------------------------|---------------------|
| Vidéo récompensée | Flux<br>flux vidéo<br>Histoires<br>Marketplace<br>Colonne de droite<br>Bobines<br>Superposition de bobines<br>Vidéo en flux continu<br>Recherche<br>Flux de disco d’entreprise<br>Flux de profil | Stories<br>Feed<br>Explore<br>Reels<br>Explore grid Home<br>Profile feed<br>Search<br>Stream | Stories<br>Inbox |

\* Voir [À propos des emplacements publicitaires dans les technologies Meta](https://www.facebook.com/business/help/407108559393196?id=369787570424415) dans le _Centre d’aide aux entreprises de Meta_.

## Performances des publicités

Les mesures d’informations peuvent vous aider à évaluer quelles annonces contribuent au succès d’une campagne et quels emplacements publicitaires sont les plus efficaces.

Le tableau suivant fournit des définitions et des informations sur les principales mesures de marketing numérique dans la vue du tableau [!UICONTROL Publicités]. Chaque mesure comprend une brève définition en ce qui concerne les noms des publicités, la manière dont la mesure est calculée et un ou plusieurs informations pour aider à comprendre sa signification et son impact sur une publicité.

| Mesure | Définition | Insight |
| ---------------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nom de l’annonce]** | Liste des publicités pour le compte du canal connecté. Filtrez les publicités en sélectionnant une campagne. | Triez la liste des publicités en cliquant sur l’une des mesures clés. |
| **[!UICONTROL Campagne]** | Une campagne est un ensemble d’annonces publicitaires conçu pour atteindre un objectif spécifique. | Lorsque vous filtrez le tableau Publicités par campagne, les mesures de synthèse de toutes les publicités de la campagne peuvent être différentes de la ligne de synthèse de la campagne dans la vue [!UICONTROL Canaux]. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilisent des calculs de synthèse légèrement différents. |
| **[!UICONTROL Emplacements]** | Nombre d’annonces [emplacements](#ad-placements), c’est-à-dire les emplacements où une annonce publicitaire est apparue dans la campagne. | Les emplacements augmentent la portée de l’audience.<p>Les annonces publicitaires qui n’affichent aucun emplacement et aucun média peuvent indiquer un [type d’annonce non pris en charge](#unsupported-placements).</p> |
| **[!UICONTROL Média]** | Nombre de ressources utilisées dans la publicité et les emplacements publicitaires | Le nombre indiqué dans le tableau Publicités peut être différent du nombre indiqué dans la vue Détails de la publicité. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilisent des calculs de synthèse légèrement différents. |
| **[!UICONTROL Impressions]** | Décompte de chaque chargement de l’emplacement ou de l’annonce publicitaire dans le canal, quelle que soit l’interaction ou l’affichage. | Un nombre d’impressions élevé peut indiquer une visibilité étendue, mais pour des performances réelles d’insight, considérez-le par rapport à d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs et utilisatrices interagissent avec un élément cliquable, tel qu’un lien ou un bouton call-to-action, dans un emplacement publicitaire. | Un nombre élevé de clics indique un intérêt et un engagement forts envers le contenu, qui peuvent être efficaces et atteindre la bonne audience. |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions ayant généré des clics sur l’annonce publicitaire dans une campagne.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le contenu est très pertinent et motivant pour le public dans la messagerie et la conception, et qu’il cible efficacement les intérêts du public. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût moyen pour mille impressions de publicité.<br>**Calcul** : montant total `spent` divisé par la portée, puis multiplié par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu’un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet de surveiller les dépenses publicitaires qui entraînent des actions client importantes. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic dans un emplacement publicitaire.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget de Campaign sur une période donnée pour placer cette annonce publicitaire. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |
| **Attributs** | Liste des fonctionnalités inhérentes présentes dans cette publicité. | Les attributs permettent d’identifier les éléments créatifs qui interagissent le plus avec votre audience. Voir [Catégories](/help/user-guide/insights/attributes.md#categories). |

## Performances de l’emplacement

Dans la vue _[!UICONTROL Page de détails de l’annonce publicitaire]_, les trois mesures principales reflètent les performances globales de l’annonce publicitaire sélectionnée. Toutefois, la section _Performances par emplacement_ affiche les mesures détaillées de chaque emplacement publicitaire. Utilisez les flèches droite et gauche pour naviguer parmi les différents emplacements publicitaires.

Le tableau suivant fournit des définitions pour les mesures de performances des emplacements publicitaires :

| Mesure | Définition | Insight |
| ---------------------------- | ----------------------------- | --------------------------------- |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions pour un emplacement publicitaire unique qui a généré des clics.<p>**Calcul**:`clicks` divisé par `impressions`<p>Cette mesure permet de déterminer l’efficacité de l’emplacement publicitaire pour séduire l’audience. | Un taux de clics élevé indique que le positionnement de l’annonce publicitaire est pertinent et attrayant pour l’audience, ce qui entraîne davantage d’interactions. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour un emplacement publicitaire unique afin d’atteindre l’action souhaitée par le client ou la cliente, comme un achat ou un abonnement.<p>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées<p>Cette mesure permet d’évaluer le rapport coût-efficacité de l’emplacement publicitaire dans la génération d’actions pertinentes. | Une CPA plus faible suggère que le placement publicitaire est efficace pour convertir les interactions d’audience en actions souhaitées à moindre coût. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic dans un seul emplacement publicitaire.<p>**Calcul** : montant total `spent` divisé par `clicks`<p>Cette mesure permet d’évaluer le rapport coût-efficacité de l’emplacement publicitaire pour la génération de clics. | Un CPC inférieur indique que l’emplacement publicitaire génère des clics à un coût inférieur, ce qui peut être bénéfique pour maximiser le retour sur investissement. |
| **[!UICONTROL Dépenses]** | Montant dépensé pour un emplacement publicitaire unique, représentant une fraction du montant total dépensé pour l’ensemble de l’annonce. Cette mesure permet de suivre l’efficacité de l’affectation budgétaire et des dépenses pour chaque emplacement publicitaire. | Le suivi des dépenses peut permettre de s’assurer que les ressources sont utilisées efficacement à différents emplacements. |
| **Attributs** | Liste des fonctionnalités inhérentes présentes dans cet emplacement publicitaire. | Les attributs permettent d’identifier les éléments créatifs qui interagissent le plus avec votre audience. Voir [Catégories](/help/user-guide/insights/attributes.md#categories). |
