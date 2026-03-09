---
title: Créer des modèles accessibles
description: Créez des modèles dans Adobe GenStudio for Performance Marketing capables d’atteindre une plus grande partie de votre audience et de fournir une expérience optimale.
feature: Media Templates
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
TQID: https://experienceleague.adobe.com/b56YHJsOAunGenV-F3u7Y2mo56f6CnnX4qPXyzczPJY
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 369
ht-degree: 0%

---

# Créer des modèles accessibles

Adobe s’engage à fournir une expérience optimale à toutes les audiences. Consultez [&#x200B; Initiatives en matière d’accessibilité dans Adobe &#x200B;](https://www.adobe.com/trust/accessibility/initiatives.html) pour plus de détails.

Dans GenStudio for Performance Marketing, vous pouvez charger des ressources et des modèles qui permettent de créer du contenu pour diverses expériences. Le respect des normes d’accessibilité permet à votre contenu d’atteindre votre audience maximale prévue.

Suivez les recommandations suivantes pour préparer vos modèles à l’aide des normes d’accessibilité optimales.

## Texte secondaire

Proposez des alternatives textuelles pour le contenu non textuel, tel que des images.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Collage d&#39;idées, livres, homme tenant crayon géant, ordinateur](/help/assets/card-create-assets.png){width="400"}

Lors de la personnalisation de votre modèle, utilisez des espaces réservés de contenu pour les attributs `alt` et `aria-label` :

- [Texte secondaire](/help/user-guide/templates/customize-template.md#alternative-text)
- [Libellé d’accessibilité](/help/user-guide/templates/customize-template.md#accessibility-label)

## Polices

Utilisez des polices faciles à lire. Par exemple, les polices Sans Serif ont propres et ressemblent à des blocs, ce qui contribue à une meilleure lisibilité.

Fournissez un contraste approprié entre le texte et l’arrière-plan. Évitez d’utiliser des couleurs de police qui produisent du texte sombre sur un arrière-plan sombre et du texte clair sur un arrière-plan clair. Appliquez les règles de contraste pour obtenir un rapport optimal :

- Texte et images du texte : rapport de contraste d’au moins 4,5:1
- Texte grand format et images de texte à grande échelle : rapport de contraste d’au moins 3:1

## Fonction du lien (lien uniquement)

Créez un texte de lien clair qui décrit l’objectif et l’emplacement du lien.

Par exemple, l’utilisation de texte de lien tel que « Cliquez ici » ou « En savoir plus » ne décrit pas clairement l’objectif du lien :

```html
<a href="product-site.html">Click here</a>
```

Il est recommandé d’utiliser un texte qui décrit clairement où va le lien. Un meilleur exemple pourrait utiliser le titre de la source du lien et l’objectif :

```html
<a href="product-site.html">Explore Product Site</a>
```

## Langue

De nombreux produits et services utilisent le langage de manière créative ou unique. Évitez le jargon, les phrases longues et les expressions complexes. Utilisez un langage clair, concis et facile à lire, compatible avec votre audience cible.

- Utilisez des descriptions claires, des définitions intégrées ou des exemples connexes lorsque cela est possible. Il peut être difficile de traduire un langage vernaculaire unique.

- Écrivez ou liez vers une définition pour les premières instances d’un acronyme ou d’une abréviation. Il peut être difficile de traduire des abréviations.

- Dans la mesure du possible, utilisez des éléments visuels pour compléter du texte ou des idées complexes.
