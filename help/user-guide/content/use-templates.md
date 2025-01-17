---
title: Utilisation de modèles
description: Découvrez comment utiliser efficacement les modèles pour rationaliser votre processus de création dans Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 72a3b62d02e391d2127982e7c3a6f437f868a3c1
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# Utilisation de modèles

GenStudio for Performance Marketing permet aux créateurs de contenu de produire rapidement du contenu marketing cohérent sur la marque à l’aide de _modèles_. Un modèle réduit considérablement le temps et les efforts requis pour générer un nouveau contenu en fournissant un point de départ qui inclut des dispositions et des éléments de conception préconfigurés.

Bien que GenStudio for Performance Marketing ne prenne pas en charge la création directe de modèles dans l’application, vous pouvez facilement concevoir et préparer des modèles à l’aide d’outils de conception courants, tels qu’Adobe InDesign, Illustrator ou Express. Une fois la conception terminée, vous pouvez l’adapter pour l’utiliser dans GenStudio for Performance Marketing. Commencez à utiliser des modèles en procédant comme suit :

1. **Concevoir le modèle** : utilisez votre outil de conception préféré pour créer la disposition visuelle de votre [modèle avec des éléments](#template-elements) tels qu’un pré-titre, un titre, un corps, un CTA, des images et un pied de page.

2. **Coder votre modèle** : convertissez votre conception en CSS HTML et intégré pour vous assurer qu’elle est propre et réactive sur différents appareils. Tenez compte des [directives d’accessibilité](accessibility-for-templates.md) pour atteindre votre audience maximale prévue.

3. **Préparation pour GenStudio for Performance Marketing** : adaptez votre modèle d’HTML à l’aide du langage de modèle Handlebars. Insérez des espaces réservés pour indiquer où GenStudio for Performance Marketing doit générer du contenu dynamiquement. Consultez la section Comment [personnaliser un modèle](customize-template.md) pour GenStudio for Performance Marketing.

En suivant ces étapes, vous pouvez créer des modèles professionnels et efficaces, prêts à être utilisés dans GenStudio for Performance Marketing, ce qui vous permet de produire rapidement et efficacement du contenu intégré à la marque.

## Éléments de modèle

Un modèle est un ensemble de directives définies avec un CSS HTML et intégré qui peut être utilisé pour produire un e-mail, une publicité sur les réseaux sociaux ou une expérience d’affichage d’annonce. Les éléments de modèle fournissent la structure pour la création de contenu.

Voici une liste des éléments utilisés dans les modèles et quelques détails sur leurs caractéristiques :

- **Preheader**

   - Agit comme une ligne d’objet secondaire dans un e-mail, améliorant la ligne d’objet principale
   - Entre 40 et 50 caractères
   - Visible dans la boîte de réception avec l’objet avant l’ouverture de l’e-mail
   - Utilisé dans les modèles d’e-mail

- **En-tête**

   - Section supérieure de l’e-mail que le destinataire voit lors de l’ouverture de l’e-mail
   - Définit le ton et fournit un contexte pour le contenu inclus
   - Utilisé dans les modèles d’e-mail

- **Titre**

   - Premier contenu vu par le destinataire
   - Devrait être contraignant de capter l&#39;intérêt
   - Utilisé dans les métamodèles

- **Corps**

   - Zone de contenu principale où le message principal est transmis
   - Possibilité d’inclure du texte, des images et d’autres médias
   - Utilisé dans les modèles d’e-mail et de métadonnées

- **CTA**

   - Le bouton d’appel à l’action utilise une expression et un lien
   - Encourage le ou la destinataire à effectuer une action spécifique, telle que cliquer sur un lien ou effectuer un achat
   - Utilisé dans les modèles d’e-mail et de métadonnées

- **Images**

   - Améliore l’attrait visuel
   - Fractionner le texte
   - Prise en charge du message
   - Doit être de haute qualité et attrayant
   - Utilisé dans les modèles d’e-mail et de métadonnées

- **Pied de page**

   - Section inférieure contenant du contenu supplémentaire, tel que des coordonnées, des liens vers les médias sociaux, des clauses de non-responsabilité et des options de désabonnement
   - Utilisé dans les modèles d’e-mail

- **Superposition de texte**

   - Texte sur une image
   - Utilisez pour soutenir et améliorer le titre et le corps
   - Utilisé dans les métamodèles

>[!TIP]
>
>Consultez les [noms de champ reconnus](customize-template.md#recognized-field-names) pris en charge par GenStudio for Performance Marketing pour les modèles de chaque type de canal.

## Personnaliser le modèle

Vous [personnalisez votre modèle](customize-template.md) à utiliser dans GenStudio for Performance Marketing en insérant des espaces réservés de contenu, ou des champs, que l’IA générative utilise pour insérer du contenu. GenStudio for Performance Marketing reconnaît certains champs, tels que le champ `body`, et adhère aux directives de canal configurées pour la marque sélectionnée.

>[!TIP]
>
>Suivez les [directives d’accessibilité](accessibility-for-templates.md) et [bonnes pratiques](/help/user-guide/content/best-practices-for-templates.md) afin de toucher davantage d’audiences et d’offrir une expérience optimale.

## Gestion des modèles

La galerie [!DNL Templates] affiche votre inventaire de modèles personnalisés pour la génération d’expériences dans GenStudio for Performance Marketing. Vous pouvez filtrer les modèles par type de canal, tels que les e-mails, les publicités display et les méta-publicités.

![Liste des modèles de contenu](/help/assets/content-templates.png){width="650" zoomable="yes"}

### Ajouter un modèle

Avant de charger un modèle, assurez-vous qu’il est entièrement préparé et prêt à être utilisé dans GenStudio for Performance Marketing en suivant les instructions du guide [Personnaliser les modèles](customize-template.md).

**Pour ajouter un modèle** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Modèles]**.

1. Cliquez sur **[!UICONTROL Ajouter un modèle]**.

1. Dans le volet _[!UICONTROL Ajouter votre modèle approuvé]_, recherchez le fichier de modèle d’HTML ou faites glisser le fichier de modèle d’HTML vers l’espace de dépôt. Cliquez sur **[!UICONTROL Suivant]**.

1. Dans le volet _[!UICONTROL Vérifier les champs découverts]_ passez en revue les champs détectés. Vérifiez que vous utilisez le modèle correct et que tous les détails sont conformes aux attentes. Cliquez sur **[!UICONTROL Suivant]**.

   Exemple de prévisualisation pour un modèle d’e-mail :

   ![Champs de prévisualisation détectés](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Si le modèle n’est pas correct, cliquez sur **[!UICONTROL Précédent]** et revenez à l’étape précédente. Chargez le fichier de modèle corrigé.

1. Dans le volet _[!UICONTROL Fournir des détails de modèle et charger]_, nommez votre modèle et sélectionnez un type **[!UICONTROL Canal]**.

   Le nom du modèle et le type de canal sont obligatoires. Les exigences supplémentaires peuvent inclure :

   - **Meta** : nécessite un format
   - **Afficher les publicités** : nécessite des Dimensions

1. Ajoutez autant de détails que possible pour améliorer l’identification du modèle dans les recherches et le filtrage.

1. Cliquez sur **[!UICONTROL Terminé]**.

### Actualiser le modèle

Les modèles peuvent inclure des fichiers statiques, tels que des icônes ou des logos. Utilisez l’option Actualiser pour mettre à jour l’aperçu du modèle avec les dernières versions de ces ressources.

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

1. Passez à [Créer](/help/user-guide/create/overview.md) une expérience.
