---
title: Éditeur de code de modèle
description: Découvrez comment utiliser l’éditeur de code de modèle dans GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 19d0b8b929e293179a091cc7b5a6a1268b0abbbd
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Éditeur de code de modèle

L’éditeur de code de modèle est conçu pour vous aider à vérifier et à affiner votre modèle pour une utilisation optimale lors de la génération de nouvelles expériences avec GenStudio for Performance Marketing. L’éditeur prend en charge la syntaxe Handlebars, qui utilise des espaces réservés dans le modèle pour indiquer où GenStudio for Performance Marketing doit générer du contenu pour vous.

>[!TIP]
>
>Avant de charger le code HTML du modèle dans la vue [!DNL Content] _Modèles_, préparez votre modèle en insérant des espaces réservés de contenu définis dans les conseils [Personnalisation des modèles](customize-template.md).

## Vérifier les champs détectés

Le volet _[!UICONTROL Vérifier les champs détectés]_ affiche une liste des champs que GenStudio for Performance Marketing reconnaît dans votre modèle. Passez en revue la liste et vous pouvez faire défiler le code HTML pour consulter la formation de votre modèle.

![Affichage de l’éditeur de code](/help/assets/template-detected-fields.png "Vérification des champs détectés"){width="600" zoomable="yes"}

Si vous remarquez qu’un champ est manquant dans la liste, recherchez votre code de modèle et recherchez l’emplacement du champ manquant. Insérez l’espace réservé approprié en utilisant la syntaxe Handlebars et un [ nom de champ reconnu ](/help/user-guide/content/customize-template.md#recognized-field-names). Utilisez le formulaire Rechercher et remplacer , qui s’affiche au bas de l’éditeur de code, pour rechercher des chaînes spécifiques dans le code. (Windows `CTRL`+`F` ou macOS `CMD`+`F`)

### Effectuer une correction

Si votre modèle contient des erreurs, un message de `Template is invalid` contenant une brève explication du problème peut s’afficher. Dans l’exemple suivant, le message indique que le champ `_image` n’est pas conforme à la convention d’affectation des noms de champ établie dans le modèle multipod. Le message indique en outre que vous devez mettre à jour le nom du champ avec le préfixe correct. Recherchez le champ `_image` dans l’éditeur de code de modèle, puis mettez à jour le nom comme indiqué.

![Corriger le modèle non valide](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

Le volet _[!UICONTROL Vérifier les champs détectés]_ se met à jour pour refléter les modifications que vous avez apportées. Une fois que vous êtes convaincu que les champs sont corrects et complets, cliquez sur **[!UICONTROL Suivant]** pour continuer [à charger votre modèle](/help/user-guide/content/use-templates.md#add-a-template).
