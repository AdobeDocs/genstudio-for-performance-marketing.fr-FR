---
title: Afficher Les Instructions Relatives Aux Modèles Publicitaires
description: Appliquez les bonnes pratiques lors de l’utilisation de modèles d’affichage et de bannières avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
TQID: https://experienceleague.adobe.com/HjkLWiyqK1quHoZB5lEE-qyB3zci12KlRAZC8ME-9Ao
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 4%

---

# Instructions relatives à l’affichage et au modèle de publicité

Les modèles d’affichage sont des mises en page préconçues utilisées pour créer des bannières et des publicités attrayantes. Ils fournissent une structure flexible pour l’intégration d’images, de texte et de call to action, ce qui garantit la cohérence et l’efficacité lors de la production de plusieurs variations d’annonces. Lors de la préparation de votre modèle pour une utilisation dans GenStudio for Performance Marketing, assurez-vous que toutes les ressources sont optimisées pour l’affichage web et répondent aux formats et tailles de fichiers requis.

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles de bannières et d’affichages publicitaires pour les utiliser avec GenStudio for Performance Marketing :

- Utiliser les polices Adobe ou Google.
- Préparation des ressources qui s’affichent correctement dans les dimensions compactes
- Un seul champ d’image est requis
- N’utilisez **** d’images d’arrière-plan incorporées ou codées
- Utilisez des images d’arrière-plan (champ `image`) chargées dans le référentiel de contenu GenStudio for Performance Marketing. Respectez les instructions de la section [Chargement d’images pour les publicités display](#uploading-images-for-display-ads) pour obtenir les meilleurs résultats
- Ne pas utiliser **JavaScript**
- Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle

## Noms de champs reconnus

Lors de la personnalisation de votre bannière ou modèle d’annonce publicitaire, utilisez des espaces réservés de contenu pour les champs obligatoires suivants :

- `headline`
- `sub_headline`
- `body`
- `image` (obligatoire, sélectionné parmi Content JPEG, PNG ou GIF)

GenStudio for Performance Marketing génère automatiquement les champs suivants : Il n’est pas nécessaire d’appliquer des espaces réservés de contenu pour :

- `cta`

Voir [Espaces réservés de contenu](/help/user-guide/templates/customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

## Dimensions prises en charge

Largeur x Hauteur (pixels) doit être défini.

| Orientation | Dimensions (pixels) | Notes |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical | 300 x 600<br>160 x 600 | Commun pour les bannières de gratte-ciel et de demi-page. |
| Horizontal | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Tableau des scores standard, rectangle moyen et tailles de bannière. |
| Valeur personnalisée | 50 x 50 à 2000 x 2000 | Utiliser pour les emplacements non standard ou uniques ; vérifiez les limites de la plateforme. |

