---
title: Plug-in Figma pour Adobe GenStudio for Performance Marketing
description: Découvrez comment configurer et utiliser le plug-in Figma pour GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 232fbbc6-c523-4525-8d26-a8ac8d62c035
TQID: https://experienceleague.adobe.com/JKHpT5m-4KZvq-iWF2u11hRaFFRhKMo-ofbWk-xvRMI
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2: id: f8fb16a4-19e5-44e1-8db9-d45f8e266e2c
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: b6ee6bef6552cf0a48316c4ce788e7a22f9daf16
workflow-type: tm+mt
source-wordcount: 1731
ht-degree: 90%

---

# Plug-in Figma pour GenStudio for Performance Marketing

Le plug-in GenStudio for Performance Marketing Figma ajoute un nouveau panneau à l’application Figma qui vous permet de générer du contenu sur la marque.
[Recherchez et installez le plug-in sur la marketplace communautaire Figma](https://www.figma.com/community/plugin/1604251370122180013/firefly-enterprise-and-genstudio).

Cette page décrit comment configurer et utiliser le plug-in .

Les fonctionnalités de ce plug-in incluent :

* Mappez des éléments de texte Figma aux champs GenStudio for Performance Marketing, tels que `headline`, `body`, `on_image_text`, etc.
* Meta Générez de nouvelles [!DNL Experiences] d’annonces publicitaires sur la marque, sur LinkedIn ou sur Display en fonction d’une marque, d’un persona, d’un produit et d’une invite de texte.
* Créez des [!DNL Experiences] directement dans le document Figma en remplaçant le texte des éléments Figma mappés par des valeurs générées par GenStudio for Performance Marketing.
* Reformuler, raccourcir, allonger ou traduire le contenu existant en fonction d’une invite.
* Traduisez le [!DNL Experiences] généré dans plusieurs langues.
* Exportez les [!DNL Experiences] générés vers une source locale sous forme d’images aplaties.
* Exportez les [!DNL Experiences] générés vers GenStudio for Performance Marketing.
* Utilisez des options de module externe qui s’adaptent aux éléments sélectionnés dans la zone de travail Figma.

>[!VIDEO](https://video.tv.adobe.com/v/3478809?learn=on)

## Créer un modèle

Le plug-in nécessite les deux premiers niveaux de votre document Figma pour respecter cette convention :

* **Section** - Il s’agit du projet parent, qui peut contenir plusieurs modèles.
* **Frame** - Représente un modèle au sein d’un projet. Le modèle peut être rempli de texte, d’images, de composants et d’autres éléments.

### Modèles Meta

Ces tailles de modèle sont prises en charge :

Pour les publications sur Instagram ou Facebook :

* Largeur : 1080 px (fixe)
* Hauteur : 1 080 px ou 1 350 px

Pour les histoires sur Instagram ou Facebook :

* Largeur : 1080 px (fixe)
* Hauteur : 1920 px

Le plug-in décide du chrome de l’expérience générée en fonction de la hauteur du modèle.

### Afficher les modèles

Il n’existe aucune exigence de taille fixe. Les modèles d’affichage prennent en charge n’importe quelle taille.

### Modèles LinkedIn

* Largeur : 1200 px (fixe)
* Hauteur : 1 200 px, 628 px, 2 292 px, 1 800 px ou 1 500 px

### Mappage du rôle de champ

Le plug-in doit comprendre les différents éléments de votre modèle, tels que le titre, le corps du texte ou l’image.

Pour attribuer des rôles d’élément :

1. Sélectionnez un élément dans votre modèle (texte, image, etc.).
1. Utilisez le menu déroulant pour attribuer un rôle.

>[!IMPORTANT]
>
> Vous devez mapper une image : attribuez le rôle de champ `image` à au moins un élément d’image dans votre modèle.

Le plug-in mémorise ces mappages à utiliser pour le contenu généré. Un rôle de champ peut être mappé à plusieurs éléments de modèle.

![Mappage du rôle de champ](./field-role-mapping.png){width="60%"}

### Exceptions de mappage de champs

{{$include /help/_includes/field-mapping-exceptions.md}}

## Générer un nouveau contenu

Utilisez l’IA dédiée au GenStudio for Performance Marketing pour générer ou modifier des éléments dans les modèles Figma.

1. Si vous utilisez le laboratoire du plug-in GenStudio ou des modèles déjà préparés, sélectionnez le nœud de section contenant vos modèles d’annonces. Vous pouvez le faire à partir du panneau **Calques** ou en cliquant directement sur la section dans la zone de travail.
   ![Sélection de section ou de variations](./plugin-playground.png){width="50%" zoomable="yes"}
1. Dans la fenêtre du plug-in, saisissez un nom de projet pour les variations, choisissez une plateforme pour le contenu et renseignez les autres informations requises. Cliquez ensuite sur le bouton **[!UICONTROL Terminer la configuration]**.
   ![Fenêtre Configurer le projet](./setup-project.png){width="30%" zoomable="yes"}
1. Sélectionnez les [!DNL Brand], [!DNL Persona] et [!DNL Product] à utiliser pour la génération de contenu.
1. Sélectionnez le nombre de variations à produire (huit au maximum).
1. Utilisez le bouton sous **[!UICONTROL Sélectionner le contenu]** pour parcourir et choisir des images dans vos ressources. Les 40 ressources ajoutées le plus récemment apparaissent en premier et vous pouvez rechercher d’autres ressources. Les images sélectionnées sont automatiquement redimensionnées pour s’adapter à vos modèles.
1. Saisissez une invite de texte. L’option **[!UICONTROL Action]** de chaque champ de la liste **[!UICONTROL Champs]** est définie sur **[!UICONTROL Générer]** pour le nouveau contenu.
1. Mappez tous les rôles de champ. Voir [ Mappage du rôle de champ ](#field-role-mapping).
1. Cliquez sur le bouton **[!UICONTROL Générer]**.

## Traduire ou générer et copier des variations d’un contenu existant

Utilisez l’IA dédiée aux GenStudio for Performance Marketing pour générer des variantes de copie d’annonces ou traduire des modèles Figma.

1. Sélectionnez le nœud de section qui contient vos modèles d’annonces publicitaires. Vous pouvez le faire à partir du panneau **Calques** ou en cliquant directement sur la section dans la zone de travail.
   ![Sélection de section ou de variations](./plugin-playground.png){width="50%" zoomable="yes"}
1. Dans la fenêtre du plug-in, saisissez un nom de projet pour les variations et choisissez une plateforme pour le contenu.
1. Dans **[!UICONTROL Quel est l’objectif ?]**, sélectionnez **[!UICONTROL Générer les variations]** ou **[!UICONTROL Traduire]**, puis cliquez sur le bouton **[!UICONTROL Terminer la configuration]**.
   ![Fenêtre Configurer le projet](./setup-project.png){width="30%" zoomable="yes"}
1. Sélectionnez les [!DNL Brand], [!DNL Persona] et [!DNL Product] à utiliser pour la génération de contenu.
1. Sélectionnez le nombre de variations à produire.
1. Utilisez le bouton sous **[!UICONTROL Sélectionner le contenu]** pour parcourir et choisir des images dans vos ressources. Les 40 ressources ajoutées le plus récemment apparaissent en premier et vous pouvez rechercher d’autres ressources. Les images sélectionnées sont automatiquement redimensionnées pour s’adapter à vos modèles.
1. Saisissez une invite de texte. L’option **[!UICONTROL Action]** de chaque champ de la liste **[!UICONTROL Champs]** est définie sur **[!UICONTROL Générer]** pour le nouveau contenu.
1. Mappez tous les rôles de champ. Voir [ Mappage du rôle de champ ](#field-role-mapping).
1. Sélectionnez chaque type de champ pour générer des variations ou effectuer une traduction dans le panneau sur le côté gauche du plug-in, puis collez le contenu initial dans chaque zone **[!UICONTROL Contenu initial]**.
   ![Exemple de texte dans la zone Contenu initial](./initial-content-box.png){width="60%" zoomable="yes"}
1. Cliquez sur le bouton **[!UICONTROL Générer]**.

## Traduire le contenu après la génération

1. Sélectionnez la génération à traduire.
   ![Sélectionner la génération](./select-generation.png){width="20%" zoomable="yes"}
1. Choisissez **[!UICONTROL Traduction]**, puis cliquez sur **[!UICONTROL Traduire]**.
1. Sélectionnez la ou les langues cibles.
1. Cliquez sur **[!UICONTROL Sélectionner]**.

Les résultats de traduction sont les suivants :

* Une nouvelle page s’affiche avec le contenu traduit.
* Chaque traduction affiche la langue ou le paramètre régional cible.
* Le contenu d’origine reste inchangé dans la page d’origine.

![Résultats de traduction](./translation-results.png){width="60%" zoomable="yes"}

## Autres actions sur les champs de contenu après génération

Lorsque vous modifiez du contenu existant dans un champ, des options utiles s’affichent dans le panneau du module externe.

![Options des actions de module externe](./figma-other-actions.png){width="30%" zoomable="yes"}

Les options disponibles sont les suivantes :

* Modifiez la **[!UICONTROL Valeur]** pour modifier directement le texte. La modification de ce contenu s’applique automatiquement à toutes les variations sélectionnées.
* L’IA peut effectuer de nombreuses options **[!UICONTROL Action]**, notamment :

| Action | Description |
| --- | --- |
| **[!UICONTROL Générer]** | Générez une nouvelle variante du texte. |
| **[!UICONTROL Reformuler]** | Générez une nouvelle variante du texte. |
| **[!UICONTROL Raccourcir]** | Générez une variante plus courte du texte. |
| **[!UICONTROL Allonger]** | Générez une variante plus longue du texte. |

Après avoir sélectionné une option **[!UICONTROL Action]**, régénérez le contenu à l’aide du bouton **[!UICONTROL Régénérer]**.

## Exporter des expériences

Les variations peuvent être exportées à partir de Figma en tant que [!DNL Experiences] GenStudio for Performance Marketing.

1. Sélectionnez le contenu à exporter dans la zone de travail Graphique en effectuant l’une des opérations suivantes :
   * Sélectionnez la section de génération dans la zone de travail, puis cliquez sur **[!UICONTROL Tout marquer pour l’exportation]** dans le panneau du plug-in.
     ![ Sélection de la section de génération ](./select-generation-section.png){width="20%" zoomable="yes"}
   * Sélectionnez une génération individuelle dans la zone de travail, puis cliquez sur **[!UICONTROL Marquer pour l’exportation]** dans le panneau du plug-in.
     ![Sélection de génération individuelle](./select-generation.png){width="20%" zoomable="yes"}
1. Sélectionnez l’élément Exporter dans le menu de la barre latérale.
   ![Bouton Marquer pour l’exportation affiché pour une publicité Meta](./mark-for-export.png){width="60%" zoomable="yes"}
1. Sélectionnez une destination.
1. Cliquez sur **[!UICONTROL Exporter]** pour exporter le contenu.

Un fichier ZIP est créé dans le panneau du plug-in ou un lien vers **[!UICONTROL Ouvrir dans GenStudio]** s’affiche. Utilisez le lien ZIP pour choisir l’emplacement d’enregistrement du fichier ou sélectionnez **[!UICONTROL Ouvrir dans GenStudio]**.

## Convertir les images Figma en Photoshop

>[!NOTE]
>
> Pour effectuer cette tâche, vous avez besoin du plug-in Figma et de [GenStudio Photoshop](photoshop-plugin.md).

Vous pouvez utiliser le module externe Figma pour convertir un cadre Figma, plusieurs cadres ou un document entier au format Photoshop et l’exporter pour l’utiliser avec [GenStudio Photoshop](photoshop-plugin.md). Actuellement, seules les propriétés majeures telles que la visibilité, la taille de police et les attributs de calque de base sont prises en charge lors de la conversion. Les fonctions telles que les caractères barrés, les exposants, les indices, l’opacité en pourcentages, les dégradés et d’autres propriétés avancées similaires ne sont pas encore prises en charge.

Le plug-in prend en charge les types de calques Figma suivants pour la conversion :

* **Cadre**
* **Groupe**
* **Instance**
* **Texte**
* **Vecteur**
* **Image**

Lorsque vous effectuez une conversion vers PSD, les calques pris en charge sont mappés vers Photoshop comme suit :

| Type de calque Figma | Convertit en Photoshop | Notes |
| --- | --- | --- |
| **Cadre** | Groupe de calques | <ul><li>Les images Figma sont converties en groupes de calques Photoshop.</li><li>Les images imbriquées deviennent des groupes imbriqués.</li><li>Les dimensions d’image deviennent le plan de travail ou les limites de groupe de PSD (selon la sélection).</li></ul> |
| **Groupe** | Groupe de calques | <ul><li>Les groupes Figma sont convertis directement en groupes de calques Photoshop.</li><li>La hiérarchie des calques et l’ordre d’empilement sont conservés.</li></ul> |
| **Instance** | Groupe de calques | <ul><li>Les composants et les instances sont aplatis en groupes de calques Photoshop standard. Les métadonnées de composant et la logique de variante ne sont pas conservées.</li><li>Tous les calques enfants restent à l’intérieur du groupe.</li></ul> |
| **Texte** | Calque de texte | <ul><li>Les calques de texte Figma sont convertis en calques de texte Photoshop modifiables.</li><li>La hiérarchie et le positionnement du texte sont conservés.</li></ul> |
| **Vecteur** | Couche de forme | <ul><li>Les calques vectoriels Figma sont convertis en calques de forme Photoshop.</li><li>Dans la mesure du possible, les chemins sont conservés.</li><li>Les vecteurs complexes peuvent être pixellisés si des effets non pris en charge sont appliqués.</li></ul> |
| **Image** | Calque pixellisé | <ul><li>Les calques d’image Figma sont convertis en calques matriciels Photoshop.</li><li>La mise à l’échelle et le positionnement de l’image sont conservés.</li></ul> |

### Comment convertir des images

Pour convertir des images :

1. Ouvrez le plug-in Firefly Enterprise et GenStudio dans Figma, puis cliquez sur l’onglet **[!UICONTROL Exporter]** dans l’interface utilisateur du plug-in.
1. Sur la zone de travail, sélectionnez le ou les cadres à exporter. Vous pouvez choisir une ou plusieurs images.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **[!UICONTROL Exporter]** pour exporter le fichier converti vers un emplacement choisi, ou
   * Cliquez sur **[!UICONTROL Transférer vers GenStudio Photoshop]** pour mettre en cache le fichier converti en vue d’une utilisation immédiate dans GenStudio Photoshop.
     ![Bouton Transférer vers GenStudio Photoshop](./transfer-to-ps-button.png){width="40%"}
1. Lorsque la boîte de dialogue **[!UICONTROL Clé de fichier requise]** s’affiche, le plug-in a besoin d’une URL de fichier Figma pour effectuer la conversion. Ajoutez l’URL de votre document :

   1. Dans Figma, cliquez sur **[!UICONTROL Partager]** dans le coin supérieur droit de la zone de travail.
   1. Dans **[!UICONTROL Partager ce fichier]**, cliquez sur **[!UICONTROL Copier le lien]**.
   1. Collez le lien copié dans le champ **[!UICONTROL URL du fichier Figma]** de la boîte de dialogue du plug-in.

1. Cliquez sur **[!UICONTROL Envoyer]**. Le module externe lit les images sélectionnées dans Figma et les convertit en document JSON, un format intermédiaire pour les données de fichier.
   ![Boîte de dialogue Clé de fichier requise](./file-key-required.png){width="35%"}
1. Dans Photoshop, ouvrez GenStudio Photoshop et cliquez sur l’onglet **[!UICONTROL Importer]**.
1. Utilisez l’une des méthodes suivantes :

   * Cliquez sur **[!UICONTROL À partir du plug-in]** pour choisir un fichier converti avec **[!UICONTROL Transférer vers GenStudio Photoshop]** dans la liste des fichiers mis en cache, ou
   * Cliquez sur **[!UICONTROL Charger JSON]** pour rechercher et sélectionner le fichier JSON à charger.
     ![Bouton Télécharger JSON](./upload-json.png){width="40%"}
1. GenStudio Photoshop convertit les informations du document JSON en document Photoshop ouvert.
1. Cliquez sur **[!UICONTROL Terminé]**. Le nouveau fichier s’ouvre dans Photoshop et est prêt à l’emploi. Ou cliquez sur **[!UICONTROL Enregistrer sous...]** pour choisir un emplacement d’enregistrement du fichier.
   ![ Boîte de dialogue du bouton Terminé ](./import-done-button.png){width="40%"}

## Historique de génération

Le plug-in conserve un historique des modifications pour chaque champ. Sur la page du modèle, choisissez **[!UICONTROL Historique de génération]** dans la barre latérale du plug-in.

![Option d’historique de génération affichée pour une publicité Meta](./generation-history.png){width="80%" zoomable="yes"}

## Dépannage

Tenez compte de ces bonnes pratiques et conseils si le texte ou les images ne sont pas remplacés dans les variations générées.

### Champs mappés

Si le texte ou les images ne sont pas remplacés, vérifiez que les champs ont été mappés à des rôles de champ GenStudio dans l’interface utilisateur du plug-in. Voir [ Mappage du rôle de champ ](#field-role-mapping).

### Confirmer que les polices sont disponibles

La police d’un champ de texte doit être disponible sur votre ordinateur pour que le remplacement puisse se produire pendant la génération. Vérifiez que toutes les polices utilisées dans le fichier sont disponibles sur votre ordinateur, en particulier si le fichier a été créé sur l’ordinateur d’une autre personne.

### Prendre en compte la prise en charge des rôles de champ

Certains canaux ne prennent en charge le remplacement que dans des champs spécifiques. Tenez compte des exceptions pour le [mappage des rôles de champ](#field-role-mapping).
