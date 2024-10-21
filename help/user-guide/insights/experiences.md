---
title: Présentation des expériences
description: Consultez un aperçu de l’engagement des clients, du budget et des dépenses pour les expériences et les performances d’emplacement publicitaire dans Adobe GenStudio for Performance Marketing.
feature: Insights, Experiences
source-git-commit: 87a8833549569aaeaa60f5760b4e9a8b710a6033
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 0%

---

# Présentation des expériences

La vue [!DNL Insights] _[!UICONTROL Expériences]_ affiche une liste des expériences pour le canal et le compte connectés. Pour Facebook, les expériences sont des noms de publicité de métadonnées.

La table _[!UICONTROL Expériences]_ est organisée à l’aide de [!UICONTROL Noms d’annonces]. Cliquez sur l’icône de paramètres (engrenage) située au-dessus du côté droit du tableau pour activer/désactiver les colonnes visibles. L’icône de filtre (entonnoir) au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtre]** où vous pouvez sélectionner les listes [!UICONTROL Compte] et [!UICONTROL Campagne] pour filtrer les noms des publicités dans le tableau.

![Filtre d’expériences et table](/help/assets/insights-experiences-filter.png){zoomable="yes"}

## Détails de l’expérience

Une _expérience_ est une ressource promotionnelle qui comprend du contenu visuel et interactif destiné à être distribué à une audience spécifique dans le cadre d’une campagne marketing.

Sélectionnez une expérience (nom de la publicité) et affichez les mesures de performances, les attributs de texte et les emplacements associés à chaque publicité. Dans la vue Détails, vous pouvez analyser les mesures d’une expérience en fonction de son emplacement publicitaire et de ses efforts marketing au cours d’une période spécifiée.

La vue Détails inclut des mesures globales `click-through rate`, `cost per action` et `spend`, c’est-à-dire la part du budget qui a été consacrée à la publicité. Comme les publicités peuvent comporter plusieurs emplacements, tels qu’un flux ou une bannière, vous pouvez consulter une ventilation des mêmes mesures pour chaque emplacement d’annonce. Utilisez les flèches gauche et droite sous **[!UICONTROL Performance by ad ad placement]** pour passer en revue les mesures d’emplacement.

![Détails de la publicité avec des mesures et des emplacements de publicité](/help/assets/insights-experience-details.png){zoomable="yes"}

### Attributs de texte

