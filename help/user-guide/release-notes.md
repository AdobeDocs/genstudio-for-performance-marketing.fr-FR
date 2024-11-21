---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substanial-update: 2024-11-14T00:00:00Z
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 720b23061d7e56a9b1e712d7787158c6a1bb771c
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 2%

---

# Notes de mise à jour de GenStudio for Performance Marketing

Les informations de cette version détaillent les dernières mises à jour apportées à l’application GenStudio for Performance Marketing.

## 2024.11.14 {#latest}

### Nouvelles fonctionnalités

Ajout de la prise en charge des modèles multimédias enrichis, qui permet aux clients de réutiliser des ressources déjà publiées par le biais de leurs propres canaux de contenu géré. <!-- GS-6107 -->

### Correctifs et améliorations

* Lorsqu’ils sont redimensionnés dans un navigateur autre que celui utilisé pour générer le contenu initial, les brouillons se chargent désormais comme prévu. <!-- GS-7204 -->

* Tous les caractères sont désormais correctement représentés dans l&#39;HTML exporté. <!-- GS-7246 -->

* Les boutons de la fenêtre contextuelle [!DNL Content] _Expériences_ **** ne sont plus tronqués dans certaines langues. <!-- GS-6873 -->

* Les publicités affichées créées avec des modèles dimensionnés à 50 x 50 sont désormais exportées dans la taille d’image attendue. Auparavant, les fichiers PNG étaient exportés au double des dimensions attendues. <!-- GS-7192 -->

* Les erreurs de modèle qui se produisaient lors du redimensionnement des publicités affichées sont désormais résolues. <!-- GS-7322 -->

### Localisation

Cette version comprend des améliorations de la localisation dans l’interface utilisateur, notamment :

* Toutes les chaînes de la fenêtre contextuelle [!DNL Content] _Télécharger la ressource_ sont désormais correctement localisées. <!-- GS-6872 6770 -->
* Toutes les info-bulles dans le champ [!DNL Content] _Vue Assets_ **[!UICONTROL Recherche]** sont localisées. <!-- GS-6879 -->
* Lors du remplacement d&#39;une image existante dans une variante d&#39;email sur le canevas [!DNL Create], la vue _Sélectionner dans le contenu_ est désormais localisée. <!-- GS-6906 -->

## Notes de mise à jour antérieures

+++Notes de 2024.11.07

### Correctifs et améliorations

* Le compteur _Enregistrer en cours_ ne s’affiche plus lorsqu’un utilisateur clique sur **[!UICONTROL Télécharger une nouvelle image]**, puis annule l’opération avant la fin du téléchargement. <!-- GS-6780 -->

* Les titres d’expérience sont désormais créés correctement lors de la régénération de l’expérience. <!-- GS-7006 -->

* Les problèmes liés aux barres de défilement scintillantes pendant le chargement du brouillon ont été résolus. <!-- GS-5587 -->

* Le lien `View documentation` de la fenêtre contextuelle [!DNL Content] _Ajouter votre modèle approuvé_ fonctionne désormais comme prévu. <!-- GS-6881 -->

* La suppression d’une image du tiroir de l’invite lors d’une opération de redimensionnement n’entraîne plus d’erreur. <!-- GS-7115 7009 -->

* Sélectionner **[!UICONTROL Supprimer]** dans le menu d’actions [!DNL Create] (...) fonctionne désormais comme prévu. <!-- GS-6871 -->

* Les utilisateurs peuvent désormais contrôler tous les éléments interactifs de modèle de métadonnées publicitaires par clavier uniquement. <!-- GS-4066 -->

* Ajout de l’extraction des dimensions de l’image des champs d’image du modèle dans les modèles d’affichage d’annonce. Les demandes de recadrage intelligent sont désormais envoyées pour la dimension réelle de l’image et non pour l’ensemble du modèle. <!-- GS-6926 -->

* Localisation de la chaîne `Zoom to fit to screen` dans le courrier électronique généré et les métadonnées publicitaires. <!-- GS-5063 -->

* Le tiroir d’invite [!DNL Create] se ferme maintenant comme prévu lorsqu’un utilisateur clique à l’extérieur. <!-- GS-5254 -->

* L’exportation des métadonnées publicitaires inclut désormais le libellé d’appel à l’action sélectionné, comme prévu. <!-- GS-6504 -->

* Le score de marque est maintenant mis à jour et conservé comme prévu pour les expériences régénérées. <!-- GS-6535 -->

