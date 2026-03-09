---
title: Instructions relatives aux modèles LinkedIn
description: Appliquez les bonnes pratiques lors de l’utilisation de modèles LinkedIn avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
TQID: https://experienceleague.adobe.com/YyG3WuMkdVAaACX03qLKzzw-fFA3WfT9K2ohjnQNPcI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 287
ht-degree: 2%

---

# Instructions relatives aux modèles LinkedIn

Les modèles LinkedIn fournissent un moyen structuré de créer et de personnaliser des contenus publicitaires pour les campagnes LinkedIn. Ces directives garantissent que vos publicités répondent aux spécifications de LinkedIn tout en rationalisant le processus de création dans GenStudio for Performance Marketing. Ce guide vous aide à vous préparer à une valorisation de marque cohérente et à des performances efficaces sur les plateformes de bureau et mobiles de LinkedIn.

Suivez ces bonnes pratiques de conception lors de la personnalisation des modèles d’annonces LinkedIn pour les utiliser avec GenStudio for Performance Marketing :

- Un seul champ d’image est requis
- Taille d’image maximale de 5 Mo
- Titre maximal de 70 caractères
- Texte d’introduction maximal de 150 caractères
- Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle

## Noms de champs reconnus

Lors de la personnalisation de votre modèle LinkedIn, appliquez des espaces réservés de contenu à ces champs obligatoires :

- `image` (obligatoire, sélectionné parmi Content JPEG, PNG ou GIF)
- `on_image_text` (texte qui apparaît sur l’image)

GenStudio for Performance Marketing génère automatiquement les champs suivants : Il n’est pas nécessaire d’appliquer des espaces réservés de contenu pour :

- `headline`
- `introductory_text`
- `cta` (Call to action)

Voir [Espaces réservés de contenu](/help/user-guide/templates/customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

## Proportions prises en charge

Toutes les largeurs du modèle LinkedIn sont codées en dur à 1 200 pixels.

| Format | Plateforme | Dimensions (px) | Notes |
|-------------------|-----------------|------------|-------------------------------------------------------------------------------------|
| Carré 1:1 | Ordinateur de bureau, mobile | 1 200 x 1 200 | Le plus polyvalent. Idéal pour un aspect cohérent sur tous les appareils et emplacements. |
| Horizontal 1,91:1 | Poste de travail | 1200 x 628 | Format paysage standard. Généralement utilisé pour le contenu sponsorisé et les annonces de flux d’actualités. |
| Vertical 1:1,91 | Mobile | 1 200 x 2 292 | Format vertical élevé. Optimisé pour l’affichage mobile, offrant une présence accrue sur l’écran. |
| Vertical 2:3 | Mobile | 1 200 x 1 800 | Légèrement moins haut que 1:1,91. Idéal pour les campagnes mobiles-first. |
| Vertical 4:5 | Mobile | 1 200 x 1 500 | Recommandé pour mobile. Équilibre visibilité et contenu, ce qui a souvent un impact plus important. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
