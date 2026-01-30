---
title: Plug-in Photoshop pour Adobe GenStudio for Performance Marketing
description: Découvrez comment installer, configurer et utiliser le plug-in Photoshop pour GenStudio for Performance Marketing.
feature: Generative AI
role: User
source-git-commit: bb6b8de80bdf6089e70756bea5dbf3e6a7945052
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 1%

---

# Plug-in Photoshop pour GenStudio for Performance Marketing

Le plug-in GenStudio for Performance Marketing Photoshop ajoute un panneau à Adobe Photoshop qui vous permet de générer du contenu sur la marque.

Cette page décrit comment installer et configurer le plug-in et comment l’utiliser.

Les fonctionnalités de ce plug-in incluent :

* Connectez-vous à une instance GenStudio for Performance Marketing avec une Adobe ID
* Mapper des champs de génération de contenu GenStudio for Performance Marketing à des calques de texte dans un document Photoshop
* Spécifiez une marque, un produit, une persona et une invite de texte pour générer du contenu
* Vous pouvez éventuellement ajouter une image pour remplacer votre image de modèle
* Prévisualiser les variations de contenu générées sur la marque
* Appliquer le contenu généré aux calques mappés dans le document actif
* Créer des traductions de contenu sur marque
* Exporter les [!DNL Experiences] générés vers GenStudio for Performance Marketing

