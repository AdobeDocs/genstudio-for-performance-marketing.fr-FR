---
title: Création d’une expérience d’affichage d’annonce
description: Découvrez comment créer des expériences d’affichage d’annonce dans Adobe [!DNL GenStudio] pour le marketing sur les performances.
feature: Brands Service, Guidelines, Content Generation, Generative AI, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 816aeb55eee92758e7ef022ced0ebc3308d27dc9
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Création d’une expérience d’affichage d’annonce

Ce tutoriel explique comment générer des [expériences d’affichage d’annonce](display-ad-experiences.md) avec GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Pour concevoir une expérience d’affichage et d’affichage attrayante, il est recommandé [d’ajouter des instructions à GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) et de consulter les [ principes de base de l’écriture d’invites](/help/user-guide/effective-prompts.md) avant de commencer.

## Choisir un modèle

Pour créer une expérience d’affichage d’annonce, utilisez un modèle disponible afin de fournir la structure de votre contenu.

**Pour choisir un modèle de publicité display** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL Afficher les publicités]**dans le_&quot;Que souhaitez-vous créer aujourd’hui ?&quot;section _.
1. Utilisez l’option de recherche, en regard de _Filtre_, pour trouver un modèle d’annonce d’affichage spécifique.
1. Dans la vue _Select template_, cliquez sur un modèle d&#39;annonce d&#39;affichage.
1. Cliquez sur **[!UICONTROL Utiliser]**.

   La zone de travail, qui sert de centre central pour la création de contenu, s’affiche.

## Ajouter des paramètres

L’ajout de [lignes guides](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans le tiroir de l’invite surcharge le processus de génération de contenu et est une étape préparatoire intégrale pour générer une expérience d’affichage publicitaire.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer le tiroir de l’invite.
1. Dans la section _Parameters_, sélectionnez des instructions—[!DNL Brands], [!DNL Personas] et [!DNL Products]—pour informer la création de contenu.

   S’il n’existe aucune marque, aucun personnage ou aucun produit disponible dans ces menus, [ ajoutez des instructions à votre GenStudio pour le Marketing des performances](/help/user-guide/guidelines/add-guidelines.md).

1. Pour ajouter du contenu à utiliser dans l’expérience *et* afin d’influencer la génération du contenu :
   * Cliquez sur **[!UICONTROL Sélectionner dans le contenu]** pour sélectionner des ressources (images) dans votre référentiel [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     Pour utiliser des ressources d’un référentiel [!DNL AEM Assets Content Hub] connecté, sélectionnez un référentiel dans le menu déroulant _Location_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des ressources dans la section **[!UICONTROL Sélectionner dans le contenu]** pour charger une ou plusieurs nouvelles ressources.
1. Cliquez sur **[!UICONTROL Utiliser]**.

Lorsque vous avez terminé d’ajouter des paramètres, réduisez le tiroir de l’invite en cliquant de nouveau sur l’icône _Paramètres_ .

## Saisissez une invite

Une fois les instructions sélectionnées, créez une invite à l’aide du langage naturel afin de commencer à générer du contenu pour votre nouvelle expérience d’affichage publicitaire. Pour améliorer la qualité des expériences d’affichage et de description générées, il est essentiel de créer des invites détaillées et descriptives.

![Entrez une invite](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l’écriture d’invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _&quot;Description des expériences que vous souhaitez générer&quot;_.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, une variation (alimentée par l’invite, les directives et le contenu que vous avez ajouté) est générée et affichée dans la zone de travail.

## Modification des publicités affichées générées

Avant de sélectionner les éléments à envoyer pour approbation ou publication sur [!DNL Content], vous pouvez modifier les sections d’affichage d’annonce et les champs de texte, ou supprimer une variante générée.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom de la version préliminaire de l’annonce d’affichage](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez dans le titre _Version préliminaire sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement une publicité display](/help/user-guide/create/manage-variants.md#manually-edit-text)**, double-cliquez dans l’un des champs ou sections de la publicité display (par exemple, la ligne d’objet, l’en-tête ou la copie de corps) et modifiez-la si nécessaire.
* **Pour [modifier la taille et les proportions de la publicité](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, cliquez sur le bouton _[!UICONTROL Redimensionner]_ (case avec une icône de bouton sur le côté gauche de la zone de travail) et sélectionnez une nouvelle taille et un nouveau format à appliquer à toutes les variantes. Les variantes sont dupliquées et redimensionnées.
* **Pour [recadrer ou repositionner des images](/help/user-guide/create/manage-variants.md#crop-assets)**, passez la souris sur l’image, cliquez sur l’icône de recadrage qui s’affiche, puis ajustez la taille et l’emplacement de l’image. Cliquez sur **[!UICONTROL Appliquer]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Commentaires sur la génération d’envoi

Pour [envoyer un commentaire](/help/user-guide/create/manage-variants.md#generation-feedback) sur la qualité de la sortie de génération, cliquez sur l’icône d’options (trois points) et sélectionnez **[!UICONTROL Bonne sortie]** ou **[!UICONTROL Mauvaise sortie]**.

## Vérifier l&#39;alignement des marques

Pour optimiser les publicités générées et garantir une stricte conformité avec l’identité de la marque, tirez parti de la puissance du [_panneau de validation de marque_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel), qui affiche des détails complets sur la validation de la marque et illumine les zones d’amélioration.

**Pour vérifier l’alignement de la marque** :

1. Cliquez sur l’icône Validation de marque dans la barre de menus supérieure pour ouvrir le [_panneau de validation de marque_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel). Vous pouvez afficher les détails des fragments et des directives qui doivent être améliorés.

1. Passez d’une publicité à l’autre pour voir comment améliorer le contenu généré afin d’être plus aligné sur la marque.
1. [Révision manuelle des publicités](#revise-generated-display-ads) pour vous assurer que vos emails sont étroitement alignés sur votre marque.

Voir [Validation de marque](/help/user-guide/guidelines/brand-validation.md).

## Obtention de révisions et d’approbations

Utilisez le panneau Approbations, accessible dans la barre de menus supérieure du Canevas, pour obtenir des révisions, suivre les commentaires de révision et obtenir les approbations des parties prenantes.

**Pour obtenir des révisions et des validations** :

1. [Lancer une demande d’approbation](/help/user-guide/approvals/request-review.md) pour demander une [approbation des expériences de messagerie préliminaires](/help/user-guide/approvals/approve-content.md).
1. [Supprimez ou ajoutez des réviseurs](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et consultez les demandes de révision.
1. Modifiez les brouillons par commentaires de révision et [publiez vos expériences d’affichage et de publicité](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md).

## Expérience Publish et export

Pour rendre les publicités display générées disponibles pour une utilisation actuelle et future, publiez-les sur [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier votre nouvelle expérience d’affichage publicitaire**, cliquez sur **[!UICONTROL Publish]** dans la barre d’outils supérieure ou dans le flux d’approbations.
   1. Sélectionnez _[!UICONTROL [!DNL Campaigns]]_et ajoutez_[!UICONTROL  Plus de détails ]_si vous le souhaitez.
   1. Cliquez sur **[!UICONTROL Publier]**.

      ![Publish a display ad](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Pour exporter votre nouvelle expérience d’affichage publicitaire**, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format JPG uniquement et cliquez sur **[!UICONTROL Exporter]**.

Consultez [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
