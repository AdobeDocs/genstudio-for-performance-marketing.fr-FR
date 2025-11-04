---
title: Bonnes pratiques relatives aux modèles
description: Appliquez les bonnes pratiques lorsque vous utilisez des modèles avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
source-git-commit: 3fe6e235b774cf5a99627d981230f96d5e51ac02
workflow-type: tm+mt
source-wordcount: '678'
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
>Pour en savoir plus sur les éléments et procédures de base des modèles, consultez la section [&#x200B; Utiliser des modèles &#x200B;](use-templates.md). Découvrez également en détail [personnalisation d’un modèle](customize-template.md) à utiliser dans votre prochaine campagne.

## Connaître les éléments du modèle

Il est recommandé de vous familiariser avec les parties d’un modèle. Chaque type de modèle utilise différents éléments pour créer une structure pour la création de contenu spécifique au canal. Pour personnaliser votre modèle, utilisez les noms de champ à la place de ces éléments où GenStudio for Performance Marketing doit générer du contenu.

Voir [Éléments de modèle](use-templates.md#template-elements).

## Configurer les instructions relatives aux canaux

Il est essentiel de définir des directives claires concernant les canaux pour vous assurer que le contenu généré correspond aux exigences et aux objectifs de votre marque. Les instructions de canal vous permettent de spécifier des règles pour des éléments tels que le ton, la longueur et le style utilisés dans votre modèle. Par exemple, vous pouvez définir un nombre maximal de caractères pour le corps du texte ou exiger un style call-to-action spécifique. En définissant ces directives à l’avance, vous réduisez la nécessité d’écrire des instructions détaillées dans chaque invite d’IA, en rationalisant le processus de génération de contenu et en assurant la cohérence entre vos e-mails.

Examinez et définissez les [directives relatives aux canaux](/help/user-guide/guidelines/brands.md#channel-guidelines) de votre marque pour tous les champs clés de votre modèle. Si vous ne définissez pas de directives, les [&#x200B; directives de canal par défaut](/help/user-guide/guidelines/brands.md#default-channel-guidelines) sont appliquées, ce qui peut ne pas refléter entièrement les exigences de votre marque.

![Spécifications du corps](/help/assets/channel-email-body.png)

Découvrez comment [les directives sur les marques, les produits et les personnes concernées](/help/user-guide/guidelines/overview.md) influencent le contenu généré et comment les adapter à vos objectifs marketing.

## Chargement des images pour les modèles

Les images utilisées dans les modèles doivent provenir du référentiel de contenu et doivent être chargées correctement pour s’assurer que l’image s’affiche correctement.

Lorsqu’un modèle comporte une image de contour à contour (fond perdu complet), l’image sélectionnée est automatiquement redimensionnée pour s’adapter aux dimensions complètes du modèle. Cependant, si l’image ne correspond pas aux proportions du modèle, elle est recadrée pour s’adapter aux dimensions du modèle et peut ne pas s’afficher comme prévu.

Il n’existe aucune fonctionnalité d’« ajustement automatique » pour les images incluses dans les modèles.

Pour résoudre le recadrage d’image, les utilisateurs doivent définir les proportions de l’image à utiliser dans le modèle lorsqu’il est chargé dans le référentiel de contenu. Lors du chargement d’un modèle approuvé :

1. [Poursuivez le processus de chargement des modèles](/help/user-guide/content/use-templates.md#add-a-template) jusqu’à la page **[!UICONTROL Ajouter des détails]**.

2. Définissez les proportions de l’image à utiliser dans le modèle en **[!UICONTROL Largeur de l’annonce publicitaire (px)]** et **[!UICONTROL Hauteur de l’annonce publicitaire (px)]**. Cette option définit la fenêtre d’image pour la section du modèle qui affiche l’image.

3. Dans la section **[!UICONTROL Plus de détails]**, sélectionnez le menu déroulant **[!UICONTROL Taille de l’image]** et choisissez _Recadrer à une taille fixe_.
   ![Recadré à une taille fixe](./images/crop-to-fixed-size.png "Recadré à une taille fixe"){width="80%"}

Pour déterminer la taille et les proportions d’une image dans le navigateur :

1. Inspectez l’image.
   - Windows/Linux :
      - Appuyez sur F12.
   - MACOS :
      - Appuyez sur Commande + Option + I.

1. Pointez sur l’image.

1. Notez les proportions. Utilisez cette option pour définir les proportions de l’image dans le modèle.

Lorsque ces détails ne sont pas appliqués lors du chargement, l’image est censée correspondre à l’intégralité des proportions du modèle et les images qui ne correspondent pas exactement à ces proportions apparaîtront recadrées.

![Image recadrée dans une publicité affichée](./images/cropped-display.png "Recadrage d’image"){width="60%"}

**❌Image recadrée dans un modèle de publicité display**

![Image affichée dans une publicité affichée](./images/full-fit.png "Image affichée dans une publicité affichée"){width="60%"}

**✅Image entièrement affichée**

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
