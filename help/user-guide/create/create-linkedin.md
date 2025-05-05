---
title: Création d’une expérience LinkedIn
description: Découvrez comment créer des expériences LinkedIn conformes à la marque avec Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
source-git-commit: d5019f1cdceccb8ce2fdd86c54cf2d36673a90aa
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 0%

---

# Création d’une expérience LinkedIn

Ce tutoriel vous explique comment générer des [expériences LinkedIn](/help/user-guide/create/meta-experiences.md) qui respectent les directives de votre marque à l’aide de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Avant de commencer à générer une publicité LinkedIn, il est important d’[ajouter des instructions](/help/user-guide/guidelines/add-guidelines.md) dans GenStudio for Performance Marketing et d’apprendre les principes de base de la [création d’une invite](/help/user-guide/effective-prompts.md).

## Choisir un modèle

Pour générer une nouvelle expérience LinkedIn, vous avez besoin d’un modèle qui fournit le framework de votre contenu. Voir [Bonnes pratiques pour les modèles](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) pour plus d’informations sur les proportions LinkedIn prises en charge.

**Pour choisir un modèle LinkedIn** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL LinkedIn]**.
1. Utilisez l’option de recherche adjacente à _Filtrer_ pour rechercher un modèle spécifique.
1. Cliquez pour sélectionner un modèle, puis cliquez sur **[!UICONTROL Utiliser]**.

   Cette action ouvre la zone de travail, qui est le centre de création de contenu.

## Ajouter des paramètres

