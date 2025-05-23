---
title: Campagnes Adobe GenStudio for Performance Marketing
description: Découvrez comment créer et gérer des campagnes marketing numériques qui tirent parti des ressources et des expériences d’IA générative.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."
source-git-commit: edbeb7f0d08e2215a23f15cfeff77a5217cd264b
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 0%

---

# Création d’une campagne

Une campagne GenStudio for Performance Marketing définit les caractéristiques essentielles d’une campagne numérique et évolue à mesure que les étapes sont déployées et évaluées. GenStudio for Performance Marketing prend en charge le processus dynamique de lancement d’une campagne, le suivi des performances des composants individuels de la campagne et le recentrage des expériences publicitaires en fonction des mesures de performances.

Les éléments clés de votre campagne sont stockés dans un objet de campagne, ce qui crée un contexte partagé pour toutes les ressources et expériences libellées avec le même nom de campagne unique. Ce libellé identifie la campagne dans GenStudio for Performance Marketing.

Les gestionnaires de système GenStudio et les éditeurs Genstudio peuvent créer des campagnes.

## Définition des détails de la campagne

{{$include /help/_includes/campaign-details.md}}


**Pour saisir les détails de la campagne** :

1. Dans [!DNL Campaigns], cliquez sur **[!UICONTROL Ajouter une campagne]**. La vue _Créer une campagne_ s’ouvre.

   Les détails englobent les champs facultatifs et obligatoires qui définissent votre campagne. Ces détails sont enregistrés dans [!DNL Campaigns] en tant qu’attributs de métadonnées de la campagne.

1. Double-cliquez sur l’en-tête _Nouvelle campagne_ et saisissez un nom informatif et unique.

   Ce nom devient un _libellé de campagne_ dans GenStudio for Performance Marketing, ce qui vous permet d’associer des ressources ou des expériences à la campagne lors du chargement et de la création.

1. Saisissez les valeurs dans les champs _Détails_ qui décrivent votre campagne. Consultez le tableau _Détails de la campagne_ pour obtenir une définition de ces fonctionnalités de campagne.

## Attribution de canaux et de régions

Les paramètres de canal et de région déterminent où la campagne est déployée et ses canaux de distribution.

GenStudio for Performance Marketing utilise des modèles prédéfinis appelés _enregistrements_ pour représenter les composants clés de la campagne, tels que les canaux, les régions, les personas et les produits. Lors de la création d’une campagne, vous devez l’associer aux enregistrements pertinents pour chacun de ces composants.

* **Paramètres de canal** : définit les canaux de distribution publics de votre campagne, y compris les comptes de médias achetés, les services de marketing par e-mail et les réseaux publicitaires display. Les données sur les performances des campagnes, des ressources et des expériences dans ces canaux sont intégrées aux [[!DNL Insights]](/help/user-guide/insights/overview.md) pour une analyse spécifique aux canaux.

* **Paramètres de région** : indique les zones géographiques dans lesquelles vous déployez votre campagne. En se connectant à des sources de données régionales, GenStudio for Performance Marketing peut adapter le contenu et la stratégie aux préférences des audiences locales. Cela permet un ciblage et une analyse des performances plus précis basés sur les mesures régionales.

**Pour sélectionner des canaux de distribution pour votre campagne** :

1. Cliquez sur le signe + (**[!UICONTROL Connecter les enregistrements +]**) en regard de **[!UICONTROL Canaux]**.

   La fenêtre contextuelle _Sélectionner des canaux_ s’ouvre.

1. Sélectionnez les canaux sur lesquels la campagne est déployée. Les valeurs valides sont les suivantes : `Email`, `Paid media`, `Web` et `Display ads`.

   Si vous le souhaitez, choisissez **[!UICONTROL Voir tout]** pour ouvrir une vue de tous les canaux pris en charge.

**Pour affecter des régions à votre campagne** :

1. Cliquez sur le signe + (**[!UICONTROL Connecter les enregistrements +]**) en regard de **[!UICONTROL Régions]**.

   La fenêtre contextuelle _Sélectionner les régions_ s’ouvre. Vous pouvez rechercher une région prise en charge spécifique.

