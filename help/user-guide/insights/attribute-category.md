---
title: Catégories d’attributs
description: Découvrez les catégories d’attributs utilisées dans GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
last-substantial-update: 2024-11-11T00:00:00Z
exl-id: c3b51ef2-56ac-4dd8-98b7-79185b5998d0
source-git-commit: 976358742e598b55b1f0c4ca4664d2bcd8f1e9b9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 2%

---

# Catégories d’attributs

Une catégorie d’attributs est un groupe de classification qui organise les attributs associés partageant une caractéristique commune. Ces catégories permettent de rationaliser la découverte, l’identification et la compréhension d’attributs spécifiques en fournissant un plus grand contexte et en facilitant leur application et leur utilisation.

GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités de machine learning pour étudier les images, les vidéos et le texte et appliquer des [!UICONTROL attributs de ressource] en fonction d’une probabilité d’exactitude. La liste des attributs d’une ressource n’est pas exhaustive. Les Assets qui contiennent un riche ensemble de fonctionnalités peuvent être limitées aux trois fonctionnalités les plus dominantes identifiées par l’IA.

## Fonctionnalités d’image

Les fonctions d’image représentent des éléments ou des modèles distincts et informatifs d’une image utilisés pour une analyse avec [!DNL Insights]. Le tableau suivant répertorie les catégories de fonctionnalités d’image reconnues par l’IA dédiée à GenStudio for Performance Marketing.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Catégorie | Description | Exemple |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Angle de la caméra | Emplacement et angle de la caméra par rapport au sujet. |                                                                                                                                                                                |
| Distance du sujet | Distance entre la caméra et le sujet d’une image. | `close up`, `mid shot`, `long shot` |
| Paramètre de la caméra | Configuration des commandes de la caméra pour produire l’image. |                                                                                                                                                                                |
| Couleur et ton | Évalue les couleurs utilisées dans les éléments d’image. Identifie une à trois couleurs parmi un ensemble de 40 couleurs prédéterminées dans les calques d’image suivants : <br>**[!UICONTROL Couleurs de premier plan ]**—Éléments du calque avant de l’image<br>**[!UICONTROL Couleurs d’arrière-plan]**—Éléments du calque arrière d’une image | Valeurs de couleur : `Red`, `Dark_Red`, `Green`, `Bright_Green`, `Dark_Green`, `Light_Green`, `Mud_Green`, `Blue`, `Dark_Blue`, `Light_Blue`, `Royal_Blue`, `Black`, `White`, `Off_White`, `Gray`, `Dark_Gray`, `Silver`, `Cream`, `Magenta`, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark_Brown`, `Violet`, `Pink`, `Dark_Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, `Orange` `Beige` `Lilac` `Olive` |
| Température de couleur | Décrit la chaleur générale ou la fraîcheur des couleurs de l’image. | Valeurs de ton ou de température : `warm`, `cool`, `neutral`<br>![couleurs et tons frais](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Style de l’image | Traitement visuel d’une image. |                                                                                                                                                                                |
| Condition d&#39;éclairage | Type de lumière dans une image. |                                                                                                                                                                                |
| Objets | Identifie un ou plusieurs éléments, entités et éléments qui constituent l’image. | ![tournesol, plan, objet floral](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Orientation | Position de l’image par rapport aux proportions. | `landscape`, `portrait`, `square` |
| Personnes | Lorsqu’au moins une personne est présente, un ou plusieurs attributs peuvent décrire la ou les personnes dans l’image. | ![femme dansant](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Genres de photographie | Détecte l’objet et la technique utilisés pour capturer une image, telle que `abstract` ou `landscape` (différente de l’orientation paysage). |           |
| Scènes | Détecte le paramètre ou l’environnement représenté dans une image. |                                             |
| Balises | Détecte les objets, les éléments et les autres caractéristiques d’image qui ne relèvent pas d’une classification spécifique. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Fonctionnalités vidéo

Les fonctions d’image représentent des éléments, des sons ou des motifs distincts et informatifs dans une vidéo en vue d’une analyse avec [!DNL Insights]. Le tableau suivant répertorie les catégories de fonctionnalités vidéo reconnues par l’IA dédiée à GenStudio for Performance Marketing.

| Catégorie | Description | Exemple |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Genre audio | En présence de musique, la vidéo peut recevoir une classification de style musical, tel que `electronic` ou `classical`. |          |
| Catégorie de genre audio | Lorsque la musique est présente, la vidéo peut recevoir une classification large de genre musical, tel que `acoustic` ou `traditional`. |          |
| Ambiance Audio | Décrit l’atmosphère générale ou le ton du son, tel que `relaxing` ou `energetic`. |          |
| Types audio | En présence d’un son, la vidéo peut recevoir une balise pour un ou plusieurs types audio, tels que `music` ou `speech`. |          |
| Objets | Identifie un ou plusieurs éléments, entités et éléments qui apparaissent tout au long de la vidéo. | ![objets en vidéo](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Orientation | Position de la vidéo par rapport au format de l’image. | `landscape`, `portrait`, `square` |
| Personnes | Lorsqu’au moins une personne est présente, un ou plusieurs attributs peuvent décrire la ou les personnes dans la vidéo. |        |
| Scènes | Le paramètre ou l’environnement représenté dans la vidéo. |        |
| Styles | Détecte les traitements visuels appliqués aux éléments de la vidéo, tels que les `matte` ou les `neon`. |        |
| Balises | Détecte les objets, les éléments et les autres caractéristiques vidéo qui ne relèvent pas d’une classification spécifique. |        |

## Fonctionnalités de texte

Les fonctions de texte incluent des nombres pour certains éléments de texte, tels que des mots, des phrases, des émoticônes, ainsi que des classifications pour la sémantique, l’émotion et le ton utilisés pour l’analyse avec [!DNL Insights]. Le texte peut également recevoir un score de lisibilité. Bientôt disponible.

<!-- Not yet approved by legal

The following table lists the image feature categories recognized by the GenStudio for Performance Marketing AI.

| Category             | Description | Example |
|----------------------|-------------|--------|
| Emojis Count         |             |        |
| HashTags Count       |             |        |
| Keywords             |             |        |
| Marketing Emotions   |             |        |
| Narratives           | Text that represents an overarching situation, theme, or a story. Narratives can communicate values, purpose, or identity that resonates with consumers on many levels.   |        |
| Persuasion Strategies|             |        |
| Readability          |             |        |
| Tone of voice        | | |
-->
