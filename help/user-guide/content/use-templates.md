---
title: Utilisation de modèles
description: Découvrez comment utiliser efficacement les modèles pour rationaliser votre processus de création dans Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 624629700d8bf7d9e4c0e6d8b4373f40b14d4e05
workflow-type: tm+mt
source-wordcount: '1157'
ht-degree: 1%

---

# Utilisation de modèles

GenStudio for Performance Marketing permet aux créateurs de contenu de produire rapidement du contenu marketing cohérent sur la marque à l’aide de _modèles_. Un modèle réduit considérablement le temps et les efforts requis pour générer un nouveau contenu en fournissant un point de départ qui inclut des dispositions et des éléments de conception préconfigurés.

Bien que GenStudio for Performance Marketing ne prenne pas en charge la création directe de modèles dans l’application, vous pouvez facilement concevoir et préparer des modèles à l’aide d’outils de conception courants, tels qu’Adobe InDesign, Illustrator ou Express. Une fois la conception terminée, vous pouvez l’adapter pour l’utiliser dans GenStudio for Performance Marketing. Commencez à utiliser des modèles en procédant comme suit :

1. **Concevoir le modèle** : utilisez votre outil de conception préféré pour créer la disposition visuelle de votre [modèle avec des éléments](#template-elements) tels qu’un pré-titre, un titre, un corps, un CTA, des images et un pied de page.

2. **Coder votre modèle** : convertissez votre conception en HTML et en CSS intégré pour vous assurer qu’il est propre et réactif sur différents appareils. Tenez compte des [directives d’accessibilité](accessibility-for-templates.md) pour atteindre votre audience maximale prévue.

3. **Préparation pour GenStudio for Performance Marketing** : adaptez votre modèle HTML à l’aide du langage de modèle Handlebars. Insérez des espaces réservés pour indiquer où GenStudio for Performance Marketing doit générer du contenu dynamiquement. Consultez la section Comment [personnaliser un modèle](customize-template.md) pour GenStudio for Performance Marketing.

En suivant ces étapes, vous pouvez créer des modèles professionnels et efficaces, prêts à être utilisés dans GenStudio for Performance Marketing, ce qui vous permet de produire rapidement et efficacement du contenu intégré à la marque.

## Éléments de modèle

Un modèle est un ensemble d’instructions définies avec HTML et un CSS intégré qui peut être utilisé pour produire un e-mail, une publicité sur les réseaux sociaux ou une expérience d’affichage des annonces. Les éléments de modèle fournissent la structure pour la création de contenu.

Voici une liste des éléments utilisés dans les modèles et quelques détails sur leurs caractéristiques :

| **Élément** | **Canal** | **Description** |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Preheader** | E-mail | Une ligne d’objet secondaire dans un e-mail, généralement entre 40 et 50 caractères, qui améliore la ligne d’objet principale. Il est visible dans la boîte de réception à côté de l’objet avant l’ouverture de l’e-mail. |
| **En-tête** | E-mail | La section supérieure de l’e-mail que le destinataire voit lors de l’ouverture de l’e-mail donne le ton et fournit un contexte pour le contenu inclus. |
| **Titre** | Méta-annonce, bannières et affichages publicitaires, LinkedIn | Le premier contenu que le destinataire voit doit être attrayant pour capter son intérêt. |
| **Texte d’introduction** | LinkedIn | Le message principal transmet le message principal, comme la copie du corps. Il peut utiliser jusqu’à 150 caractères, y compris les espaces, quatre émoticônes au maximum et la ponctuation. |
| **Corps** | E-mail, méta-annonce, bannière et publicité display | Le texte principal de l’annonce véhicule le message principal. Il doit être engageant, informatif et persuasif pour encourager l&#39;action souhaitée de la part du public. |
| **CTA** | E-mail, Méta-annonce, bannières et publicités display, LinkedIn | Un bouton d’appel à l’action utilise une expression et un lien pour encourager le destinataire à effectuer une action spécifique, comme cliquer sur un lien ou effectuer un achat. |
| **Images** | E-mail, Méta-annonce, bannières et publicités display, LinkedIn | Améliorez l’attrait visuel, fractionnez le texte et prenez en charge le message. Les images doivent être de haute qualité et accrocheuses. |
| **Pied de page** | E-mail | La section inférieure de l’e-mail contient du contenu supplémentaire, tel que des coordonnées, des liens vers les médias sociaux, des clauses de non-responsabilité et des options de désabonnement. |
| **Superposition de texte** | Méta-annonce | Texte placé sur une image pour prendre en charge et améliorer le titre et le contenu du corps. |

>[!TIP]
>
>Consultez les [noms de champ reconnus](customize-template.md#recognized-field-names) pris en charge par GenStudio for Performance Marketing pour les modèles de chaque type de canal.

## Personnaliser le modèle

Vous [personnalisez votre modèle](customize-template.md) à utiliser dans GenStudio for Performance Marketing en insérant des espaces réservés de contenu, ou des champs, que l’IA générative utilise pour insérer du contenu. GenStudio for Performance Marketing reconnaît certains champs, tels que le champ `body`, et adhère aux directives de canal configurées pour la marque sélectionnée.

>[!TIP]
>
>Suivez les [directives d’accessibilité](accessibility-for-templates.md) et [bonnes pratiques](/help/user-guide/content/best-practices-for-templates.md) afin de toucher davantage d’audiences et d’offrir une expérience optimale.

## Gestion des modèles

La galerie _[!DNL Templates]_affiche votre inventaire de modèles personnalisés pour la génération d’expériences dans GenStudio for Performance Marketing. Vous pouvez filtrer les modèles par type de canal, tels que les e-mails, les publicités display, les méta-publicités et les publicités LinkedIn.

![Liste des modèles de contenu](/help/assets/content-templates-filter.png "Rechercher les modèles LinkedIn"){width="650" zoomable="yes"}

### Ajouter un modèle

Avant de charger un modèle, assurez-vous qu’il est entièrement préparé et prêt à être utilisé dans GenStudio for Performance Marketing en suivant les instructions du guide [Personnaliser les modèles](customize-template.md).

**Pour ajouter un modèle** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Modèles]**.

1. Cliquez sur **[!UICONTROL Ajouter un modèle]**.

1. Dans le volet _[!UICONTROL Ajouter votre modèle approuvé]_, recherchez le fichier de modèle HTML ou faites glisser le fichier de modèle HTML vers l’espace de dépôt. Cliquez sur **[!UICONTROL Suivant]**.

1. Dans le volet _[!UICONTROL Vérifier les champs détectés]_ passez en revue les champs. Vérifiez que vous utilisez le modèle correct et que tous les détails sont conformes aux attentes.

   Exemple de prévisualisation pour un modèle d’e-mail :

   ![Champs de prévisualisation détectés](/help/assets/template-detected-fields.png){width="650" zoomable="yes"}

   >[!TIP]
   >
   >Si le modèle n’est pas correct, cliquez sur **[!UICONTROL Précédent]** et revenez à l’étape précédente. Chargez le fichier de modèle corrigé. Vous pouvez également utiliser l’[éditeur de code de modèle](/help/user-guide/content/code-editor.md) pour apporter des corrections simples.

1. Cliquez sur **[!UICONTROL Suivant]** lorsque vous êtes satisfait(e) de l’aperçu du modèle.

1. Dans le volet _[!UICONTROL Fournir des détails de modèle et charger]_, nommez votre modèle et sélectionnez un type **[!UICONTROL Canal]**.

   Le nom du modèle et le type de canal sont obligatoires. Les exigences supplémentaires peuvent inclure :

   - **Meta** : nécessite un format
   - **Bannière et publicité display** : nécessite des dimensions.

1. Ajoutez autant de détails que possible pour améliorer l’identification du modèle dans les recherches et le filtrage.

1. Cliquez sur **[!UICONTROL Terminé]**.

### Actualiser le modèle

Les modèles peuvent inclure des fichiers statiques, tels que des icônes ou des logos. Le [contenu statique](/help/user-guide/content/customize-template.md#static-content) n’est pas stocké après la création de l’aperçu du modèle. GenStudio for Performance Marketing continue de référencer le lien source fourni dans le modèle. Utilisez l’option Actualiser pour mettre à jour l’aperçu du modèle avec les dernières versions de ces ressources.

**Pour actualiser le modèle** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Modèles]**.

1. Cliquez sur un modèle pour obtenir une vue complète et une liste de détails.

1. Cliquez sur **[!UICONTROL Actualiser]** (flèches tournantes) dans le coin supérieur droit pour actualiser toutes les ressources utilisées dans le modèle.

### Création d’une expérience avec un modèle

Recherchez et utilisez un modèle existant dans GenStudio for Performance Marketing pour créer d’autres expériences.

**Pour créer une expérience avec un modèle** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Modèles]**.

