---
title: Instructions relatives aux modèles de publicité Meta
description: Appliquez les bonnes pratiques lors de l’utilisation de modèles d’annonces Meta avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
TQID: https://experienceleague.adobe.com/-WHH1xjWFaizXTKjuF-K9UtaR12V3QpMezSqRfwbMIU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 1%

---

# Instructions relatives aux modèles de publicité Meta

Les modèles d’annonces Meta vous permettent de créer des annonces visuellement cohérentes et efficaces sur les plateformes Meta. En suivant les pratiques de conception recommandées et en utilisant les champs pris en charge, vous pouvez vous assurer que vos modèles sont optimisés pour GenStudio for Performance Marketing. Ce guide explique comment structurer, personnaliser et préparer des modèles d’annonce Meta pour une intégration transparente et des résultats performants.

Suivez ces bonnes pratiques de conception lors de la personnalisation des modèles d’annonce publicitaire Meta pour les utiliser avec GenStudio for Performance Marketing :

- Utiliser une largeur de 360 pixels pour les mises en page de colonnes
- Utilisez une résolution minimale de 1 080 x 1 080 pixels pour les images
- Un seul champ d’image est requis
- N’utilisez **&#x200B;**&#x200B;de taille de police relative
- Ne **pas définir** fenêtre d’affichage
- N’utilisez **&#x200B;**&#x200B;JavaScript
- Ne remplacez **&#x200B;**&#x200B;un élément HTML dans le CSS
- Utiliser la balise `<img>` au lieu de `background-image`
- Utilisez le masquage pour améliorer la lisibilité du texte sur les images d’arrière-plan
- Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle

## Noms de champs reconnus

Lors de la personnalisation de votre modèle de publicités Meta, appliquez des espaces réservés de contenu à ces champs obligatoires :

- `image` (obligatoire, sélectionné parmi Content JPEG, PNG ou GIF)
- `on_image_text` (texte qui apparaît sur l’image)

GenStudio for Performance Marketing génère automatiquement les champs suivants : Il n’est pas nécessaire d’appliquer des espaces réservés de contenu pour :

- `headline`
- `body`
- `cta`

Voir [Espaces réservés de contenu](/help/user-guide/templates/customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

## Proportions prises en charge

| Format | Dimensions (pixels) | Notes |
|------------------|----------------------------|-----------------------------------------------------------------------|
| Carré 1:1 | 1080 x 1080 | Standard pour la plupart des emplacements Meta ; recommandé pour une compatibilité étendue. |
| Portrait 4:5 | 1080 x 1350 | Optimisé pour les flux mobiles ; offre plus d’espace vertical. |
| Histoire 9:16 | 1080 x 1920 | Idéal pour les histoires et les rouleaux ; remplit tout l&#39;écran mobile. |
| Paysage 1.91:1 | 1080 x 566 | Idéal pour les annonces de liens et les emplacements de flux d’actualités ; format large. |
| Valeur personnalisée | Minimum 50 x 50 (largeur) | À utiliser uniquement si nécessaire ; peut entraîner un recadrage ou une mise à l’échelle. |

Si la publicité n’est pas conçue dans l’un de ces proportions, GenStudio for Performance Marketing recadre automatiquement l’image à la taille appropriée.

## Exemple de modèle

+++Exemple : modèle d’annonce Meta

<!-- Does this need to be a precise size? -->

Voici un exemple de base de modèle d’annonce Meta. L’en-tête contient le CSS intégré pour la mise en forme. Le corps utilise des [espaces réservés de contenu](#content-placeholders) tels que `image` et `on_image_text`, pour indiquer où GenStudio for Performance Marketing peut générer du contenu.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