>[!VIDEO](https://video.tv.adobe.com/v/3478822?captions=fre_fr&learn=on)

## Installation du plug-in

Suivez ces instructions pour installer le plug-in .

### Conditions préalables

* Application de bureau Creative Cloud
* Photoshop, version minimale 25.6.0

### Etapes d&#39;installation

1. Téléchargez et mettez à jour le plug-in depuis Creative Cloud Marketplace dans Adobe Exchange.
1. Recherchez le plug-in **GenStudio pour Photoshop** dans Adobe Exchange.
1. Suivez les invites pour installer le plug-in.

### Désinstallation du plug-in

1. Lancez l’application de bureau Creative Cloud.
1. Cliquez sur l’option **[!UICONTROL Plugins]**.
1. Cliquez sur les points de suspension, **[!UICONTROL (...)]** sur la vignette GenStudio for Creative Cloud pour afficher les options.
1. Choisissez **Désinstaller**.

## Créer un modèle

Pour générer du contenu, vous avez besoin d’un modèle GenStudio for Performance Marketing créé à partir de votre document Photoshop.

Pour créer un modèle prêt pour GenStudio, procédez comme suit :

1. Ouvrez un document dans Photoshop.
1. Identifiez un calque de texte pour le contenu généré.
1. Renommez le calque avec le format de convention de nom de champ : `{<name_of_generated_field>}`. Par exemple : `{body}`, `{headline}`, `{cta}`.
1. Renommez les calques pour tous les champs [champs requis par le canal destiné au type de modèle](../../user-guide/templates/customize-template.md#recognized-field-names).

| Canal | Champs obligatoires pour la génération | Champs facultatifs pour la génération |
| --- | --- | --- |
| LinkedIn | `{on_image_text}`, `{image}` | `{headline}`, `{introductory_text}`, `{cta}`, `{website_url}` |
| Meta | `{on_image_text}`, `{image}` | `{body}`, `{headline}`, `{cta}`, `{website_url}`, `{display_link}` |
| Affichage | `{body}`, `{image}` | `{headline}`, `{cta}`, `{website_url}` |

Notez que plusieurs calques peuvent partager la même désignation de champ, mais chaque calque ne peut spécifier qu’un seul champ. Par exemple, s’il existe plusieurs plans de travail dans le document :

* Vous pouvez spécifier un calque `{headline}` dans chaque plan de travail.
* Vous pouvez spécifier plusieurs calques de `{headline}` dans un plan de travail unique.
* Vous ne pouvez pas spécifier qu’un seul calque reçoive à la fois les noms des champs `{headline}` et `{cta}`.

### Exigences de taille des modèles

#### Modèles Meta

Pour les publications sur Instagram et Facebook :

* Largeur : 1080 px (fixe)
* Hauteur : 1 080 px ou 1 350 px

Pour les histoires sur Instagram et Facebook :

* Largeur : 1080 px (fixe)
* Hauteur : 1920 px

Le plug-in décide du chrome de l’expérience générée en fonction de la hauteur du modèle.

#### Afficher les modèles

Il n’existe aucune exigence de taille fixe. Les modèles d’affichage prennent en charge n’importe quelle taille.

#### Modèles LinkedIn

* Largeur : 1200 px (fixe)
* Hauteur : 1 200 px, 628 px, 2 292 px, 1 800 px ou 1 500 px

Le document est maintenant prêt à être utilisé avec le plug-in .

## Générer un nouveau contenu

1. Ouvrez Photoshop.
1. Ouvrez un document de modèle prêt pour GenStudio que vous avez créé (voir les instructions ci-dessus) ou utilisez le modèle de démarrage GenStudio for Performance Marketing : `branding-template-acrobat-handlebars.psd`.
1. Ouvrez le panneau de plug-in à l’adresse **[!UICONTROL Plugins]** > **[!UICONTROL GenStudio]**.
1. Cliquez sur le bouton **[!UICONTROL Connexion]**. Si vous êtes invité à ouvrir une URL, cochez éventuellement la case **Mémoriser mon choix**, puis cliquez sur **[!UICONTROL Autoriser]**.
1. Utilisez le navigateur web pour vous connecter avec un profil ayant accès à GenStudio for Performance Marketing.
1. Sélectionnez le canal (Meta, LinkedIn ou Affichage) qui s’applique au modèle que vous avez ouvert.
   ![Sélection du canal](./ps-select-channel.png){width="300" zoomable="yes"}
1. Sélectionnez le contexte de [!DNL Brand], de [!DNL Persona] et de [!DNL Product] pour la génération de contenu.
   ![Marque, persona et sélection de produits](./ps-select-box.png){width="300" zoomable="yes"}
1. Sélectionnez le nombre de variations à produire.
1. Utilisez le bouton sous **[!UICONTROL Sélectionner le contenu]** pour parcourir et choisir des images dans vos ressources. Les 40 ressources ajoutées le plus récemment apparaissent en premier et vous pouvez rechercher d’autres ressources. Les images sélectionnées sont automatiquement redimensionnées pour s’adapter à vos modèles.
1. Fournissez une invite de texte pour le contenu dans la zone **[!UICONTROL Invite de texte]**.
1. Cliquez sur le bouton **[!UICONTROL Générer]**. Les variations apparaissent sur les cartes dans le panneau du plug-in.

De nouveaux documents sont ajoutés à votre espace de travail Photoshop avec le contenu généré appliqué aux champs du modèle. Ces documents sont nommés avec un suffixe de variation numéroté.

## Traduction du contenu

Les utilisateurs peuvent traduire le contenu dans les langues prises en charge après la génération de la copie.

1. Cliquez sur **[!UICONTROL Traduire]** après avoir généré une copie de publicité avec le plug-in.
1. Sélectionnez une ou plusieurs langues pour la traduction.
1. Cliquez sur le bouton **[!UICONTROL Traduire]**.

De nouveaux documents sont ajoutés à votre espace de travail Photoshop avec le contenu généré appliqué aux champs du modèle. Ces documents sont nommés avec un suffixe de variation numéroté.

## Exporter des expériences vers GenStudio

Les utilisateurs peuvent sélectionner exporter après la génération ou la traduction du contenu. Les expériences exportées sont renseignées dans la section contenu de GenStudio for Performance Marketing.

![&#x200B; Ressources exportées affichées dans la section Contenu &#x200B;](./content-assets.png){width="90%"}

## Dépannage

Tenez compte de ces bonnes pratiques et conseils si le texte ou les images ne sont pas remplacés dans les variations générées.

### Champs mappés

Si le texte ou les images ne sont pas remplacés, vérifiez que les champs sont correctement mappés avec des accolades `{}` (et non des parenthèses `()`).

### Confirmer que les polices sont disponibles

La police d’un champ de texte doit être disponible sur votre ordinateur pour que le remplacement puisse se produire pendant la génération. Vérifiez que toutes les polices utilisées dans le fichier sont disponibles sur votre ordinateur, en particulier si le fichier a été créé sur l’ordinateur d’une autre personne.

### Exceptions de mappage de champs

{{$include /help/_includes/field-mapping-exceptions.md}}
