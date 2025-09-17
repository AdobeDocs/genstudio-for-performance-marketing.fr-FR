---
title: Attribuer  [!DNL Brand]  Autorisations
description: Découvrez comment attribuer des droits aux créateurs et  [!DNL Brand]  éditeurs GenStudio for Performance Marketing.
level: Intermediate
feature: Brand Personalization, Generative AI
exl-id: fc33ecd3-4403-4045-87af-012a0377226c
source-git-commit: adb1d34eb76d7594933fe9951c4c1885e6d6369b
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 1%

---

# Attribuer des autorisations [!DNL Brand]

Par défaut, les responsables système de GenStudio peuvent créer et modifier des [!DNL Brands]. Les rôles d&#39;éditeur de contenu et de collaborateur disposent d&#39;autorisations de modification et de création, mais peuvent ne pas nécessiter de droits de gestion du système.

Pour accorder aux éditeurs et aux collaborateurs de contenu ces droits liés à [!DNL Brand], un administrateur système Adobe doit effectuer des tâches de configuration supplémentaires dans Adobe Admin Console. Voir [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html#Overview) dans _Guide d’administration pour les entreprises et les équipes_.

L’ajout d’utilisateurs et de groupes d’utilisateurs est une tâche de base commune à tous les produits Adobe avec des droits gérés via Admin Console. Consultez [Utilisateurs Adobe Admin Console](https://helpx.adobe.com/fr/enterprise/using/users.html) dans le _Guide d’administration d’entreprise et d’équipes_ pour obtenir un aperçu de la gestion des utilisateurs et des procédures d’ajout d’utilisateurs et de groupes d’utilisateurs.

Regardez cette présentation vidéo ou suivez les étapes ci-dessous.

>[!VIDEO](https://video.tv.adobe.com/v/3474996?learn=on&enablevpops)

## Étape 1 : créer un groupe d’utilisateurs

**Pour créer un groupe d’utilisateurs** :

1. Connectez-vous à Admin Console et accédez à **[!UICONTROL Utilisateurs]** > **[!UICONTROL Groupes d’utilisateurs]**.

1. Cliquez sur **[!UICONTROL Nouveau groupe d’utilisateurs]**. La fenêtre contextuelle _Créer un groupe d’utilisateurs_ s’ouvre.

1. Ajoutez un nom de groupe d’utilisateurs informatif au champ **[!UICONTROL Nom du groupe d’utilisateurs]** pour identifier l’objectif du nouveau groupe. Par exemple, « Brand Manager ».

1. Vous pouvez éventuellement ajouter une description du groupe et de son objectif.

1. Cliquer sur **[!UICONTROL Enregistrer]**. Admin Console ouvre la fenêtre contextuelle _Nouveau groupe_ avec le nom du groupe nouvellement créé.

Voir [Gérer les groupes d’utilisateurs](https://helpx.adobe.com/fr/enterprise/using/user-groups.html) dans le _Guide d’administration pour les entreprises et les équipes_.

## Étape 2 : affecter un profil de gestionnaire système GenStudio au groupe d’utilisateurs

Une fois que vous avez créé un nouveau groupe d&#39;utilisateurs et ajouté des utilisateurs, vous pouvez affecter le profil **gestionnaire système Adobe GenStudio** à ce groupe. Le droit associé au profil affecté donne à tous les utilisateurs de ce groupe des autorisations de [!DNL Brands] GenStudio (création, mise à jour et suppression de marques).

**Pour attribuer un profil au groupe d’utilisateurs** :

1. Accédez au groupe d’utilisateurs nouvellement créé et cliquez sur l’onglet _Profils de produit attribués_.

1. Dans l’onglet _Profils de produit attribués_ cliquez sur **[!UICONTROL Attribuer un profil]**. La fenêtre contextuelle _Attribuer des produits et des profils_ s’ouvre.

1. Sélectionnez `Adobe GenStudio` dans la liste _Sélectionner des produits_.

1. Cliquez sur **[!UICONTROL Appliquer]**. La fenêtre contextuelle _Sélectionner des profils de produit_ s’ouvre, affichant les profils de produit associés à Adobe GenStudio.

1. Sélectionnez `Adobe GenStudio system manager`.

1. Cliquez sur **[!UICONTROL Appliquer]**. La fenêtre contextuelle _Attribuer des produits et des profils_ s’ouvre, affichant le profil de produit du groupe d’utilisateurs nouvellement créé.

1. Cliquer sur **[!UICONTROL Enregistrer]**.

Voir [Attribuer des profils de produit à des groupes d’utilisateurs](https://helpx.adobe.com/fr/enterprise/using/user-groups.html) dans _Guide d’administration pour les entreprises et les équipes_.

## Étape 3 : ajouter des utilisateurs au groupe d’utilisateurs

Pour attribuer aux utilisateurs l’autorisation de créer, modifier et publier des [!DNL Brands], ajoutez-les au groupe d’utilisateurs nouvellement créé.

>[!NOTE]
>
>Vous devez ajouter au moins un utilisateur à ce groupe d’utilisateurs avant d’ajouter le groupe à votre projet.

**Pour ajouter des utilisateurs au groupe d’utilisateurs** :

1. Dans _Admin Console_, accédez à **[!UICONTROL Utilisateurs]** > **[!UICONTROL Groupes d’utilisateurs]**.

1. Sélectionnez le nom du groupe d’utilisateurs que vous avez créé précédemment. La fenêtre contextuelle _Ajouter des utilisateurs à ce groupe d’utilisateurs_ s’ouvre.

1. Ajoutez un utilisateur nouveau ou existant en utilisant le nom d’utilisateur ou l’adresse électronique. Lorsque vous saisissez un nom ou une adresse e-mail pour un utilisateur existant, ce champ est automatiquement renseigné avec des noms correspondants pour les utilisateurs connus qui appartiennent à cette organisation IMS. Découvrez la gestion des groupes d’utilisateurs dans [Gérer les groupes d’utilisateurs](https://helpx.adobe.com/fr/enterprise/using/user-groups.html) dans _Guide d’administration pour les entreprises et les équipes_.

Les utilisateurs disposent des autorisations de création, de modification et de publication [!DNL Brand] des responsables système d’Adobe GenStudio lorsqu’ils sont ajoutés au groupe. Les utilisateurs reçoivent également une invitation par e-mail automatisée pour modifier le projet Adobe GenStudio for Performance Marketing [!DNL Brands].

## Étape 4 : créer un projet [!DNL Brands]

Un _projet_ fournit un emplacement de stockage où certains utilisateurs peuvent enregistrer des ressources (dans ce cas, des ressources [!DNL Brands]).

**Pour créer un projet [!DNL Brands] à partir de l’onglet _Stockage_** :

1. Accédez à l’onglet _Stockage_ dans Admin Console.

1. Cliquez sur **[!UICONTROL Projets]** dans la navigation latérale. L’onglet _Projets_ s’ouvre.

1. Cliquez sur **[!UICONTROL Créer un projet]**. La fenêtre contextuelle _Nouveau projet_ s’ouvre.

1. Saisissez `Adobe GenStudio Brands` dans le champ du nom du projet. Saisissez le nom de ce projet tel qu&#39;il est affiché ici. N’insérez pas d’espaces supplémentaires et ne modifiez pas la casse.

1. Cliquez sur **[!UICONTROL Créer]**. La fenêtre contextuelle _Inviter au projet_ s’ouvre.

Voir [Gérer les projets](https://helpx.adobe.com/enterprise/using/projects-in-business-storage.html) dans le guide d’administration _Entreprise et équipes_.

## Étape 5 : inviter un groupe d’utilisateurs à rejoindre le projet

Vous êtes maintenant prêt à ajouter le groupe d’utilisateurs que vous venez de créer au projet `Adobe GenStudio [!DNL Brands]`.

**Pour inviter le groupe d’utilisateurs au projet nouvellement créé** :

1. Dans la fenêtre contextuelle _Inviter au projet_, ajoutez le groupe d’utilisateurs que vous venez de créer à ce projet.

1. Sélectionnez l’option **Peut modifier** autorisations .

1. Cliquez sur **[!UICONTROL Inviter]**.
