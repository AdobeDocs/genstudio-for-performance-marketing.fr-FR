---
title: Connexion à Meta Ads
description: Connectez un compte Meta Ads pour activer et surveiller vos publicités et médias avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Data Engineer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
source-git-commit: 40c7d2d40f1c4bea9794e706d8e1ce7bf92042e3
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

# Connexion à Meta Ads

Cette page explique comment connecter et gérer votre compte de profil Meta Ads vers GenStudio for Performance Marketing afin de gérer les campagnes, d’exporter le contenu et d’accéder aux données publicitaires pour vos campagnes actives.

>[!BEGINSHADEBOX]

**Conditions préalables** :

- Login Facebook/Meta pouvant accéder à tous les services Meta

- _Contrôle total_ sur Meta Business Portfolio et les comptes publicitaires, notamment :

   - Gestion des campagnes
   - Affichage des performances
   - Gestion des maquettes du Hub Creative
   - Analyses avancées

- Désactivez tous les bloqueurs de fenêtres contextuelles dans votre navigateur.

>[!ENDSHADEBOX]

## Connexion à un compte Meta Ads

1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Paramètres]**.

1. Dans la section _Connecteurs de données_, cliquez sur **[!UICONTROL Se connecter]** sur la carte _Meta Ads_.

1. Connectez-vous à votre compte Facebook.

   Vous devrez peut-être supprimer les bloqueurs de pop-up, puis utiliser **[!UICONTROL Actualiser]** pour réessayer.

1. Suivez les instructions d’authentification Facebook, vérifiez les informations du compte, puis cliquez sur **[!UICONTROL Continuer comme ...]**

1. Dans _[!UICONTROL Facebook Login for Business]_ (symbole Meta vers Adobe), parcourez les sélections suivantes pour accorder l’accès à GenStudio for Performance Marketing :

   - Sélectionnez un ou plusieurs profils Meta Business et cliquez sur **[!UICONTROL Continuer]**
   - Sélectionnez une ou plusieurs pages Meta, puis cliquez sur **[!UICONTROL Continuer]**
   - Sélectionnez un ou plusieurs comptes Instagram et cliquez sur **[!UICONTROL Continuer]**
   - Vérifiez les sélections et cliquez sur **[!UICONTROL Enregistrer]**

     ![Vérifier sélections](/help/assets/meta/meta-review-selections.png "Vérifier sélections"){width="400" zoomable="yes"}

1. Une fois que vous avez reçu la vérification que votre compte est connecté, cliquez sur **[!UICONTROL Compris]**.

   Cette étape permet à GenStudio for Performance Marketing d’accéder à toutes les publicités, métadonnées et mesures pour des performances optimales.

1. Dans _[!UICONTROL Meta Ads]_, sélectionnez un ou plusieurs comptes à inclure dans [!DNL Insights] et cliquez sur **[!UICONTROL Sélectionner]**.

1. Une fois que vous avez reçu une confirmation _Connecté à Platform_, cliquez sur **[!UICONTROL Afficher les comptes]**.

   La vue _[!UICONTROL Comptes Meta Ads]_ répertorie les `Account name`, `Added by`, `Date added` et `Status`.

   ![Liste &#x200B;](/help/assets/meta/meta-accounts-list.png " comptes MetaListe des comptes Meta connectés"){zoomable="yes"}

Utilisez **[!UICONTROL Ajouter un compte]** pour ajouter d’autres comptes à la liste. Le flux d’autorisation peut différer légèrement lorsque vous ajoutez des comptes liés au même profil Meta Business. Vous sélectionnez uniquement les nouveaux comptes Meta Ads pendant le processus de connexion.

## Déconnexion et dépannage d’une intégration Meta Ads

Il arrive qu’une instance GenStudio for Performance Marketing ne soit pas correctement connectée à un compte Meta Ads. Les configurations les plus courantes pouvant entraîner des problèmes sont les suivantes :

- Un compte Instagram est sélectionné sans sélectionner sa page Facebook associée
- Autorisations révoquées pour un utilisateur qui a effectué la connexion initiale

Dans ce cas, il est préférable de reconnecter le compte publicitaire Meta à l’instance GenStudio for Performance Marketing. Tout d’abord, l’utilisateur doit supprimer l’intégration de l’application directement depuis son Meta Business Manager, ce qui permet de réinitialiser les autorisations. Pour ce faire, un accès administrateur à Meta Business Manager est nécessaire.

Ces étapes effacent les autorisations mises en cache et réinitialisent le flux d’intégration :

1. Accédez à [Meta Business Manager](https://business.facebook.com) en consultant le site web Facebook.
1. Connectez-vous avec votre compte. Le compte doit avoir un accès administrateur au Business Manager.
1. Cliquez sur l’icône représentant un engrenage **[!UICONTROL Paramètres]** dans le coin inférieur gauche pour accéder aux paramètres de Business Portfolio.
1. Dans le menu de gauche, cliquez sur **[!UICONTROL Intégrations]**.
1. Sélectionnez **[!UICONTROL Applications connectées]**. Adobe GenStudio apparaît dans la liste des applications connectées .
   ![Meta Business Manager Connected Apps](./meta-connected-apps.png "Volet Meta Business Manager Connected Apps")
1. Cliquez sur le nom de l’application.
1. Cliquez sur **[!UICONTROL Supprimer]**.
1. Confirmez la suppression lorsque vous y êtes invité.

Vous pouvez désormais reconnecter vos comptes publicitaires Meta, vos profils Instagram et vos pages Facebook.
