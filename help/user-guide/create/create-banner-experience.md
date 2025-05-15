---
title: Création d’une expérience de bannière
description: Découvrez comment créer des expériences de bannière dans Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c5d541a9-a97b-44da-a15c-61aceefd0e8c
source-git-commit: f49a2bd241f98dda23f6612f8c699ec49d222a12
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 0%

---

# Création d’une expérience de bannière

Ce tutoriel vous explique comment créer des expériences de bannière de marque [banner](banner-experiences.md) à l’aide de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Pour concevoir une expérience de bannière attrayante, il est recommandé d’[ajouter des directives à GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) et de consulter les [principes de base de la rédaction d’invites](/help/user-guide/effective-prompts.md) avant de commencer.

## Choisir un modèle

Pour créer une expérience de bannière, utilisez un modèle disponible pour fournir le framework de votre contenu. Consultez [ Bonnes pratiques pour les modèles ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) pour plus d’informations sur les dimensions de bannière prises en charge.

**Pour choisir un modèle de bannière** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL Bannières]**.
1. Utilisez l’option de recherche adjacente à _Filtrer_ pour rechercher un modèle de bannière spécifique.
1. Dans la vue _Sélectionner un modèle_, cliquez sur un modèle de bannière.
1. Cliquez sur **[!UICONTROL Utiliser]**.

   La zone de travail, qui sert de base à la création de contenu, s’affiche.

## Ajouter des paramètres

