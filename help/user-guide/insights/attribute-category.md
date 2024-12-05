---
title: Catégories d’attributs
description: Découvrez les catégories d’attributs utilisées dans GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
recommendations: noDisplay
last-substantial-update: 2024-11-11T00:00:00Z
exl-id: c3b51ef2-56ac-4dd8-98b7-79185b5998d0
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 2%

---

# Catégories d’attributs

Une catégorie d’attributs est un groupe de classifications qui organise les attributs connexes partageant une caractéristique commune. Ces catégories permettent de rationaliser la découverte, l’identification et la compréhension d’attributs spécifiques en fournissant un meilleur contexte et en facilitant leur application et leur utilisation.

GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités d’apprentissage automatique pour étudier les images, les vidéos et le texte et appliquer les [!UICONTROL attributs de ressource] en fonction d’une probabilité d’exactitude. La liste des attributs d’une ressource n’est pas exhaustive. Assets qui contient un ensemble riche de fonctionnalités peut être limité aux trois fonctionnalités les plus dominantes identifiées par l’IA.

## Fonctionnalités d’image

Les fonctions d’image représentent des éléments ou des modèles distincts et informatifs au sein d’une image qui sont utilisés pour l’analyse avec [!DNL Insights]. Le tableau suivant répertorie les catégories de fonctionnalités d’image reconnues par l’IA GenStudio for Performance Marketing.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Catégorie | Description | Exemple |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Angle de la caméra | Emplacement et angle de la caméra par rapport à l’objet. |                                                                                                                                                                                |
| Distance du sujet | Distance entre la caméra et le sujet d’une image. | `close up`, `mid shot`, `long shot` |
| Paramètre de caméra | Configuration des commandes de la caméra pour produire l’image. |                                                                                                                                                                                |
| Couleur et ton | Évalue les couleurs utilisées dans les éléments d’image. Identifie une à trois couleurs à partir d’un ensemble de 40 couleurs prédéterminées dans les calques d’image suivants :<br>**[!UICONTROL Couleurs de premier plan ]**—éléments dans la couche avant de l’image<br>**[!UICONTROL Couleurs de fond]**—éléments dans la couche arrière d’une image<p>**[!UICONTROL Température des couleurs]** décrit la chaleur ou la fraîcheur générales des couleurs dans l’image.<br>Valeurs de tonalité ou de température : `warm`, `cool`, `neutral` | ![couleurs et tons frais](../../assets/category/image-color-temp.png){width="200" zoomable="yes"} |
| Style d’image | Traitement visuel d’une image. |                                                                                                                                                                                |
| Condition d’éclairage | Type de lumière dans une image. |                                                                                                                                                                                |
| Objets | Identifie un ou plusieurs éléments, entités et éléments qui constituent l’image. | ![tournesol, plan, objet de fleur](../../assets/category/image-objects.png){width="200" zoomable="yes"} |
| Orientation | Position de l’image par rapport aux proportions. | `landscape`, `portrait`, `square` |
| Personnes | Lorsqu’au moins une personne est présente, un ou plusieurs attributs peuvent décrire la ou les personnes dans l’image. | ![femme dansant](../../assets/category/image-people.png){width="200" zoomable="yes"} |
| Genre de la photographie | Détecte l’objet et la technique utilisés pour capturer une image, par exemple `abstract` ou `landscape` (différent de l’orientation paysage). |           |
| Scènes | Détecte le paramètre ou l’environnement représenté dans une image. |                                             |
| Balises | Détecte les objets, éléments et autres caractéristiques d’image qui ne tombent pas sous une classification spécifique. |                                      |

<!-- Not yet approved by legal
| Attention distribution  | The level of viewer attention spread across an image.                                                 | `high`, `medium`, `low`                                                                                                                                                                                                    |
| Content density         | The amount of information or detail in an image.                                                      | `high`, `medium`, `low`                                                                                                                                                                                                    |
-->

## Fonctionnalités vidéo

Les fonctionnalités d’image représentent des éléments, des sons ou des motifs distincts et informatifs dans une vidéo pour une analyse avec [!DNL Insights]. Le tableau suivant répertorie les catégories de fonctionnalités vidéo reconnues par l’IA GenStudio for Performance Marketing.

| Catégorie | Description | Exemple |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Audio Genre | En présence de musique, la vidéo peut recevoir une classification de style musical, telle que `electronic` ou `classical`. |          |
| Catégorie de genre audio | Lorsque de la musique est présente, la vidéo peut recevoir une classification large de genre musical, comme `acoustic` ou `traditional`. |          |
| Mode audio | Décrit l’atmosphère ou la tonalité générale de l’audio, par exemple `relaxing` ou `energetic`. |          |
| Types audio | En cas de présence audio, la vidéo peut recevoir une balise pour un ou plusieurs types audio, tels que `music` ou `speech`. |          |
| Objets | Identifie un ou plusieurs éléments, entités et éléments qui apparaissent dans la vidéo. | ![ objets dans video](../../assets/category/video-objects.png){width="200" zoomable="yes"} |
| Orientation | Position de la vidéo par rapport aux proportions de l’image. | `landscape`, `portrait`, `square` |
| Personnes | Lorsqu’au moins une personne est présente, un ou plusieurs attributs peuvent décrire la ou les personnes dans la vidéo. |        |
| Scènes | Paramètre ou environnement décrit dans la vidéo. |        |
| Styles | Détecte les traitements visuels appliqués aux éléments de la vidéo, tels que `matte` ou `neon`. |        |
| Balises | Détecte les objets, les éléments et d’autres caractéristiques vidéo qui ne relèvent pas d’une classification spécifique. |        |

## Fonctionnalités textuelles

Les fonctionnalités de texte incluent le nombre de certains éléments de texte, tels que les mots, les phrases, les émoticônes et les classifications pour la sémantique, l’émotion et le ton, qui sont utilisés pour l’analyse avec [!DNL Insights]. Le texte peut également recevoir un score de lisibilité. Bientôt.

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
