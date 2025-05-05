---
title: Générer des images
description: Créez une image correspondant au style d’une image de référence dans Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."
role: User
level: Beginner
recommendations: noDisplay
source-git-commit: 277731aeea966da3cbd1fdabf015bfab3b907d39
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# Générer des images

Avec GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (icône de pinceau), vous pouvez générer des ressources générées par _[!DNL On-brand images]_&#x200B;qui s’inspirent d’une image choisie, en capturant son impact visuel et son esthétique globale.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL On-brand images]_ and _[!DNL Similar images]_. -->

Pour concevoir une image attrayante et efficace, il est recommandé d’[ajouter des instructions à GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) et de consulter les [principes de base de la création d’invites](/help/user-guide/effective-prompts.md).

## Types d’images

Les _[!DNL On-brand images]_&#x200B;sont des ressources générées qui s’inspirent d’une image choisie, en capturant son impact visuel et son esthétique globale. Ces images sont créées à l’aide d’images déjà disponibles dans [!DNL Content] et d’une invite soigneusement conçue qui guide la conception. Ils suivent strictement les directives de la marque et les paramètres choisis au cours du processus de génération.

_[!DNL On-brand images]_<!-- and _[!DNL Similar images]_ --> intégrer des directives, des paramètres et une [invite soigneusement conçue](/help/user-guide/effective-prompts.md) pour offrir des ressources d’images attrayantes.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Générer des images sur la marque

Vous pouvez générer des [!DNL On-brand images] à l’aide de directives, de paramètres et d’une image de référence sélectionnée. Ces éléments, ainsi que votre invite, guident la génération de variations de [!DNL On-brand image] cohérentes.

### Choisir une image de référence

Pour créer une _[!DNL On-brand images]_, sélectionnez une image existante enregistrée dans [!DNL Content]. Voir [ Bonnes pratiques pour les modèles ](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) pour plus d’informations sur les dimensions de [!DNL on-brand image] prises en charge.

**Pour choisir une image de référence** :

1. Dans _[!DNL Create]_, cliquez sur **[!UICONTROL Image de marque]**.
1. Utilisez l’option de recherche adjacente à _Filtrer_ pour rechercher une image spécifique.

   ![Sélectionner l’image de référence](/help/assets/select-img.png){width="400" zoomable="yes"}

   Pour utiliser des ressources à partir d’un référentiel de [!DNL AEM Assets Content Hub] connecté, choisissez un référentiel dans le menu déroulant _Emplacement_. Filtrez et sélectionnez une image.

1. Dans la vue _Sélectionner une image_, cliquez sur une image.

   La taille de l’image sélectionnée peut atteindre 10 Mo.

1. Cliquez sur **[!UICONTROL Utiliser]**.

   La zone de travail, qui sert de hub central pour la création de contenu, s’affiche.

### Ajouter des paramètres

L’intégration de [directives](/help/user-guide/guidelines/overview.md) et de paramètres améliore le processus de génération de contenu et constitue une étape préparatoire cruciale pour la production d’un [!DNL on-brand image].

**Pour ajouter des instructions et des paramètres** :

