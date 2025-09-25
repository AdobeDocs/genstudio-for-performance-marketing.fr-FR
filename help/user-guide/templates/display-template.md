---
title: Afficher Les Instructions Relatives Aux Modèles Publicitaires
description: Appliquez les bonnes pratiques lors de l’utilisation de modèles d’affichage et de bannières avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---

# Instructions relatives à l’affichage et au modèle de publicité

Les modèles d’affichage sont des mises en page préconçues utilisées pour créer des bannières et des publicités attrayantes. Ils fournissent une structure flexible pour l’intégration d’images, de texte et de call to action, ce qui garantit la cohérence et l’efficacité lors de la production de plusieurs variations d’annonces. Lors de la préparation de votre modèle pour une utilisation dans GenStudio for Performance Marketing, assurez-vous que toutes les ressources sont optimisées pour l’affichage web et répondent aux formats et tailles de fichiers requis.

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles de bannières et d’affichages publicitaires pour les utiliser avec GenStudio for Performance Marketing :

- Utilisation des polices Adobe ou Google
- Préparation des ressources qui s’affichent correctement dans les dimensions compactes
- Un seul champ d’image est requis
- N’utilisez **&#x200B;**&#x200B;d’images d’arrière-plan incorporées ou codées
- Utiliser des images d’arrière-plan (champ `image`) chargées dans le référentiel de contenu GenStudio for Performance Marketing
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
| Vertical | 300 x 600<br>160 x 600 | Commun pour les bannières de gratte-ciel et de demi-page |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Tableau des scores standard, rectangle moyen et tailles de bannière |
| Valeur personnalisée | 50 x 50 à 2000 x 2000 | Utiliser pour les emplacements non standard ou uniques ; vérifier les limites de la plateforme |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
