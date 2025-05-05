---
title: Bonnes pratiques relatives aux modèles
description: Appliquez les bonnes pratiques lorsque vous utilisez des modèles avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 0f296fe6ec92178498e2e0eeb3e190a194e46aa0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# Bonnes pratiques relatives à l’utilisation des modèles

Les modèles réduisent considérablement le temps et les efforts nécessaires à la génération d’un nouveau contenu en fournissant un point de départ qui inclut des dispositions préconfigurées et des éléments de conception.

Suivez les recommandations ci-dessous lors de l’utilisation de modèles avec GenStudio for Performance Marketing :

1. En savoir plus sur les [éléments de modèle](#know-about-template-elements)
1. Configurez [directives relatives aux canaux](#configure-channel-guidelines) pour une personnalisation efficace du contenu
1. Concevez avec des [normes d’accessibilité](accessibility-for-templates.md) pour une expérience optimale
1. Suivez les [directives relatives aux modèles spécifiques aux canaux](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Pour en savoir plus sur les éléments et procédures de base des modèles, consultez la section [ Utiliser des modèles ](use-templates.md). Découvrez également en détail [personnalisation d’un modèle](customize-template.md) à utiliser dans votre prochaine campagne.

## Connaître les éléments du modèle

Il est recommandé de vous familiariser avec les parties d’un modèle. Chaque type de modèle utilise différents éléments pour créer une structure pour la création de contenu spécifique au canal. Pour personnaliser votre modèle, utilisez les noms de champ à la place de ces éléments où GenStudio for Performance Marketing doit générer du contenu.

Voir [Éléments de modèle](use-templates.md#template-elements).

## Configurer les instructions relatives aux canaux

Configurez les instructions de canal pour chaque marque avant d’utiliser des modèles dans GenStudio for Performance Marketing. Les recommandations relatives aux canaux influencent directement le type de contenu généré lors de l’utilisation du modèle. Par exemple, vous pouvez définir des limites de caractères pour le corps d’un e-mail.

![Spécifications du corps](/help/assets/channel-email-body.png)

Voir [instructions relatives aux canaux](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Suivre les instructions relatives aux modèles spécifiques aux canaux

Lors de la création de modèles, assurez-vous qu’ils répondent aux exigences spécifiques du canal prévu. Créez des modèles qui s’adaptent à la mise en page et aux exigences visuelles de chaque canal. Des instructions générales s’appliquent à tous les modèles, notamment :

- Utilisation d’HTML et de CSS intégré propres et réactifs
- Utilisation des polices Adobe ou Google
- N’utilisez **&#x200B;**&#x200B;JavaScript

Tenez compte des conseils et contraintes suivants lorsque vous utilisez chaque type de modèle pour garantir des performances et une compatibilité optimales :

>[!BEGINTABS]

>[!TAB E-mail]

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles d’e-mail pour travailler avec GenStudio for Performance Marketing :

- Utilisation des polices Adobe ou Google
- Utilisation d’HTML et de CSS intégré propres et réactifs
- N’utilisez **&#x200B;**&#x200B;JavaScript
- N **utilisez pas** largeur fixe dans le corps ou le conteneur
- N’utilisez **pas** codage base64 pour les images, car il peut augmenter considérablement la taille du modèle

**Contraintes** :

- Utilisation des [sections](customize-template.md#sections-or-groups) :
   - Un modèle de base (une seule section) peut générer un seul ensemble d’éléments de modèle.
   - Un modèle complexe (plusieurs sections) peut générer jusqu’à trois ensembles d’éléments de modèle.
- Le nombre maximal de champs autorisés dans un modèle est de 20
- La taille maximale du fichier HTML est de 102 Ko

**Noms de champs reconnus** :

Pour l’e-mail, le champ `subject` est automatiquement inclus. Utilisez des espaces réservés de contenu pour les champs suivants :

- `pre_header`
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (sélectionné parmi Content JPEG, PNG ou GIF)

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

>[!TAB Méta-annonce]

Suivez ces bonnes pratiques de conception lors de la personnalisation de Métadonnées et de modèles d’annonce publicitaire pour les utiliser avec GenStudio for Performance Marketing :

- Utiliser une largeur de 360 pixels pour les mises en page de colonnes
- Utilisez une résolution minimale de 1 080 x 1 080 pixels pour les images
- N’utilisez **&#x200B;**&#x200B;de taille de police relative
- Ne **pas définir** fenêtre d’affichage
- N’utilisez **&#x200B;**&#x200B;JavaScript
- Ne remplacez **&#x200B;**&#x200B;un élément HTML dans le CSS
- Utiliser la balise `<img>` au lieu de `background-image`
- Utilisez le masquage pour améliorer la lisibilité du texte sur les images d’arrière-plan

**Contraintes** :

- Utilisation des [sections](customize-template.md#sections-or-groups) :
   - Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle.

**proportions prises en charge** :

- Carré 1:1 (1 080 x 1 080 pixels)
- Vertical 4:5 (1 080 x 1 350 pixels)
- Histoire 9:16 (1080 x 1920 pixels)
- Taille d’image personnalisée : (largeur d’image minimale de 50 x 50 pixels)

**Noms de champs reconnus** :

Pour les Méta-publicités, les champs `headline`, `body` et `CTA` sont automatiquement générés. Utilisez des espaces réservés de contenu pour les champs suivants :

- `image` (sélectionné parmi Content JPEG, PNG ou GIF)
- `on_image_text`

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

>[!TAB Bannière et publicité display]

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles de bannières et d’affichages publicitaires pour les utiliser avec GenStudio for Performance Marketing :

- Utilisation des polices Adobe ou Google
- Préparation des ressources qui s’affichent correctement dans les dimensions compactes
- N’utilisez **&#x200B;**&#x200B;d’images d’arrière-plan incorporées ou codées
- Utiliser des images d’arrière-plan (champ `image`) chargées dans le référentiel de contenu GenStudio for Performance Marketing
- N’utilisez **&#x200B;**&#x200B;JavaScript

**Contraintes** :

- Utilisation des [sections](customize-template.md#sections-or-groups) :
   - Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle.

**Dimensions prises en charge** :

- Vertical : (pixels)
   - 300 x 600
   - 160 x 600&#x200B;
- Horizontal : (pixels)
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250&#x200B;
- Personnalisé : (pixels)
   - 50 x 50 à 2000 x 2000

**Noms de champs reconnus** :

Pour les bannières publicitaires et les publicités display, le champ `CTA` est généré automatiquement. Utilisez des espaces réservés de contenu pour les champs suivants :

- `headline`
- `sub_headline`
- `body`
- `image` (sélectionné parmi Content JPEG, PNG ou GIF)

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

>[!TAB Annonce LinkedIn]

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Suivez ces bonnes pratiques de conception lors de la personnalisation des modèles d’annonces LinkedIn pour les utiliser avec GenStudio for Performance Marketing :

**Contraintes** :

- Utilisation des [sections](customize-template.md#sections-or-groups) :
   - Une seule section peut être utilisée, générant un seul ensemble d’éléments de modèle.
- Taille d’image maximale de 5 Mo
- Titre maximal de 70 caractères
- Texte d’introduction maximal de 150 caractères

**proportions prises en charge** :

- Carré 1:1
   - ordinateur de bureau ou mobile
   - Min. : 360 x 360 pixels
   - Maximum : 4 320 x 4 320 pixels
- Horizontal 1,91:1
   - ordinateur de bureau
   - Min. : 640 x 360 pixels
   - Maximum : 7 680 x 4 320 pixels
- Vertical 1:1,91
   - mobile
   - Min. : 360 x 640 pixels
   - Maximum : 2 430 x 4 320 pixels
- Vertical 2.3
   - mobile
   - Min. : 360 x 640 pixels
   - Maximum : 2 430 x 4 320 pixels
- Vertical 4.5 (recommandé)
   - mobile
   - Min. : 360 x 640 pixels
   - Maximum : 2 430 x 4 320 pixels

**Noms de champs reconnus** :

Pour les publicités LinkedIn, les champs `headline`, `introductory_text` et `CTA` sont automatiquement générés. Utilisez des espaces réservés de contenu pour les champs suivants :

- `image` (sélectionné parmi Content JPEG, PNG ou GIF)
- `on_image_text`

Voir [Espaces réservés de contenu](customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

>[!ENDTABS]