* L’exportation HTML des métadonnées publicitaires et des publicités affichées n’inclut plus les éléments wrapper `div` et `chrome` . <!-- GS-7116 -->

* Les problèmes de rendu des brouillons de courrier électronique lors de la publication sont désormais résolus. <!-- GS-6394 -->

* Le bouton **[!UICONTROL Marque]** de la zone de travail est maintenant désactivé lorsqu’un score de marque n’est pas généré. <!-- GS-6429 -->

* Le bouton bascule Facebook/Instagram sur la barre d’actions Canevas met désormais à jour les rendus d’expérience comme prévu lorsque le paramètre `ReadOnly` Canevas est activé. <!-- GS-7039 -->

#### Régénération de l’image

* Le redimensionnement de plusieurs variantes de métadonnées fonctionne désormais comme prévu. Auparavant, la zone de travail n’affichait pas de variantes régénérées, mais restait vide. <!-- GS-7010 -->

* La régénération de fragments fonctionne désormais comme prévu pour les expériences redimensionnées. <!-- GS-6836 -->

* La régénération des métadonnées après leur redimensionnement ne provoque plus d’erreur. Auparavant, le redimensionnement des images avant la régénération modifiait les métadonnées du canal de `meta` à `facebook`. <!-- GS-7042 -->

+++

+++Notes de 2024.10.31

### Nouvelles fonctionnalités

* Le filtre de recherche **[!DNL Content]** prend désormais en charge la recherche par balise de couleur. <!-- GS-5501 -->

* Le canevas **[!DNL Create]** affiche désormais le nombre de caractères pour les fragments de courrier électronique. <!-- GS-5819 -->

### Correctifs et améliorations

* Des libellés de lecteur d’écran manquants ont été ajoutés aux éléments mobiles et de bureau `view`. <!-- GS-5624 4729 -->

* La hauteur de l’objet de l’email dans le canevas et les zones de texte du pré-en-tête sont désormais dynamiques. <!-- GS-6258 -->**[!DNL Create]**

* Les problèmes de mise en page avec les bordures des emails ont été résolus. <!-- GS-6631 -->

* La mise au point du clavier fonctionne désormais comme prévu sur le bouton **[!DNL Content]** **[!UICONTROL Supprimer]** . Auparavant, ce bouton n’était pas accessible ni utilisé par le clavier.  <!-- GS-4065 -->

## 2024.10.14 Disponibilité générale

Cette version présente Adobe GenStudio for Performance Marketing, une application basée sur l’IA générative qui accélère la planification, le développement et l’analyse des campagnes marketing. GenStudio for Performance Marketing permet aux équipes marketing de créer du contenu multicanal sur la marque pour les publicités, les emails et les campagnes, tout en fournissant des informations en temps réel afin d’optimiser les performances du contenu.

### Fonctionnalités

Les principales fonctionnalités du produit sont les suivantes :

**[!DNL Create]** introduit le Canevas, qui offre une expérience d’invite structurée qui permet aux éditeurs de contenu de générer rapidement du contenu et des variantes. Les responsables système forment le produit en fonction des directives de la marque de l’entreprise. [!DNL Create] assure l’alignement de tout le contenu généré par l’IA sur vos directives de marque (branding, personnages clients et descriptions de produits) et simplifie la production de contenu marketing à fort impact et cohérent pour la marque.

**[!DNL Content]** stocke des ressources et des expériences traitées et conformes à la marque. Les utilisateurs de GenStudio for Performance Marketing peuvent facilement rechercher, modifier, réutiliser et partager des ressources approuvées, ce qui réduit la nécessité de recréer entièrement le contenu pour chaque campagne.

**[!DNL Reviews and Approvals]** établit un cadre permettant aux parties prenantes de passer en revue et d’approuver les variantes générées avant de les enregistrer dans **[!DNL Content]** ou de les exporter.

**[!DNL Campaigns]** organise et gère des campagnes marketing, ce qui simplifie l’exécution et le suivi. Les collaborateurs peuvent visualiser, planifier et suivre des campagnes pour gérer efficacement plusieurs initiatives et assurer une diffusion en temps voulu.

**[!DNL Insights]** offre une évaluation en temps réel des performances du contenu, ce qui permet aux marketeurs d’optimiser leurs stratégies et de prendre des décisions basées sur les données.

GenStudio for Performance Marketing s’intègre à d’autres produits Adobe Experience Cloud, y compris Adobe Express et Adobe AEM Assets.

+++
