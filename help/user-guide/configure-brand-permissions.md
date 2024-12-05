---
title: 'Attribuer des autorisations  [!DNL Brand] '
description: Découvrez comment affecter des droits aux créateurs et aux éditeurs de GenStudio for Performance Marketing [!DNL Brand] .
level: Intermediate
feature: Brands Service, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# Attribuer des autorisations [!DNL Brand]

Par défaut, les gestionnaires de système GenStudio peuvent créer et modifier [!DNL Brands]. Les rôles de l’éditeur de contenu et du collaborateur disposent d’autorisations de modification et de création, mais peuvent ne pas nécessiter de droits de gestion du système. Pour accorder aux éditeurs de contenu et aux collaborateurs ces droits [!DNL Brand] liés, un administrateur système d’Adobe doit effectuer certaines tâches de configuration supplémentaires dans Adobe Admin Console. Voir [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) dans le _guide d’administration Enterprise and Teams_.

L’ajout d’utilisateurs et de groupes d’utilisateurs est une tâche de base commune à tous les produits Adobe disposant de droits gérés par l’Admin Console. Voir [Utilisateurs de Adobe Admin Console](https://helpx.adobe.com/fr/enterprise/using/users.html) dans le _Guide d’administration Enterprise and Teams_ pour un aperçu de la gestion des utilisateurs et des procédures d’ajout d’utilisateurs et de groupes d’utilisateurs.

## Étape 1 : création d’un groupe d’utilisateurs

**Pour créer un groupe d’utilisateurs** :

1. Connectez-vous à l’Admin Console et accédez à **[!UICONTROL Utilisateurs]** > **[!UICONTROL Groupes d’utilisateurs]**.

1. Cliquez sur **[!UICONTROL Nouveau groupe d’utilisateurs]**. La fenêtre contextuelle _Créer un groupe d’utilisateurs_ s’ouvre.

1. Ajoutez un nom informatif de groupe d’utilisateurs au champ **[!UICONTROL Nom du groupe d’utilisateurs]** pour identifier l’objectif du nouveau groupe. Par exemple, &quot;Chargés de marques&quot;.

1. Vous pouvez éventuellement ajouter une description du groupe et son objectif.

1. Cliquer sur **[!UICONTROL Enregistrer]**. L’Admin Console ouvre la fenêtre contextuelle _Nouveau groupe_ avec le nom du groupe nouvellement créé.

Voir [Gérer les groupes d’utilisateurs](https://helpx.adobe.com/fr/enterprise/using/user-groups.html) dans le _Guide d’administration Enterprise and Teams_.

## Étape 2 : attribuer un profil de gestionnaire de système GenStudio au groupe d’utilisateurs

Une fois que vous avez créé un groupe d’utilisateurs et ajouté des utilisateurs, vous pouvez attribuer le profil **Adobe GenStudio system manager** à ce groupe. Les droits associés au profil affecté donnent à tous les utilisateurs de ce groupe des autorisations [!DNL Brands] de GenStudio (créer, mettre à jour et supprimer des marques).

**Pour attribuer un profil au groupe d’utilisateurs** :

1. Accédez au groupe d’utilisateurs nouvellement créé et cliquez sur l’onglet _Profils de produit attribués_ .

1. Dans l’onglet _Profils de produit affectés_ , cliquez sur **[!UICONTROL Attribuer le profil]**. La fenêtre contextuelle _Attribuer des produits et des profils_ s’ouvre.

1. Sélectionnez `Adobe GenStudio` dans la liste _Select products_.

1. Cliquez sur **[!UICONTROL Apply]**. La fenêtre contextuelle _Sélectionner les profils de produit_ s’ouvre, affichant les profils de produit associés à l’Adobe GenStudio.

1. Sélectionnez `Adobe GenStudio system manager`.

1. Cliquez sur **[!UICONTROL Apply]**. La fenêtre contextuelle _Attribuer des produits et des profils_ s’ouvre, affichant le profil de produit du groupe d’utilisateurs nouvellement créé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

Voir [Attribuer des profils de produit aux groupes d’utilisateurs](https://helpx.adobe.com/fr/enterprise/using/user-groups.html) dans le _Guide d’administration Enterprise and Teams_.

## Étape 3 : Ajout d’utilisateurs au groupe d’utilisateurs

Pour attribuer aux utilisateurs l&#39;autorisation de créer, modifier et publier [!DNL Brands], ajoutez-les au groupe d&#39;utilisateurs nouvellement créé.

>[!NOTE]
>
>Vous devez ajouter au moins un utilisateur à ce groupe avant de l’ajouter à votre projet.

**Pour ajouter des utilisateurs au groupe d’utilisateurs** :

1. À partir de _Admin Console_, accédez à **[!UICONTROL Utilisateurs]** > **[!UICONTROL Groupes d’utilisateurs]**.

1. Sélectionnez le nom du groupe d’utilisateurs que vous avez créé précédemment. La fenêtre contextuelle _Ajouter des utilisateurs à ce groupe d’utilisateurs_ s’ouvre.

1. Ajoutez un utilisateur nouveau ou existant par nom d’utilisateur ou adresse électronique. Lorsque vous saisissez un nom ou une adresse électronique pour un utilisateur existant, ce champ est automatiquement renseigné avec les noms correspondants pour les utilisateurs connus appartenant à cette organisation IMS. Découvrez la gestion des groupes d’utilisateurs dans [Gérer les groupes d’utilisateurs](https://helpx.adobe.com/fr/enterprise/using/user-groups.html) dans le _Guide d’administration Enterprise and Teams_.

Lorsqu’ils sont ajoutés au groupe, les utilisateurs disposent des autorisations de création, de modification et de publication [!DNL Brand] des gestionnaires de système d’Adobe GenStudio. Les utilisateurs reçoivent également une invitation par courrier électronique automatisée pour modifier le projet Adobe GenStudio for Performance Marketing [!DNL Brands].

## Étape 4 : création d’un projet [!DNL Brands]

Un _projet_ fournit un emplacement de stockage où certains utilisateurs peuvent enregistrer des ressources, dans ce cas des ressources [!DNL Brands].

**Pour créer un projet [!DNL Brands] à partir de l’onglet _Storage_** :

1. Accédez à l’onglet _Stockage_ dans l’Admin Console.

1. Cliquez sur **[!UICONTROL Projets]** dans le volet de navigation latéral. L’onglet _Projets_ s’ouvre.

1. Cliquez sur **[!UICONTROL Créer un projet]**. La fenêtre contextuelle _Nouveau projet_ s’ouvre.

1. Saisissez `Adobe GenStudio Brands` dans le champ du nom du projet. Saisissez le nom de ce projet tel qu’il s’affiche ici. N’incluez pas d’espaces supplémentaires ni ne modifiez la casse de la lettre.

1. Cliquez sur **[!UICONTROL Créer]**. La fenêtre contextuelle _Invitation au projet_ s’ouvre.

Voir [Gérer les projets](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) dans le _guide d’administration Entreprise et équipes_.

## Étape 5 : inviter un groupe d’utilisateurs à rejoindre le projet

Vous êtes maintenant prêt à ajouter le groupe d’utilisateurs que vous venez de créer au projet `Adobe GenStudio [!DNL Brands]`.

**Pour inviter le groupe d’utilisateurs au projet nouvellement créé** :

1. Dans la fenêtre contextuelle _Invitation au projet_, ajoutez le groupe d’utilisateurs que vous venez de créer à ce projet.

1. Sélectionnez l’option **Autorisations de modification** .

1. Cliquez sur **[!UICONTROL Invitation]**.
