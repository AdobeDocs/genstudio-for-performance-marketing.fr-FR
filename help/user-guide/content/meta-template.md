---
title: Préparation d’un modèle de méta-annonce pour Adobe GenStudio for Performance Marketing
description: Découvrez comment créer un modèle de méta-annonce personnalisé pour Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
hidefromtoc: true
recommendations: noCatalog
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Préparation d’un modèle de méta-annonce pour Adobe GenStudio for Performance Marketing

La création d’un MetaAdTemplate implique une approche structurée et adaptée aux médias sociaux. Une fois qu’un modèle de méta-annonce a été conçu et testé, vous pouvez le préparer pour le télécharger et l’utiliser dans GenStudio for Performance Marketing.

## Ajout d’instructions

Avant de préparer un modèle de méta-annonce, assurez-vous d’avoir ajouté des [directives](/help/user-guide/guidelines/overview.md) à votre GenStudio for Performance Marketing et de les avoir renseignées avec des informations complètes pour les marques pertinentes. Les [ directives de la marque ](/help/user-guide/guidelines/brands.md) influencent directement le contenu généré.

**Exemple** : si vous souhaitez que le corps d’un modèle de méta-annonce ne dépasse pas 500 caractères, ajoutez cette exigence aux [directives relatives aux canaux](/help/user-guide/guidelines/brands.md#channel-guidelines) pour le champ « corps ».

Si des instructions ne sont pas ajoutées à GenStudio for Performance Marketing, les valeurs par défaut sont utilisées.

## Conception d’un modèle

En règle générale, un concepteur crée la conception visuelle d’un modèle dans un programme de conception tel qu’Adobe XD.

Voir [Éléments de modèle](use-templates.md#template-elements) et [Exemples de modèle](/help/user-guide/content/customize-template.md#template-examples).

### Spécifications publicitaires

GenStudio for Performance Marketing prend en charge les proportions suivantes pour les méta-annonces :

* Carré (1:1) : 1 080 x 1 080 pixels
* Vertical (4:5) : 1 080 x 1 350 pixels
* Histoire (9:16) : 1080 x 1920 pixels

Si la publicité n’est pas conçue dans l’un de ces proportions, GenStudio for Performance Marketing recadre automatiquement l’image à la taille appropriée.

## Test d’un modèle de métadonnées

Testez votre modèle à l’aide du Creative Hub de Meta pour voir à quoi ressemble la publicité dans différents emplacements, tels qu’un flux ou une histoire.

Utilisez votre plateforme de diffusion ou de relecture par e-mail pour tester votre e-mail et vérifier qu’il s’affiche correctement sur différents clients de messagerie et appareils.

## Définir les zones de contenu générées

Définissez les zones de votre modèle d’e-mail qui doivent être renseignées dynamiquement avec le contenu de GenStudio for Performance Marketing.

Pour définir les zones de contenu générées :

* Identifiez les éléments de texte du modèle que GenStudio for Performance Marketing doit générer automatiquement, tels que le titre ou CTA.
* Adaptez votre modèle HTML en y insérant des espaces réservés à l’aide de la syntaxe Handlebars.

Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders).

## Prévisualiser le modèle

Contrôlez la visibilité de zones de contenu spécifiques à l’aide des assistants intégrés. Par exemple, incluez les paramètres de suivi aux liens dans un modèle exporté tout en conservant des liens d’aperçu propres.

Voir [ Aperçu du modèle ](/help/user-guide/content/customize-template.md#template-preview).

## Télécharger et utiliser le modèle

Une fois votre modèle conçu, codé, testé et prévisualisé, chargez-le dans GenStudio for Performance Marketing pour l’utiliser dans la génération d’un tout nouveau contenu marketing.

Voir [Utilisation de modèles](use-templates.md).
