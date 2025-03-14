---
title: Détails de la ressource
description: Adobe GenStudio for Performance Marketing stocke le contenu approuvé avec des métadonnées riches pour le suivi de la capacité de recherche et des performances.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
source-git-commit: f401f93e7dd08db4837b8709e28acec5571052f7
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 1%

---

# Détails de la ressource

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
| [!UICONTROL Période] | Période pour laquelle la ressource est utilisée, telle que trimestre, saison, année, etc. Exemple : `Winter 2023` |
| Région   | Régions pour lesquelles la ressource est utilisée. Exemples : `North America`, `APAC`, `Italy` |
| Langue | Langues pour lesquelles la ressource est utilisée. Exemple : `Spanish` |
| Mots-clés | Les mots-clés définis par l’utilisateur sont utilisés pour identifier plus précisément les caractéristiques et l’objectif des ressources |

>[!TIP]
>
>Cliquez sur **[!UICONTROL Modifier les détails]** (crayon) pour modifier les métadonnées de la ressource. Par exemple, vous pouvez modifier le nom de la ressource ou ajouter ou supprimer des mots-clés.

## Contexte génératif

La section [!UICONTROL Contexte génératif] indique quelles informations ont été utilisées pour générer l’expérience, telles que les `Prompt` utilisées pendant le processus de [!DNL Create]. Ces informations peuvent vous aider à créer des variantes encore plus efficaces.

Ces informations peuvent inclure :

- `Brand`, `Product` et `Persona` paramètres sélectionnés lors du processus de [!DNL Create]
- `Subject line` et `Preheader` pour les expériences d’e-mail
- `Headline` et `Body` pour les méta-annonces

## Historique

Développez la section _[!UICONTROL Historique]_ d’une expérience pour afficher une chronologie des approbations et des activités. Par exemple, une expérience approuvée affiche la date d’approbation, l’heure et le nom de l’approbateur :

```
Approved

December 10, 2024 at 6:00 PM by Username
```
