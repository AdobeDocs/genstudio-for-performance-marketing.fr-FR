---
title: Préparation d’un modèle de métadonnées publicitaires pour Adobe GenStudio for Performance Marketing
description: Découvrez comment créer un modèle de métadonnées publicitaires personnalisé pour Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
source-git-commit: ce08231cb723bec3d80a732837b72a435d3b552d
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Préparation du modèle de métadonnées publicitaires pour Adobe GenStudio for Performance Marketing

La création d’un modèle de méta-publicité implique une approche structurée adaptée aux médias sociaux. Une fois qu’un modèle de métadonnées publicitaires a été conçu et testé, vous pouvez le préparer pour le chargement et l’utilisation dans GenStudio for Performance Marketing.

## Ajouter des instructions

Avant de préparer un modèle de métadonnées publicitaires, assurez-vous d’avoir ajouté [des instructions](/help/user-guide/guidelines/overview.md) à votre GenStudio for Performance Marketing et de leur avoir fourni des informations complètes sur les marques pertinentes. Les [directives de marque](/help/user-guide/guidelines/brands.md) influent directement sur le contenu généré.

**Exemple** : si vous souhaitez que le corps d’un modèle de métadonnées publicitaires ne dépasse pas 500 caractères, ajoutez cette exigence au [guide du canal](/help/user-guide/guidelines/brands.md#channel-guidelines) pour le champ &quot;body&quot;.

Si des instructions ne sont pas ajoutées à GenStudio for Performance Marketing, les valeurs par défaut sont utilisées.

## Concevoir un modèle

En règle générale, un concepteur crée la conception visuelle d’un modèle dans un programme de conception tel qu’Adobe XD.

Voir [Eléments de modèle](use-templates.md#template-elements) et [Exemples de modèles](/help/user-guide/content/customize-template.md#template-examples).

### Spécifications des publicités

GenStudio for Performance Marketing prend en charge ces proportions pour les métadonnées publicitaires :

* Carré (1:1) : 1 080 x 1 080 pixels
* Vertical (4:5) : 1 080 x 1 350 pixels
* Article (9:16) : 1 080 x 1 920 pixels

Si la publicité n’est pas conçue dans l’une de ces proportions, GenStudio for Performance Marketing recadre automatiquement l’image à la taille appropriée.

## Test d’un modèle de métadonnées publicitaires

Testez votre modèle à l’aide de Meta’s Creative Hub pour voir à quoi ressemble la publicité à différents emplacements, comme dans un flux ou un article.

Utilisez votre diffusion email ou votre plateforme de vérification pour tester votre email et vérifier qu’il s’affiche correctement sur différents clients et appareils de messagerie.

## Définition des zones de contenu générées

Définissez les zones de votre modèle de courrier électronique qui doivent être renseignées dynamiquement avec le contenu de GenStudio for Performance Marketing.

Pour définir les zones de contenu générées :

* Identifiez les éléments de texte dans le modèle que GenStudio for Performance Marketing doit générer automatiquement, tels que le titre ou CTA.
* Adaptez votre modèle d’HTML en y insérant des espaces réservés à l’aide de la syntaxe Handlebars .

Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders).

## Prévisualiser le modèle

Contrôlez la visibilité de zones de contenu spécifiques avec des assistants intégrés. Par exemple, incluez des paramètres de suivi aux liens dans un modèle exporté tout en conservant des liens d’aperçu propres.

Voir [Aperçu du modèle](/help/user-guide/content/customize-template.md#template-preview).

## Télécharger et utiliser un modèle

Une fois votre modèle conçu, codé, testé et prévisualisé, téléchargez-le dans GenStudio for Performance Marketing afin de l’utiliser pour générer du contenu marketing entièrement nouveau.

Voir [Utilisation de modèles](use-templates.md).
