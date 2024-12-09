---
title: Bonnes pratiques relatives aux modèles
description: Suivez les bonnes pratiques lors de l’utilisation de modèles avec Adobe GenStudio for Performance Marketing.
feature: Templates, Content
last-substantial-update: 2024-12-09T00:00:00Z
source-git-commit: 7ba2ecfbdd6853934be5210685bf447848715d28
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Bonnes pratiques relatives à l’utilisation des modèles

Les modèles réduisent considérablement le temps et les efforts nécessaires à la génération d’un nouveau contenu en fournissant un point de départ qui inclut des mises en page préconfigurées et des éléments de conception.

Suivez les recommandations suivantes lorsque vous utilisez des modèles avec GenStudio for Performance Marketing :

1. Connaître [les éléments de modèle](#know-about-template-elements)
1. Configurez les [directives de canal](#configure-channel-guidelines) pour une personnalisation efficace du contenu
1. Conception avec des [normes d’accessibilité](accessibility-for-templates.md) pour une expérience optimale
1. Suivez les [ instructions de modèle spécifiques au canal ](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Pour en savoir plus sur les éléments et les procédures de base des modèles, voir [Utilisation des modèles](use-templates.md). Découvrez également comment [personnaliser un modèle](customize-template.md) pour l’utiliser dans votre campagne suivante.

## Connaître les éléments de modèle

Il est recommandé de se familiariser avec les parties d’un modèle. Chaque type de modèle utilise différents éléments pour créer une structure pour la création de contenu spécifique au canal. Pour personnaliser votre modèle, utilisez les noms de champ à la place de ces éléments dans lesquels vous avez besoin de GenStudio for Performance Marketing pour générer du contenu.

Voir [Eléments de modèle](use-templates.md#template-elements).

## Configuration des directives de canal

Configurez les directives de canal pour chaque marque avant d’utiliser des modèles dans GenStudio for Performance Marketing. Les directives de canal influent directement sur le type de contenu généré lors de l’utilisation du modèle. Par exemple, vous pouvez définir des limites de caractères sur le corps d’un email.

![Spécifications du corps](/help/assets/channel-email-body.png)

Voir [directives sur les canaux](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Suivez les directives relatives aux modèles spécifiques aux canaux.

Créez des modèles adaptés à la mise en page et aux exigences visuelles de chaque canal. Tenez compte des conseils et contraintes suivants lorsque vous utilisez chaque type de modèle afin d’optimiser les performances et la compatibilité :

>[!BEGINTABS]

>[!TAB E-mail]

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles d’email pour travailler avec GenStudio for Performance Marketing :

- Utilisation de polices Adobe ou Google
- Utilisation d’un HTML propre et réactif et d’une page CSS intégrée
- N’utilisez pas **not** JavaScript
- **not** utilisez une largeur fixe dans le corps ou le conteneur
- N’utilisez pas **le codage base64 pour les images, car cela peut augmenter considérablement la taille du modèle.**

**Contraintes** :

- Utilisation de [sections](customize-template.md#sections-or-groups) :
   - Un modèle de base (une seule section) peut générer un seul ensemble d’éléments de modèle.
   - Un modèle complexe (plusieurs sections) peut générer jusqu’à trois ensembles d’éléments de modèle.
- Le nombre maximal de champs autorisés dans un modèle est de 20.
- La taille maximale du fichier d’HTML est de 102 Ko.

**Noms de champ reconnus** :

Pour le courrier électronique, le champ `subject` est automatiquement inclus. Utilisez des espaces réservés au contenu pour les champs suivants :

- `pre_header`
- `headline`
- `body`
- `cta`
- `image` (sélectionné à partir du contenu)
- `brand_logo`

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation des noms de champ dans les modèles.

>[!TAB Métadonnées ]

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles de métadonnées publicitaires pour travailler avec GenStudio for Performance Marketing :

- Utiliser une largeur de 360 pixels pour les dispositions en colonnes
- Utiliser une résolution minimale de 1 080 x 1 080 pixels pour les images
- **not** utilisent-ils la taille de police relative ?
- Ne **not** définissez pas les fenêtres d’affichage
- N’utilisez pas **not** JavaScript
- Ne remplacez pas **not** un élément HTML dans le CSS
- Utilisez les paramètres suivants pour les images d’arrière-plan :

  Ajoutez la valeur `object-fit: cover` à la classe CSS `background-image` :

  ```css
  .background-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  ```

**Contraintes** :

- Utilisation de [sections](customize-template.md#sections-or-groups) :
   - Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle.

**Formats pris en charge** :

- Carré 1:1 (1 080 x 1 080 pixels)
- 4:5 vertical (1 080 x 1 350 pixels)
- Article 9:16 (1 080 x 1 920 pixels)

**Noms de champ reconnus** :

Pour les métadonnées publicitaires, les champs `headline`, `body` et `CTA` sont générés automatiquement. Utilisez des espaces réservés au contenu pour les champs suivants :

- `image` (sélectionné à partir du contenu)
- `on-image-text`
- `brand_logo`

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation des noms de champ dans les modèles.

>[!TAB Publicité d’affichage]

Suivez les bonnes pratiques de conception suivantes lorsque vous personnalisez des modèles d’annonce d’affichage pour qu’ils fonctionnent avec GenStudio for Performance Marketing :

- Utilisation de polices Adobe ou Google
- Préparation des ressources qui s’affichent bien dans des dimensions minces
- N’utilisez **pas** d’images d’arrière-plan incorporées ou codées.
- Utiliser des images d’arrière-plan (`image` champ) chargées dans le référentiel de contenu GenStudio for Performance Marketing
- N’utilisez pas **not** JavaScript

**Contraintes** :

- Utilisation de [sections](customize-template.md#sections-or-groups) :
   - Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle.

**Dimensions prises en charge** :

- Vertical : (pixels)
   - 300 x 600
   - 160 x 600 &#x200B;
- Horizontal : (pixels)
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250 &#x200B;

**Noms de champ reconnus** :

Utilisez des espaces réservés au contenu pour les champs suivants :

- `headline`
- `body`
- `cta`
- `image` (sélectionné à partir du contenu)

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation des noms de champ dans les modèles.

>[!ENDTABS]
