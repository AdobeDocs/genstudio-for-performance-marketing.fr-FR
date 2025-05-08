---
title: Fonctionnalités d’image
description: Découvrez la fonctionnalité d’image des catégories d’attributs utilisées dans GenStudio for Performance Marketing.
level: Intermediate
feature: Reporting and Insights, Image Attributes, Generative AI
exl-id: b7e3d202-4085-48a4-a6ba-c950dfd52233
source-git-commit: e3534ace3679e512cce6a137aadd4c483b5a868a
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 0%

---

# Fonctionnalités d’image

Les fonctions d’image représentent des éléments ou des modèles distincts et informatifs d’une image utilisés pour une analyse avec [!DNL Insights]. Ces fonctionnalités permettent de catégoriser et de comprendre le contenu visuel, ce qui permet d’obtenir des informations plus précises et plus détaillées. En identifiant divers attributs tels que le style, la couleur et les objets, l’IA peut fournir une analyse complète de l’image, ce qui contribue à une meilleure prise de décision et à une meilleure formulation de la stratégie.

## Détection des styles

La définition du _style d’image_ sert de base pour identifier d’autres caractéristiques d’image. L’IA peut appliquer les techniques d’analyse appropriées et reconnaître les caractéristiques pertinentes, ce qui permet une compréhension plus complète de l’image. Chaque style possède des caractéristiques visuelles distinctes qui influencent la manière dont l’image est perçue et analysée.

Si le style d’image est identifié comme un `photograph`, l’IA analyse les caractéristiques supplémentaires pour `camera settings`, `camera proximity` et `Photography genres`. Ces caractéristiques sont spécifiques aux photographies et fournissent des informations plus précises sur la composition et la qualité de l’image. Consultez les [28 types de styles de photographie](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html) dans Adobe _Découvrez la photographie_ et découvrez les types de photographie les plus populaires ainsi que la terminologie fondamentale.

Si le style d’image est identifié comme un `sketch` ou un `digital cartoon`, un autre ensemble de caractéristiques peut s’avérer pertinent. Cette approche hiérarchique permet de s’assurer que l’analyse est contextuellement précise et adaptée au type spécifique d’image examiné.

## Rechercher des fonctionnalités d’image

**Pour afficher des images dans une catégorie d’attributs spécifique** :

1. Dans _[!DNL Insights]_, sélectionnez la vue **[!UICONTROL Attributs]**.

1. Modifiez l’affichage du tableau en sélectionnant **[!UICONTROL Images]**.

1. Sélectionnez une fonction d’image dans la liste **[!UICONTROL Catégorie d’attributs]**, par exemple `Scenes`.

1. Sélectionnez un attribut pour obtenir une vue détaillée des images qui partagent cette catégorie.

   Par exemple, la catégorie `Scenes` peut avoir `restaurant` comme attribut .

1. La page _Détails de l’attribut_ répertorie toutes les images avec cet attribut.

Le tableau suivant répertorie les catégories de fonctionnalités d’image reconnues par l’IA dédiée à GenStudio for Performance Marketing. La liste des attributs détectés pour le contenu multimédia n’est pas exhaustive. Les médias qui contiennent un ensemble riche de fonctionnalités peuvent être limités aux trois fonctionnalités les plus dominantes identifiées par l’IA.

<!-- For the writer: turn off word wrap to work with these tables. Option + Z -->