L’ajout de [instructions](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans le tiroir d’invite améliore le processus de génération de contenu et constitue une étape cruciale dans la préparation à la génération d’une expérience LinkedIn.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer le tiroir d’invite.
1. Dans la section _Paramètres_, sélectionnez les instructions ([!DNL Brands], [!DNL Personas] et [!DNL Products]) pour informer la création de contenu.

   ![Choisir une persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Si aucune marque, personnage ou produit n’est disponible à partir de ces menus, [ajoutez des conseils à votre GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Ajoutez du contenu à utiliser dans l’expérience *et* pour influencer la génération de contenu :
   * Cliquez sur **[!UICONTROL Sélectionner à partir du contenu]** pour sélectionner des ressources (images) à partir de votre référentiel [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     ![Choisir le contenu visuel](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Pour utiliser des ressources à partir d’un référentiel de [!DNL AEM Assets Content Hub] connecté, choisissez un référentiel dans le menu déroulant _Emplacement_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des ressources dans la section **[!UICONTROL Sélectionner à partir du contenu]** pour charger une ou plusieurs nouvelles ressources.
1. Cliquez sur **[!UICONTROL Utiliser]**.

Lorsque vous avez terminé d&#39;ajouter des paramètres, vous pouvez réduire le tiroir d&#39;invite en cliquant de nouveau sur l&#39;icône _Paramètres_.

## Saisir une invite

Après avoir sélectionné des instructions, créez une invite en langage naturel pour commencer à générer du contenu pour votre nouvelle expérience LinkedIn. Des invites détaillées garantissent une bonne qualité et une sortie utile.

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l&#39;écriture d&#39;invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _« Décrire les expériences que vous souhaitez générer »_.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, quatre variations, toutes alimentées par l’invite, les instructions et le contenu que vous avez ajouté, sont générées et affichées dans la zone de travail.

Le contenu généré se charge progressivement ; au fur et à mesure que chaque section des expériences LinkedIn est générée, elles apparaissent dans la zone de travail. Consultez [Expériences LinkedIn](/help/user-guide/create/linkedin-experiences.md#progressive-loading) pour savoir comment ces modifications sont chargées dans la zone de travail.

## Réviser les publicités LinkedIn générées

Avant d’envoyer des variantes pour approbation ou publication sur [!DNL Content], vous pouvez modifier les annonces LinkedIn ou supprimer une variante de l’ensemble des annonces générées.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom du brouillon d’annonce LinkedIn](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez sur le titre _Brouillon sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement une publicité LinkedIn](/help/user-guide/create/manage-variants.md#manually-edit-text)**, cliquez sur l’une des sections de la publicité (comme l’objet, l’en-tête ou le corps du texte) et modifiez-la si nécessaire.
* **Pour modifier ou sélectionner l’appel à l’action** cliquez sur le bouton call-to-action et sélectionnez les options de texte du bouton disponibles. Dans _Lien_, saisissez l’URL du texte call-to-action.
* **Pour [régénérer une section d’une variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, cliquez sur un champ de texte modifiable et utilisez les options _[!UICONTROL Modifications suggérées]_ ou saisissez une nouvelle invite dans la section _[!UICONTROL Générer un nouveau texte_ &#x200B;] puis cliquez sur **[!UICONTROL Générer]**.
* **Pour [recadrer ou repositionner des images](/help/user-guide/create/manage-variants.md#crop-assets)**, pointez sur une image, cliquez sur l’icône de recadrage qui s’affiche, puis ajustez la taille et l’emplacement de l’image.
* **Pour [supprimer une publicité LinkedIn](/help/user-guide/create/manage-variants.md#delete-variant)**, cliquez sur le menu d’options d’une variante et cliquez sur **[!UICONTROL Supprimer la variante]**.

## Envoyer le retour d’informations de génération

Pour [soumettre des commentaires](/help/user-guide/create/manage-variants.md#generation-feedback) sur la qualité de la sortie de génération, cliquez sur l&#39;icône d&#39;options (points de suspension) et sélectionnez **[!UICONTROL Bonne sortie]** ou **[!UICONTROL Mauvaise sortie]**.

## Vérifier l’alignement de la vérification du contenu

Pour optimiser les variantes générées et garantir une stricte conformité à l’identité de la marque, aux directives de la plateforme et aux normes d’accessibilité, tirez parti de la puissance du panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Ce panneau affiche des détails complets de vérification du contenu et illumine les zones d’amélioration.

**Pour effectuer des vérifications de contenu sur une variante** :

1. Cliquez sur l’icône du panneau _Vérification de contenu_ dans la barre d’actions de droite pour ouvrir le panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Affichez un résumé des contrôles *Révision requise* et *Réussite* pour identifier les sections et directives à améliorer.

   ![_Vérification de contenu_ panneau](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Révisez manuellement les variantes](#revise-generated-variants) pour vous assurer que vos variantes sont étroitement alignées avec les contrôles de contenu effectués.

Voir [ Validation de la marque ](/help/user-guide/guidelines/brand-validation.md).

## Obtention des révisions et des approbations

Utilisez le panneau Approbations, accessible dans la barre de menu supérieure de la zone de travail, pour obtenir des révisions, suivre les commentaires des révisions et obtenir les approbations des parties prenantes.

**Pour obtenir des examens et des approbations** :

1. [Lancez une demande d’approbation](/help/user-guide/approvals/request-review.md) pour solliciter une [approbation des versions préliminaires des métadonnées et des expériences](/help/user-guide/approvals/approve-content.md).

   ![Envoyer des brouillons pour révision et approbation](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Supprimer ou ajouter des réviseurs et réviseuses](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et affichez les demandes de révision.
1. Modifiez les brouillons par commentaire de révision et [publiez vos Métadonnées et expériences](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md) pour plus d’informations.

## Expérience de publication et d’exportation

Pour rendre les annonces LinkedIn générées disponibles pour une utilisation actuelle et future, publiez-les dans [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier votre ou vos nouvelles expériences)** cliquez sur **[!UICONTROL Publier]** dans la barre d’outils supérieure ou dans le flux d’approbations.
1. **Pour exporter votre ou vos nouvelle(s) expérience(s)**, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (JPG, PNG ou GIF), puis cliquez sur **[!UICONTROL Exporter]**.

Voir [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) pour plus d’informations.
