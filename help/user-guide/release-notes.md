---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
source-git-commit: b502e0a558cbc26c70d813938734a2f6f230dc8e
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 3%

---

# Notes de mise à jour de GenStudio for Performance Marketing

Les informations de cette version détaillent les dernières mises à jour apportées à l’application GenStudio for Performance Marketing.

## 2024.11.07 {#latest}

### Correctifs

* Le compteur _Enregistrer en cours_ ne s’affiche plus lorsqu’un utilisateur clique sur **[!UICONTROL Télécharger une nouvelle image]**, puis annule l’opération avant la fin du téléchargement. <!-- GS-6780 -->

* Les titres d’expérience sont désormais créés correctement lors de la régénération de l’expérience. <!-- GS-7006 -->

* Les problèmes liés aux barres de défilement scintillantes pendant le chargement du brouillon ont été résolus. <!-- GS-5587 -->

* Le lien `View documentation` de la fenêtre contextuelle [!DNL Content] _Ajouter votre modèle approuvé_ fonctionne désormais comme prévu. <!-- GS-6881 -->

* La suppression d’une image du tiroir de l’invite lors d’une opération de redimensionnement n’entraîne plus d’erreur. <!-- GS-7115 7009 -->

* Sélectionner **[!UICONTROL Supprimer]** dans le menu d’actions [!DNL Create] (...) fonctionne désormais comme prévu. <!-- GS-6871 -->

* Les utilisateurs peuvent désormais contrôler tous les éléments interactifs de modèle de métadonnées publicitaires par clavier uniquement. <!-- GS-4066 -->

* Ajout de l’extraction des dimensions de l’image à partir des champs d’image du modèle pour afficher les modèles d’annonce. Les demandes de recadrage intelligent sont désormais envoyées pour la dimension réelle de l’image et non pour l’ensemble du modèle. <!-- GS-6926 -->

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

## 2024.10.31

### Nouvelles fonctionnalités

* Le filtre de recherche **[!DNL Content]** prend désormais en charge la recherche par balise de couleur. <!-- GS-5501 -->

* Le canevas **[!DNL Create]** affiche désormais le nombre de caractères pour les fragments de courrier électronique. <!-- GS-5819 -->

### Correctifs

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

### Informations supplémentaires

Consultez les ressources utiles suivantes :

* [Guide de l’utilisateur Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/home)

* [Adobe GenStudio Academy](genstudioacademy.md), plateforme d’apprentissage en ligne d’Adobe permettant d’utiliser des technologies d’IA générative dans le processus de création. [Inscrivez-vous à l’Académie GenStudio](http://adobe.ly/genstudioacademyregistration).
