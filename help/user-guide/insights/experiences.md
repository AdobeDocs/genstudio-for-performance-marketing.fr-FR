---
title: Présentation des expériences
description: Consultez un aperçu de l’engagement des clients, du budget et des dépenses pour les expériences et les performances des emplacements publicitaires dans Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences, Attributes
exl-id: e3827b1a-53d0-465c-8125-15b0e298ef3a
source-git-commit: 4284026bf14d58eecb547d80b4bdae6ac0422078
workflow-type: tm+mt
source-wordcount: '1265'
ht-degree: 0%

---

# Présentation des expériences

La vue [!DNL Insights] _[!UICONTROL Expériences]_ affiche une liste d’expériences pour le compte publicitaire du canal connecté. Pour Facebook, les expériences sont des Meta et des noms.

{{connect-insights}}

Le tableau _[!UICONTROL Expériences]_ est organisé à l’aide de [!UICONTROL noms d’annonces]. Cliquez sur l’icône des paramètres (cog) au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles. L’icône de filtre (entonnoir) située au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtre]** dans lequel vous pouvez effectuer une sélection parmi les listes [!UICONTROL Compte] et [!UICONTROL Campagne] pour filtrer les noms des annonces dans le tableau. Cliquez sur **Réinitialiser** pour effacer toutes les sélections de filtres.

![ Filtre et tableau des expériences ](/help/assets/insights-experiences-filter.png){zoomable="yes"}

{{$include /help/_includes/download-insights.md}}

## Détails de l’expérience

Une _expérience_ est une ressource promotionnelle qui comprend du contenu visuel et interactif destiné à être distribué à une audience spécifique dans le cadre d’une campagne marketing.

Sélectionnez une expérience et affichez les mesures de performances, les attributs de texte et les emplacements associés à chaque publicité. Dans la vue des détails, vous pouvez analyser les mesures d’une expérience en fonction de son positionnement publicitaire et de ses efforts marketing au cours d’une période spécifiée.

La vue des détails inclut des mesures générales sur les `click-through rate`, les `cost per action` et les `spend` de la publicité, à savoir la part du budget consacrée à la publicité. Comme les publicités peuvent avoir plusieurs emplacements, tels qu’un flux ou une bannière, vous pouvez voir une répartition des mêmes mesures pour chaque emplacement publicitaire. Utilisez les flèches gauche et droite sous **[!UICONTROL Performances par emplacement publicitaire]** pour parcourir les mesures d’emplacement.

![Détails de l’annonce avec des mesures et des emplacements publicitaires](/help/assets/insights-experience-details.png){zoomable="yes"}

### Attributs de texte

