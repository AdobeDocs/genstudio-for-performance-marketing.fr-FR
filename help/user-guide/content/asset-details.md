---
title: Détails de la ressource
description: Adobe GenStudio for Performance Marketing stocke le contenu approuvé avec des métadonnées riches pour le suivi de la capacité de recherche et des performances.
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
TQID: https://experienceleague.adobe.com/Hm7qcrP6VcXf6IqZ2pYybduNyjjV8kdWj571gcRpglI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a8b28c00-da6e-4d27-8667-80f790ad8972
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
  - id: b03d2162-d906-40a0-9cbd-001391e22d4a
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 732
ht-degree: 1%

---

# Détails des ressources

Adobe GenStudio for Performance Marketing stocke le contenu approuvé avec des métadonnées riches pour le suivi de la capacité de découverte et des performances.

Chaque ressource (y compris les expériences et les modèles) est associée à des _détails_ (métadonnées) qui permettent d’identifier, de suivre, d’utiliser et d’apprendre des performances du contenu.

**Pour afficher les détails d’une ressource** :

1. Dans _[!DNL Content]_, sélectionnez une ressource, une expérience ou un modèle. Cliquer sur une ressource ouvre une vue ciblée de la ressource.

1. Dans la vue de la ressource, passez en revue la section _[!UICONTROL Détails]_ à droite.

1. Si la section _[!UICONTROL Détails]_ n’est pas visible, cliquez sur l’icône **[!UICONTROL Informations]** (i).

Les détails de la ressource incluent les métadonnées appliquées pendant le processus de création ou de chargement. Les types de métadonnées des ressources incluent les [métadonnées système](#system-metadata) et [métadonnées définies par l’utilisateur](#user-defined-metadata).

La ressource d’image suivante contient des métadonnées système décrivant le type, la taille et d’autres caractéristiques du fichier, un mot-clé défini par l’utilisateur, ainsi que plusieurs attributs et couleurs détectés par l’IA.

![détails d’une ressource avec plusieurs balises](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets à partir des référentiels AEM affiche des métadonnées différentes. Voir [Configurer la visibilité des ressources](connect-aem-repo.md#step-4-configure-asset-visibility) pour savoir comment configurer les détails d’une ressource [!DNL AEM Assets Content Hub].

## Métadonnées système

Certaines métadonnées de ressources sont automatiquement collectées lorsqu’une ressource est chargée, telles que le type de fichier, la taille, les dimensions, la source, etc. À l’exception du nom de fichier, vous ne pouvez pas modifier les métadonnées système par défaut.

### Balises générées

Lorsque vous stockez une ressource approuvée dans [!DNL Content], GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités de machine learning pour étudier la ressource et appliquer des balises en fonction des fonctionnalités de la ressource. Par exemple, l’image d’un chat peut donner lieu à des balises d’attributs telles que `pet photography` ou `cat`, ainsi qu’à des balises de couleurs qui identifient les couleurs dominantes dans l’image. Vous ne pouvez pas modifier les balises détectées et automatiquement appliquées.

Voir [!DNL Insights] [Catégories d’attributs](/help/user-guide/insights/attributes.md#categories) pour obtenir des listes détaillées des fonctionnalités d’image, de vidéo et de texte.

### Métadonnées de contenu générées

Les informations utilisées pour générer une nouvelle ressource ou expérience deviennent des métadonnées, telles que l’invite utilisée. Vous ne pouvez pas modifier l’invite une fois le contenu approuvé, mais vous pouvez l’utiliser comme point de départ pour générer quelque chose de nouveau.

## Métadonnées définies par l’utilisateur

Les métadonnées définies par l’utilisateur ajoutent un contexte marketing au contenu de la ressource, ce qui permet aux spécialistes marketing de comprendre comment utiliser la ressource et interagir avec elle.

Lorsque vous [chargez une ressource](/help/user-guide/content/manage-assets.md#add-assets) vous pouvez définir un ensemble de détails de ressource facultatifs qui existent dans GenStudio for Performance Marketing sous forme de métadonnées. L’ajout de détails supplémentaires peut améliorer l’identification des ressources dans les recherches et le filtrage.

**Pour modifier les métadonnées définies par l’utilisateur** :

1. Dans _[!DNL Content]_, sélectionnez une ressource, une expérience ou un modèle. Cliquer sur une ressource ouvre une vue ciblée de la ressource.

1. Dans la vue de la ressource, passez en revue la section _[!UICONTROL Détails]_ à droite.

1. Cliquez sur **[!UICONTROL Modifier les détails]** (crayon) pour modifier les métadonnées d’une ressource, d’une expérience ou d’un modèle.

   Plus vous fournissez de détails, plus vous bénéficiez des fonctionnalités robustes de GenStudio for Performance Marketing. Sélectionnez un ou plusieurs détails dans la liste, ou saisissez-en un nouveau le cas échéant, par exemple avec des mots-clés. Chaque détail que vous ajoutez apparaît sous la liste. Cliquez sur **`x`** pour supprimer un détail.

### Détails des métadonnées

Le tableau suivant détaille les métadonnées (détails de la ressource) que vous pouvez définir lors de la création d’une ressource.

| champ | Description |
| -------------- | ----------- |
| Titre | Nom de la ressource ; le titre par défaut peut être le nom de fichier original |
| [!DNL Campaigns] | [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) inclure du contenu promotionnel avec un message cohérent dans le but d’atteindre un objectif commercial<br>cliquer sur un lien de campagne vous conduit à la page d’aperçu de la campagne |
| [!DNL Brands] | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) ajoutée à GenStudio for Performance Marketing et publiée pour utilisation |
| [!DNL Products] | [[!DNL Products]](/help/user-guide/guidelines/products.md) ajoutée à GenStudio for Performance Marketing pour utilisation |
| [!DNL Personas] | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) ajoutée à GenStudio for Performance Marketing pour utilisation |
| Canaux | Plateformes de distribution de certains types de contenu, tels que les e-mails, les bannières et les publicités display |
| [!UICONTROL Période] | Période pour laquelle la ressource est utilisée, telle que trimestre, saison, année, etc. Exemple : `Winter 2023` |
| Région | Régions pour lesquelles la ressource est utilisée. Exemples : `North America`, `APAC`, `Italy` |
| Langue | Langues pour lesquelles la ressource est utilisée. Exemple : `Spanish` |
| Mots-clés | Les mots-clés définis par l’utilisateur sont utilisés pour identifier plus précisément les caractéristiques et l’objectif des ressources |

>[!TIP]
>
>Cliquez sur **[!UICONTROL Modifier les détails]** (crayon) pour modifier les métadonnées de la ressource. Par exemple, vous pouvez modifier le nom de la ressource ou ajouter ou supprimer des mots-clés.

## Contexte génératif

La section [!UICONTROL Contexte génératif] indique quelles informations ont été utilisées pour générer l’expérience, telles que les `Prompt` utilisées pendant le processus de [!DNL Create]. Cette insight peut vous aider à créer des variantes encore plus performantes.

Ces informations peuvent inclure :

- `Brand`, `Product` et `Persona` paramètres sélectionnés lors du processus de [!DNL Create]
- `Subject line` et `Preheader` pour les expériences d’e-mail
- `Headline` et `Body` pour les publicités Meta

## Historique

Développez la section _[!UICONTROL Historique]_ d’une expérience pour afficher une chronologie des approbations et des activités. Par exemple, une expérience approuvée affiche la date d’approbation, l’heure et le nom de l’approbateur :

```
Approved

December 10, 2024 at 6:00 PM by Username
```
