---
title: Fonctionnalités vidéo
description: Découvrez la fonctionnalité vidéo des catégories d’attributs utilisées dans GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Video Attributes, Generative AI
exl-id: 0dfdd735-b365-4a15-a6fd-e981697442cb
source-git-commit: 8a5d15df7a347c4ee7767610fc9bb23fc7b71db4
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 1%

---

# Fonctionnalités vidéo

Les fonctions vidéo représentent des éléments, des sons ou des motifs distincts et informatifs dans une vidéo en vue d’une analyse avec [!DNL Insights]. Ces fonctionnalités permettent de classer et de comprendre le contenu vidéo, pour des informations plus précises et plus détaillées. En identifiant divers attributs tels que l&#39;humeur audio, le genre musical et les objets, l&#39;IA peut fournir une analyse complète de la vidéo, aidant à une meilleure prise de décision et la formulation de la stratégie.

## Détection audio

La détection audio dans GenStudio for Performance Marketing implique l’analyse de la piste audio d’une vidéo pour identifier divers attributs. Ce processus de détection détermine l&#39;humeur globale de l&#39;audio en identifiant les types d&#39;audio présents, en marquant des genres ou catégories spécifiques de musique et en extrayant des mots-clés de la parole. En comprenant ces éléments audio, l’IA peut fournir des informations plus précises sur le contenu et le contexte de la vidéo, ce qui améliore le processus global d’analyse et de catégorisation.

## Rechercher des fonctionnalités vidéo

**Pour prévisualiser une vidéo et entendre un échantillon de son** :

1. Dans _[!DNL Insights]_, sélectionnez la vue **[!UICONTROL Attributs]**.

1. Modifiez l’affichage du tableau en sélectionnant **[!UICONTROL Vidéo]**.

1. Sélectionnez une fonctionnalité dans la liste **[!UICONTROL Catégorie d’attributs]**. Pour un exemple audio, sélectionnez **Genre musical**.

1. Sélectionnez un attribut pour une vue détaillée des vidéos qui partagent cette catégorie.

   Par exemple, la catégorie `Music genre` peut avoir `electronic` comme attribut .

1. La page _Détails de l’attribut_ répertorie toutes les vidéos avec cet attribut. Placez le pointeur de la souris sur une vidéo de la liste pour démarrer l’aperçu de la vidéo.

1. Activez le bouton **activer le son** (situé dans le coin inférieur gauche d’un aperçu vidéo) et écoutez le son de l’aperçu vidéo.

Le tableau suivant répertorie les catégories de fonctionnalités vidéo reconnues par l’IA dédiée à GenStudio for Performance Marketing. La liste des attributs détectés pour un contenu multimédia n’est pas exhaustive. Les médias qui contiennent un ensemble riche de fonctionnalités peuvent être limités aux trois fonctionnalités les plus dominantes identifiées par l’IA.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Catégorie | Description | Exemple |
| ------------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| Ambiance Audio | Détermine le ton émotionnel global ou l’atmosphère de la piste audio, comme `calm`, `upbeat` ou `tense`. | `Energetic`, `Happy`, `Emotional Ambient/atmospheric`, `Relaxing`, `Dramatic`, `Expressive/characterful`, `Intense`, `Slow`, `Neutral` |
| Types audio | Ajoute un ou plusieurs types d’audio à la vidéo, tels que `music` ou `speech`. | `Music`, `Speech`, `Silence`, `Special effects`, `Ambience` |
| Catégories | Classe la vidéo dans une ou plusieurs grandes catégories de contenu. | `Entertainment`, `Sports`, `Music`, `Gaming`, `Howto tutorials`, `Fashion and style`, `Film and animation`, `Science and technology`, `Autos and vehicles`, `Pets and animals`, `People and blogs`, `News and politics`, `Social causes and activism`, `Travel and events`, `Education` `Sales and offers` |
| Catégorie de musique | Classification large du genre musical lorsque la musique est présente dans la vidéo. Cela permet d’identifier le type général de musique, tel que les styles `contemporary` ou `traditional`. | `Contemporary/pop music`, `Traditional/folk-based music`, `Instrumental/orchestral music`, `Rock music`, `Acoustic/unplugged music`, `Specialised/occasional music`, `Experimental/unique music` |
| Genre de musique | Classification spécifique du style musical lorsque la musique est présente dans la vidéo, ce qui permet une identification plus détaillée de la musique, telle que la `electronic` ou la `jazz`. | `electronic`, `hip-hop`, `dance`, `novelty`, `rock`, `world`, `reggae`, `pop`, `film`, `jazz`, `background`, `latin` |
| Objets | Identifie un ou plusieurs éléments, entités et éléments qui apparaissent dans la vidéo. | Les valeurs sont trop nombreuses, mais certains exemples incluent : `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap` |
| Orientation | Alignement de la vidéo par rapport à sa largeur et sa hauteur. Détecte s’il est plus large que haut (paysage), plus haut que large (portrait) ou égal en largeur et en hauteur (carré). | `landscape`, `portrait`, `square` |
| Personnes | Lorsqu’au moins une personne est présente, un ou plusieurs attributs peuvent décrire la personne ou les personnes présentes dans la vidéo. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people` |
| Scènes | Identifie le paramètre ou l’environnement au sein d’une vidéo, fournissant un contexte sur l’endroit où la vidéo a été réalisée ou le type d’emplacement représenté. | Les valeurs sont trop nombreuses, mais certains exemples incluent : `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge` |
| Styles | Détecte les traitements visuels appliqués aux éléments vidéo, tels que ceux utilisés dans After Effects ou Lightroom. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `matte`, `neon` |
| Balises | Détecte d’autres caractéristiques vidéo qui ne relèvent pas d’une classification spécifique. Les balises fournissent un contexte et des métadonnées supplémentaires sur la vidéo. | Les valeurs sont trop nombreuses, mais certains exemples incluent : `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing` |
