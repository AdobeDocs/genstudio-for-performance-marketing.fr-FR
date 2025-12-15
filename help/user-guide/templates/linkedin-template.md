---
title: Instructions relatives aux modèles LinkedIn
description: Appliquez les bonnes pratiques lors de l’utilisation de modèles LinkedIn avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 85432185-8311-411b-b57b-f482c3d45854
source-git-commit: ff694925dea4741d13ae71a68e23a5e604134521
workflow-type: tm+mt
source-wordcount: '287'
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
| Horizontal 1,91:1 | Ordinateur de bureau | 1200 x 628 | Format paysage standard. Généralement utilisé pour le contenu sponsorisé et les annonces de flux d’actualités. |
| Vertical 1:1,91 | Mobile | 1 200 x 2 292 | Format vertical élevé. Optimisé pour l’affichage mobile, offrant une présence accrue sur l’écran. |
| Vertical 2:3 | Mobile | 1 200 x 1 800 | Légèrement moins haut que 1:1,91. Idéal pour les campagnes mobiles-first. |
| Vertical 4:5 | Mobile | 1 200 x 1 500 | Recommandé pour mobile. Équilibre visibilité et contenu, ce qui a souvent un impact plus important. |

<!-- Potentially add an example

## Template example

+++Example: LinkedIn template

+++

-->