| Catégorie | Description | Exemple |
| ----------------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Répartition de l’attention | Niveau d’attention de la visionneuse réparti sur une image, indiquant le degré de mise au point que différentes zones de l’image peuvent recevoir. Une distribution plus élevée signifie qu&#39;aucune zone ne domine le focus du spectateur, tandis qu&#39;une distribution plus faible signifie qu&#39;un ou deux points focaux captent l&#39;attention du spectateur. | `high`, `medium`, `low`<p>Exemple de répartition `low` à gauche et de répartition `high` à droite :<p>![jeu de balle à faible et à forte distribution](/help/assets/category/image-attn-lowhigh.png "différence de distribution faible et élevée"){width="200" zoomable="yes"} |
| Angle de la caméra | Perspective à partir de laquelle la caméra capture le sujet, ce qui affecte la perception et l&#39;interprétation de l&#39;image par le spectateur. Si le style d’image est `photograph`, cette caractéristique est identifiée. | `Low angle`, `High angle`, `Eye level`, `Neutral angle`, `Overhead view`, `Bird's eye view`<p>Exemple de `Overhead view` :<p>![Vue de dessus](/help/assets/category/image-camera-angle.png "Paire de shorts depuis le dessus"){width="200" zoomable="yes"} |
| Paramètre de la caméra | Réglages et configurations spécifiques des commandes de la caméra qui influencent l&#39;aspect final et la qualité de l&#39;image. Si le style d’image est `photograph`, cette caractéristique est identifiée. | `Fast shutter speed`, `Long exposure`, `Bokeh blur`, `Motion blur`, `Tilt-shift blur`, `Flash`, `Wide-angle`, `Black and white`, `Double-exposure`, `Macro`, `Normal mode`<p>Exemple de paramétrage `Fast shutter speed` :<p>![Vitesse d&#39;obturation rapide](/help/assets/category/image-camera-setting.png "Surfer sur une vague"){width="200" zoomable="yes"} |
| Couleur et ton | Les couleurs et les qualités tonales d’une image. Identifie jusqu’à trois couleurs à partir d’un jeu prédéfini de 40 couleurs dans différents calques d’image :<p>**[!UICONTROL Couleurs de premier plan]**—couleurs du calque avant de l’image<br>**[!UICONTROL Couleurs d’arrière-plan ]**—couleurs du calque arrière de l’image | Valeurs de couleur : `Red`, `Dark Red`, `Green`, `Bright Green`, `Dark Green`, `Light Green`, `Mud Green`, `Blue`, `Dark Blue`, `Light Blue`, `Royal Blue`, `Black`, `White`, `Off White`, `Gray`, `Dark Gray`, `Silver`, `Cream`, `Magenta`, `Cyan`, `Yellow`, `Mustard`, `Khaki`, `Brown`, `Dark Brown`, `Violet`, `Pink`, `Dark Pink`, `Maroon`, `Tan`, `Purple`, `Lavender`, `Turquoise`, `Plum`, `Gold`, `Emerald`, `Orange` `Beige` `Lilac` `Olive` |
| Température de couleur | Décrit la chaleur générale ou la fraîcheur des couleurs de l’image. | Valeurs de ton ou de température : `warm`, `cool`, `neutral`<br>![couleurs et tons frais](/help/assets/category/image-color-temp.png "température de couleur avec arrière-plan frais et plusieurs objets colorés"){width="200" zoomable="yes"} |
| Densité du contenu | Concentration des éléments visuels et des détails dans une image, indiquant la quantité d’informations regroupées dans l’espace visuel.<p>Contrairement à la distribution de l’attention, qui mesure la manière dont la mise au point est répartie sur différentes zones d’une image, la densité de contenu se concentre sur la quantité d’informations visuelles présentes. Une densité de contenu plus élevée signifie que davantage d’éléments sont présents. | `high`, `medium`, `low`<p>Exemple de densité de `low` à gauche et de densité de `high` à droite :<p>![jeu de balle faible et haute densité](/help/assets/category/image-attn-lowhigh.png "différence de densité de contenu faible et élevée"){width="200" zoomable="yes"} |
| Style de l’image | Traitement visuel d’une image, telle qu’une photographie ou un schéma. Une fois que l’IA détermine le style d’image, d’autres caractéristiques peuvent être identifiées. Par exemple, si l’image est une photographie, les paramètres de l’appareil photo, sa proximité et les conditions d’éclairage peuvent s’appliquer. | `Photograph`, `Photograph with text overlay`, `Sketch`, `Painting`, `Digital cartoon`, `Infographics`, `Graphic design`, `Collage`, `Software screenshot`<p>Exemple de dessin animé de style![style d’image](/help/assets/category/image-style.png "style d’image `digital cartoon` d’un chat"){width="200" zoomable="yes"} |
| Condition d&#39;éclairage | Décrit la qualité et les caractéristiques de la lumière dans une image, affectant son humeur, son ton et sa visibilité. | `Golden hour`, `Blue hour`, `Midday`, `Overcast`, `Night`, `Daylighting`, `Incandescent`, `Fluorescent`, `Colorful`, `Studio`<p>Exemple de condition `daylighting` :<p>![Personne et chien sur le trottoir en condition d&#39;éclairage ](/help/assets/category/image-lighting.png " jourCondition d&#39;éclairage de jour"){width="200" zoomable="yes"} |
| Objets | Identifie un ou plusieurs éléments, entités et éléments qui constituent l’image. | Les valeurs sont trop nombreuses, mais certains exemples incluent : `backpack`, `book`, `hawk`, `glasses`, `fish`, `pencil`, `mountain bike`, `soap`<p>Exemple d&#39;objets `toucan` et `bird` :<p>![oiseau, objet toucan](/help/assets/category/image-objects-bird.png "Conception graphique de l&#39;objet Toucan oiseau"){width="200" zoomable="yes"} |
| Orientation | Alignement de l’image par rapport à sa largeur et sa hauteur. Détecte s’il est plus large que haut (paysage), plus haut que large (portrait) ou égal en largeur et en hauteur (carré). | `landscape`, `portrait`, `square`<p>Exemple d&#39;orientation `square` :<p>![croquis carré](/help/assets/category/image-orientation-square.png "croquis floral d&#39;orientation carrée"){width="200" zoomable="yes"} |
| Personnes | Lorsqu’au moins une personne est présente, un ou plusieurs attributs peuvent décrire la ou les personnes dans l’image. | `person`, `woman`, `man`, `girl`, `boy`, `social group`, `kid`, `crowd`, `people`<p>Exemple de personnes `woman` et `person` catégories :<p>![personne femme avec caméra](/help/assets/category/image-people.png "personne gérant une caméra"){width="200" zoomable="yes"} |
| Genres de photographie | Détecte l’objet et la technique utilisés pour capturer une image, telle que `Abstract` ou `Landscape` (différente de l’orientation paysage). | `Architecture`, `Astro`, `Landscape`, `Pet`, `Interior`, `Wildlife`, `Night`, `Cityscape`, `Seascape`, `Underwater`, `Storm`, `Adventure sports`, `Fashion`, `Portrait`, `Sports`, `Food`, `Street`, `Event`, `Lifestyle`, `Commercial`, `Group`, `Abstract`, `Minimalist`, `Composite` `Surreal` <p>Voir [Types de photographie](https://www.adobe.com/creativecloud/photography/discover/types-of-photography.html).<p>Exemple de `Adventure sports` :<p>![Personne debout avec un canot](/help/assets/category/image-photography-genres.png "Personne avec une rame debout près d&#39;un canot"){width="200" zoomable="yes"} |
| Scènes | Identifie le paramètre ou l’environnement au sein d’une image, fournissant un contexte sur l’emplacement où l’image a été capturée ou le type d’emplacement représenté. | Les valeurs sont trop nombreuses, mais certains exemples incluent : `lake`, `underwater`, `highway`, `hill`, `log cabin`, `island`, `beach`, `lounge`<p>Exemple de scènes `snow`, `sky`, `winter` et `mountain` reflétées sur un casque :<p>![scène de neige d&#39;hiver](/help/assets/category/image-scenes.png "hiver, neige, ciel et réflexion de scène de montagne"){width="200" zoomable="yes"} |
| Distance du sujet | Distance entre la caméra et le sujet d’une image. | `close up`, `mid shot`, `long shot`<p>Exemple de `Long shot` :<p>![Sommet de montagne long shot](/help/assets/category/image-subject-distance.png "Homme sur un sommet de montagne lointain"){width="200" zoomable="yes"} |
| Styles | Détecte les traitements visuels appliqués aux éléments d’image, tels que ceux utilisés dans Lightroom ou Photoshop. | `design`, `illustration`, `logo`, `square`, `cartoon`, `art`, `circle`, `circular`<p>Exemple de style de `circular` :<p>![passerelle circulaire dans un récif corallien](/help/assets/category/image-styles-circular.png "portail circulaire dans un récif corallien"){width="200" zoomable="yes"} |
| Balises | Détecte d’autres caractéristiques d’image qui ne relèvent pas d’une classification spécifique. Les balises fournissent un contexte et des métadonnées supplémentaires sur l’image. Par exemple, l’IA peut détecter des objets `helmet` et `motorobike` dans une image et inclure des `riding` sous forme de balise. | Les valeurs sont trop nombreuses, mais certains exemples incluent : `construction`, `gothic`, `healing`, `military`, `selfie`, `football`, `typing`, `dancer`, `dancing`<p>Exemple de balises `dancer` et `dancing` :<p>![balises pour danseur et danseuse](/help/assets/category/image-tags.png "Personne dansante"){width="200" zoomable="yes"} |