1. Dans l’onglet _De base_, sélectionnez un [!DNL Brand] pour informer la création de contenu.

   Si aucune marque n’est disponible dans ce menu, [ajoutez des instructions à votre GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Sélectionnez la catégorie d’image qui correspond le mieux au résultat souhaité dans _[!UICONTROL Catégorie d’image]_.

   Les catégories d’images sont disponibles si une [!DNL Brand] a été sélectionnée. Les options sont déterminées par le [!DNL Brand] sélectionné.

<!-- 1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. -->

1. Sélectionnez le format souhaité dans _[!UICONTROL Format]_.
1. Cliquez sur **[!UICONTROL Sélectionner à partir du contenu]** dans _[!UICONTROL Référence de style]_ pour ajouter une image de référence. L’image que vous sélectionnez influence l’esthétique visuelle et la profondeur des images que vous générez.

   Pour utiliser des ressources à partir d’un référentiel de [!DNL AEM Assets Content Hub] connecté, choisissez un référentiel dans le menu déroulant _Emplacement_. Filtrez et sélectionnez une image.

1. Dans l&#39;onglet _Avancé_, sélectionnez le _Type de contenu_.

   Cette option est présélectionnée en fonction de la catégorie d’image présente pour le [!DNL Brand] sélectionné (_Art_ ou _Photo_) et n’est pas modifiable.

1. Ajustez l’intensité globale des caractéristiques visuelles existantes de l’image dans _[!UICONTROL Intensité visuelle]_.

### Saisir une invite

Après avoir sélectionné les paramètres, créez une invite en utilisant le langage naturel pour commencer à générer des images de marque.

Voir [Rédiger des invites efficaces](/help/user-guide/effective-prompts.md).

**Pour saisir une invite** :

1. Entrez une invite dans la zone d&#39;invite.
1. Cliquez sur **[!UICONTROL Générer]**.

Par défaut, quatre variations, alimentées par l’invite, les paramètres et le contenu que vous avez ajouté, sont générées et affichées dans la zone de travail.

### Modifier dans Adobe Express

Après avoir généré des variantes d’image, vous pouvez les modifier directement dans Adobe GenStudio for Performance Marketing à l’aide d’Adobe Express.

**Pour modifier une image individuelle à l’aide d’Adobe Express** :

1. Passez la souris sur une variante d’image générée et cliquez sur _[!UICONTROL Modifier dans Adobe Express]_.

   Une fenêtre _Optimisée par Adobe Express_ s’affiche.

1. Effectuez la modification de l’image, comme [recadrage d’une image](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html), [suppression d’un objet](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html) et application d’effets.

   Consultez la [documentation Adobe Express](https://helpx.adobe.com/express/user-guide.html) pour savoir comment réviser des images dans GenStudio for Performance Marketing avec Adobe Express.

1. Cliquez sur _[!UICONTROL Appliquer les modifications]_ pour enregistrer vos modifications.
1. Continuez à modifier individuellement les variantes d’image selon vos besoins et à appliquer les modifications pour enregistrer votre progression.

### Vérifier l’alignement de la vérification du contenu

Pour optimiser les variantes générées et garantir une stricte conformité à l’identité de la marque, aux directives de la plateforme et aux normes d’accessibilité, tirez parti de la puissance du panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Ce panneau affiche des détails complets de vérification du contenu et illumine les zones d’amélioration.

**Pour effectuer des vérifications de contenu** :

1. Cliquez sur l’icône du panneau _Vérification de contenu_ dans la barre d’actions de droite pour ouvrir le panneau [_Vérification de contenu_](/help/user-guide/guidelines/brand-validation.md#content-check-panel). Affichez un résumé des contrôles *Révision requise* et *Réussite* pour identifier les sections et directives à améliorer.

   ![_Vérification de contenu_ panneau](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Révisez les variantes d’image pour vous assurer que vos variantes sont étroitement alignées avec les contrôles de contenu effectués.

Voir [ Validation de la marque ](/help/user-guide/guidelines/brand-validation.md).

<!-- ## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} -->

## Publication et exportation d’images

Les brouillons d’image générés sont affichés dans la section _Récents_ de la page d’accueil [!DNL Create].

Pour rendre les images générées disponibles pour une utilisation actuelle et future, publiez-les dans [!UICONTROL Contenu] et exportez-les pour les utiliser dans vos campagnes marketing.

1. **Pour publier vos nouvelles images**, cliquez sur **[!UICONTROL Publier]** dans la barre d’outils supérieure.
   1. _[!UICONTROL Ajoutez des détails]_ tels que _[!UICONTROL Campagnes]_ ou _[!UICONTROL Canaux]_, le cas échéant.
   1. Cliquez sur **[!UICONTROL Publier]**.

1. **Pour exporter vos nouvelles images**, cliquez sur **[!UICONTROL Exporter]** dans la barre d’outils supérieure.
   1. Sélectionnez le format (JPG ou PNG), puis cliquez sur **[!UICONTROL Exporter]**.

Consultez [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