Sous l’aperçu de l’expérience se trouve une liste d’attributs [!UICONTROL texte] associés à la publicité. Lorsque les ressources et les expériences sont approuvées et stockées dans [!DNL Content], GenStudio for Performance Marketing génère des balises en fonction de leurs fonctionnalités inhérentes. Voir [Détails de la ressource](/help/user-guide/content/asset-details.md#system-metadata) pour plus d’informations sur les métadonnées système.

### Ajouter des emplacements

Au moment où vous avez créé une campagne avec des méta-annonces, vous avez peut-être sélectionné où exécuter vos annonces en fonction de l’[objectif](channels.md#objectives) de la campagne. Les emplacements publicitaires élargissent la portée de l’audience de votre publicité.

GenStudio for Performance Marketing prend en charge les formats d’annonce, tels que les flux de ressources, les annonces de liens et les images ou vidéos uniques. Voici une liste des formats d’annonce publicitaire par plateforme :

| Instagram | Facebook/Meta | Messager | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Explore<br>Explore home<br>Explore grid Home<br>Feed<br>Reels<br>Profile feed<br>Search<br>Shop<br>Stories | Business Explorer<br>Feed<br>In-stream video<br>Marketplace<br>Reels<br>Reels overlay<br>Right column<br>Search results<br>Stories<br>Video feeds<br>Ads on Facebook reels | Boîte<br>Réception | Vidéo native, de bannière et <br> récompensée |

#### Emplacements non pris en charge

GenStudio for Performance Marketing ne prend pas en charge les emplacements publicitaires suivants :

- Collaboratif
- Catalogue/Avantage+ catalogue
- Expérience de l’instance
- Carrousel

## Performances de l’expérience

Les mesures d’informations peuvent vous aider à évaluer les expériences qui contribuent au succès d’une campagne et les emplacements publicitaires les plus efficaces.

Le tableau suivant fournit des définitions et des informations sur les principales mesures de marketing numérique dans la vue de tableau [!UICONTROL Expériences]. Chaque mesure comprend une brève définition en ce qui concerne les noms d’annonces, la manière dont la mesure est calculée et un ou plusieurs informations pour aider à comprendre son importance et son impact sur une expérience.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nom de l’expérience]** | Liste des expériences pour le compte de canal connecté. Filtrez les publicités en sélectionnant une campagne. | Triez la liste des expériences en cliquant sur l’une des mesures clés. |
| **[!UICONTROL Campagne]** | Une campagne est un ensemble d’expériences conçues pour atteindre un objectif spécifique. | Lorsque vous filtrez le tableau Expériences par campagne, les mesures de synthèse de toutes les expériences de la campagne peuvent être différentes de la ligne de synthèse de la campagne dans la vue [!UICONTROL Canaux]. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilise des calculs de synthèse légèrement différents. |
| **[!UICONTROL Emplacements]** | Nombre d’annonces [emplacements](#ad-placements), emplacements où une expérience est apparue dans la campagne. | Les emplacements augmentent la portée de l’audience.<p>Les annonces publicitaires qui n’affichent aucun emplacement et aucune ressource peuvent indiquer un [type d’annonce non pris en charge](#unsupported-placements).</p> |
| **[!UICONTROL Assets]** | Nombre de ressources utilisées dans la publicité ou l’expérience. | Le nombre dans le tableau Expériences peut être différent du nombre dans la vue Détails de l’expérience. Cette incohérence peut se produire si la source du canal, telle que Meta et GenStudio, utilise des calculs de synthèse légèrement différents. |
| **[!UICONTROL Impressions]** | Décompte de chaque chargement de l’emplacement ou de l’expérience publicitaire dans le canal, quelle que soit l’interaction ou l’affichage. | Un nombre d’impressions élevé peut indiquer une visibilité étendue, mais pour obtenir de véritables informations sur les performances, considérez-les par rapport à d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs et utilisatrices interagissent avec un élément cliquable, tel qu’un lien ou un bouton d’appel à l’action, dans un emplacement d’expérience. | Un nombre élevé de clics indique un intérêt et un engagement forts envers le contenu, qui peuvent être efficaces et atteindre la bonne audience. |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions ayant généré des clics sur l’emplacement d’expérience dans une campagne.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clic publicitaire élevé indique que le contenu est très pertinent et motivant pour le public dans la messagerie et la conception, et qu’il cible efficacement les intérêts du public. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût pour mille impressions publicitaires pour l’emplacement de l’expérience.<br>**Calcul** : montant total `spent` divisé par la portée, puis multiplié par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clic publicitaire élevé. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour réaliser une action spécifique du client, telle qu’un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées | Permet de surveiller les dépenses liées aux expériences qui entraînent des actions client importantes. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic dans un emplacement d’expérience.<br>**Calcul** : montant total `spent` divisé par `clicks` | Une baisse des coûts moyens peut indiquer un bon rapport coût/efficacité des dépenses publicitaires, surtout si on les compare à une augmentation des conversions. |
| **[!UICONTROL Dépenses]** | Montant dépensé à partir du budget de la campagne sur une période donnée pour placer cette expérience publicitaire. | Un montant de dépenses élevé sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à un épuisement précoce des ressources. Effectuez le suivi des montants dépensés par rapport aux mesures de rendement clés pour vous aider à surveiller le rendement global du capital investi. |

## Performances de l’emplacement

Dans la vue _Détails de l’expérience_, les trois principales mesures reflètent les performances globales de l’expérience sélectionnée. Toutefois, la section _Performances par emplacement_ affiche les mesures détaillées de chaque emplacement publicitaire. Utilisez les flèches droite et gauche pour naviguer parmi les différents emplacements publicitaires.

Le tableau suivant fournit des définitions pour les mesures de performances des emplacements publicitaires :

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | ----------- |
| **[!UICONTROL Taux de clics ]**<br>_CTR_ | Pourcentage (%) d’impressions pour un emplacement publicitaire unique qui a généré des clics.<p>**Calcul**:`clicks` divisé par `impressions`<p>Cette mesure permet de déterminer l’efficacité de l’emplacement publicitaire pour séduire l’audience. | Un taux de clics élevé indique que le positionnement de l’annonce publicitaire est pertinent et attrayant pour l’audience, ce qui entraîne davantage d’interactions. |
| **[!UICONTROL Coût ]**<br>_CPA par action_ | Coût moyen dépensé pour un emplacement publicitaire unique afin d’atteindre l’action souhaitée par le client ou la cliente, comme un achat ou un abonnement.<p>**Calcul** : montant total `spent` divisé par le nombre d&#39;actions du client effectuées<p>Cette mesure permet d’évaluer le rapport coût-efficacité de l’emplacement publicitaire dans la génération d’actions pertinentes. | Une CPA plus faible suggère que le placement publicitaire est efficace pour convertir les interactions d’audience en actions souhaitées à moindre coût. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen associé à chaque clic dans un seul emplacement publicitaire.<p>**Calcul** : montant total `spent` divisé par `clicks`<p>Cette mesure permet d’évaluer le rapport coût-efficacité de l’emplacement publicitaire pour la génération de clics. | Un CPC inférieur indique que l’emplacement publicitaire génère des clics à un coût inférieur, ce qui peut être bénéfique pour maximiser le retour sur investissement. |
| **[!UICONTROL Dépenses]** | Montant dépensé pour un emplacement publicitaire unique, représentant une fraction du montant total dépensé pour l’ensemble de l’expérience. Cette mesure permet de suivre l’efficacité de l’affectation budgétaire et des dépenses pour chaque emplacement publicitaire. | Le suivi des dépenses peut permettre de s’assurer que les ressources sont utilisées efficacement à différents emplacements. |
