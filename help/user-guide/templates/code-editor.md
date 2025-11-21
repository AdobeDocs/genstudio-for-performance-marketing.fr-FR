---
title: Éditeur de code de modèle
description: Découvrez comment utiliser l’éditeur de code de modèle dans GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
source-git-commit: 9e51e853542d20f0b90b10071f4f26aaae1d6aad
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 1%

---

# Éditeur de code de modèle

L’éditeur de code de modèle est conçu pour vous aider à vérifier et à affiner votre modèle pour une utilisation optimale lors de la génération de nouvelles expériences avec GenStudio for Performance Marketing. L’éditeur prend en charge la syntaxe Handlebars, qui utilise des espaces réservés dans le modèle pour indiquer où GenStudio for Performance Marketing doit générer du contenu pour vous.

>[!TIP]
>
>Avant de charger le code HTML du modèle dans la vue [!DNL Content] _Modèles_, préparez votre modèle en insérant des espaces réservés de contenu définis dans les conseils [Personnalisation des modèles](customize-template.md).

## Vérifier les champs détectés

Le volet _[!UICONTROL Vérifier les champs détectés]_ affiche une liste des champs que GenStudio for Performance Marketing reconnaît dans votre modèle. Passez en revue la liste et vous pouvez faire défiler le code HTML pour consulter la formation de votre modèle.

![Affichage de l’éditeur de code](/help/assets/template-detected-fields.png "Vérification des champs détectés"){width="600"}

Si vous remarquez qu’un champ est manquant dans la liste, recherchez votre code de modèle et recherchez l’emplacement du champ manquant. Insérez l’espace réservé approprié en utilisant la syntaxe Handlebars et un [&#x200B; nom de champ reconnu &#x200B;](/help/user-guide/templates/customize-template.md#recognized-field-names). Utilisez le formulaire Rechercher et remplacer , qui s’affiche au bas de l’éditeur de code, pour rechercher des chaînes spécifiques dans le code. (Windows `CTRL`+`F` ou macOS `CMD`+`F`)

## Ajuster les rôles d’une variable

Vous pouvez sélectionner et modifier des rôles de champ pour les rôles de champ basés sur du texte (par exemple, `headline`, `sub_headline`, `body`, `cta`, `on_image_text`, `custom`) avec une liste déroulante lors de la vérification de la structure du modèle. Les sélections de rôles de champ persistent lors des modifications du modèle afin que les personnalisations ne soient pas perdues, ce qui améliore l’efficacité des workflows.

>[!NOTE]
>
>Les rôles des variables d’image ne peuvent pas être ajustés.

![Sélection de champs multirôles](/help/assets/multirole-dropdown-field.png "Sélection de champs multirôles"){width="600"}

Pour attribuer un rôle à une variable :

1. Recherchez la variable dans le volet _[!UICONTROL Vérifier les champs détectés]_. Ces variables sont automatiquement découvertes.
2. Passez en revue les rôles affectés à chaque variable. Les rôles sont automatiquement attribués mais peuvent être ajustés à l’aide de la liste déroulante pour toute variable du modèle.
3. Ajustez un rôle en sélectionnant un nouveau rôle dans la liste déroulante.
4. Cliquez sur **[!UICONTROL Suivant]** pour continuer.

## Effectuer une correction

Si votre modèle contient des erreurs, un message de `Template is invalid` contenant une brève explication du problème peut s’afficher. Dans l’exemple suivant, le message indique que le champ `_image` n’est pas conforme à la convention d’affectation des noms de champ établie dans le modèle multipod. Le message indique en outre que vous devez mettre à jour le nom du champ avec le préfixe correct. Recherchez le champ `_image` dans l’éditeur de code de modèle, puis mettez à jour le nom comme indiqué.

![Corriger le modèle non valide](/help/assets/animation/template-code-editor.gif){width="600"}

Le volet _[!UICONTROL Vérifier les champs détectés]_ se met à jour pour refléter les modifications que vous avez apportées. Une fois que vous êtes convaincu que les champs sont corrects et complets, cliquez sur **[!UICONTROL Suivant]** pour continuer [à charger votre modèle](/help/user-guide/templates/use-templates.md#add-a-template).

## Problèmes courants liés aux modèles et solutions

| **Erreur** | **Description** | **Solution** |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Échec de l’analyse | Le contenu du modèle n’a pas pu être analysé en tant que barres de contrôle valides. | Recherchez les erreurs de syntaxe HTML et Handlebars dans votre modèle et corrigez-les pour garantir une mise en forme valide des [espaces réservés de contenu](/help/user-guide/templates/customize-template.md#content-placeholders). |
| Groupe non affecté | Un champ d’image dans un modèle d’e-mail multigroupe n’est affecté à aucun groupe. | Vérifiez l’utilisation cohérente des préfixes de section. Chaque [section](/help/user-guide/templates/customize-template.md#sections-or-groups) ne peut utiliser qu’un seul type de champ (`headline`, `body` `image` `cta`). Affectez le champ `image` à un groupe valide dans votre modèle. |
| Image manquante | Un champ d’image obligatoire est manquant. | Un seul champ `image` est requis pour certains types de modèles, tels qu’un Meta, un affichage ou une bannière publicitaire. Ajoutez le champ de `image` requis à votre modèle. |
| Groupe unique non valide | Le modèle d’e-mail contient exactement un groupe, qui n’est pas valide. | Un modèle d’e-mail de base contient un seul ensemble d’éléments de modèle, qui ne nécessitent pas la convention de nommage de groupe telle que définie dans [Sections ou groupes](/help/user-guide/templates/customize-template.md#sections-or-groups). Ajustez votre modèle pour qu’il ne comporte aucune section en supprimant la syntaxe de dénomination des groupes. |
| Aucun champ | Le modèle ne contient aucun champ. | Ajoutez [noms de champ reconnus](/help/user-guide/templates/customize-template.md#recognized-field-names) en utilisant la syntaxe Handlebars à votre modèle dans lequel vous avez besoin de GenStudio for Performance Marketing pour générer un certain type de contenu. |
| Propriétés requises manquantes | Certaines propriétés de métadonnées obligatoires sont manquantes. | Chaque type de modèle a des exigences et des contraintes basées sur les directives du canal. Par exemple, Meta nécessite un format et les publicités display nécessitent des dimensions. [Suivez les instructions relatives aux modèles spécifiques aux canaux](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Nom réservé utilisé | Un nom de champ interdit ou réservé est utilisé. | Certains [noms de champ](/help/user-guide/templates/customize-template.md#recognized-field-names) tels que `subject` ou `introductory_text`, sont réservés. Renommez les champs qui utilisent des noms réservés ou interdits. |
| Trop de champs | Le nombre de champs dépasse la limite globale de 20. | Supprimez les champs inutiles pour vous assurer que le total ne dépasse pas 20. |
| Trop de groupes | Le nombre de groupes dépasse le maximum autorisé pour le canal. | Les modèles Meta, display et LinkedIn n’autorisent pas les sections multiples. L’e-mail nécessite un nom de groupe lors de la définition de deux ou trois sections. Réduisez le nombre de groupes dans votre modèle pour répondre aux exigences du [canal](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Champ non pris en charge | Le modèle utilise un champ que le canal ne prend pas en charge. | Remplacez ou supprimez les champs non pris en charge en fonction des [noms de champ reconnus](/help/user-guide/templates/customize-template.md#recognized-field-names). |
