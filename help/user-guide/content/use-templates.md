---
title: Utilisation des modèles
description: Découvrez comment utiliser efficacement les modèles pour rationaliser votre processus de création dans Adobe GenStudio for Performance Marketing.
feature: Templates, Content
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
source-git-commit: 61a939ae81eb5ff61d741bb1092e9e4c82119f7e
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 1%

---

# Utilisation des modèles

GenStudio for Performance Marketing permet aux créateurs de contenu de produire rapidement du contenu marketing sur marque cohérent à l’aide de _modèles_. Un modèle réduit considérablement le temps et les efforts nécessaires à la génération d’un nouveau contenu en fournissant un point de départ qui inclut des mises en page et des éléments de conception préconfigurés.

## Éléments de modèle

Un modèle est un ensemble d’instructions définies avec des feuilles de style CSS intégrées et HTML qui peuvent être utilisées pour produire une expérience de type email ou méta-publicité.

Vous trouverez ci-dessous une liste des éléments utilisés dans les modèles et quelques détails sur leurs caractéristiques.

- **Preheader**

   - Agit comme objet secondaire dans un email, améliorant l’objet principal
   - Entre 40 et 50 caractères
   - Visible dans la boîte de réception à côté de l’objet avant l’ouverture de l’email
   - Utilisé dans les modèles de courrier électronique

- **En-tête**

   - Section supérieure de l&#39;email que le destinataire voit lors de l&#39;ouverture de l&#39;email
   - Définit le ton et fournit le contexte du contenu inclus.
   - Utilisé dans les modèles de courrier électronique

- **Titre**

   - Premier contenu vu par le destinataire
   - Doit être convaincant pour attirer l&#39;attention
   - Utilisé dans les modèles de métadonnées publicitaires

- **Body**

   - Zone de contenu principale où le message principal est transmis
   - Possibilité d’inclure du texte, des images et d’autres médias
   - Utilisé dans les modèles de courrier électronique et de métadonnées publicitaires

- **CTA (Appel à l’action)**

   - encourage le destinataire à effectuer une action spécifique, par exemple cliquer sur un lien ou effectuer un achat.
   - Utilisé dans les modèles de courrier électronique et de métadonnées publicitaires

- **Images**

   - Améliore l’attrait visuel
   - Ventiler le texte
   - Prise en charge du message
   - Doit être de haute qualité et attrayant pour les yeux
   - Utilisé dans les modèles de courrier électronique et de métadonnées publicitaires

- **Pied de page**

   - Section inférieure qui contient du contenu supplémentaire tel que les coordonnées, les liens vers les médias sociaux, les clauses de non-responsabilité et les options de désabonnement.
   - Utilisé dans les modèles de courrier électronique

- **Superposition de texte**

   - Texte d’une image
   - Utilisez pour prendre en charge et améliorer le titre et le corps
   - Utilisé dans les modèles de métadonnées publicitaires

>[!TIP]
>
>Voir les [noms de champ reconnus](customize-template.md#recognized-field-names) pris en charge par GenStudio for Performance Marketing pour les modèles de chaque type de canal.

## Configuration des directives de canal

Il est recommandé de configurer les [directives de canal](../guidelines/brands.md#channel-guidelines) pour chaque marque avant d’utiliser des modèles dans GenStudio for Performance Marketing. Les directives de canal influent directement sur le type de contenu généré lors de l’utilisation du modèle. Par exemple, vous pouvez définir des limites de caractères sur le corps d’un email.

![Spécifications du corps](/help/assets/channel-email-body.png)

## Personnaliser le modèle

Vous [personnalisez votre modèle](customize-template.md) pour l’utiliser dans GenStudio for Performance Marketing en insérant des espaces réservés de contenu, ou champs, que l’IA générative utilise pour insérer du contenu. GenStudio for Performance Marketing reconnaît certains champs, tels que le champ `body`, et respecte les directives de canal configurées pour la marque sélectionnée.

>[!TIP]
>
>Suivez les [consignes d’accessibilité pour créer des modèles](accessibility-for-templates.md) afin que vous puissiez atteindre plus de votre audience et offrir une expérience optimale.

## Chargement d’un modèle

Utilisez [Personnaliser les modèles](customize-template.md) comme guide lors de la préparation d’un modèle pour GenStudio for Performance Marketing. Voir les [consignes d’accessibilité pour les modèles](accessibility-for-templates.md) pour obtenir des conseils sur la manière de fournir une meilleure expérience à toutes les audiences.

**Pour ajouter un modèle** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Modèles]**.

1. Cliquez sur **[!UICONTROL Ajouter un modèle]**.

1. Dans le volet _[!UICONTROL Ajouter votre modèle approuvé]_, recherchez le fichier de modèle d’HTML ou faites glisser le fichier de modèle d’HTML vers l’espace de dépôt. Cliquez sur **[!UICONTROL Suivant]**.

1. Dans le volet _[!UICONTROL Vérifier les champs découverts]_, passez en revue les champs détectés. Vérifiez que vous utilisez le modèle correct et que tous les détails sont conformes à vos attentes. Cliquez sur **[!UICONTROL Suivant]**.

   Exemple d&#39;aperçu pour un modèle de courrier électronique :

   ![Champs d’aperçu détectés](../../assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >Si le modèle n’est pas correct, cliquez sur **[!UICONTROL Précédent]** et revenez à l’étape précédente. Téléchargez le fichier de modèle corrigé.

1. Dans le volet _[!UICONTROL Fournir des détails sur le modèle et charger]_, nommez votre modèle et sélectionnez un type **[!UICONTROL Canal]**.

   Le nom du modèle et le type de canal sont requis. D’autres exigences peuvent inclure :

   - **Meta** : nécessite des proportions
   - **Publicités affichées** : nécessite des Dimensions

1. Ajoutez autant de détails que possible pour améliorer l’identification du modèle dans les recherches et le filtrage.

1. Cliquez sur **[!UICONTROL Terminé]**.

## Créer avec un modèle

Recherchez et utilisez un modèle existant dans GenStudio for Performance Marketing pour créer d’autres expériences.

**Pour créer une expérience avec un modèle** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Modèles]**.

   ![Liste de modèles de contenu](../../assets/content-templates.png){width="650" zoomable="yes"}

1. Sélectionnez un modèle pour une vue complète et une liste de détails.

1. Cliquez sur **[!UICONTROL Créer une expérience]** (pinceau) dans le coin supérieur droit pour utiliser le modèle.

1. Passez à [Créer](/help/user-guide/create/overview.md) une expérience.