1. Sélectionnez les régions d’une ou plusieurs régions cibles pour votre campagne. Les régions valides sont les suivantes : `AMER`, `LATAM`, `EMEA`, `APAC` et `Japan`.

   Si vous le souhaitez, choisissez **[!UICONTROL Voir tout]** pour ouvrir une vue de toutes les régions prises en charge.

## Attribuer des rôles et des produits

[Personas](/help/user-guide/guidelines/personas.md) et [products](/help/user-guide/guidelines/products.md) sont enregistrés en tant qu’enregistrements. Un enregistrement de persona définit les caractéristiques d’un segment client spécifique : votre audience cible pour le contenu généré. Il peut inclure des détails démographiques et un historique des interactions client.

Les enregistrements de produit définissent les spécifications et attributs clés du produit dans le contexte des directives de votre marque. Les attributs peuvent inclure des fonctionnalités, des images associées et le positionnement du produit au sein de votre marque.

Les options des menus déroulants _Personnes_ et _Produits_ sont définies au niveau de l’entreprise. Lors de la création d’une campagne, vous effectuez une sélection parmi ces enregistrements prédéfinis afin d’assurer une représentation cohérente du produit et de prendre en charge un ciblage, un message et un suivi des performances précis.

**Pour attribuer des rôles à votre campagne** :

1. Cliquez sur le signe + (**[!UICONTROL Connecter les enregistrements +]**) en regard de **[!UICONTROL Personnes]**.

   La fenêtre contextuelle _Sélectionner les personnes_ s’ouvre. Vous pouvez rechercher des personnages pris en charge spécifiques.

1. Sélectionnez les personnes ciblées par votre campagne. Les rôles valides sont définis par votre organisation lors de la [création des directives](/help/user-guide/guidelines/personas.md).

   Si vous le souhaitez, choisissez **[!UICONTROL Voir tout]** pour ouvrir une vue de toutes les personnes disponibles.

**Pour affecter des produits à votre campagne** :

1. Cliquez sur le signe + (**[!UICONTROL Connecter les enregistrements +]**) en regard de **[!UICONTROL Produits]**.

   La fenêtre contextuelle _Sélectionner des produits_ s’ouvre. Vous pouvez rechercher un produit pris en charge spécifique.

1. Sélectionnez un ou plusieurs produits. Les produits sont définis par votre organisation lors de la [création d’instructions](/help/user-guide/guidelines/products.md).

   Si vous le souhaitez, choisissez **[!UICONTROL Voir tout]** pour ouvrir une vue de tous les produits disponibles.

## Création complète de la campagne

Cliquez sur **[!UICONTROL Créer]** pour enregistrer les valeurs saisies et créer la campagne.

Le nouveau nom de campagne est désormais disponible sous la forme d’un libellé de campagne dans [!DNL Content] et [!DNL Create]. Vous pouvez ajouter des ressources et des expériences approuvées à votre campagne par le biais de [!DNL Content] ou attribuer une ressource et une expérience à une campagne lors de la création de contenu.

## Ajouter du contenu à votre campagne

GenStudio for Performance Marketing lie le contenu aux campagnes à l’aide de libellés de campagne stockés dans les métadonnées [!DNL Content]. Un seul élément de contenu peut être associé à plusieurs campagnes.

Les libellés de campagne identifient la campagne et ses attributs. L’attribution d’un libellé à une ressource ou à une expérience la connecte à la campagne correspondante.

**Pour ajouter des ressources et des expériences à partir d’[!DNL Content]** :

1. Dans la galerie [!DNL Content] _Expériences_ ou _Assets_, choisissez l’expérience ou la ressource approuvée.

1. Dans la vue _Détails_, sélectionnez le nom de la campagne dans le menu déroulant _Campagnes_.

**Pour ajouter des ressources et des expériences lors de la création de contenu** :

Lors de la création de contenu, vous pouvez publier la ressource ou l’expérience nouvellement créée dans [!DNL Content].

1. Dans la fenêtre contextuelle _Confirmer les détails de votre contenu approuvé_, sélectionnez une campagne dans le menu déroulant _Campagnes_.

1. Cliquez sur **[!UICONTROL Publier]**.

Cette campagne est désormais disponible dans le tableau de bord _Campagnes_.
