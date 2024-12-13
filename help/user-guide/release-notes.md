---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substantial-update: 2024-12-13T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 00359960b6cf314203382d74faa23bae3e753875
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Notes de mise à jour de GenStudio for Performance Marketing

Ces informations de mise à jour détaillent les dernières mises à jour de l’application GenStudio for Performance Marketing.

## 2024.12.12 {#latest}

### Nouvelles fonctionnalités

Les éditeurs peuvent désormais effectuer les tâches liées aux métadonnées suivantes :

* Modifiez les métadonnées de la ressource, de l’expérience et du modèle. Voir [Détails de la ressource](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* Affichez les balises générées par une ressource dans la vue _Détails_ de toute expérience qui utilise la ressource. Voir _Balises générées_ dans [Détails de la ressource](/help/user-guide/content/asset-details.md#generated-tags). <!-- GS-3705 -->

Les éditeurs peuvent désormais spécifier des valeurs personnalisées pour ces aspects des variantes générées :

* Largeur et hauteur des bannières web dans les modèles d’affichage publicitaire. Ces valeurs sont désormais enregistrées en tant que métadonnées de modèle. <!-- GS-6735 -->

* Dimensions d’images dans les expériences de publicité display lors du chargement d’images.<!-- GS-7166 -->

* Consultez les instructions spécifiques aux canaux dans la section [Bonnes pratiques pour les modèles](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

Les options d’exportation incluent désormais :

* Exportez les publicités display et les méta-publicités sous la forme d’HTML, de JPEG ou de PNG. Voir [Créer une expérience d’affichage publicitaire](/help/user-guide/create/create-display-ad.md) et [Créer une expérience de méta-annonce](/help/user-guide/create/create-meta-ad.md). <!-- GS-7093 6655 5152-->

De nouvelles fonctionnalités supplémentaires permettent aux éditeurs de :

* Utilisez le bouton **[!UICONTROL Actualiser]** sur la vue Modèle de [!DNL Content] _Détails de la ressource_ pour actualiser le modèle sélectionné. <!-- GS-7102 -->

* Régénérer les sections des variantes d’annonces publicitaires et d’emails. Voir [Créer une expérience d’affichage d’annonce publicitaire](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) et [Créer une expérience d’e-mail](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Dupliquez les marques existantes. Voir [Gérer les marques](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

### Correctifs et améliorations

* Les titres des publicités display sont désormais enregistrés dans [!DNL Content] comme prévu. <!-- GS-7239 -->

* Le tiroir d’invite ne se ferme plus lorsqu’un éditeur clique en dehors du menu déroulant du tiroir. <!-- GS-7275 -->

* Le menu déroulant [!DNL Create] [!DNL Persona]/[!DNL Product] se charge désormais comme prévu lorsqu’une erreur de service d’URL de miniature se produit. <!-- GS-7277 -->

* Les publicités display qui contiennent des éléments qui recouvrent des fragments sont désormais modifiables. <!-- GS-7186 -->

* Le bouton Zone de travail **[!UICONTROL Marque]** est désormais désactivé lorsque les scores de la marque ne sont pas générés pour une expérience. <!-- GS-6429 -->

* La zone de travail affiche désormais les expériences redimensionnées dans un ordre cohérent. <!-- GS-7123 -->

* Le recadrage manuel utilise désormais les dimensions d’image, et non celles du modèle, lors de la modification des publicités. Auparavant, lorsqu’une image était plus petite que les dimensions spécifiées dans l’affichage et le modèle, le cadre de sélection utilisait les dimensions du modèle, et non les dimensions de l’image. <!-- GS-7315 -->

* Les éditeurs et éditrices peuvent désormais sélectionner jusqu’à quatre images lors de la création d’une publicité display. <!-- GS-7189 -->

* Les brouillons Afficher l’annonce et Méta-annonce se chargent désormais comme prévu lorsqu’ils sont redimensionnés sur un autre navigateur. <!-- GS-7204 -->

* Les champs de modèle inutilisés ne s’affichent plus dans le contenu généré.  <!-- GS-5670 -->

* Les éditeurs peuvent désormais cliquer une seule fois sur les liens pour les modifier comme prévu dans les variantes générées. <!-- GS-7423 -->

* [!DNL Create] respecte désormais correctement les privilèges des collaborateurs. <!-- GS-7614 -->

* Le bouton Zone de travail **[!UICONTROL Redimensionner]** est désormais désactivé une fois toutes les options de redimensionnement sélectionnées et rendues. <!-- GS-5940 -->

* Les réviseurs et réviseuses disposant d’un accès en lecture seule peuvent désormais effectuer un zoom avant ou arrière sur les variantes lors des révisions. <!-- GS-7371 -->

* La sélection au clavier a été ajoutée uniquement aux boutons exploitables dans la vue [!DNL Create] _Travail récent_. <!-- GS-4060 -->

* Le message **Enregistrement en cours** affiché pendant les opérations d’enregistrement de fragment d’e-mail s’affiche désormais uniquement pendant l’opération d’enregistrement. Auparavant, la zone de travail affichait ce message indéfiniment. <!-- GS-6964 -->

* Les éditeurs voient désormais un message d’erreur comme prévu lorsqu’un brouillon ne parvient pas à se charger dans la zone [!DNL Create] _Travail récent_.  <!-- GS-8081 -->

* La zone de travail affiche désormais les méta-annonces redimensionnées et les annonces dans le bon ordre.  <!-- GS-7375 -->

* Les éditeurs peuvent désormais cliquer simultanément dans les champs de l’e-mail et afficher des publicités. <!-- GS-6297 -->

* La fonctionnalité de modification de fragment pour les e-mails et les méta-annonces est désormais déclenchée comme prévu par un seul clic. <!-- GS-8081 -->

* Amélioration des performances du bouton [!DNL Create] **[!UICONTROL Précédent]**. <!-- GS-6767 -->

## Notes de mise à jour antérieures

+++Notes de la version 2024.11.14

### Nouvelles fonctionnalités

Ajout de la prise en charge des modèles de médias riches, ce qui permet aux clients de réutiliser des ressources déjà publiées par le biais de leurs propres canaux de contenu géré. <!-- GS-6107 -->

### Correctifs et améliorations

* Lorsqu’ils sont redimensionnés dans un navigateur autre que celui utilisé pour générer le contenu initial, les brouillons se chargent désormais comme prévu. <!-- GS-7204 -->

* Tous les caractères sont désormais correctement représentés à l’HTML exporté. <!-- GS-7246 -->

* Les boutons de la fenêtre contextuelle [!DNL Content] _Expériences_ **[!UICONTROL Exporter]** ne sont plus tronqués dans certaines langues. <!-- GS-6873 -->

* Les publicités display créées avec des modèles dimensionnés à 50x50 sont désormais exportées dans la taille d’image attendue. Auparavant, les fichiers PNG étaient exportés à des dimensions deux fois supérieures à celles attendues. <!-- GS-7192 -->

* Les erreurs de modèle qui se sont produites lorsque les publicités display ont été redimensionnées sont désormais résolues. <!-- GS-7322 -->

### Localisation

Cette version comprend des améliorations de la localisation dans toute l’interface utilisateur, notamment :

* Toutes les chaînes de la fenêtre contextuelle [!DNL Content] _Charger une ressource_ sont désormais correctement localisées. <!-- GS-6872 6770 -->
* Toutes les info-bulles du champ [!DNL Content] _Assets_ view **[!UICONTROL Search]** sont localisées. <!-- GS-6879 -->
* Lors du remplacement d’une image existante dans une variante d’e-mail sur la zone de travail [!DNL Create], la vue _Sélectionner à partir du contenu_ est désormais localisée. <!-- GS-6906 -->

+++

+++Notes de la version 2024.11.07

### Correctifs et améliorations

* L’icône _Enregistrement en cours_ ne s’affiche plus lorsqu’un utilisateur clique sur **[!UICONTROL Charger une nouvelle image]** puis annule l’opération avant la fin du chargement. <!-- GS-6780 -->

* Les titres des expériences sont désormais créés correctement lors de la régénération des expériences. <!-- GS-7006 -->

* Les problèmes liés au scintillement des barres de défilement lors du chargement du brouillon ont été résolus. <!-- GS-5587 -->

* Le lien `View documentation` dans la fenêtre contextuelle [!DNL Content] _Ajouter votre modèle approuvé_ fonctionne désormais comme prévu. <!-- GS-6881 -->

* La suppression d’une image du tiroir d’invite lors d’une opération de redimensionnement n’entraîne plus d’erreur. <!-- GS-7115 7009 -->

* Sélectionnez **[!UICONTROL Supprimer]** dans le menu d’actions [!DNL Create] (...) pour continuer. <!-- GS-6871 -->

* Les utilisateurs peuvent désormais contrôler tous les éléments interactifs Meta et de modèle uniquement à l’aide du clavier. <!-- GS-4066 -->

* Ajout de l’extraction des dimensions d’image des champs d’image de modèle aux modèles d’affichage publicitaire. Les demandes de recadrage intelligent sont désormais envoyées pour la dimension réelle de l’image et non pour le modèle entier. <!-- GS-6926 -->

* Chaîne de `Zoom to fit to screen` localisée dans l’e-mail généré et les métadonnées publicitaires. <!-- GS-5063 -->

* Le tiroir d’invite [!DNL Create] se ferme désormais comme prévu lorsqu’un utilisateur clique dessus. <!-- GS-5254 -->

* L’exportation des métadonnées inclut désormais le libellé d’appel à l’action sélectionné comme prévu. <!-- GS-6504 -->

* Le score de la marque est maintenant mis à jour et conservé comme prévu pour les expériences régénérées. <!-- GS-6535 -->

* L’exportation HTML des métadonnées publicitaires et des publicités display n’inclut plus de `div` wrapper et d’éléments `chrome`. <!-- GS-7116 -->

* Les problèmes de rendu des brouillons d’e-mails lors de la publication sont désormais résolus. <!-- GS-6394 -->

* Le bouton Zone de travail **[!UICONTROL Marque]** est désormais désactivé lorsqu’un score de marque n’est pas généré. <!-- GS-6429 -->

* Le bouton (bascule) Facebook/Instagram de la barre d’actions Zone de travail met désormais à jour les rendus d’expérience comme prévu lorsque le paramètre Zone de travail `ReadOnly` est activé. <!-- GS-7039 -->

#### Régénération de l&#39;image

* Le redimensionnement de plusieurs variantes Meta et fonctionne désormais comme prévu. Auparavant, la zone de travail n’affichait pas les variantes régénérées, mais restait vide. <!-- GS-7010 -->

* La régénération de fragment fonctionne désormais comme prévu pour les expériences redimensionnées. <!-- GS-6836 -->

* La régénération des métadonnées et des images après leur redimensionnement n’entraîne plus d’erreur. Auparavant, le redimensionnement des images avant la régénération modifiait les métadonnées du canal de `meta` en `facebook`. <!-- GS-7042 -->

+++

+++Notes de la version 2024.10.31

### Nouvelles fonctionnalités

* Le filtre de recherche **[!DNL Content]** prend désormais en charge la recherche par balise de couleur. <!-- GS-5501 -->

* La zone de travail **[!DNL Create]** affiche désormais le nombre de caractères des fragments d’e-mail. <!-- GS-5819 -->

### Correctifs et améliorations

* Des libellés de lecteur d’écran manquants ont été ajoutés aux éléments de `view` mobiles et de bureau. <!-- GS-5624 4729 -->

* Les zones d’objet et de texte pré-en-tête de l’e-mail **[!DNL Create]** Canvas sont désormais dynamiques en hauteur. <!-- GS-6258 -->

* Les problèmes de disposition liés aux bordures des emails ont été résolus. <!-- GS-6631 -->

* Le focus au clavier fonctionne désormais comme prévu sur le bouton **[!DNL Content]** **[!UICONTROL Supprimer]**. Auparavant, les utilisateurs ne pouvaient pas accéder à ce bouton à l’aide du clavier.  <!-- GS-4065 -->

+++

+++Notes de la version 2024.10.14 Disponibilité générale

Cette version présente Adobe GenStudio for Performance Marketing, une application générative basée sur l’IA qui accélère la planification, le développement et l’analyse des campagnes marketing. GenStudio for Performance Marketing permet aux équipes marketing de créer du contenu multicanal sur la marque pour les publicités, les e-mails et les campagnes, tout en fournissant des informations en temps réel pour optimiser les performances du contenu.

### Fonctionnalités

Les principales fonctionnalités du produit sont les suivantes :

**[!DNL Create]** présente la zone de travail, qui offre une expérience d’invite structurée qui permet aux éditeurs de contenu de générer rapidement du contenu et des variantes. Les responsables système forment le produit aux directives de la marque de l’entreprise. [!DNL Create] garantit que tout le contenu généré par l’IA s’aligne sur les directives de votre marque (marque, personnages clients et descriptions de produits) et rationalise la production de contenu marketing à fort impact et cohérent avec la marque.

**[!DNL Content]** stocke des ressources et des expériences approuvées organisées et conformes à la marque. Les utilisateurs de GenStudio for Performance Marketing peuvent facilement rechercher, modifier, réutiliser et partager des ressources approuvées, ce qui réduit la nécessité de recréer du contenu pour chaque campagne.

**[!DNL Reviews and Approvals]** établit un cadre permettant aux parties prenantes d’examiner et d’approuver les variantes générées avant de les enregistrer pour **[!DNL Content]** ou l’exportation.

**[!DNL Campaigns]** organise et gère les campagnes marketing, assurant ainsi une exécution et un tracking rationalisés. Les collaborateurs peuvent visualiser, planifier et suivre les campagnes afin de gérer plusieurs initiatives efficacement et d’assurer une diffusion rapide.

**[!DNL Insights]** permet d’évaluer en temps réel les performances du contenu, ce qui aide les spécialistes marketing à optimiser leurs stratégies et à prendre des décisions éclairées.

GenStudio for Performance Marketing s’intègre à d’autres produits Adobe Experience Cloud, notamment Adobe Express et Adobe AEM Assets.

+++
