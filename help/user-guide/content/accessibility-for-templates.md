---
title: Créer des modèles accessibles
description: Créez des modèles dans Adobe GenStudio for Performance Marketing capables d’atteindre un plus grand nombre de votre audience et de fournir une expérience optimale.
feature: Templates, Content
exl-id: eaaa5d9f-ad45-4fd0-826d-c250deb6d238
source-git-commit: cc1d750a8a520c793b1b605747c091f8a5f5e1a2
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Créer des modèles accessibles

Adobe s’engage à fournir une expérience optimale à toutes les audiences. Voir [Initiatives d’accessibilité à l’Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) pour en savoir plus.

Dans GenStudio for Performance Marketing, vous pouvez charger des ressources et des modèles qui permettent la création de contenu pour diverses expériences. Le respect des normes d’accessibilité permet à votre contenu d’atteindre l’audience maximale prévue.

Suivez les recommandations ci-dessous pour préparer vos modèles à l’aide de normes d’accessibilité optimales.

## Texte de remplacement

Fournissez des équivalents textuels pour le contenu non textuel, comme les images.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Collage d&#39;idées, de livres, homme tenant un crayon géant, ordinateur](/help/assets/card-create-assets.png){width="400"}

## Polices

Utilisez des polices faciles à lire. Par exemple, les polices Sans Serif ont un aspect propre, similaire à un bloc, ce qui contribue à une lisibilité plus élevée.

Fournissez un contraste approprié entre le texte et l’arrière-plan. Évitez d’utiliser des couleurs de police qui produisent du texte sombre sur un arrière-plan sombre et du texte clair sur un arrière-plan clair. Tenez compte des consignes de contraste pour obtenir un rapport optimal :

- Texte et images de texte : rapport de contraste d’au moins 4,5:1
- Texte de grande taille et images de texte à grande échelle : rapport de contraste d’au moins 3:1

## Fonction du lien (lien uniquement)

Créez un texte de lien clair qui décrit l’objectif et l’emplacement du lien.

Par exemple, l’utilisation de texte de lien tel que &quot;Cliquez ici&quot; ou &quot;En savoir plus&quot; ne décrit pas clairement l’objectif du lien :

```html
<a href="product-site.html">Click here</a>
```

Il est recommandé d’utiliser un texte qui décrit clairement l’emplacement du lien. Un meilleur exemple peut utiliser le titre de la source du lien et son objectif :

```html
<a href="product-site.html">Explore Product Site</a>
```

## Langue

De nombreux produits et services utilisent la langue de manière créative ou unique. Évitez le jargon, les phrases longues et les expressions complexes. Utilisez un langage clair, concis et facile à lire compatible avec votre audience cible.

- Lorsque cela est possible, utilisez des descriptions claires, des définitions intégrées ou des exemples pertinents. Il peut être difficile de traduire un vernaculaire unique.

- Exprimez ou liez une définition pour les premières instances d’un acronyme ou d’une abréviation. Il peut être difficile de traduire des abréviations.

- Lorsque cela est possible, utilisez des éléments visuels pour compléter du texte ou des idées complexes.
