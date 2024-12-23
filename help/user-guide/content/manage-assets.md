---
title: Gestion des ressources et des expériences
description: Simplifiez et améliorez la gestion des ressources approuvées par la marque en vue de leur utilisation et réutilisation dans votre parcours de marketing numérique.
feature: Content, Assets, Experiences
exl-id: e2ce8797-6d3b-46d4-b12f-f5f80e26c669
source-git-commit: d5efabbaf3dd0817bd3158acb59d997a727e5f62
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Gestion des ressources et des expériences

Adobe GenStudio for Performance Marketing [!DNL Content] simplifie et améliore la gestion des ressources approuvées par la marque pour une utilisation et une réutilisation dans votre parcours de marketing numérique.

## galerie [!DNL Content]

La galerie affiche un inventaire des ressources, expériences ou modèles approuvés en fonction de la vue sélectionnée. L’icône de filtre (entonnoir) située au-dessus du côté gauche du tableau ouvre le menu **[!UICONTROL Filtrer]**, qui vous permet de sélectionner une catégorie pour filtrer le contenu affiché dans la galerie. Dans la vue _[!UICONTROL Assets]_, cliquez sur l’icône de recherche (loupe) pour utiliser un mot-clé afin de rechercher une ressource.

Vous trouverez ci-dessous une recherche sur le terme `dog` dans la galerie [!UICONTROL Assets] :

![Vue Assets avec recherche sur chien](/help/assets/content-assets.png)

### Recherche de contenu

L’interface de filtrage et de recherche est rapide et réactive, et fournit une expérience de recherche productive. Chaque vue de [!DNL Content] fournit des options de filtre permettant d’affiner votre recherche de la ressource, de l’expérience ou du modèle idéal. Pour les ressources et les expériences, vous pouvez sélectionner une campagne et des directives spécifiques, telles que le contenu créé pour un produit spécifique.

