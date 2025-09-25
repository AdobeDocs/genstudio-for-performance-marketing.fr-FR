---
title: Bonnes pratiques relatives aux modèles
description: Appliquez les bonnes pratiques lorsque vous utilisez des modèles avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '384'
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

Il est essentiel de définir des directives claires concernant les canaux pour vous assurer que le contenu généré correspond aux exigences et aux objectifs de votre marque. Les instructions de canal vous permettent de spécifier des règles pour des éléments tels que le ton, la longueur et le style utilisés dans votre modèle. Par exemple, vous pouvez définir un nombre maximal de caractères pour le corps du texte ou exiger un style call-to-action spécifique. En définissant ces directives à l’avance, vous réduisez la nécessité d’écrire des instructions détaillées dans chaque invite d’IA, en rationalisant le processus de génération de contenu et en assurant la cohérence entre vos e-mails.

Examinez et définissez les [directives relatives aux canaux](/help/user-guide/guidelines/brands.md#channel-guidelines) de votre marque pour tous les champs clés de votre modèle. Si vous ne définissez pas de directives, les [ directives de canal par défaut](/help/user-guide/guidelines/brands.md#default-channel-guidelines) sont appliquées, ce qui peut ne pas refléter entièrement les exigences de votre marque.

![Spécifications du corps](/help/assets/channel-email-body.png)

Découvrez comment [les directives sur les marques, les produits et les personnes concernées](/help/user-guide/guidelines/overview.md) influencent le contenu généré et comment les adapter à vos objectifs marketing.

## Suivre les instructions relatives aux modèles spécifiques aux canaux

Lors de la création de modèles, assurez-vous qu’ils répondent aux exigences spécifiques du canal prévu. Créez des modèles qui s’adaptent à la mise en page et aux exigences visuelles de chaque canal. Des instructions générales s’appliquent à tous les modèles, notamment :

- Utilisation d’HTML et de CSS intégré propres et réactifs
- Utilisation des polices Adobe ou Google
- N’utilisez **&#x200B;**&#x200B;JavaScript

{{note-css-effects}}

Consultez d’autres conseils et contraintes lorsque vous utilisez chaque type de modèle pour garantir des performances optimales :

- [E-mails](/help/user-guide/templates/email-template.md)
- [Affichage et bannières publicitaires](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Métadonnées publicitaires](/help/user-guide/templates/meta-template.md)
