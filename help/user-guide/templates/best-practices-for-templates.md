---
title: Bonnes pratiques relatives aux modèles
description: Appliquez les bonnes pratiques lorsque vous utilisez des modèles avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: cc72dcf1-72e1-48cc-b434-e7c27d62d67cid: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 3322f783cd49ddcb897942e5e91590d53b554bdd
workflow-type: tm+mt
source-wordcount: 1347
ht-degree: 0%

---

# Bonnes pratiques relatives à l’utilisation des modèles

Les modèles réduisent considérablement le temps et les efforts nécessaires à la génération d’un nouveau contenu en fournissant un point de départ qui inclut des dispositions préconfigurées et des éléments de conception.

Appliquez les recommandations suivantes lors de l’utilisation de modèles avec GenStudio for Performance Marketing :

1. En savoir plus sur les [éléments de modèle](#know-about-template-elements)
1. Configurez [directives relatives aux canaux](#configure-channel-guidelines) pour une personnalisation efficace du contenu
1. Concevez avec des [normes d’accessibilité](accessibility-for-templates.md) pour une expérience optimale
1. Suivez les [directives relatives aux modèles spécifiques aux canaux](#follow-channel-specific-template-guidelines)
1. Lors de l’utilisation de [modèles Express](/help/user-guide/templates/express-templates.md), tenez compte des conseils spécifiques sous [Bonnes pratiques relatives aux modèles Express à GenStudio](#express-to-genstudio-template-best-practices).
>>
Découvrez les principes de base des éléments et des procédures de modèle dans [Utilisation de modèles](use-templates.md). Découvrez également en détail [personnalisation d’un modèle](customize-template.md) pour obtenir des instructions spécifiques à utiliser dans votre prochaine campagne.

## Utiliser les éléments de modèle appropriés

Chaque type de modèle utilise différents éléments pour créer une structure pour la création de contenu spécifique au canal. [Familiarisez-vous avec les parties d’un modèle](use-templates.md#template-elements) et incluez les meilleurs éléments pour votre contenu et votre type de modèle.

Lors de la personnalisation de votre modèle, utilisez les noms de champ à la place de ces éléments où vous avez besoin de GenStudio for Performance Marketing pour générer du contenu.

Voir [Éléments de modèle](use-templates.md#template-elements).

## Utilisation de texte d’espace réservé dans les modèles

Le texte d’espace réservé peut aider à définir la syntaxe ou la structure du contenu à remplir ultérieurement dans un modèle par un utilisateur. Par exemple, {first_name}.{last_name}@email.etc. pour définir une adresse électronique. Cependant, certains délimiteurs communs sont déjà réservés à d’autres significations dans GenStudio for Performance Marketing :

❌ `< >` - Utilisé pour les balises HTML.
❌ `{{ }}` - Utilisé pour les expressions Handlebar.

Utilisez des crochets simples (droits ou courbes) pour indiquer le texte de l’espace réservé afin d’éviter toute confusion avec les balises existantes.

✅ `{first_name}` - Espace réservé pour le prénom.

## Configurer les instructions relatives aux canaux

Il est essentiel de définir des directives claires concernant les canaux pour vous assurer que le contenu généré correspond aux exigences et aux objectifs de votre marque. Les instructions de canal vous permettent de spécifier des règles pour des éléments tels que le ton, la longueur et le style utilisés dans votre modèle. Par exemple, vous pouvez définir un nombre maximal de caractères pour le corps du texte ou exiger un style call-to-action spécifique. En définissant ces directives à l’avance, vous réduisez la nécessité d’écrire des instructions détaillées dans chaque invite d’IA, en rationalisant le processus de génération de contenu et en assurant la cohérence entre vos e-mails.

Examinez et définissez les [directives relatives aux canaux](/help/user-guide/guidelines/brands.md#channel-guidelines) de votre marque pour tous les champs clés de votre modèle. Si vous ne définissez pas de directives, les [ directives de canal par défaut](/help/user-guide/guidelines/brands.md#default-channel-guidelines) sont appliquées, ce qui peut ne pas refléter entièrement les exigences de votre marque.

![Spécifications du corps](/help/assets/channel-email-body.png)

Découvrez comment [les directives sur les marques, les produits et les personnes concernées](/help/user-guide/guidelines/overview.md) influencent le contenu généré et comment les adapter à vos objectifs marketing.

## Chargement des images pour les modèles

Les images utilisées dans les modèles doivent provenir du référentiel de contenu et doivent être chargées correctement pour s’assurer que l’image s’affiche correctement.

Lorsqu’un modèle comporte une image de contour à contour (fond perdu complet), l’image sélectionnée est automatiquement redimensionnée pour s’adapter aux dimensions complètes du modèle. Cependant, si l’image ne correspond pas aux proportions du modèle, elle est recadrée pour s’adapter aux dimensions du modèle et peut ne pas s’afficher comme prévu.

Il n’existe aucune fonctionnalité d’« ajustement automatique » pour les images incluses dans les modèles.

Pour résoudre le recadrage d’image, les utilisateurs doivent définir les proportions de l’image à utiliser dans le modèle lorsqu’il est chargé dans le référentiel de contenu. Lors du chargement d’un modèle approuvé :

1. [Poursuivez le processus de chargement des modèles](/help/user-guide/templates/use-templates.md#add-a-template) jusqu’à la page **[!UICONTROL Ajouter des détails]**.

2. Définissez les proportions de l’image à utiliser dans le modèle en **[!UICONTROL Largeur de l’annonce publicitaire (px)]** et **[!UICONTROL Hauteur de l’annonce publicitaire (px)]**. Cette option définit la fenêtre d’image pour la section du modèle qui affiche l’image.

3. Dans la section **[!UICONTROL Plus de détails]**, sélectionnez le menu déroulant **[!UICONTROL Taille de l’image]** et choisissez _Recadrer à une taille fixe_.
   ![Recadré à une taille fixe](images/crop-to-fixed-size.png "Recadré à une taille fixe"){width="80%"}

Pour déterminer la taille et les proportions d’une image dans le navigateur :

1. Inspectez l’image.
   - Sous Windows/Linux :
      - Appuyez sur F12.
   - Sous macOS :
      - Appuyez sur Commande + Option + I.

1. Pointez sur l’image.

1. Notez les proportions. Utilisez cette option pour définir les proportions de l’image dans le modèle.

Lorsque ces détails ne sont pas appliqués lors du chargement, l’image est censée correspondre à l’intégralité des proportions du modèle et les images qui ne correspondent pas exactement à ces proportions apparaîtront recadrées.

![Image recadrée dans une publicité affichée](images/cropped-display.png "Recadrage d’image"){width="60%"}

**❌Image recadrée dans un modèle de publicité display**

![Image affichée dans une publicité affichée](images/full-fit.png "Image affichée dans une publicité affichée"){width="60%"}

**✅Image entièrement affichée**

## Suivre les instructions relatives aux modèles spécifiques aux canaux

Lors de la création de modèles, assurez-vous qu’ils répondent aux exigences spécifiques du canal prévu. Créez des modèles qui s’adaptent à la mise en page et aux exigences visuelles de chaque canal. Des instructions générales s’appliquent à tous les modèles, notamment :

- Utilisation d’HTML et de CSS intégré propres et réactifs
- Utilisation des polices Adobe ou Google
- N’utilisez **** JavaScript

{{note-css-effects}}

Consultez d’autres conseils et contraintes lorsque vous utilisez chaque type de modèle pour garantir des performances optimales :

- [E-mails](/help/user-guide/templates/email-template.md)
- [Affichage et bannières publicitaires](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta ads](/help/user-guide/templates/meta-template.md)

## Bonnes pratiques relatives aux modèles Express to GenStudio

Les conseils suivants vous aident à obtenir des résultats fiables lorsque vous convertissez des conceptions à partir de [!DNL Adobe Express] en modèles à [!DNL GenStudio for Performance Marketing].

### Utilisation de modèles à plusieurs variations

Dans [!DNL Adobe Express], les pages peuvent représenter plusieurs variations de taille ou de format dans un fichier de modèle.
Lorsque vous sélectionnez le modèle dans [!DNL GenStudio for Performance Marketing], toutes les variations apparaissent dans la zone de travail.

Ce comportement s’améliore par rapport aux modèles HTML, qui ne prennent en charge qu’une seule variation par fichier.

### Verrouillage de champs pour contrôler ce que les marketeurs peuvent modifier

Utilisez le verrouillage pour communiquer l’intention. Par exemple, verrouillez une clause de non-responsabilité légale afin qu’elle ne soit jamais générée par l’IA, mais laissez un titre flexible pour la génération.

Cliquez avec le bouton droit de la souris sur un élément de [!DNL Adobe Express] pour définir le comportement du verrouillage :

- **[!UICONTROL Verrouillage complet]** — L’élément est statique et l’IA ne génère pas de contenu pour lui.
- **[!UICONTROL Verrouiller, autoriser le remplacement de l&#39;image]** — Verrouille la taille et la position mais permet aux utilisateurs de permuter l&#39;image. Cette option fonctionne bien pour les logos.
- **[!UICONTROL Verrouiller, autoriser le remplacement du texte]** — Verrouille la taille et la position mais permet aux utilisateurs de modifier le texte. L’IA ne génère pas automatiquement de contenu pour elle.
- **Entièrement flexible** (déverrouillé) : les utilisateurs peuvent déplacer et redimensionner l’élément, que l’IA traite comme du contenu à générer.

### Nommer les calques pour un meilleur mappage IA

Lorsque vous convertissez une conception en modèle, l’IA analyse la conception et mappe les champs tels que l’en-tête, le CTA et la copie du corps. L’IA mappe les modèles simples avec précision plus souvent que les mises en page très complexes.

**Bonne pratique :** dans la copie d’espace réservé, incluez le type de champ prévu (par exemple, `headline`, `sub-headline` ou `CTA`) pour aider l’IA à mapper correctement les champs. Cette approche peut réduire les erreurs de mappage.

### Convertir en modèle

1. Dans [!DNL Adobe Express], cliquez sur **[!UICONTROL Partager]** > **[!UICONTROL Convertir en modèle]**.
1. Seuls les onglets **[!UICONTROL Info]** et **[!UICONTROL Verrouillages]** sont transférés vers [!DNL GenStudio for Performance Marketing].
1. Au moment de la conversion, choisissez comment fonctionne le déverrouillage :
   - **[!UICONTROL Autoriser les utilisateurs à déverrouiller]**
   - **[!UICONTROL Empêcher tout déverrouillage]**
   - **[!UICONTROL Définissez une phrase secrète]** — Un juste milieu qui décourage les changements occasionnels sans bloquer l&#39;accès de manière permanente.

### Conserver une copie du fichier de conception d’origine

La conversion crée un fichier de modèle de [!DNL Adobe Express] distinct, mais le fichier de conception d’origine reste modifiable.

**Conseil :** conservez l’original afin de pouvoir réviser la conception, créer des variations et générer de nouveaux modèles ultérieurement.

### Partager pour plus de visibilité

Après la conversion, le modèle n’est visible que par défaut pour vous. Vous pouvez le partager avec des personnes ou avec l’ensemble de l’organisation.

**Exigence :** les [!DNL Adobe Express] et [!DNL GenStudio for Performance Marketing] doivent utiliser la même organisation IMS pour que les modèles soient synchronisés. Les modèles apparaissent généralement dans [!DNL GenStudio for Performance Marketing] presque immédiatement après la conversion.

### Mappage des champs de l’IA dédiée au contrôle

Après avoir sélectionné un modèle, l’IA mappe les champs une fois par modèle, en attribuant des libellés tels que **[!UICONTROL média principal]**, **[!UICONTROL généré]** ou **[!UICONTROL verrouillé]**. Vous pouvez ajuster manuellement les mappages lorsque l’IA attribue des champs de manière incorrecte.

Utilisez le bouton (bascule) **[!UICONTROL Activer la génération]** par champ pour activer ou désactiver la génération avant la génération. Vous pouvez ajuster manuellement les mappages lorsque l’IA attribue des champs de manière incorrecte. Des corrections permanentes des mappages de modèle sont prévues pour une version ultérieure.

### Conception dans [!DNL Adobe Express], assemblage dans [!DNL GenStudio for Performance Marketing]

Tenez compte de ces workflows de conception pour utiliser au mieux chaque service :

- Effectuez des tâches de conception complètes, telles que des couleurs, des mises en page et des graphiques dans [!DNL Adobe Express].
- Utilisez [!DNL GenStudio for Performance Marketing] pour assembler et générer du contenu à partir de ces modèles.
- Utilisez des marques [!DNL Adobe Express] (couleurs, logos, polices et graphiques) pour la gouvernance de la conception.
- Utilisez les marques [!DNL GenStudio for Performance Marketing] pour les changements de couleur de police après la génération.

### Limites des e-mails

L’e-mail n’est **pas** pris en charge sur la zone de travail Horizon pour le workflow de modèle de [!DNL Adobe Express]. L’e-mail continue à utiliser le processus de modèle HTML traditionnel.

### Tirer parti des polices personnalisées

Les équipes demandent souvent comment les polices personnalisées fonctionnent avec les modèles de [!DNL Adobe Express]. Les administrateurs peuvent être amenés à accepter l’offre de qualification des polices personnalisées dans Admin Console avant que ces polices ne soient disponibles ; voir [Utilisation  [!DNL Adobe Express]  modèles](express-templates.md).