1. Cliquez sur un modèle pour obtenir une vue complète et une liste de détails.

1. Cliquez sur **[!UICONTROL Créer une expérience]** (pinceau) dans le coin supérieur droit pour utiliser le modèle.

1. Passez à [Créer](/help/user-guide/create/overview.md#create-use-cases) une expérience.

## Modèles AJO et Marketo

Vous pouvez charger un modèle que vous avez créé dans Adobe Journey Optimizer (AJO) ou Marketo. GenStudio for Performance Marketing détecte les modèles spécifiques à l’application et les ignore, préservant ainsi le formulaire d’origine pour une utilisation continue dans AJO ou Marketo. Vous n’avez pas besoin de modifier la syntaxe d’origine d’AJO ou de Marketo.

Les modèles d’application reconnus sont les suivants :

- **AJO** : `{{profile.*}}`, `{{context.*}}`
- **Marketo** : `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Conditions préalables**

- L’application (AJO, Marketo) et GenStudio for Performance Marketing doivent appartenir à la même organisation IMS pour l’intégration
- Les utilisateurs doivent avoir le rôle « Collaborateur » (niveau le plus bas) ou un niveau supérieur

>[!ENDSHADEBOX]

Ensuite, [personnalisez votre modèle](/help/user-guide/content/customize-template.md) avec des espaces réservés pour indiquer où GenStudio for Performance Marketing doit générer du contenu pour vous. [Ajoutez votre modèle](#add-a-template) au référentiel [!DNL Content] et validez le modèle. Effectuez des corrections mineures à l’aide de l’éditeur de code.
