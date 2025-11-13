---
title: Création d’une expérience publicitaire Meta
description: Découvrez comment créer des expériences publicitaires Meta sur la marque, pour Facebook ou Instagram, avec Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 42111bbf-70cd-4fd2-a7a9-15abe072d720
source-git-commit: 4658a759f5a4e03c54f645cfa1d1bbcc84fe1d91
workflow-type: tm+mt
source-wordcount: '1393'
ht-degree: 0%

---

# Création d’une expérience publicitaire Meta

Ce tutoriel explique comment générer des expériences publicitaires Meta de marque [](/help/user-guide/create/meta-experiences.md) à l’aide de GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau dans la zone de navigation de gauche).

Avant de commencer à générer une expérience publicitaire Meta, il est important d’[incorporer des instructions](/help/user-guide/guidelines/add-guidelines.md) dans GenStudio for Performance Marketing et de vous familiariser avec les principes de base de la [création d’une invite](/help/user-guide/effective-prompts.md).

## Choisir un modèle

Pour commencer à générer une nouvelle expérience publicitaire Meta, utilisez un modèle disponible pour fournir le framework de votre contenu. Consultez les [directives relatives aux modèles de publicité Meta](/help/user-guide/templates/meta-template.md) pour plus d’informations sur les proportions de publicité Meta prises en charge.

Lors de la sélection d’un modèle, vous avez la possibilité d’utiliser l’un des modèles chargés ou un modèle de démarrage.

**Pour choisir un modèle d’annonce Meta** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL Meta ads]**.
1. Sélectionnez **[!UICONTROL Modèles personnalisés]** pour parcourir les modèles chargés ou **[!UICONTROL Modèles de démarrage]** pour parcourir les modèles préconfigurés.

   Si vous prévoyez d’ajouter des ressources vidéo à vos variantes Meta, vous devez choisir un modèle de démarrage. Ils sont préchargés avec des zones de contenu définies par le système qui facilitent l’utilisation des vidéos.

1. Cliquez pour sélectionner un modèle, puis cliquez sur **[!UICONTROL Utiliser]**.

   Cette action ouvre la zone de travail, qui est le centre de création de contenu.

## Ajouter des paramètres

L’ajout de [instructions](/help/user-guide/guidelines/overview.md) et de ressources dans _Paramètres_ dans le tiroir d’invite améliore le processus de génération de contenu et constitue une étape essentielle dans la préparation de la génération d’une publicité Meta.

Si vous utilisez un modèle avec des directives prédéfinies (telles que [!DNL Brands], [!DNL Personas] ou [!DNL Products]), ces directives s’appliquent à vos variantes. Vous pouvez les modifier si vous le souhaitez.

**Pour ajouter des paramètres et des ressources** :

