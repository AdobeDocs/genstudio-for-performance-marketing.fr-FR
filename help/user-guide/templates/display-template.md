---
title: Afficher Les Instructions Relatives Aux Modèles Publicitaires
description: Appliquez les bonnes pratiques lors de l’utilisation de modèles d’affichage et de bannières avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: f4bc3442678e6366e185d0c7a91c784d43b8e455
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Instructions relatives à l’affichage et au modèle de publicité

Les modèles d’affichage sont des mises en page préconçues utilisées pour créer des bannières et des publicités attrayantes. Ils fournissent une structure flexible pour l’intégration d’images, de texte et de call to action, ce qui garantit la cohérence et l’efficacité lors de la production de plusieurs variations d’annonces. Lors de la préparation de votre modèle pour une utilisation dans GenStudio for Performance Marketing, assurez-vous que toutes les ressources sont optimisées pour l’affichage web et répondent aux formats et tailles de fichiers requis.

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles de bannières et d’affichages publicitaires pour les utiliser avec GenStudio for Performance Marketing :

- Utilisation des polices Adobe ou Google
- Préparation des ressources qui s’affichent correctement dans les dimensions compactes
- Un seul champ d’image est requis
- N’utilisez **&#x200B;**&#x200B;d’images d’arrière-plan incorporées ou codées
- Utilisez des images d’arrière-plan (champ `image`) chargées dans le référentiel de contenu GenStudio for Performance Marketing. Respectez les instructions de la section [Chargement d’images pour les publicités display](#uploading-images-for-display-ads) pour obtenir les meilleurs résultats
- N’utilisez **&#x200B;**&#x200B;JavaScript
- Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle

## Noms de champs reconnus

Lors de la personnalisation de votre bannière ou modèle d’annonce publicitaire, utilisez des espaces réservés de contenu pour les champs obligatoires suivants :

- `headline`
- `sub_headline`
- `body`
- `image` (obligatoire, sélectionné parmi Content JPEG, PNG ou GIF)

GenStudio for Performance Marketing génère automatiquement les champs suivants : Il n’est pas nécessaire d’appliquer des espaces réservés de contenu pour :

- `cta`

Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

## Dimensions prises en charge

Largeur x Hauteur (pixels) doit être défini.

| Orientation | Dimensions (pixels) | Notes |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical | 300 x 600<br>160 x 600 | Commun pour les bannières de gratte-ciel et de demi-page. |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Tableau des scores standard, rectangle moyen et tailles de bannière. |
| Valeur personnalisée | 50 x 50 à 2000 x 2000 | Utiliser pour les emplacements non standard ou uniques ; vérifiez les limites de la plateforme. |

## Chargement des images pour les publicités display

Les images utilisées dans les publicités doivent provenir du référentiel de contenu et doivent être chargées correctement pour garantir un affichage précis de l’image dans le modèle.

Lorsqu’un modèle d’affichage comporte une image de contour à contour (fond perdu complet), l’image sélectionnée est automatiquement redimensionnée pour s’adapter aux dimensions complètes du modèle. Cependant, si l’image ne correspond pas aux proportions du modèle, elle est recadrée pour s’adapter aux dimensions du modèle et peut ne pas s’afficher comme prévu.

Il n’existe aucune fonctionnalité d’« ajustement automatique » pour les images dans les modèles d’affichage publicitaire.

Pour résoudre le recadrage d’image, les utilisateurs doivent définir les proportions de l’image dans le modèle lorsqu’elle est chargée dans le référentiel de contenu. Lors du chargement d’un modèle de publicité display approuvé :

1. [Poursuivez le processus de chargement des modèles](/help/user-guide/content/use-templates.md#add-a-template) jusqu’à la page **[!UICONTROL Ajouter des détails]**.

1. Définissez les proportions de l’image à utiliser dans le modèle en **[!UICONTROL Largeur de l’annonce publicitaire (px)]** et **[!UICONTROL Hauteur de l’annonce publicitaire (px)]**. Cette option définit la fenêtre d’image pour la section du modèle qui affiche l’image.

1. Dans la section **[!UICONTROL Plus de détails]**, sélectionnez le menu déroulant **[!UICONTROL Taille de l’image]** et choisissez _Recadrer à une taille fixe_.
   ![Recadré à une taille fixe](./crop-to-fixed-size.png "Recadré à une taille fixe"){width="80%"}

Pour déterminer la taille et les proportions d’une image dans le navigateur :

1. Inspectez l’image.
   - Windows/Linux :
      - Appuyez sur F12.
   - MACOS :
      - Appuyez sur Commande + Option + I.

1. Pointez sur l’image.

1. Notez les proportions. Utilisez cette option pour définir les proportions de l’image dans le modèle.

Lorsque ces détails ne sont pas appliqués lors du chargement, l’image est censée correspondre à l’intégralité des proportions du modèle et les images qui ne correspondent pas exactement à ces proportions apparaîtront recadrées.

![Image recadrée dans une publicité affichée](./cropped-display.png "Recadrage d’image"){width="60%"}

**❌Image recadrée dans un modèle de publicité display**

![Image affichée dans une publicité affichée](./full-fit.png "Image affichée dans une publicité affichée"){width="60%"}

**✅Image entièrement affichée**
