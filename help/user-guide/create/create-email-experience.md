---
title: Créer une expérience d’e-mail
description: Découvrez comment créer des expériences e-mail dans Adobe GenStudio for Performance Marketing.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 4fae540faafdf3f3b32e567e033ea6e8e44ad978
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# Créer une expérience d’e-mail

Ce tutoriel explique comment générer des expériences d’e-mail de marque [expériences](/help/user-guide/create/email-experiences.md) à l’aide de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Pour créer une expérience d’e-mail efficace, il est recommandé d’[ajouter des instructions à GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) et de vous familiariser avec les [principes de base de la conception d’une invite](/help/user-guide/effective-prompts.md) avant de commencer.

## Choisir un modèle

Pour créer une expérience d’e-mail, utilisez un modèle disponible pour fournir le framework de votre contenu.

**Pour choisir un modèle d’e-mail** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL E-mail]**dans le_ « Que souhaitez-vous créer aujourd’hui ? »_section.
1. Utilisez l’option de recherche, adjacente à _Filtrer_, pour rechercher un modèle d’e-mail spécifique.
1. Cliquez pour sélectionner un modèle d’e-mail, puis cliquez sur **[!UICONTROL Utiliser]**.

   La zone de travail, l’épicentre de la création de contenu, s’affiche.

## Ajouter des paramètres

