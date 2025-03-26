---
title: Configuration d’Adobe GenStudio for Performance Marketing
description: Découvrez comment configurer le produit GenStudio for Performance Marketing.
level: Beginner
feature: Generative AI
role: Admin
exl-id: 7a9f8de1-79e7-455c-ae0f-e7646febc483
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Configuration d’Adobe GenStudio for Performance Marketing

Un administrateur système Adobe effectue les tâches d’approvisionnement initiales dans le [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview). Depuis Admin Console, un administrateur système Adobe peut accéder au profil de produit GenStudio et attribuer des licences de produit disponibles aux utilisateurs.

>[!NOTE]
>
>Seuls les administrateurs système Adobe peuvent implémenter des tâches d’activation nécessitant un accès à Adobe Admin Console.

>[!IMPORTANT]
>
>N’ajoutez pas de nouveaux profils de produit, ni ne modifiez ou ne supprimez pas les profils existants. La modification des profils de produit par défaut peut perturber gravement votre déploiement GenStudio for Performance Marketing.

## Étape 1 : accéder au profil de produit dans Adobe Admin Console

Dans Admin Console, le profil de produit définit les règles et les profils utilisateur qui sont uniques à la création et à la gestion de marques et de campagnes dans GenStudio for Performance Marketing.

**Pour accéder au profil de produit GenStudio**

1. Cliquez sur le lien **Commencer** dans l’e-mail de bienvenue pour accéder à [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview).

1. Connectez-vous à Admin Console à l’aide de votre Adobe ID.

   Une fois la connexion établie, l’onglet _Aperçu_ du Adobe Admin Console s’affiche.

1. Accédez à l’onglet _Produits_. Cet onglet affiche tous les produits Adobe achetés par votre organisation.

1. Sélectionnez **[!UICONTROL GenStudio]** dans la liste des produits. La console affiche le profil de produit GenStudio, qui contient des informations essentielles sur les licences de produit achetées par votre entreprise. Il propose également des options pour gérer ces licences.

Vous êtes maintenant prêt à attribuer des licences aux utilisateurs (configuration) de GenStudio for Performance Marketing. Si vous vous êtes connecté à la mauvaise organisation, basculez vers la bonne organisation avant d’essayer d’attribuer des droits aux utilisateurs. Pour modifier votre organisation, cliquez sur le nom de l’organisation dans le coin supérieur droit et sélectionnez l’organisation **GenStudio**.

## Étape 2 : configurer les utilisateurs

L’attribution de privilèges d’accès aux utilisateurs dans Admin Console est le processus d’attribution de licences de produit aux utilisateurs. Ces utilisateurs doivent appartenir à l’organisation IMS spécifiée dans le profil de produit. Vous pouvez mettre en service des utilisateurs pour votre organisation GenStudio for Performance Marketing de la même manière que vous mettez en service des utilisateurs pour d’autres produits Adobe. Vous pouvez ajouter des utilisateurs manuellement ou importer des utilisateurs en bloc.

>[!TIP]
>
>Attribuez-vous les droits de gestionnaire système de GenStudio pour effectuer des tâches de gestion système dans GenStudio for Performance Marketing.

**Conditions préalables** :

Préparez le provisionnement en identifiant d’abord les informations de base :

* Prénom et nom
* Adresse e-mail de l’entreprise
* Type des droits à attribuer aux utilisateurs

Voir [Rôles utilisateur et autorisations](user-roles.md) pour obtenir des conseils sur l’attribution de rôles utilisateur GenStudio for Performance Marketing.

Vous pouvez ajouter des utilisateurs individuellement ou importer des informations de compte pour plusieurs utilisateurs :

* [Gérer les utilisateurs individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#add-users)

* [Gérer plusieurs utilisateurs/chargement CSV en bloc](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html)

Une fois que vous avez intégré les utilisateurs à GenStudio for Performance Marketing de votre entreprise, un gestionnaire de système GenStudio peut [configurer les directives relatives à la marque et aux médias de votre entreprise](get-started.md).