1. Cliquez sur l’icône _Paramètres_ pour développer le tiroir d’invite.
1. Dans la section _Paramètres_, sélectionnez les instructions ([!DNL Brands], [!DNL Personas] et [!DNL Products]) pour informer la création de contenu.

   ![Choisir une persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   Si aucune marque, personnage ou produit n’est disponible à partir de ces menus, [ajoutez des conseils à votre GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Ajoutez du contenu (images ou vidéos) à utiliser dans l’expérience *et* pour influencer la génération de contenu :
   * Cliquez sur **[!UICONTROL Sélectionner dans le contenu]** pour sélectionner des ressources dans votre référentiel de [!DNL Content], filtrer et sélectionner une ou plusieurs images.

     Si vous utilisez un modèle qui comporte une section pour les vidéos, le contenu vidéo (.mp4) sera présélectionné et filtré pour vous. Pointez sur une vidéo pour afficher un aperçu lu automatiquement.

     ![Choisir le contenu visuel](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

     Pour utiliser des ressources à partir d’un référentiel de [!DNL AEM Assets Content Hub] connecté, choisissez un référentiel dans le menu déroulant _Emplacement_. Filtrez et sélectionnez une ou plusieurs images.

   * Vous pouvez également faire glisser et déposer des images dans la section **[!UICONTROL Sélectionner à partir du contenu]** pour charger une ou plusieurs nouvelles ressources.

1. Cliquez sur **[!UICONTROL Utiliser]**.

Lorsque vous avez terminé d&#39;ajouter des paramètres, vous pouvez réduire le tiroir d&#39;invite en cliquant de nouveau sur l&#39;icône _Paramètres_.

## Saisir une invite

Une fois les instructions sélectionnées, créez une invite en langage naturel pour commencer à générer du contenu pour votre nouvelle expérience publicitaire Meta. Les invites détaillées génèrent une sortie de meilleure qualité que les invites vagues ou ambiguës.

Voir [Écrire des invites efficaces](/help/user-guide/effective-prompts.md) pour en savoir plus sur l&#39;écriture d&#39;invites.

**Pour saisir une invite** :

1. Saisissez une invite dans la zone d’invite _« Décrire les expériences que vous souhaitez générer »_.
1. Cliquez sur **[!UICONTROL Générer]**.

   Consultez la section [Gérer les vidéos](#manage-videos) pour comprendre comment elles sont générées et comment les gérer.

Par défaut, quatre variations, toutes alimentées par l’invite, les instructions et le contenu que vous avez ajouté, sont générées et affichées dans la zone de travail.

Le contenu généré se charge progressivement ; au fur et à mesure que chaque section des expériences Meta est générée, elle apparaît dans la zone de travail. Voir [Expériences Meta](/help/user-guide/create/meta-experiences.md#progressive-loading) pour savoir comment ces modifications sont chargées dans la zone de travail.

## Choisir le canal des publicités Meta

Lors de la génération d’une publicité Meta, vous pouvez choisir entre les publicités Facebook ou Instagram.

Dans la barre de menu de droite (icônes Facebook et Instagram **, activez l’option de canal Meta ads, entre** Facebook et **Instagram**, pour afficher et gérer les variantes de chaque canal.

Lors de la [révision des publicités Meta](#revise-generated-variants), vous pouvez modifier le format des publicités Facebook et Instagram.

## Réviser les variantes générées

Avant de sélectionner les éléments à envoyer pour approbation ou publication à [!DNL Content], vous pouvez modifier les annonces Meta ou supprimer une variante de l’ensemble des annonces générées.

Pour mettre en surbrillance un calque individuel à réviser, cliquez sur un champ ou une image modifiable, puis sur _[!UICONTROL Afficher les calques]_.

**Pour réviser les variantes générées** :

* **Pour [modifier le nom du brouillon d’annonce publicitaire Meta](/help/user-guide/create/manage-variants.md#change-draft-name)**, cliquez sur le titre _Brouillon sans titre_ en haut de la zone de travail et saisissez un nouveau titre.
* **Pour [modifier manuellement une publicité Meta](/help/user-guide/create/manage-variants.md#manually-edit-text)**, cliquez sur l’une des sections de publicité (comme l’objet,
en-tête ou copie du corps) et modifiez-les si nécessaire.
* **Pour modifier ou sélectionner le call to action**, cliquez sur le bouton call-to-action , puis sélectionnez l’une des options de texte de bouton disponibles. Dans _Lien_, saisissez l’URL du texte call-to-action.
* **Pour [appliquer une mise en forme de texte](/help/user-guide/create/manage-variants.md#manually-edit-text)** dans une variante, cliquez sur le texte sur l’image ou sur le lien intégré d’une variante, puis cliquez sur **[!UICONTROL Mettre en forme le texte]**.
<!-- **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_. -->
* **Pour [ajouter un lien à une image dans une variante](/help/user-guide/create/manage-variants.md#add-image-link)**, cliquez sur une ressource image (ou dans la zone de ressource image si une image n’existe pas actuellement) et cliquez sur l’icône de lien.
* **Pour [modifier la taille et les proportions de l’annonce](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, cliquez sur le bouton _[!UICONTROL Redimensionner]_ (encadrez-le d’une icône de bouton sur le côté gauche de la zone de travail) et sélectionnez une nouvelle taille et de nouvelles proportions à appliquer à toutes les variantes. Les variantes sont dupliquées et redimensionnées.
* **Pour [régénérer une section d’une variante](/help/user-guide/create/manage-variants.md#re-generate-sections)**, cliquez sur un champ de texte modifiable et utilisez les options _[!UICONTROL Modifications suggérées]_ ou saisissez une nouvelle invite et cliquez sur **[!UICONTROL Générer]**.
* **Pour [ajouter ou permuter des images dans une variante](/help/user-guide/create/manage-variants.md#swap-image)**, cliquez sur une ressource image (ou dans la zone de ressource image si une image n’existe pas actuellement) et cliquez sur l’icône **[!UICONTROL Permuter depuis le contenu]**.
* **Pour [recadrer ou repositionner des images](/help/user-guide/create/manage-variants.md#crop-assets)**, cliquez sur une image, puis sur **[!UICONTROL Modifier]** (icône représentant un crayon) et enfin sur **[!UICONTROL Recadrer]**. Ajustez la taille et l’emplacement de l’image.
* **Pour [utiliser l’option Développement génératif pour dimensionner et ajuster les images](/help/user-guide/create/manage-variants.md#use-generative-expand) à votre modèle de travail**, cliquez sur une image, puis sur **[!UICONTROL Modifier]** (icône en forme de crayon) et **[!UICONTROL Développer]**. Ajustez l’image pour qu’elle s’adapte au format et au modèle nécessaires.
* **Pour [ajouter du texte de remplacement pour les images d’une variante](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, cliquez sur une ressource d’image et utilisez l’option _Texte de remplacement_ pour ajouter ou générer manuellement un texte de remplacement par image.
* **Pour [ajouter des libellés d’accessibilité](/help/user-guide/create/manage-variants.md#add-accessibility-labels) à vos variantes** cliquez sur une image ou un lien call-to-action, puis fournissez une brève description expliquant la fonction du lien ou du bouton.
* **Pour [supprimer une publicité Meta](/help/user-guide/create/manage-variants.md#delete-variant)**, cliquez sur le menu d’options d’une variante et cliquez sur **[!UICONTROL Supprimer la variante]**.

### Gestion des vidéos

Pointez sur chacune des vidéos pour afficher la lecture automatique en boucle.

Les vidéos sont recadrées pour s’adapter aux proportions sélectionnées pendant la génération. Revenez à la vidéo non recadrée d’origine en cliquant sur **[!UICONTROL Recadrer la vidéo]** et en la désactivant.

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

Utilisez le panneau Approbations , accessible sous forme d’icône dans la barre d’actions de droite de la zone de travail, pour obtenir des révisions, suivre les commentaires des révisions et obtenir les approbations des parties prenantes.

**Pour obtenir des examens et des approbations** :

1. [Lancez une demande d’approbation](/help/user-guide/approvals/request-review.md) pour solliciter une [approbation des brouillons d’expériences publicitaires Meta](/help/user-guide/approvals/approve-content.md).

   ![Envoyer des brouillons pour révision et approbation](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Supprimer ou ajouter des réviseurs et réviseuses](/help/user-guide/approvals/review-and-edit.md#manage-approvals) pendant le processus de révision.
1. [Accédez au contenu à réviser](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) et affichez les demandes de révision.
1. Modifiez les brouillons par commentaire de révision et [publiez vos expériences publicitaires Meta](#publish-and-export-experience).

Voir [Révisions et approbations](/help/user-guide/approvals/overview.md) pour plus d’informations.

## Expérience de publication et d’exportation

Pour rendre les annonces Meta générées disponibles pour une utilisation actuelle et future, publiez-les dans [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier vos nouvelles expériences publicitaires Meta** cliquez sur **[!UICONTROL Publier]** dans la barre d’outils supérieure ou dans le flux d’approbations.
1. **Pour exporter vos nouvelles expériences publicitaires Meta** cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (HTML et images ou CSV et images (JPG ou PNG)), puis cliquez sur **[!UICONTROL Exporter]**.

Voir [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) pour plus d’informations.

## Connecter Meta

Vous pouvez connecter GenStudio for Performance Marketing à Meta pour recevoir des analyses avancées et des informations sur les performances du contenu.

Voir [Meta ads connect](/help/user-guide/connectors/meta-ads.md).
