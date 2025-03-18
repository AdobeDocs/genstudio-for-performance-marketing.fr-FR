---
title: Préparation d’un modèle d’e-mail pour Adobe GenStudio for Performance Marketing
description: Découvrez comment créer un modèle d’e-mail personnalisé pour Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
hidefromtoc: true
recommendations: noCatalog
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Préparation du modèle d’e-mail pour Adobe GenStudio for Performance Marketing

En règle générale, un concepteur crée la conception visuelle d’un modèle dans un programme de conception tel qu’Adobe XD. Une fois qu’un modèle d’e-mail a été conçu, codé et testé, vous pouvez le préparer pour le charger et l’utiliser dans GenStudio for Performance Marketing.

Voir [Éléments de modèle](use-templates.md#template-elements).

## Ajout d’instructions

Avant de préparer un modèle de méta-annonce, assurez-vous d’avoir ajouté des [directives](/help/user-guide/guidelines/overview.md) à votre GenStudio for Performance Marketing et de les avoir renseignées avec des informations complètes pour les marques pertinentes. Les [ directives de la marque ](/help/user-guide/guidelines/brands.md) influencent directement le contenu généré.

**Exemple** : si vous souhaitez que le corps d’un modèle d’e-mail ne dépasse pas 500 caractères, ajoutez cette exigence aux [instructions de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) pour le champ « corps ».

Si des instructions ne sont pas ajoutées à GenStudio for Performance Marketing, les valeurs par défaut sont utilisées.

## Coder un modèle d’e-mail

Une fois qu’un modèle est conçu, il est codé à l’aide d’HTML et du code CSS intégré. Le code doit être propre et réactif pour divers appareils.

Voir [ Exemples de modèles ](/help/user-guide/content/customize-template.md#template-examples).

### Emails à plusieurs sections

Vous pouvez utiliser des [invites structurées](/help/user-guide/effective-prompts.md#structured-prompts) lors de la génération du contenu pour demander à GenStudio for Performance Marketing de générer un contenu variable par section d’un email.

Par exemple, si les sections de votre modèle d’e-mail comportent le préfixe `Pod`—`Pod1` et `Pod2`, l’invite structurée de génération de contenu peut inclure des directives spécifiques pour ces sections d’e-mail. GenStudio for Performance Marketing fait correspondre la directive spécifique à la section de votre invite à la section d’e-mail associée et génère du contenu aligné sur les directives.

Voir [Invites structurées](/help/user-guide/effective-prompts.md#structured-prompts).

## Test d’un modèle d’e-mail

Utilisez votre plateforme de diffusion ou de relecture par e-mail pour tester votre e-mail et vérifier qu’il s’affiche correctement sur différents clients de messagerie et appareils.

Testez pour vous assurer que votre modèle d’e-mail répond aux critères suivants :

* La disposition s’adapte à différentes tailles d’écran à l’aide de requêtes multimédias CSS
* Vous pouvez cliquer sur les boutons et accéder à l’emplacement prévu
* Le modèle d’e-mail est lisible et utilisable sur les appareils mobiles

## Définir les zones de contenu générées

Définissez les zones de votre modèle d’e-mail qui doivent être renseignées dynamiquement avec le contenu de GenStudio for Performance Marketing.

Pour définir les zones de contenu générées :

* Identifiez les éléments de texte du modèle que GenStudio for Performance Marketing doit générer automatiquement, tels que le titre ou CTA.
* Adaptez votre modèle HTML en y insérant des espaces réservés à l’aide de la syntaxe Handlebars.

Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders).

## Prévisualiser le modèle

Contrôlez la visibilité de zones de contenu spécifiques à l’aide des assistants intégrés. Par exemple, vous pouvez inclure des paramètres de suivi aux liens d’un modèle exporté tout en conservant des liens d’aperçu propres.

Voir [ Aperçu du modèle ](/help/user-guide/content/customize-template.md#template-preview).

## Télécharger et utiliser le modèle

Une fois votre modèle conçu, codé, testé et prévisualisé, vous pouvez le charger dans GenStudio for Performance Marketing pour l’utiliser dans la génération d’un tout nouveau contenu marketing.

Voir [Utilisation de modèles](use-templates.md).
