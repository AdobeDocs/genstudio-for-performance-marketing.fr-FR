---
title: Activation d’une métadonnée
description: Découvrez comment activer une expérience de métadonnées.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
source-git-commit: 6ee58b22761be357bb9ff753cf9e5bd5b431c513
workflow-type: tm+mt
source-wordcount: '1411'
ht-degree: 2%

---

# Activation d’une métadonnée

Adobe GenStudio for Performance Marketing prend en charge l’activation des Méta-annonces, ou contenus publicitaires, sur Instagram et Facebook.

Vous pouvez [créer une méta-expérience](/help/user-guide/create/create-meta-ad.md) dans GenStudio for Performance Marketing et la sélectionner pour activation, ou créer une nouvelle expérience à partir de ressources approuvées dans [!DNL Activate].

L’activation d’une publicité Meta suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux payants. Le processus d’activation prend en charge la préparation de vos expériences publicitaires aux exigences spécifiques de Meta . Après avoir activé une expérience Meta, ou contenu créatif, dans GenStudio for Performance Marketing, utilisez [Gestionnaire de métadonnées publicitaires](https://adsmanager.facebook.com/) pour affiner l’expérience pour des emplacements de métadonnées publicitaires spécifiques avant la publication finale.

## Étape 1 : Configurer vos comptes Meta

Avant de lancer une activation, [connectez-vous à Meta](https://adsmanager.facebook.com/) pour accéder à votre compte Meta Ads Manager. Vérifiez que les comptes de métadonnées connectés incluent :

* Page Facebook
* Méta-campagne
* Ensemble de métadonnées
* Profil Instagram (facultatif)

Vous devez disposer des autorisations nécessaires pour publier du contenu dans le Gestionnaire de métadonnées publicitaires.

## Étape 2 : Connexion à vos comptes Meta

Avant que votre entreprise puisse activer des expériences, un responsable système GenStudio doit connecter vos comptes Meta à GenStudio for Performance Marketing. Cette connexion permet aux données de circuler entre GenStudio et les outils marketing externes tels que les métadonnées, ce qui active les processus d’activation.

**Pour connecter GenStudio for Performance Marketing à vos comptes Meta** :

1. Dans _Paramètres_, cliquez sur **[!UICONTROL Se connecter]** sur la mosaïque Méta-publicités. La vue _Compte de métadonnées publicitaires_ s’ouvre.

1. Sélectionnez **[!UICONTROL Autoriser les pop-ups]** dans votre navigateur, si vous y êtes invité.

1. Sélectionnez un ou plusieurs de vos comptes publicitaires à connecter, puis cliquez sur **[!UICONTROL Sélectionner]**.

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés. La synchronisation de grandes quantités de données prend plus de temps.

## Étape 3 : préparer votre expérience pour l’activation

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

**Pour préparer votre expérience en vue de l’activation** :

1. Dans _[!DNL Activate]_, cliquez sur **[!UICONTROL Nouveau]**sur la mosaïque Métadonnées du produit . La vue_ Configuration de Creative _s’ouvre.

   La page de configuration de Creative fournit un emplacement central pour préparer l’activation de vos métadonnées. La préparation de votre publicité comprend les trois tâches suivantes :

1. Attribuez un nom à votre expérience. Après l’activation, vous pouvez utiliser ce nom pour rechercher cette expérience dans le tableau _Expériences activées_.
1. Sélectionnez des ressources multimédias. Vous pouvez utiliser des ressources à partir de Contenu ou charger des ressources externes (par exemple, à partir de OneDrive ou de Dropbox).
1. [Ajouter du texte](#add-ad-text).
1. [Ajout de métadonnées](#assign-metadata).

   Le _panneau d’aperçu_ prend en charge une vue interactive de votre texte et de vos ressources dans le contexte d’un emplacement publicitaire spécifique. Utilisez le menu déroulant _Sélectionner l’emplacement_ pour basculer entre les emplacements publicitaires pris en charge. Les aperçus permettent de finaliser les décisions concernant les éléments publicitaires pour des emplacements spécifiques. Lorsque vous sélectionnez un emplacement dans le panneau _Aperçu_, seule votre vue de l’annonce est affectée. Votre sélection d’emplacement dans le panneau _Aperçu_ n’est pas enregistrée.

### Sélection des ressources multimédias

Utilisez la section _Média_ pour sélectionner au moins une ressource d’image à inclure dans votre expérience. Les emplacements publicitaires sont associés à des proportions d’image prises en charge, qui sont répertoriées en tant qu’options dans le menu déroulant _Emplacements_. Ce menu affiche les emplacements publicitaires pris en charge pour les publications Facebook ou les articles Instagram, organisés par rapport aux proportions.

Après le chargement, les ressources sont enregistrées dans _[!DNL Content]_. La zone_ Média _affiche l’image par défaut avec un rapport d’aspect de 1:1. Les autres proportions incluent uniquement les valeurs prises en charge par le canal publicitaire payant. Ils sont regroupés par orientation verticale et horizontale. GenStudio for Performance Marketing prend en charge l’inclusion de jusqu’à six proportions par expérience activée.

**Pour charger une ressource à partir du contenu** :

_[!DNL Content]_fournit une vue centrale des ressources et expériences approuvées de votre organisation. Vous pouvez cibler la galerie de[_[!DNL Content]_](/help/user-guide/content/manage-assets.md) l’inventaire affiché des ressources à l’aide des options de menu **[!UICONTROL Rechercher]** (loupe) et _Filtrer_.

1. Dans _[!DNL Activate]_, cliquez sur **[!UICONTROL Nouveau]**dans la mosaïque Méta-publicités. La vue_ Configuration de Creative _s’ouvre.

1. Cliquez sur **[!UICONTROL Sélectionner]**, puis sélectionnez **[!UICONTROL Sélectionner dans le contenu]**. La vue _Sélectionner le contenu_ s’ouvre, affichant une galerie de ressources d’image que vous parcourez ou filtrez.

1. Utilisez les outils de recherche et de filtrage de _[!DNL Content]_galerie pour sélectionner au moins une ressource à charger.

1. Cliquez sur **[!UICONTROL Utiliser]** pour inclure la ressource sélectionnée dans votre élément créatif. La fenêtre _Configuration de Creative_ inclut la ressource dans ses proportions par défaut dans la zone _Média_. Le panneau _Aperçu_ prévisualise la ressource dans l’emplacement publicitaire qui prend en charge ce rapport d’aspect.

Si le chargement échoue, un message d’erreur informatif contenant un lien vers la ressource dans _[!DNL Content]_s’ouvre.

**Pour charger une ressource externe** :

Vous pouvez charger jusqu’à six images statiques externes à la galerie _[!DNL Content]_à partir de Microsoft OneDrive ou de Dropbox.

1. Dans _[!DNL Activate]_, cliquez sur **[!UICONTROL Nouveau]**sur la mosaïque Métadonnées. La fenêtre_ Configuration de Creative _s’ouvre.

1. Dans la section _Média_, cliquez sur **[!UICONTROL Sélectionner]**. Un menu déroulant affiche des options _Sélectionner à partir du contenu_ ou _Télécharger_.

1. Cliquez sur **[!UICONTROL Charger]**. La fenêtre _Ajouter des proportions_ s’ouvre.

1. Sélectionnez les images selon les proportions prises en charge en faisant glisser et en déposant les fichiers image dans la zone de chargement des images. Vous pouvez également rechercher des ressources sur votre appareil.

1. (Facultatif) Pour charger des ressources à partir de votre appareil, cliquez sur **[!UICONTROL Parcourir]**, puis sélectionnez _Parcourir les fichiers_ ou _Parcourir les dossiers_ pour identifier les ressources à charger.

1. Dans la zone _Ajouter des détails_, ajoutez des informations détaillées à vos ressources chargées pour faciliter la recherche et le filtrage dans les _[!DNL Content]_. Ces détails sont enregistrés en tant que métadonnées.

1. Une fois vos ressources chargées et les détails attribués, cliquez sur **[!UICONTROL Ajouter Assets]** en bas à droite.

### Ajouter du texte publicitaire

Utilisez la section _Texte_ de la page _Activer la méta-annonce_ pour ajouter du texte attrayant et conforme à la marque aux champs de texte obligatoires. Le texte comprend le texte principal (corps) de la publicité et le texte d’appel à l’action.

| champ | Requis | Limite de caractères (max.) |
|-----------------|---------------------------|---------------------------------|
| Nom de la publicité | oui | 500 |
| Texte du Principal | oui | 500 |
| Titre | oui | 255 |
| Description | Non | 125 |
| Appel à l’action | oui | options de menu déroulant uniquement |
| Afficher l’URL | Non | 1 000 |
| URL du site web | oui | 1 000 |
| Image | au moins un obligatoire |                                 |

_Le texte en Principal_ et le _titre_ sont requis par GenStudio for Performance Marketing uniquement, et non par Meta.

### Attribution de métadonnées

Les détails de l’expérience sont enregistrés en tant que métadonnées et aident les utilisateurs lors de la recherche d’une expérience. Ces détails augmentent la visibilité de l’expérience dans [!DNL Content]. Utilisez ces détails facultatifs définis par l’utilisateur ou l’utilisatrice pour identifier l’objectif de l’expérience et le ou les campagnes dans lesquelles elle est déployée.

| Détail | Description |
|------------|-------------|
| Campagnes | Toutes les campagnes GenStudio for Performance Marketing auxquelles appartient l’expérience publicitaire |
| Marque | Directives, définies par l&#39;utilisateur ou par défaut, qui permettent aux utilisateurs d&#39;établir des directives de marque capturant l&#39;essence de l&#39;identité d&#39;une marque. |
| Produits | Produits associés à votre organisation et identifiés dans GenStudio for Performance Marketing |
| Personnes | Personnes associées à votre organisation et identifiées dans GenStudio for Performance Marketing |
| Échéancier | Trimestre, saison, année ou autre unité de temps définie par l’organisation pendant laquelle l’expérience publicitaire est active |
| Région   | Région géographique dans laquelle l’expérience est lancée |
| Langue | Langues pour lesquelles l’expérience publicitaire est utilisée |
| Mots-clés | Mots-clés définis par l’utilisateur qui facilitent la recherche et la catégorisation de l’expérience publicitaire |

Après avoir assemblé votre contenu créatif, cliquez sur **[!UICONTROL Suivant]** pour confirmer la configuration des métadonnées.

## Étape 4 : confirmer la configuration du méta-compte

Après avoir préparé votre contenu créatif, vous devez confirmer les informations de votre compte Meta et attribuer un identifiant de suivi à l’expérience publicitaire. La vue _Configuration des publicités Meta_ est renseignée avec des options dérivées des comptes Meta configurés.

| Détail | Description |
|------------|-------------|
| Comptes | Méta-comptes connectés à GenStudio for Performance Marketing |
| Page Facebook | Page Facebook sur laquelle l’expérience est publiée |
| Compte Instagram | Comptes Instagram ayant été connectés à GenStudio for Performance Marketing |
| Campagnes | Métacaractères auxquelles appartient l’expérience publicitaire |
| Visionneuses d’annonces | Métadonnées publicitaires auxquelles appartient l’expérience publicitaire activée. Les paramètres déterminent les emplacements finaux de la publicité. |

### Identifiant de tracking

Les identifiants de suivi (nom de l’annonce publicitaire) fournissent un mécanisme de collecte des mesures liées aux performances de l’expérience. Saisissez le nom de l’annonce publicitaire dans ce champ.

Cliquez sur **[!UICONTROL Suivant]** en haut à droite pour prévisualiser votre expérience publicitaire et finaliser l’activation.

## Étape 5 : Prévisualiser et activer votre publicité

La page _Réviser_ affiche votre expérience publicitaire telle qu’elle a été assemblée dans la configuration de _Creative_ et offre une dernière occasion d’afficher et de modifier votre expérience. Cliquez sur **[!UICONTROL Modifier la section]** à côté du libellé _Configuration de Creative_ pour apporter vos modifications. Vous pouvez également cliquer sur **[!UICONTROL Précédent]** en haut à droite pour revenir à la page _Configuration de Creative_.

### Activation complète de votre expérience publicitaire

Cliquez sur **[!UICONTROL Publier]**. L’expérience complète des métadonnées et les métadonnées associées sont directement transmises au jeu de publicités du Gestionnaire de métadonnées sélectionné. Les expériences sont diffusées au Gestionnaire de métadonnées désactivé. À partir du Gestionnaire de métadonnées publicitaires, vous pouvez gérer les dernières étapes de déploiement de l’expérience publicitaire et de la méta-campagne.

### Connectez-vous au Gestionnaire de métadonnées publicitaires pour terminer l’activation

Une fois l’activation terminée, vous devez vous connecter au Gestionnaire de métadonnées publicitaires. À partir du [Gestionnaire de publicités Meta](https://adsmanager.facebook.com/), vous pouvez passer en revue votre expérience publicitaire et finaliser la publication sur des canaux Meta spécifiques.
