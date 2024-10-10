---
title: Création d’une expérience de courrier électronique
description: Découvrez comment créer des expériences par e-mail dans Adobe GenStudio pour le marketing sur les performances.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
source-git-commit: 63d1e568cc265a4aaf98af0a9f3f52ebff2a02b5
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# Création d’une expérience de courrier électronique

Ce tutoriel explique comment générer des [expériences e-mail](/help/user-guide/create/email-experiences.md) de marque à l’aide de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Pour créer une expérience d’e-mail efficace, il est recommandé d’[ ajouter des directives à GenStudio pour le marketing de performances](/help/user-guide/guidelines/add-guidelines.md) et de détailler les [ principes de base de création d’une invite](/help/user-guide/effective-prompts.md) avant de commencer.

## Choisir un modèle

Pour créer une expérience de courrier électronique, utilisez un modèle disponible afin de fournir la structure de votre contenu.

**Pour choisir un modèle d&#39;email** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL Email]**dans le_&quot;Que souhaitez-vous créer aujourd&#39;hui ?&quot;section _.
1. Utilisez l’option de recherche, en regard de _Filtre_, pour trouver un modèle de courrier électronique spécifique.
1. Cliquez pour sélectionner un modèle d&#39;email et cliquez sur **[!UICONTROL Utiliser]**.

   La zone de travail, épicentre de la création de contenu, s’affiche.

## Ajouter des paramètres

