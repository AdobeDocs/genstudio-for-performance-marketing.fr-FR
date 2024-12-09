---
title: Écrire les invites efficaces
description: Découvrez comment écrire des invites efficaces pour Adobe GenStudio for Performance Marketing.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 79430c3279529c4871141489e409240852e1f4fc
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Écrire les invites efficaces

La communication avec l’IA générative est essentielle pour travailler efficacement dans Adobe GenStudio for Performance Marketing.

GenStudio for Performance Marketing fournit une invite d’IA générative chaque fois qu’il est possible de modifier une ressource. Les composants d’une invite efficace doivent inclure un langage descriptif, des exemples et des informations qui ne sont pas fournis par le biais de vos instructions configurées.

En règle générale, fournissez à GenStudio for Performance Marketing des informations sur votre marque en utilisant [des instructions](/help/user-guide/guidelines/overview.md), puis vous pouvez exploiter pleinement l’IA générative pour produire des expériences de contenu alignées sur la marque.

## Langage descriptif

Vous pouvez utiliser un langage naturel pour articuler vos idées pour créer des expériences. Votre invite guide l’IA pour générer du contenu de canal personnalisé et des images qui complètent votre vision. Plus vous fournissez de détails, plus grande est la probabilité de produire une image ou une expérience qui répond à vos besoins. Utilisez un langage clair et descriptif afin de fournir le plus de détails possible :

- Pour **images**, utilisez des mots qui décrivent l’ambiance, l’humeur, la couleur, la composition et le style.
- Pour **copy**, utilisez des mots qui décrivent l’audience, l’objectif, les nouvelles descriptions de fonctionnalités, les exemples et les actions.

Vous trouverez ci-dessous un exemple d’invite qui fournit des informations sur votre intention, votre audience cible et votre style.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Voir les exemples de résultats

![trois emails générés](/help/assets/sample-email.png)

+++

## Critères d’invite

Dans GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md), vous pouvez utiliser les **[!UICONTROL critères d’invite]** ([_Paramètres_](/help/user-guide/create/overview.md#parameters) et une invite) dans le tiroir de l’invite pour ajouter des détails par le biais de la sélection afin d’améliorer l’interprétation de l’IA.

Pour [emails](/help/user-guide/create/email-experiences.md), les critères d’invite peuvent inclure l’ajout de [guidelines](/help/user-guide/guidelines/overview.md) dans _Parameters_, le chargement d’une ressource à utiliser dans les variantes d’email et une invite descriptive. Pour une [méta-publicité](/help/user-guide/create/create-meta-ad.md), les critères d’invite peuvent inclure une ligne directrice de la marque dans _Paramètres_, la sélection ou le chargement d’une ressource existante, des paramètres liés aux images ou aux ressources tels que les proportions et une invite. La puissance réelle commence par [configurer les instructions](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Si des instructions sont ajoutées dans _Parameters_ dans le tiroir de l’invite, vous n’avez pas besoin d’y inclure de référence dans votre invite. GenStudio for Performance Marketing exploite ces [!DNL Brands], [!DNL Products] et [!DNL Personas] dans la génération du contenu.

### Instructions

Les instructions de GenStudio for Performance Marketing aident l’IA générative à personnaliser la composition de vos ressources. Lorsque des critères d’invite s’affichent, vous pouvez choisir un [[!DNL Brand]](/help/user-guide/guidelines/brands.md), un [[!DNL Persona]](/help/user-guide/guidelines/personas.md) et un [[!DNL Product]](/help/user-guide/guidelines/products.md) parmi les instructions que vous avez configurées.

>[!TIP]
>
>Vous contrôlez comment et quand GenStudio for Performance Marketing utilise vos instructions [!DNL Brand]. Voir [Instructions](/help/user-guide/guidelines/overview.md) pour savoir comment configurer et gérer les directives de votre marque.

### Etapes structurées

Pour les emails à plusieurs sections, vous pouvez structurer les invites afin de fournir des instructions spécifiques aux sections afin de générer un contenu variable pour chaque section d’un email. Les invites structurées doivent faire directement référence aux [noms de section dans le modèle d’email](/help/user-guide/content/customize-template.md#sections-or-groups) afin que le contenu généré puisse être inséré dans les espaces réservés de contenu correspondant.

Par exemple, vous pouvez demander à GenStudio for Performance Marketing de générer du contenu pour un email qui promeut un nouveau produit dans la première section et détaille les avantages liés aux économies de coûts dans la seconde section.

L’invite structurée doit :

- Utilisez l’une des références suivantes au nom de la section dans le modèle d’email :
   - Pod
   - Groupe
   - Section
   - Module

  Par exemple, si votre modèle utilise `moduleA` ou `Group-3` comme nom de section, vous pouvez référencer ces noms de section dans l’invite.

- Suivez les règles/structures recommandées. Si la structure de l’invite ne respecte pas le format fourni, l’invite s’applique aux sections d’email *all* et facilite tout de même la génération du contenu.
- Utilisez les noms de section tels que définis dans votre modèle de courrier électronique. Les références d’invite doivent correspondre aux noms de section codés dans votre modèle de courrier électronique.
- Soyez insensible à la casse. Par exemple, vous pouvez utiliser `Pod` ou `pod` dans votre modèle de courrier électronique et une invite structurée.
- Référencez d’abord l’invite utilisateur générique, puis les directives spécifiques à la section.
- Utilisez un deux-points, un trait d’union, une virgule ou une autre démarcation (`,:;#$!~|@=-%&*^_`) comme séparation entre la référence de nom de section et la directive . Par exemple, vous pouvez utiliser ce qui suit comme directive d’invite spécifique à une section : `Pod1; Describe how to easily edit text and swap images.`

Voici un exemple d’invite qui articulera la structure d’invite recommandée et exploite un modèle de courrier électronique qui utilise le terme d’identification `Pod` comme dans `Pod1`, `Pod2` et `Pod3`.

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Voir [Bonnes pratiques pour l’utilisation des modèles](/help/user-guide/content/best-practices-for-templates.md).

## Réessayer

Prompter est un processus itératif. Si les résultats ne répondent pas à vos attentes, passez en revue votre invite et apportez des modifications ou ajoutez des détails supplémentaires. Vous pouvez également coller des sections dans un résumé de campagne. Vous pouvez même demander à GenStudio for Performance Marketing d’éviter certains mots, éléments ou thèmes.

## Bonnes pratiques

Quelques bonnes pratiques simples pour concevoir des invites efficaces :

- Soyez précis et fournissez des détails sur ce qu’il faut faire ou non.
- Fournir du contexte à l’aide de références externes.
- Appliquez les directives de GenStudio for Performance Marketing.
- Examinez et ajustez régulièrement les consignes.
- Itérer et affiner.
- Apprenez par l&#39;expérimentation.

{{in-academy}}