Il existe des filtres basés sur [mots-clés](asset-details.md#user-defined-metadata) et [catégories d’attributs](/help/user-guide/insights/attribute-category.md) pour limiter les résultats de recherche. Par exemple, vous pouvez rechercher une ressource d’un type de fichier ou d’un objet spécifique afin de vous aider à créer une expérience pour votre campagne. Vous pouvez également filtrer le contenu en fonction de votre nom d’utilisateur ou du nom d’un membre de l’équipe :

- Le filtre **[!UICONTROL Chargé par]** limite la liste _[!UICONTROL Assets]_ pour n’afficher que les ressources que vous ou une personne spécifique avez chargées.
- Le filtre **[!UICONTROL Créé par]** limite la liste _[!UICONTROL Expériences]_ pour n’afficher que les expériences créées par vous ou par une personne spécifique.

**Pour rechercher du contenu à réutiliser** :

1. Dans _[!DNL Content]_, sélectionnez la section **[!UICONTROL Assets]**.

1. Sélectionnez un référentiel de ressources dans la liste **[!UICONTROL Emplacement]** ou vérifiez que vous recherchez le référentiel de ressources approprié. `GenStudio assets` est le référentiel par défaut.

   >[!IMPORTANT]
   >
   >La liste _Emplacement_ n’est disponible que lorsque vous [vous connectez à un référentiel AEM](connect-aem-repo.md).

1. Cliquez sur **[!UICONTROL Rechercher]** (loupe) pour saisir un mot-clé ou une description.

1. Affinez votre recherche en sélectionnant une catégorie dans la liste _[!UICONTROL Filtrer]_. Par exemple, si vous recherchez un fichier PNG, cliquez sur **[!UICONTROL Format de fichier]** et choisissez **PNG**.

   Plus vous affinez votre recherche, moins il y a d’options de filtre disponibles. Cliquez sur **[!UICONTROL Effacer tout]** pour supprimer tous les filtres.

1. Sélectionnez une ressource pour obtenir une vue complète et une liste de détails.

   Cliquez sur **[!UICONTROL Télécharger]** (flèche vers le bas) pour utiliser la ressource sur votre station de travail locale.

### Emplacement

Par défaut, les ressources que vous ajoutez aux [!DNL Content] par le biais du processus de [!DNL Create] ou du téléchargement sont stockées dans le référentiel `GenStudio assets`. Le référentiel `GenStudio assets` est un référentiel en lecture/écriture de GenStudio for Performance Marketing. Cela signifie que vous pouvez enregistrer, modifier et supprimer des ressources dans le référentiel `GenStudio assets`.

La liste **[!UICONTROL Emplacement]** située au-dessus de la galerie _[!UICONTROL Assets]_ sur le côté droit vous permet de choisir parmi les référentiels [!DNL Assets Content Hub] de Adobe Experience Manager connecté (AEM).

![Liste des emplacements des référentiels](../../assets/content-location-selection.png){width="350"}

Lorsque vous sélectionnez un référentiel AEM, la galerie affiche un inventaire des ressources de ce référentiel, ce qui vous permet d’exploiter les ressources approuvées de ces référentiels en tant qu’entrées pour la création de contenu. Les options de filtre changent pour refléter les catégories configurées dans [!DNL AEM Assets Content Hub].

Voir [Connexion à un référentiel AEM](connect-aem-repo.md) pour obtenir des conseils sur l’ajout de votre référentiel [!DNL AEM Assets Content Hub] à GenStudio for Performance Marketing.

Le référentiel AEM est en lecture seule, ce qui signifie que vous pouvez accéder au contenu, mais que vous ne pouvez pas enregistrer de brouillons, de nouvelles ressources ou de nouvelles métadonnées dans le référentiel AEM. Toutes les mises à jour préliminaires et finales des ressources, expériences et modèles sont enregistrées dans le référentiel `GenStudio assets` avec de nouvelles [métadonnées système](asset-details.md#system-metadata).

{{note-aem-assets}}

Un référentiel AEM peut appliquer certaines exigences de licence, telles que l’expiration des ressources. Ces ressources peuvent ne pas être disponibles pour une utilisation dans les workflows [!DNL Create]. Les ressources arrivées à expiration peuvent devoir être renouvelées ou remplacées pour assurer la continuité de vos projets. Consultez votre administrateur [!DNL AEM Assets Content Hub] pour obtenir de l’aide sur ces ressources.

## Gestion d’Assets

Dans [!UICONTROL Content], vous pouvez facilement stocker, récupérer et gérer vos ressources numériques. En utilisant à la fois le référentiel `GenStudio assets` et les référentiels AEM, vous pouvez vous assurer que vos ressources sont bien organisées et accessibles pour diverses campagnes marketing. Cette approche multi-référentiels offre de la flexibilité et un contrôle sur l’utilisation des ressources dans les environnements, ce qui garantit que seules les ressources approuvées et à jour sont utilisées dans les efforts marketing.

Le tableau suivant répertorie les tâches de gestion disponibles pour les ressources, les expériences et les modèles :

| Tâches | Ressources | Expériences | Modèles |
| --------------------------------------------------------- | :----: | :---------: | :-------: |
| [Afficher les détails](/help/user-guide/content/asset-details.md) | ✓ | ✓ | ✓ |
| [Créer une expérience](/help/user-guide/create/overview.md) |        |             | ✓ |
| [Modifier dans l’Adobe Express ](#edit-in-express) | ✓ |             |           |
| [Exporter pour activation](#export-for-activation) |        | ✓ |           |
| [Actualiser](/help/user-guide/content/use-templates.md#refresh-template) |   |      | ✓ |
| [Télécharger](#download-assets) | ✓ |             | ✓ |
| [Supprimer](#delete-assets) | ✓ | ✓ | ✓ |

### Ajouter des ressources

Lors de l’ajout de ressources à [!DNL Content], elles sont stockées par défaut dans le référentiel `GenStudio assets`. Le bouton _[!UICONTROL Ajouter des ressources]_ n’est disponible que lorsque l’_[!UICONTROL Emplacement]_ est le référentiel `GenStudio assets`.

![Champ Emplacement](../../assets/content-location.png){width="350"}

**Pour ajouter une ou plusieurs ressources** :

1. Dans _[!DNL Content]_, cliquez sur **[!UICONTROL Ajouter des ressources]**.

1. Sur la vue _Ajouter vos ressources approuvées_, déposez un ou plusieurs fichiers dans l’espace de dépôt. Vous pouvez éventuellement sélectionner des fichiers locaux à l’aide de **[!UICONTROL Parcourir]** ou importer des fichiers à partir de Dropbox ou de Microsoft OneDrive.

1. Dans la section _Ajouter des détails_, sélectionnez un **[!UICONTROL nom de campagne]** ou saisissez un nouveau nom.

1. Pour améliorer la visibilité, ajoutez des informations facultatives telles que _nom de la marque_, _personnes_, _région_ et _mots-clés_ dans la section **Plus de détails**.

   Plus vous fournissez de détails, plus vous bénéficiez des fonctionnalités robustes de GenStudio for Performance Marketing. Sélectionnez un ou plusieurs détails dans la liste, ou saisissez-en un nouveau le cas échéant, par exemple avec des mots-clés. Chaque détail que vous ajoutez apparaît sous la liste. Cliquez sur **`x`** pour supprimer un détail.

   Tous les détails ajoutés s’appliquent à toutes les ressources ajoutées dans cette action.

   Voir [Détails des métadonnées](/help/user-guide/content/asset-details.md#system-metadata).

1. Cliquez sur **[!UICONTROL Ajouter des ressources]**.

1. Une fois le chargement des ressources terminé, cliquez sur **Terminé**.

1. Pour afficher les nouvelles ressources chargées, cliquez sur **[!UICONTROL Actualiser]** dans la notification _Nouvelles ressources disponibles_ située au bas de la zone de travail.

### Télécharger des ressources

**Pour télécharger une ressource** :

1. Dans _[!DNL Content]_, sélectionnez une ressource ou un modèle. Cliquer sur une ressource ouvre une vue ciblée de la ressource.

1. Dans la vue des ressources, cliquez sur l’icône **[!UICONTROL Télécharger]** (flèche pointant vers le bas) dans le coin supérieur droit.

1. Le téléchargement commence par placer une copie de la ressource à l’emplacement de téléchargement par défaut.

### Suppression des ressources

**Pour supprimer une ressource** :

1. Dans _[!DNL Content]_, sélectionnez une ressource, une expérience ou un modèle. Cliquer sur une ressource ouvre une vue ciblée de la ressource.

1. Dans l’affichage des ressources, cliquez sur **[!UICONTROL Supprimer]** (corbeille) en haut à droite.

1. Dans la fenêtre contextuelle _Supprimer l’élément_, vérifiez l’élément et cliquez sur **[!UICONTROL Supprimer]**.

## Exporter pour activation

Vous pouvez exporter une expérience approuvée pour activation dans un format compatible avec votre canal cible.

**Pour exporter une expérience** :

1. Dans _[!DNL Content]_, sélectionnez une expérience. Cliquez sur une expérience pour ouvrir la vue des détails ou cliquez sur le menu contextuel (`...`).

1. Cliquez sur **[!UICONTROL Exporter pour activation]** (encadré avec une flèche pointant vers l’extérieur).

1. Dans la fenêtre contextuelle _Exporter pour activation_, sélectionnez l’un des formats disponibles :

   - Adresse électronique : `HTML`, `CSV`
   - Méta-publicités et publicité display : `HTML`, `JPEG`, `PNG`

Voir [Activation](/help/user-guide/activation/overview.md).

## Modifier dans Express

Vous pouvez modifier des ressources d’image (JPG ou PNG) directement dans GenStudio for Performance Marketing à l’aide d’Adobe Express. La zone de travail _[!UICONTROL optimisée par l’Adobe Express]_ offre des fonctionnalités pratiques pour améliorer vos images sans quitter l’application GenStudio. Vous pouvez facilement supprimer des arrière-plans, appliquer des remplissages génératifs, ajuster des effets et recadrer des images.

>[!BEGINSHADEBOX]

Critères d’amélioration des images avec la fonction [!DNL Edit in Adobe Express] :

- Les types MIME pris en charge comprennent `image/png` et `image/jpeg`
- Les dimensions minimales de l’image sont de 50 x 50 pixels
- Les dimensions maximales de l’image sont de 8 000 x 8 000 pixels
- La taille maximale est de 40 Mo (40 000 000 octets)

>[!ENDSHADEBOX]

**Pour modifier une ressource avec Express** :

1. Dans _[!DNL Content]_, sélectionnez une ressource image. Cliquer sur une ressource ouvre une vue ciblée de la ressource.

1. Dans la vue des ressources, cliquez sur l’icône **[!UICONTROL Modifier dans l’Adobe Express]** en haut à droite.

1. Dans la zone de travail _[!UICONTROL Optimisée par l’Adobe Express]_, utilisez les commandes express du panneau de gauche pour améliorer votre image.

1. Lorsque vous êtes satisfait(e) de l’image mise à jour, cliquez sur **[!UICONTROL Enregistrer une copie]** en haut à droite.

1. Sélectionnez le format du fichier (JPG ou PNG), puis cliquez sur **[!UICONTROL Enregistrer une copie]**.

1. Dans la fenêtre contextuelle _[!UICONTROL Enregistrer une copie de ressource]_, mettez à jour le **[!UICONTROL Nom de la ressource]**.

   - Sélectionnez **[!UICONTROL Mêmes détails que la ressource d’origine]** pour transférer les détails de la ressource vers la nouvelle image.

   - Développez la section **[!UICONTROL Plus de détails]** pour mettre à jour les instructions et d’autres métadonnées.

   >[!TIP]
   >
   >Plus vous fournissez de détails, plus vous bénéficiez des fonctionnalités robustes de GenStudio for Performance Marketing. Sélectionnez un ou plusieurs détails dans la liste, ou saisissez-en un nouveau le cas échéant, par exemple avec des mots-clés. Chaque détail que vous ajoutez apparaît sous la liste. Cliquez sur **`x`** pour supprimer un détail.

1. Cliquer sur **[!UICONTROL Enregistrer]**.
