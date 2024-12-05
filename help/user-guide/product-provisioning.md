---
title: Configuration d’Adobe GenStudio for Performance Marketing
description: Découvrez comment configurer le produit GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: 7a9f8de1-79e7-455c-ae0f-e7646febc483
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Configuration d’Adobe GenStudio for Performance Marketing

Un administrateur système Adobe effectue les tâches initiales de mise en service dans le [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview). Depuis l’Admin Console, un administrateur système Adobe peut accéder au profil de produits GenStudio et attribuer des licences de produits disponibles aux utilisateurs.

>[!NOTE]
>
>Seuls les administrateurs système d’Adobe peuvent mettre en oeuvre des tâches d’activation nécessitant un accès à Adobe Admin Console.

>[!IMPORTANT]
>
>N’ajoutez pas de nouveaux profils de produit existants, ni ne les modifiez ou ne les supprimez. La modification des profils de produit par défaut peut perturber considérablement votre déploiement GenStudio for Performance Marketing.

## Étape 1 : accès au profil de produits dans Adobe Admin Console

Dans l’Admin Console, le profil de produit définit des règles et des profils utilisateur uniques à la création et à la gestion de marques et de campagnes dans GenStudio for Performance Marketing.

**Pour accéder au profil de produit GenStudio**

1. Cliquez sur le lien **Commencer** de votre e-mail de bienvenue pour accéder à [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview).

1. Connectez-vous à l’Admin Console à l’aide de votre Adobe ID.

   Une fois la connexion établie, l’onglet _Aperçu_ de Adobe Admin Console s’affiche.

1. Accédez à l’onglet _Produits_ . Cet onglet affiche tous les produits Adobes achetés par votre entreprise.

1. Sélectionnez **[!UICONTROL GenStudio]** dans la liste des produits. La console affiche le profil de produit GenStudio, qui affiche des informations clés sur les licences de produit achetées par votre entreprise. Il fournit également des options de gestion de ces licences.

Vous êtes maintenant prêt à attribuer des licences aux utilisateurs (de type payement) de GenStudio for Performance Marketing. Si vous vous êtes connecté à la mauvaise organisation, basculez vers la bonne organisation avant d’essayer d’affecter des droits aux utilisateurs. Pour modifier votre organisation, cliquez sur le nom de l’organisation dans le coin supérieur droit et choisissez l’organisation **GenStudio**.

## Étape 2 : configuration des utilisateurs

L’attribution de privilèges d’accès aux utilisateurs dans l’Admin Console est le processus d’attribution de licences de produit aux utilisateurs. Ces utilisateurs doivent appartenir à l’organisation IMS spécifiée dans le profil de produit. Vous pouvez fournir des utilisateurs à votre organisation GenStudio for Performance Marketing de la même manière que vous configurez des utilisateurs à d’autres produits Adobe. Vous pouvez ajouter des utilisateurs manuellement ou importer des utilisateurs en bloc.

>[!TIP]
>
>Attribuez-vous les droits du gestionnaire système GenStudio pour effectuer des tâches de gestion du système dans GenStudio for Performance Marketing.

**Conditions préalables** :

Préparez la mise en service en commençant par identifier les informations de base :

* Prénom et nom
* Adresse électronique de l’entreprise
* Type de droits à affecter aux utilisateurs

Voir [Rôles utilisateur et autorisations](user-roles.md) pour obtenir des conseils sur l’affectation de rôles utilisateur GenStudio for Performance Marketing.

Vous pouvez ajouter des utilisateurs individuellement ou importer des informations de compte pour plusieurs utilisateurs :

* [Gérer l’utilisateur individuellement](https://helpx.adobe.com/enterprise/using/manage-users-individually.html#add-users)

* [Gérer plusieurs utilisateurs/chargement CSV en masse](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html)

Une fois que vous avez intégré les utilisateurs à GenStudio for Performance Marketing de votre entreprise, un gestionnaire de système GenStudio peut [ configurer les directives de marque et de média de votre entreprise ](get-started.md).