L’ajout de [directives](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans le tiroir d’invite surcharge le processus de génération de contenu et constitue une étape préparatoire intégrale pour la génération d’une expérience d’e-mail.

Si vous utilisez un modèle avec des directives prédéfinies ([!DNL Brands], [!DNL Personas] ou [!DNL Products]), ces directives s’appliquent à vos variantes. Vous pouvez les modifier si vous le souhaitez.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer le tiroir d’invite.
1. Dans la section _Paramètres_, sélectionnez les instructions ([!DNL Brands], [!DNL Personas] et [!DNL Products]) pour informer la création de contenu.

   ![Choisir une persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Si aucune marque, personnage ou produit n’est disponible à partir de ces menus, [ajoutez des conseils à votre GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Ajoutez du contenu à utiliser dans l’expérience *et* pour influencer la génération de contenu :
   * Cliquez sur **[!UICONTROL Sélectionner à partir du contenu]** pour sélectionner des ressources (images) à partir de votre référentiel [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     ![Choisir le contenu visuel](/help/assets/content-select-email.png){width="500" zoomable="yes"}

     Pour utiliser des ressources à partir d’un référentiel de [!DNL AEM Assets Content Hub] connecté, choisissez un référentiel dans le menu déroulant _Emplacement_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des ressources dans la section **[!UICONTROL Sélectionner à partir du contenu]** pour charger une ou plusieurs nouvelles ressources.
1. Cliquez sur **[!UICONTROL Utiliser]**.

   >[!NOTE]
   >Si votre modèle d’e-mail comporte plusieurs sections, sélectionnez [!DNL Products] et contenu (ressources visuelles) pour chaque section d’e-mail dans _E-mails à plusieurs sections_. Les e-mails à plusieurs sections prennent en charge une ressource visuelle par section. Vous pouvez uniquement ajouter des ressources visuelles aux e-mails à plusieurs sections à partir de [!DNL Content]. Vous ne pouvez pas faire glisser ni charger des ressources à partir de votre source locale.
   >![Ajouter du contenu et des paramètres pour chaque section d’e-mail](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

Lorsque vous avez terminé d&#39;ajouter des paramètres, vous pouvez réduire le tiroir d&#39;invite en cliquant de nouveau sur l&#39;icône _Paramètres_.

## Saisir une invite

Une fois les instructions sélectionnées, créez une invite en langage naturel pour commencer à générer du contenu pour votre nouvelle expérience d’e-mail. Les invites détaillées génèrent une sortie de meilleure qualité que les invites vagues ou ambiguës.

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l&#39;écriture d&#39;invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _« Décrire les expériences que vous souhaitez générer »_.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, quatre variations, toutes alimentées par l’invite, les instructions et le contenu que vous avez ajouté, sont générées et affichées dans la zone de travail.

Le contenu généré se charge progressivement ; à mesure que chaque section des expériences e-mail est générée, elles apparaissent dans la zone de travail. Voir [Expériences e-mail](/help/user-guide/create/meta-experiences.md#progressive-loading) pour savoir comment ces modifications sont chargées dans la zone de travail.

## Réviser les variantes générées

Avant de sélectionner les éléments à envoyer pour approbation ou publication à [!DNL Content], vous pouvez modifier les sections d’e-mail ou supprimer une variante de l’ensemble des e-mails générés.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom du brouillon d’e-mail](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez sur le titre _Brouillon sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement un e-mail](/help/user-guide/create/manage-variants.md#manually-edit-text)**, cliquez dans l’un des champs de texte modifiables (comme l’objet, l’en-tête ou la copie du corps) et modifiez-le si nécessaire
* **Pour [modifier ou sélectionner l’appel à l’action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, cliquez sur le bouton d’appel à l’action et sélectionnez _[!UICONTROL Reformuler]_ ou _[!UICONTROL Ajouter un lien]_.
* **Pour [régénérer une section d’une variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, cliquez sur un champ de texte modifiable et utilisez les options _[!UICONTROL Modifications suggérées]_ ou saisissez une nouvelle invite et cliquez sur **[!UICONTROL Générer]**.
* **Pour [ajouter ou permuter des images dans une variante](/help/user-guide/create/manage-variants.md#swap-image)**, cliquez sur une ressource image (ou dans la zone de ressource image si une image n’existe pas actuellement) et cliquez sur l’icône **[!UICONTROL Permuter depuis le contenu]**.
* **Pour [ajouter un lien à une image dans une variante](/help/user-guide/create/manage-variants.md#add-image-link)**, cliquez sur une ressource image (ou dans la zone de ressource image si une image n’existe pas actuellement) et cliquez sur l’icône de lien.
* **Pour [supprimer un e-mail](/help/user-guide/create/manage-variants.md#delete-variant)**, cliquez pour sélectionner le titre de l’e-mail (par exemple, « E-mail 1/4 ») et cliquez sur **[!UICONTROL Supprimer la variante]**.

## Envoyer le retour d’informations de génération

Pour [soumettre des commentaires](/help/user-guide/create/manage-variants.md#generation-feedback) sur la qualité de la sortie de génération, cliquez sur l&#39;icône d&#39;options (points de suspension) et sélectionnez **[!UICONTROL Bonne sortie]** ou **[!UICONTROL Mauvaise sortie]**.

## Aperçu pour l’appareil

Lors de la révision et de la préparation des expériences e-mail, vous pouvez [basculer entre les aperçus pour les vues de bureau et mobile](/help/user-guide/create/manage-variants.md#preview-for-device) afin d’assurer la cohérence et l’attrait visuel des variantes de brouillon.

## Vérifier l’alignement de la vérification du contenu

Pour optimiser les variantes générées et garantir une stricte conformité à l’identité de la marque, aux directives de la plateforme et aux normes d’accessibilité, tirez parti de la puissance du panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Ce panneau affiche des détails complets de vérification du contenu et illumine les zones d’amélioration.

**Pour effectuer des vérifications de contenu sur une variante** :

1. Cliquez sur l’icône du panneau _Vérification de contenu_ dans la barre d’actions de droite pour ouvrir le panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Affichez un résumé des contrôles *Révision requise* et *Réussite* pour identifier les sections et directives à améliorer.

   ![_Vérification de contenu_ panneau](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Révisez manuellement les variantes](#revise-generated-variants) pour vous assurer que vos variantes sont étroitement alignées avec les contrôles de contenu effectués.

Voir [ Validation de la marque ](/help/user-guide/guidelines/brand-validation.md).

## Obtention des révisions et des approbations

Utilisez le panneau Approbations , accessible sous forme d’icône dans la barre d’actions de droite de la zone de travail, pour obtenir des révisions, suivre les commentaires des révisions et obtenir les approbations des parties prenantes.

**Pour obtenir des examens et des approbations** :

1. [Lancez une demande d’approbation](/help/user-guide/approvals/request-review.md) pour solliciter une [approbation des brouillons d’expériences d’e-mail](/help/user-guide/approvals/approve-content.md).
1. [Supprimer ou ajouter des réviseurs et réviseuses](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et affichez les demandes de révision.
1. Modifiez les brouillons par commentaire de révision et [publiez vos expériences e-mail](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md) pour plus d’informations.

## Expérience de publication et d’exportation

Pour rendre les e-mails générés disponibles pour une utilisation actuelle et future, publiez-les dans [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier votre ou vos nouvelles expériences d’e-mail**, cliquez sur **[!UICONTROL Publier]** dans la barre d’outils supérieure ou dans le flux d’approbations.
1. **Pour exporter votre ou vos nouvelle(s) expérience(s)** par e-mail, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (CSV et images ou HTML uniquement), puis cliquez sur **[!UICONTROL Exporter]**.

Voir [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) pour plus d’informations.