Sous l’aperçu de l’expérience se trouve une liste d’ [!UICONTROL attributs de texte] associés à la publicité. Lorsque les ressources et les expériences sont approuvées et stockées dans [!DNL Content], GenStudio for Performance Marketing génère des balises en fonction de leurs fonctionnalités inhérentes. Pour plus d’informations sur les métadonnées du système, voir [Détails de la ressource](../content/asset-details.md#system-metadata) .

### Emplacements de publicité

Au moment de la création d’une campagne avec des métadonnées publicitaires, vous avez peut-être sélectionné l’emplacement où exécuter vos publicités en fonction de l’ [objectif](channels.md#objectives) de la campagne. Les emplacements de publicité élargissent la portée du public pour votre publicité.

GenStudio for Performance Marketing prend en charge les formats d’annonces, tels que les flux de ressources, les annonces de liens et les images ou vidéos uniques. Voici une liste des formats d’annonce par plateforme :

| Instagram | Facebook/Meta | Messenger | Audience Network |
| ------------ | ---------------- | ------------ | ---------------- |
| Explore<br>Explorer La Page D’Accueil<br>Explorer La Grille À L’Accueil<br>Flux<br>Reels<br>Flux De Profil<br>Rechercher<br>Shop<br>Articles | Exploration de l’entreprise <br>Flux<br>Vidéo en flux continu<br>Marketplace<br>Reels<br>Superposition de sous-marins<br>Colonne de droite<br>Résultats de la recherche<br>Articles<br>Flux vidéo<br>Publicités sur des sous-marins Facebook | Inbox<br>Stories | Natif, bannière et spot<br>Vidéo récompensée |

## Mesures des expériences

Les mesures de statistiques peuvent vous aider à évaluer quelles expériences contribuent au succès d’une campagne et quels emplacements publicitaires sont les plus efficaces.

<!-- For example, -->

### Détails des mesures

Le tableau suivant fournit des définitions et des informations sur les mesures de marketing numérique clés dans la vue de tableau [!UICONTROL Expériences]. Chaque mesure comprend une brève définition en ce qui concerne les noms des publicités, la manière dont la mesure est calculée et une ou plusieurs informations pour mieux comprendre son importance et son impact sur une expérience.

| Mesure | Définition | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Nom de l’expérience]** | Liste d’expériences pour le compte de canal connecté. Filtrez les publicités en sélectionnant une campagne. | Triez la liste des expériences en cliquant sur l’une des mesures clés. |
| **[!UICONTROL Campaign]** | Une campagne est un ensemble d’expériences conçues pour atteindre un objectif spécifique. | |
| **[!UICONTROL Emplacements]** | Nombre d’emplacements [de publicité](#ad-placements), emplacements où une expérience s’est affichée dans la campagne. | Les emplacements accroissent la portée de l’audience. |
| **[!UICONTROL Assets]** | Nombre de ressources utilisées dans la publicité ou l’expérience. | |
| **[!UICONTROL Impressions]** | Comptage de chaque chargement de l’emplacement ou de l’expérience publicitaire dans le canal, indépendamment de l’interaction ou de l’affichage. | Un nombre d’impressions élevé peut indiquer une large visibilité, mais pour obtenir de vraies informations sur les performances, prenez en compte d’autres mesures d’engagement. |
| **[!UICONTROL Clics]** | Nombre de fois où les utilisateurs interagissent avec un élément cliquable, tel qu’un lien ou un bouton d’appel à l’action, dans un emplacement d’expérience. | Un nombre de clics élevé indique un fort intérêt et un engagement envers le contenu, ce qui peut être efficace et atteindre la bonne audience. |
| **[!UICONTROL CTR ]**<br>_Taux de clics_ | Pourcentage (%) d’impressions ayant généré des clics sur l’emplacement de l’expérience au sein d’une campagne.<br>**Calcul** : `clicks` divisé par `impressions` | Un taux de clics élevé indique que le contenu est très pertinent et motivant pour le public dans la messagerie et la conception, et cible effectivement les intérêts du public. |
| **[!UICONTROL CPM ]**<br>_Coût par millier_ | Coût ($) pour chaque millier d’impressions publicitaires pour l’emplacement d’expérience.<br>**Calcul** : somme `spent` divisée par portée, puis multipliée par 1 000 | Une valeur faible peut indiquer une visibilité rentable, en particulier lorsqu’elle est associée à un taux de clics élevé. |
| **[!UICONTROL CPA ]**<br>_Coût par action_ | Coût moyen ($) dépensé pour réaliser une action client spécifique, comme un achat ou un abonnement.<br>**Calcul** : montant total `spent` divisé par le nombre d’actions client terminées | Utilisez pour surveiller les dépenses liées aux expériences qui génèrent des actions précieuses de la part des clients. |
| **[!UICONTROL CPC ]**<br>_Coût par clic_ | Coût moyen ($) associé à chaque clic dans un emplacement d’expérience.<br>**Calcul** : montant total `spent` divisé par `clicks` | Des coûts moyens inférieurs peuvent indiquer des dépenses publicitaires rentables, en particulier par rapport à une augmentation des conversions. |
| **[!UICONTROL Dépenser]** | Montant ($) dépensé dans le budget sur une période donnée. | Un montant élevé de dépenses sur une courte période peut indiquer une utilisation rapide, ce qui pourrait conduire à une diminution rapide des ressources. Effectuez le suivi du montant des dépenses par rapport aux mesures de performances clés pour mieux surveiller le retour sur investissement global. |
