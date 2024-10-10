---
title: Création d’une expérience de métadonnées publicitaires
description: Découvrez comment créer des expériences de métadonnées de marque (pour Facebook ou Instagram) avec Adobe GenStudio pour le marketing de performances.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 63d1e568cc265a4aaf98af0a9f3f52ebff2a02b5
workflow-type: tm+mt
source-wordcount: '1016'
ht-degree: 0%

---

# Création d’une expérience de métadonnées publicitaires

Ce tutoriel explique comment générer des [expériences de métadonnées](/help/user-guide/create/meta-experiences.md) de marque à l’aide de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Avant de commencer à générer une expérience de métadonnées publicitaires, il est important d’ [incorporer des instructions](/help/user-guide/guidelines/add-guidelines.md) dans GenStudio pour le marketing sur les performances et de vous familiariser avec les principes de base de la [création d’une invite](/help/user-guide/effective-prompts.md).

## Choisir un modèle

Pour commencer à générer une nouvelle expérience de métadonnées publicitaires, utilisez un modèle disponible afin de fournir la structure de votre contenu.

**Pour choisir un modèle de métadonnées publicitaires** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL Métadonnées]**dans le_&quot;Que souhaitez-vous créer aujourd’hui ?&quot;section _.
1. Utilisez l’option de recherche, en regard de _Filtre_, pour trouver un modèle de métadonnées de publicité spécifique.
1. Cliquez pour sélectionner un modèle et cliquez sur **[!UICONTROL Utiliser]**.

   Cette action ouvre le canevas, qui est le centre central de la création de contenu.

## Ajouter des paramètres