L’intégration de [directives](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans le tiroir d’invite améliore le processus de génération de contenu et constitue une étape préparatoire essentielle pour créer une expérience de bannière.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer le tiroir d’invite.
1. Dans la section _Paramètres_, sélectionnez les instructions ([!DNL Brands], [!DNL Personas] et [!DNL Products]) pour informer la création de contenu.

   Si aucune marque, personnage ou produit n’est disponible à partir de ces menus, [ajoutez des conseils à votre GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Pour ajouter du contenu à utiliser dans l’expérience *et* pour influencer la génération de contenu :
   * Cliquez sur **[!UICONTROL Sélectionner à partir du contenu]** pour sélectionner des ressources (images) à partir de votre référentiel [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     Pour utiliser des ressources à partir d’un référentiel de [!DNL AEM Assets Content Hub] connecté, choisissez un référentiel dans le menu déroulant _Emplacement_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des ressources dans la section **[!UICONTROL Sélectionner à partir du contenu]** pour charger une ou plusieurs nouvelles ressources.
1. Cliquez sur **[!UICONTROL Utiliser]**.

Lorsque vous avez terminé d&#39;ajouter des paramètres, réduisez le tiroir d&#39;invite en cliquant de nouveau sur l&#39;icône _Paramètres_.

## Saisir une invite

Une fois que vous avez sélectionné les instructions, utilisez le langage naturel pour créer une invite afin de lancer la génération du contenu pour votre nouvelle expérience de bannière. Pour garantir des résultats de haute qualité, il est essentiel de concevoir des invites détaillées et descriptives.

![Saisissez une invite](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l&#39;écriture d&#39;invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _« Décrire les expériences que vous souhaitez générer »_.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, quatre variantes (alimentées par l’invite, les instructions et le contenu que vous avez ajouté) sont générées et affichées dans la zone de travail.

## Révision des bannières générées

Avant de sélectionner les éléments à envoyer pour approbation ou publication à [!DNL Content], vous pouvez modifier les sections de bannière et les champs de texte, ou supprimer une variante générée.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom du brouillon de bannière](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez dans le titre _Brouillon sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement une bannière](/help/user-guide/create/manage-variants.md#manually-edit-text)**, double-cliquez dans l’une des sections ou l’un des champs de bannière (comme le titre ou le CTA) et effectuez les modifications nécessaires.
* **Pour [régénérer une section d’une variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, cliquez sur un champ de texte modifiable et utilisez les options _[!UICONTROL Modifications suggérées]_ ou saisissez une nouvelle invite dans la section _[!UICONTROL Générer un nouveau texte_ ] puis cliquez sur **[!UICONTROL Générer]**.
* **Pour [ajouter ou permuter des images dans une variante](/help/user-guide/create/manage-variants.md#swap-image)**, cliquez sur une ressource image (ou dans la zone de ressource image si une image n’existe pas actuellement) et cliquez sur l’icône **[!UICONTROL Permuter depuis le contenu]**.
* **Pour [ajouter un lien à une image dans une variante](/help/user-guide/create/manage-variants.md#add-image-link)**, cliquez sur une ressource image (ou dans la zone de ressource image si une image n’existe pas actuellement) et cliquez sur l’icône de lien.
* **Pour [ajouter du texte de remplacement pour les images d’une variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, cliquez sur une ressource d’image et utilisez l’option _Texte de remplacement_ pour ajouter ou générer manuellement un texte de remplacement par image.
* **Pour [modifier la taille et les proportions de l’annonce](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, cliquez sur le bouton _[!UICONTROL Redimensionner]_ (encadrez-le d’une icône de bouton sur le côté gauche de la zone de travail) et sélectionnez une nouvelle taille et de nouvelles proportions à appliquer à toutes les variantes. Les variantes sont dupliquées et redimensionnées.
* **Pour [recadrer ou repositionner des images](/help/user-guide/create/manage-variants.md#crop-assets)**, pointez sur l’image, cliquez sur l’icône de recadrage qui s’affiche, puis ajustez la taille et l’emplacement de l’image. Cliquez sur **[!UICONTROL Appliquer]**.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Envoyer le retour d’informations de génération

Pour [soumettre des commentaires](/help/user-guide/create/manage-variants.md#generation-feedback) sur la qualité de la sortie de génération, cliquez sur l&#39;icône d&#39;options (points de suspension) et sélectionnez **[!UICONTROL Bonne sortie]** ou **[!UICONTROL Mauvaise sortie]**.

## Vérifier l’alignement de la vérification du contenu

Pour optimiser les variantes générées et garantir une stricte conformité à l’identité de la marque, aux directives de la plateforme et aux normes d’accessibilité, tirez parti de la puissance du panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Ce panneau affiche des détails complets de vérification du contenu et illumine les zones d’amélioration.

**Pour effectuer des vérifications de contenu sur une variante** :

1. Cliquez sur l’icône du panneau _Vérification de contenu_ dans la barre d’actions de droite pour ouvrir le panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Affichez un résumé des contrôles _Révision requise_ et _Réussite_ pour identifier les sections et directives à améliorer.

   ![_Vérification de contenu_ panneau](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Révisez manuellement les variantes](#revise-generated-variants) pour vous assurer que vos variantes sont étroitement alignées avec les contrôles de contenu effectués.

Voir [ Validation de la marque ](/help/user-guide/guidelines/brand-validation.md).

## Obtention des révisions et des approbations

Utilisez le panneau _Approbations_, accessible sous forme d’icône dans la barre d’actions de droite de la zone de travail, pour obtenir des révisions, suivre les commentaires des révisions et obtenir les approbations des parties prenantes.

**Pour obtenir des examens et des approbations** :

1. [Lancez une demande d’approbation](/help/user-guide/approvals/request-review.md) pour solliciter une [approbation des brouillons d’expériences de bannière](/help/user-guide/approvals/approve-content.md).
1. [Supprimer ou ajouter des réviseurs et réviseuses](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et affichez les demandes de révision.
1. Modifiez les brouillons par commentaire de révision et [publiez vos expériences de bannière](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md).

## Expérience de publication et d’exportation

Pour rendre les bannières générées disponibles pour une utilisation actuelle et future, publiez-les dans [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier vos nouvelles expériences de bannière**, cliquez sur **[!UICONTROL Publier]** dans la barre d’outils supérieure ou dans le flux d’approbations.
   1. Sélectionnez _[!UICONTROL [!DNL Campaigns]]_et ajoutez_[!UICONTROL  Plus de détails ]_si vous le souhaitez.
   1. Cliquez sur **[!UICONTROL Publier]**.

      ![Publier une bannière](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **Pour exporter vos nouvelles bannières**, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (HTML et images, PNG ou JPG), puis cliquez sur **[!UICONTROL Exporter]**.

      Les HTML exportées doivent être placées dans une propriété web prédéfinie, telle qu’un modèle ou un conteneur `div`. Sans ces dimensions définies, les images peuvent sembler déformées lorsqu’elles sont vues indépendamment.

Consultez [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
