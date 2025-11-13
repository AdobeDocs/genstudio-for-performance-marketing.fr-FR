---
title: Écrire des invites efficaces
description: Découvrez comment écrire des prompts efficaces pour Adobe GenStudio for Performance Marketing.
role: User
level: Beginner
feature: Create Prompt, Generative AI
exl-id: 0cd4db4f-d031-4c1f-a4e7-adc220f947fc
source-git-commit: 299ebb88cb1e2b25580151b7620eafc0e59224d0
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 2%

---

# Écrire des invites efficaces

La communication avec l’IA générative est essentielle pour travailler efficacement dans Adobe GenStudio for Performance Marketing.

GenStudio for Performance Marketing fournit une invite d’IA générative chaque fois qu’il est possible de modifier une ressource. Les composants d’une invite efficace doivent inclure un langage descriptif, des exemples et des informations qui ne sont pas fournis dans vos directives configurées.

Il est recommandé de fournir à GenStudio for Performance Marketing vos informations de marque à l’aide de [directives](/help/user-guide/guidelines/overview.md), puis d’exploiter pleinement l’IA générative pour produire des expériences de contenu alignées sur la marque.

## Langage descriptif

Vous pouvez utiliser le langage naturel pour articuler vos idées afin de créer des expériences. Votre invite guide l’IA pour générer le contenu de canal personnalisé et les images qui complètent votre vision. Plus vous fournissez de détails, plus vous avez de chances de produire une image ou une expérience qui répond à vos besoins. Utilisez un langage clair et descriptif pour fournir autant de détails que possible :

- Pour **images**, utilisez des mots qui décrivent l’ambiance, l’humeur, la couleur, la composition et le style.
- Pour **copier**, utilisez des mots qui décrivent l’audience, l’objectif, les nouvelles descriptions de fonctionnalités, les exemples et les actions.

Voici un exemple d’invite qui articule des informations sur votre intention, l’audience cible et le style.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Voir les exemples de résultats

![trois emails générés](/help/assets/sample-email.png)

+++

## Critères d’invite

Dans GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md), vous pouvez utiliser **[!UICONTROL Critères d’invite]** ([_Paramètres_](/help/user-guide/create/overview.md#parameters) et une invite) dans le tiroir d’invite pour ajouter des détails par sélection afin d’améliorer l’interprétation de l’IA.

Pour les [e-mails](/help/user-guide/create/email-experiences.md), les critères d’invite peuvent inclure l’ajout de [directives](/help/user-guide/guidelines/overview.md) dans _Paramètres_, le chargement d’une ressource à utiliser dans les variantes d’e-mail et une invite descriptive. Pour une publicité [Meta](/help/user-guide/create/create-meta-ad.md), les critères d’invite peuvent inclure une ligne directrice de marque dans _Paramètres_, la sélection ou le chargement d’une ressource existante, des paramètres liés aux images ou aux ressources telles que les proportions, ainsi qu’une invite. Le vrai pouvoir commence avec [la configuration des directives](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Si des directives sont ajoutées dans _Paramètres_ dans le tiroir de l&#39;invite, il n&#39;est pas nécessaire d&#39;y faire référence dans l&#39;invite. GenStudio for Performance Marketing exploite automatiquement ceux de la génération de contenu.

### Directives

Les instructions de GenStudio for Performance Marketing aident l’IA générative à personnaliser la composition de vos ressources. Lorsque des critères d’invite vous sont présentés, vous pouvez choisir un [[!DNL Brand]](/help/user-guide/guidelines/brands.md), un [[!DNL Persona]](/help/user-guide/guidelines/personas.md) et un [[!DNL Product]](/help/user-guide/guidelines/products.md) parmi vos instructions configurées.

>[!TIP]
>
>Vous contrôlez quand et comment GenStudio for Performance Marketing utilise vos directives de [!DNL Brand]. Consultez [Recommandations](/help/user-guide/guidelines/overview.md) pour savoir comment configurer et gérer vos recommandations de marque.

### Invites structurées

Pour les e-mails à plusieurs sections, vous pouvez structurer des invites pour fournir des instructions spécifiques à la section afin de générer un contenu variable pour chaque section d&#39;un e-mail. Les invites structurées doivent référencer directement les [noms de section dans le modèle d&#39;email](/help/user-guide/content/customize-template.md#sections-or-groups) afin que le contenu généré puisse être inséré dans les espaces réservés de contenu correspondants.

Par exemple, vous pouvez demander à GenStudio for Performance Marketing de générer du contenu pour un e-mail qui promeut un nouveau produit dans la première section et détaille les avantages en termes de réduction des coûts dans la seconde section.

L’invite structurée doit :

- Utilisez l’une des références suivantes pour le nom de la section dans le modèle d’e-mail :
   - Pod
   - Groupe
   - Section
   - Module

  Par exemple, si votre modèle utilise `moduleA` ou `Group-3` comme nom de section, vous pouvez référencer ces noms de section dans l&#39;invite.

- Suivez les règles/structures recommandées. Si la structure de l’invite ne respecte pas le format fourni, l’invite s’applique à *toutes* les sections d’e-mail et facilite toujours la génération de contenu.
- Utilisez les noms de section tels que définis dans votre modèle d’e-mail. Les références d’invite doivent correspondre aux noms de section codés dans votre modèle d’e-mail.
- Ne pas respecter la casse. Par exemple, vous pouvez utiliser `Pod` ou `pod` dans votre modèle d’e-mail et votre invite structurée.
- Référencez d’abord l’invite utilisateur générique, puis les directives spécifiques à la section.
- Utilisez un signe deux-points, un trait d&#39;union, une virgule ou une autre démarcation (`,:;#$!~|@=-%&*^_`) comme séparation entre la référence de nom de section et la directive. Par exemple, vous pouvez utiliser ce qui suit comme directive d’invite spécifique à une section : `Pod1; Describe how to easily edit text and swap images.`

Voici un exemple d’invite qui articule la structure d’invite recommandée et utilise un modèle d’e-mail qui utilise le terme d’identification `Pod` que dans `Pod1`, `Pod2` et `Pod3`.

```properties
Create an exciting multi-pod email focusing on Creative Cloud and its powerful generative AI capabilities.

Encourage customers to convert to Photoshop or use a free Photoshop trial. We want to better educate them about app features.

Pod1: Focus on Adobe Photoshop and its new generative AI tools that enable creators to bring images to life in minutes.

Pod2: Focus on Adobe Illustrator and its new generative AI tools, such as Generative Shape Fill, which allows you to quickly fill your vector outline and explore a variety of options that match the look and feel of your own artwork.

Pod3: Focus on Adobe Acrobat Pro. Make users aware that with Acrobat Pro they can edit images and text inside a PDF.
```

Voir [Bonnes pratiques relatives à l’utilisation des modèles](/help/user-guide/content/best-practices-for-templates.md).

## Réessayez

L’invite est un processus itératif. Si les résultats ne répondent pas à vos attentes, vérifiez votre invite et apportez des modifications ou ajoutez plus de détails. Vous pouvez également coller des sections à partir d’un résumé de campagne. Vous pouvez même demander à GenStudio for Performance Marketing d’éviter certains mots, éléments ou thèmes.

## Bonnes pratiques

Bonnes pratiques simples pour concevoir des invites efficaces :

- Soyez précis et donnez des détails sur ce que vous devez faire et ne pas faire.
- Fournissez du contexte à l’aide de références externes.
- Appliquez les directives de GenStudio for Performance Marketing.
- Examinez et ajustez régulièrement les directives.
- Itérez et affinez.
- Apprenez par l’expérimentation.

{{in-academy}}