L’ajout de [ instructions](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans la zone d’invite surcharge le processus de génération de contenu et est une étape préparatoire intégrale pour générer une expérience de courrier électronique.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer la zone d’invite.
1. Dans la section _Parameters_, sélectionnez des instructions—[!DNL Brands], [!DNL Personas] et [!DNL Products]—pour informer la création de contenu.

   S’il n’existe aucune marque, aucun personnage ou aucun produit disponible dans ces menus, [ ajoutez des instructions à votre GenStudio pour le Marketing des performances](/help/user-guide/guidelines/add-guidelines.md).

1. Ajoutez du contenu à utiliser dans l’expérience *et* pour influencer la génération du contenu :
   * Cliquez sur **[!UICONTROL Sélectionner dans le contenu]** pour sélectionner des ressources (images) dans votre référentiel [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     Pour utiliser des ressources d’un référentiel [!DNL AEM Assets Content Hub] connecté, sélectionnez un référentiel dans le menu déroulant _Location_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des ressources dans la section **[!UICONTROL Sélectionner dans le contenu]** pour charger une ou plusieurs nouvelles ressources.
1. Cliquez sur **[!UICONTROL Utiliser]**.

>[!NOTE]
>
>Si votre modèle de courrier électronique comporte plusieurs sections, sélectionnez [!DNL Products] et contenu (ressources visuelles) pour chaque section d’email dans les _emails à plusieurs sections_. Les emails à plusieurs sections prennent en charge une ressource visuelle par section.

Lorsque vous avez terminé d’ajouter des paramètres, vous pouvez réduire la zone d’invite en cliquant de nouveau sur l’icône _Paramètres_ .

## Saisissez une invite

Une fois les instructions sélectionnées, concevez une invite en utilisant un langage naturel afin de commencer à générer du contenu pour votre nouvelle expérience par e-mail. Les invites détaillées génèrent des résultats de qualité supérieure aux invites vagues ou indescriptives.

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l’écriture d’invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _&quot;Description des expériences que vous souhaitez générer&quot;_.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, quatre variantes, toutes alimentées par l’invite, les directives et le contenu que vous avez ajoutés, sont générées et affichées dans la zone de travail.

Le contenu généré se charge progressivement : à mesure que chaque section des expériences de courrier électronique est générée, elles apparaissent dans la zone de travail. Voir [Expériences par e-mail](/help/user-guide/create/meta-experiences.md#progressive-loading) pour savoir comment ces modifications sont chargées dans la zone de travail.

## Modification des emails générés

Avant de sélectionner les éléments à envoyer pour approbation ou publication sur [!DNL Content], vous pouvez modifier les sections d&#39;email ou supprimer une variante de l&#39;ensemble des emails générés.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom du brouillon de l’email](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez dans le titre _Brouillon sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement un email](/help/user-guide/create/manage-variants.md#manually-edit-text)**, double-cliquez dans l’un des champs de texte modifiables (par exemple, la ligne d’objet, l’en-tête ou la copie de corps) et modifiez-le si nécessaire.
* **Pour [régénérer une section d&#39;une variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, cliquez sur un champ de texte modifiable et utilisez les options _[!UICONTROL Modifications proposées]_ ou saisissez une nouvelle invite et cliquez sur **[!UICONTROL Générer]**.
* **Pour [ajouter ou permuter des images dans une variante](/help/user-guide/create/manage-variants.md#swap-image)**, cliquez sur une ressource image (ou sur la zone de ressource image si aucune image n’existe actuellement) et cliquez sur **[!UICONTROL Sélectionner/permuter à partir du contenu]** ou **[!UICONTROL Télécharger une nouvelle image]** pour ajouter ou permuter une image dans une variante individuelle.
* **Pour [supprimer un email](/help/user-guide/create/manage-variants.md#delete-variant)**, cliquez pour sélectionner le titre de l&#39;email (par exemple, &quot;E-mail 1/4&quot;) et cliquez sur **[!UICONTROL Supprimer la variante]**.

## Commentaires sur la génération d’envoi

Pour [envoyer un commentaire](/help/user-guide/create/manage-variants.md#generation-feedback) sur la qualité de la sortie de génération, cliquez sur l’icône d’options (trois points) et sélectionnez **[!UICONTROL Bonne sortie]** ou **[!UICONTROL Mauvaise sortie]**.

## Aperçu pour le périphérique

Lors de la révision et de la préparation des expériences par e-mail, vous pouvez [ basculer entre les aperçus pour les vues de bureau et mobiles ](/help/user-guide/create/manage-variants.md#preview-for-device) afin d’assurer la cohérence et l’attrait visuel des variantes de brouillons.

## Vérifier l&#39;alignement des marques

Pour optimiser les e-mails générés et garantir une stricte conformité avec l’identité de la marque, utilisez la puissance de la [_vérification des directives sur les marques_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check), ce qui fournit un résumé de l’alignement de la marque pour une variante, et le [_panneau de validation de marque_}, qui affiche des détails complets sur la validation de la marque et éclaire les améliorations.](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)

**Pour vérifier l’alignement de la marque** :

1. Cliquez sur l’icône [**[!UICONTROL [!DNL Brand] de vérification de directives]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) pour une variante et affichez un résumé de son fonctionnement lors de la vérification de votre marque.
1. Pour obtenir les détails des sections et des directives qui doivent être améliorées, cliquez sur **[!UICONTROL Réviser]** _ou_ cliquez sur l’icône Validation de marque dans la barre de menu supérieure pour ouvrir le [_panneau de validation de marque_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel).

1. Passez d’un courrier électronique à l’autre pour voir comment améliorer le contenu généré pour qu’il soit davantage aligné sur la marque.
1. [Révision manuelle des emails](#revise-generated-emails) pour vous assurer que vos emails sont étroitement alignés sur votre marque.

Voir [Validation de marque](/help/user-guide/guidelines/brand-validation.md).

## Obtention de révisions et d’approbations

Utilisez le panneau Approbations, accessible dans la barre de menus supérieure du Canevas, pour obtenir des révisions, suivre les commentaires de révision et obtenir les approbations des parties prenantes.

**Pour obtenir des révisions et des validations** :

1. [Lancer une demande d’approbation](/help/user-guide/approvals/request-review.md) pour demander une [approbation des expériences de messagerie préliminaires](/help/user-guide/approvals/approve-content.md).
1. [Supprimez ou ajoutez des réviseurs](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et consultez les demandes de révision.
1. Modifiez les brouillons par commentaires de révision et [publiez vos expériences de messagerie](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md) pour plus d’informations.

## Expérience Publish et export

Pour rendre les emails générés disponibles pour une utilisation actuelle et future, publiez-les sur [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier votre ou vos nouvelles expériences de messagerie**, cliquez sur **[!UICONTROL Publish]** dans la barre d’outils supérieure ou dans le flux d’approbations.
1. **Pour exporter votre nouvelle expérience de messagerie**, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (CSV et images ou HTML uniquement) et cliquez sur **[!UICONTROL Exporter]**.

Voir [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) pour plus d’informations.
