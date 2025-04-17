---
title: Connecter un média payant
description: Connectez un compte de canal pour activer et surveiller vos publicités et médias avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
feature: Reporting and Insights
exl-id: e699041e-b462-45b3-8c4c-4de0d52cf0e6
source-git-commit: af354448ef609db3c51026ee0e9991ac5cedeba5
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Connecter des comptes de médias achetés

_[!DNL Data connectors]_une intégration transparente entre GenStudio for Performance Marketing et vos comptes de réseau de médias achetés. En vous connectant à des comptes de canaux tiers, vous pouvez échanger des données essentielles, telles que les mesures de performances des campagnes dans [[!DNL Insights]](/help/user-guide/insights/overview.md), et diffuser de nouveaux emplacements publicitaires avec [[!DNL Activate]](/help/user-guide/activation/overview.md). Cette intégration permet à GenStudio for Performance Marketing de gérer vos médias et publicités tout en recevant des informations précieuses, notamment des impressions, des clics et des conversions, de vos campagnes actives.

**Pour vous connecter à un compte de média payant** :

1. Cliquez sur le **[!UICONTROL ... Plus]** dans le volet de navigation inférieur gauche.

1. Sélectionnez **[!UICONTROL Paramètres]** avec l’icône engrenage.

1. Dans _[!UICONTROL Paramètres]_, choisissez un type de connecteur dans la section _[!UICONTROL Connecteurs de données]_, puis cliquez sur **[!UICONTROL Connecter]**.

   S’il existe des comptes connectés, vous pouvez cliquer sur _comptes connectés_ pour afficher une liste de noms de compte, de détails et de statuts.

1. Affichez le [type de connecteur](#connector-types) que vous avez sélectionné, passez en revue les conditions préalables et continuez les étapes de connexion.

## Connexions de médias payantes

GenStudio for Performance Marketing prend en charge divers types de connecteurs à intégrer à vos plateformes marketing préférées. Chaque type de connecteur comporte des conditions préalables spécifiques et des étapes de configuration à effectuer pour une connexion réussie.

### Connexion à Google Campaign Manager 360

>[!BEGINSHADEBOX]

**Conditions préalables** :

- Compte Google Campaign Manager 360
- Supprimez tous les bloqueurs de pop-up dans votre navigateur

>[!ENDSHADEBOX]

**Pour connecter un compte Google Campaign Manager 360** :

1. Dans la section _Connecteurs de données_, cliquez sur **[!UICONTROL Se connecter]** sur la vignette _Google Campaign Manager 360_.

1. Connectez-vous à votre compte Google Campaign Manager 360.

   Vous devrez peut-être supprimer les bloqueurs de pop-up, puis utiliser **[!UICONTROL Actualiser]** pour réessayer.

1. Lisez les conditions générales et cliquez sur **[!UICONTROL Autoriser]** pour accorder l’accès.

1. Dans la vue _[!UICONTROL Google Campaign Manager 360]_, sélectionnez un ou plusieurs annonceurs et cliquez sur **[!UICONTROL Sélectionner]**.

La vue _[!UICONTROL Comptes Google Campaign Manager 360]_ répertorie les `Account name`, `Added by`, `Date added` et `Status`. Utilisez **[!UICONTROL Ajouter un compte]** pour ajouter d’autres comptes à la liste.

### Connexion des métadonnées publicitaires

>[!BEGINSHADEBOX]

**Conditions préalables** :

- Compte Facebook/Meta ads
- Accès au compte Méta-publicités avec `View performance` niveau d’autorisation pour accéder aux rapports et afficher les publicités
- Supprimez tous les bloqueurs de pop-up dans votre navigateur

>[!ENDSHADEBOX]

**Pour connecter un compte Meta Ads** :

1. Dans la section _Connecteurs de données_, cliquez sur **[!UICONTROL Se connecter]** sur la carte _Méta-annonces_.

1. Connectez-vous à votre compte Facebook.

   Vous devrez peut-être supprimer les bloqueurs de pop-up, puis utiliser **[!UICONTROL Actualiser]** pour réessayer.

1. Suivez les instructions d&#39;authentification Facebook.

1. Dans le pop-up _[!UICONTROL Connexion Facebook à l’entreprise]_ (symbole Meta à Adobe), effectuez les sélections suivantes.

   - Vérifiez les informations du compte et cliquez sur **[!UICONTROL Continuer comme]**
   - Accordez l’accès à certaines pages et cliquez sur **[!UICONTROL Continuer]**
   - Accordez l’accès à certaines entreprises et cliquez sur **[!UICONTROL Continuer]**
   - Inscrivez-vous à un ou plusieurs comptes Instagram et cliquez sur **[!UICONTROL Continuer]**
   - Vérifiez les sélections et cliquez sur **[!UICONTROL Enregistrer]**

1. Dans la vue _[!UICONTROL Méta-publicités]_, sélectionnez un ou plusieurs comptes et cliquez sur **[!UICONTROL Sélectionner]**.

La vue _[!UICONTROL Comptes de méta-annonces]_ répertorie les `Account name`, `Added by`, `Date added` et `Status`. Utilisez **[!UICONTROL Ajouter un compte]** pour ajouter d’autres comptes à la liste.

## Ingestion des données

Dans un premier temps, GenStudio for Performance Marketing importe les données historiques des six derniers mois. Cette pratique vous garantit un accès immédiat à des informations pertinentes pour analyser les tendances, évaluer les performances et prendre des décisions éclairées. Le processus d’ingestion peut prendre entre un et cinq jours selon le volume de données présent dans votre compte.

>[!BEGINSHADEBOX]

**Politique d’ingestion et de conservation des données**

GenStudio for Performance Marketing conserve les données de canal pendant 13 mois. Cette politique de conservation comprend les 6 mois de données ingérées lors de la connexion initiale, ce qui garantit une analyse complète des données historiques et la création de rapports.

>[!ENDSHADEBOX]