L’ajout de [lignes directrices](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans la zone d’invite améliore le processus de génération de contenu et est une étape essentielle dans la préparation de la génération d’une méta-publicité.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer la zone d’invite.
1. Dans la section _Parameters_, sélectionnez des instructions—[!DNL Brands], [!DNL Personas] et [!DNL Products]—pour informer la création de contenu.

   S’il n’existe aucune marque, aucun personnage ou aucun produit disponible dans ces menus, [ ajoutez des instructions à votre GenStudio pour le Marketing des performances](/help/user-guide/guidelines/add-guidelines.md).

1. Ajoutez du contenu à utiliser dans l’expérience *et* pour influencer la génération du contenu :
   * Cliquez sur **[!UICONTROL Sélectionner dans le contenu]** pour sélectionner des ressources (images) dans votre référentiel [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     Pour utiliser des ressources d’un référentiel [!DNL AEM Assets Content Hub] connecté, sélectionnez un référentiel dans le menu déroulant _Location_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des ressources dans la section **[!UICONTROL Sélectionner dans le contenu]** pour charger une ou plusieurs nouvelles ressources.
1. Cliquez sur **[!UICONTROL Utiliser]**.

Lorsque vous avez terminé d’ajouter des paramètres, vous pouvez réduire la zone d’invite en cliquant de nouveau sur l’icône _Paramètres_ .

## Saisissez une invite

Une fois les instructions sélectionnées, créez une invite à l’aide du langage naturel afin de commencer à générer du contenu pour votre nouvelle expérience de métadonnées publicitaires. Les invites détaillées génèrent des résultats de qualité supérieure aux invites vagues ou indescriptives.

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l’écriture d’invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _&quot;Description des expériences que vous souhaitez générer&quot;_.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, quatre variantes, toutes alimentées par l’invite, les directives et le contenu que vous avez ajoutés, sont générées et affichées dans la zone de travail.

Le contenu généré se charge progressivement : à mesure que chaque section des expériences de métadonnées est générée, elles apparaissent dans la zone de travail. Voir [Métadonnées des expériences](/help/user-guide/create/meta-experiences.md#progressive-loading) pour savoir comment ces modifications sont chargées dans la zone de travail.

## Choisir le canal Métadonnées

Lors de la génération d’une méta-publicité, vous pouvez choisir entre les publicités Facebook ou Instagram.

Activez l’option de canal Métadonnées (entre **Facebook** et **Instagram**) dans la barre de menu de droite (icônes Facebook et Instagram) pour afficher et gérer les variantes de chaque canal.

Lors de la [révision des métadonnées publicitaires](#revise-generated-meta-ads), vous pouvez modifier les proportions des publicités Facebook et Instagram.

## Modification des métadonnées générées

Avant de sélectionner les éléments à envoyer pour approbation ou publication sur [!DNL Content], vous pouvez modifier les Métadonnées ou supprimer une variante de l’ensemble de publicités générées.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom de la version préliminaire de la méta-publicité](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez dans le titre _Brouillon sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement une méta-publicité](/help/user-guide/create/manage-variants.md#manually-edit-text)**, double-cliquez dans l’une des sections de publicité (par exemple, la ligne d’objet),
en-tête ou copie du corps) et modifiez-la selon vos besoins.
* **Pour modifier ou sélectionner l’appel à l’action**, cliquez sur le bouton d’appel à l’action et sélectionnez l’une des options de texte de bouton disponibles. Dans _[!UICONTROL Lien]_, saisissez une URL pour le texte d’appel à l’action.
* **Pour [régénérer une section d&#39;une variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, cliquez sur un champ de texte modifiable et utilisez les options _[!UICONTROL Modifications proposées]_ ou saisissez une nouvelle invite et cliquez sur **[!UICONTROL Générer]**.
* **Pour [recadrer ou repositionner des images](/help/user-guide/create/manage-variants.md#crop-assets)**, passez la souris sur une image, cliquez sur l’icône de recadrage qui s’affiche, puis ajustez la taille et l’emplacement de l’image.
* **Pour [supprimer une méta-publicité](/help/user-guide/create/manage-variants.md#delete-variant)**, cliquez sur le titre de la publicité (par exemple, &quot;Meta 4&quot;) et cliquez sur **[!UICONTROL Supprimer la variante]**.

## Commentaires sur la génération d’envoi

Pour [envoyer un commentaire](/help/user-guide/create/manage-variants.md#generation-feedback) sur la qualité de la sortie de génération, cliquez sur l’icône d’options (trois points) et sélectionnez **[!UICONTROL Bonne sortie]** ou **[!UICONTROL Mauvaise sortie]**.

## Vérifier l&#39;alignement des marques

Pour optimiser les publicités générées et garantir une stricte conformité avec l’identité de la marque, tirez parti de la puissance de la [_vérification des directives sur la marque_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check), qui fournit un résumé de l’alignement de la marque pour une variante, et du [_panneau de validation de marque_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel), qui affiche des détails complets sur la validation de la marque et éclaire les améliorations.

**Pour vérifier l’alignement de la marque** :

1. Cliquez sur l’icône [**[!UICONTROL [!DNL Brand] de vérification de directives]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) pour une variante et affichez un résumé de son fonctionnement lors de la vérification de votre marque.
1. Pour obtenir les détails des sections et des directives qui doivent être améliorées, cliquez sur **[!UICONTROL Réviser]** _ou_ cliquez sur l’icône Validation de marque dans la barre de menu supérieure pour ouvrir le [_panneau de validation de marque_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel).

1. Passez d’une publicité à l’autre pour voir comment améliorer le contenu généré afin d’être plus aligné sur la marque.
1. [Révision manuelle des publicités](#revise-generated-meta-ads) pour vous assurer que vos publicités sont étroitement alignées sur votre marque.

Voir [Validation de marque](/help/user-guide/guidelines/brand-validation.md).

## Obtention de révisions et d’approbations

Utilisez le panneau Approbations, accessible dans la barre de menus supérieure du Canevas, pour obtenir des révisions, suivre les commentaires de révision et obtenir les approbations des parties prenantes.

**Pour obtenir des révisions et des validations** :

1. [Lancer une demande d’approbation](/help/user-guide/approvals/request-review.md) pour demander une [approbation des expériences de métadonnées préliminaires](/help/user-guide/approvals/approve-content.md).
1. [Supprimez ou ajoutez des réviseurs](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et consultez les demandes de révision.
1. Modifiez les brouillons par commentaires de révision et [publiez vos expériences de métadonnées publicitaires](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md) pour plus d’informations.

## Expérience Publish et export

Pour rendre les métadonnées générées disponibles pour une utilisation actuelle et future, publiez-les sur [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier votre nouvelle expérience de métadonnées publicitaires**, cliquez sur **[!UICONTROL Publish]** dans la barre d’outils supérieure ou dans le flux d’approbations.
1. **Pour exporter vos nouvelles expériences de métadonnées publicitaires**, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (CSV et images ou HTML uniquement) et cliquez sur **[!UICONTROL Exporter]**.

Voir [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) pour plus d’informations.

## Connect Meta

Vous pouvez connecter GenStudio for Performance Marketing à Meta afin de recevoir des analyses avancées et des [insights](/help/user-guide/insights/overview.md) sur les performances du contenu.

Pour plus d’informations, voir [Connexion au compte de canal](/help/user-guide/insights/connect-channel.md) .
