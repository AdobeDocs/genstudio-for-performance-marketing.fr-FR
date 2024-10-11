---
title: Préparation d’un modèle de courrier électronique pour Adobe GenStudio for Performance Marketing
description: Découvrez comment créer un modèle de courrier électronique personnalisé pour Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 478815d74a742cdc05d3f1faebf27d5adc04d417
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Préparer le modèle de courrier électronique pour Adobe GenStudio for Performance Marketing

En règle générale, un concepteur crée la conception visuelle d’un modèle dans un programme de conception tel qu’Adobe XD. Une fois qu’un modèle d’email a été conçu, codé et testé, vous pouvez le préparer pour le chargement et l’utilisation dans GenStudio for Performance Marketing.

Voir [Eléments de modèle](use-templates.md#template-elements).

## Ajouter des instructions

Avant de préparer un modèle de métadonnées publicitaires, assurez-vous d’avoir ajouté [des instructions](/help/user-guide/guidelines/overview.md) à votre GenStudio for Performance Marketing et de leur avoir fourni des informations complètes sur les marques pertinentes. Les [directives de marque](/help/user-guide/guidelines/brands.md) influent directement sur le contenu généré.

**Exemple** : si vous souhaitez que le corps d’un modèle de courrier électronique ne dépasse pas 500 caractères, ajoutez cette exigence au [guide du canal](/help/user-guide/guidelines/brands.md#channel-guidelines) pour le champ &quot;body&quot;.

Si des instructions ne sont pas ajoutées à GenStudio for Performance Marketing, les valeurs par défaut sont utilisées.

## Code un modèle de courrier électronique

Une fois le modèle conçu, il est codé à l’aide d’HTML et de CSS intégré. Le code doit être propre et réactif pour divers appareils.

Voir [Exemples de modèles](/help/user-guide/content/customize-template.md#template-examples).

### Emails multi-section

Vous pouvez utiliser des [invites structurées](/help/user-guide/effective-prompts.md#structured-prompts) pendant la génération du contenu pour demander à GenStudio for Performance Marketing de générer des contenus variables par section d&#39;un email.

Par exemple, si les sections de votre modèle de courrier électronique comportent le préfixe `Pod`—`Pod1` et `Pod2`, l’invite structurée de génération de contenu peut inclure des directives spécifiques pour ces sections de courrier électronique. GenStudio for Performance Marketing correspond à la directive spécifique à la section dans votre invite de la section d’email associée et génère du contenu aligné sur les directives.

Voir [ invites structurées](/help/user-guide/effective-prompts.md#structured-prompts).

## Tester un modèle d&#39;email

Utilisez votre diffusion email ou votre plateforme de vérification pour tester votre email et vérifier qu’il s’affiche correctement sur différents clients et appareils de messagerie.

Vérifiez que votre modèle d&#39;email répond aux critères suivants :

* La mise en page s’ajuste pour différentes tailles d’écran à l’aide de requêtes multimédias CSS
* Vous pouvez cliquer sur les boutons et accéder à l’emplacement prévu
* Le modèle d’email est lisible et utilisable sur les appareils mobiles

## Définition des zones de contenu générées

Définissez les zones de votre modèle de courrier électronique qui doivent être renseignées dynamiquement avec le contenu de GenStudio for Performance Marketing.

Pour définir les zones de contenu générées :

* Identifiez les éléments de texte dans le modèle que GenStudio for Performance Marketing doit générer automatiquement, tels que le titre ou CTA.
* Adaptez votre modèle d’HTML en y insérant des espaces réservés à l’aide de la syntaxe Handlebars .

Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders).

## Prévisualiser le modèle

Contrôlez la visibilité de zones de contenu spécifiques avec des assistants intégrés. Par exemple, vous pouvez inclure des paramètres de suivi aux liens dans un modèle exporté tout en conservant des liens d’aperçu propres.

Voir [Aperçu du modèle](/help/user-guide/content/customize-template.md#template-preview).

## Télécharger et utiliser un modèle

Une fois votre modèle conçu, codé, testé et prévisualisé, vous pouvez le charger dans GenStudio for Performance Marketing afin de l’utiliser pour générer du nouveau contenu marketing.

Voir [Utilisation de modèles](use-templates.md).
