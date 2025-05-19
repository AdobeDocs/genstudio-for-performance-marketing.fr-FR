---
title: Workflow d’activation
description: Découvrez le workflow d’activation des expériences publicitaires.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
source-git-commit: 46453d7cf1901312001aa3b304be9d0832a46079
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 0%

---

# Workflow d’activation

_[!DNL Activate]_&#x200B;prend en charge l’activation des expériences publicitaires dans des formats spécifiques à un canal, tels qu’une expérience publicitaire Meta ou Google Campaign Manager 360.

Une expérience GenStudio for Performance Marketing est un composant de campagne marketing, tel qu’une annonce, préparé en tant qu’expérience publicitaire pour une audience spécifique sur un canal d’annonce payante ou un e-mail. Les expériences d’activation contiennent trois composants principaux :

* **Ressources multimédias** : les ressources multimédias sont les images (GIF, PNG, JPEG) incluses dans votre expérience publicitaire. L’activation prend actuellement en charge les images statiques.

  La sélection d’une ressource d’image pour votre expérience publicitaire nécessite le choix d’un format approprié. Les proportions définissent la relation proportionnelle entre la largeur et la hauteur d’une image. Elles sont essentielles pour l’efficacité des emplacements publicitaires. Les canaux médias payants spécifient avec soin des proportions valides pour chaque emplacement publicitaire sur leur plateforme. Lors de l’ajout de ressources d’image à votre activation, vous devez sélectionner les proportions en fonction des emplacements publicitaires finaux pour votre expérience. Les types de fichiers sont limités à JPEG, PNG et GIF.

* **Texte** : le texte comprend toutes les formes de copie incluses dans votre publicité, y compris les titres, le corps du texte et les éléments d’appel à l’action.

* **Métadonnées** : attributs définis par l’utilisateur que vous pouvez affecter au contenu. Les métadonnées améliorent l’analyse, le filtrage et le suivi des performances. Il n’est généralement pas visible par les utilisateurs et utilisatrices.

La création d’une activation implique l’affinement de chacun de ces composants publicitaires pour un positionnement de canal et une campagne marketing désignés. GenStudio for Performance Marketing prend en charge l’activation d’une expérience sur un canal payant.

## Phases du workflow

Bien que des exigences d’emplacement uniques définissent chaque canal payant, toutes les activations d’annonces publicitaires partagent les mêmes étapes de haut niveau. L’activation d’une expérience sur n’importe quel canal payant comporte trois phases principales :

1. **Connexion de GenStudio for Performance Marketing à votre canal cible**. Un responsable système GenStudio doit connecter les comptes de vos canaux avant de pouvoir activer une expérience.

1. **Préparez votre expérience pour l’activation**. Vous pouvez préparer des expériences pour l’activation de deux manières :

   * Activez une expérience approuvée avec des paramètres prédéfinis directement depuis _[!DNL Content]_. Cette méthode simplifiée d’activation d’une ou de plusieurs expériences publicitaires sur un seul canal. Une fois que vous avez sélectionné une expérience dans la galerie&#x200B;_[!DNL Content]_, vous ne pouvez plus modifier ni ajouter de ressources à votre expérience publicitaire. L’option Activer à partir de _[!DNL Content]_&#x200B;est disponible pour les expériences de publicité Meta et Google Campaign Manager 360 .

   * Assemblez votre expérience publicitaire en sélectionnant des ressources visuelles dans _[!DNL Content]_, en ajoutant des éléments de texte et en sélectionnant des proportions. Cette méthode implique davantage d’étapes, mais offre une plus grande flexibilité créative. La préparation comprend la sélection des ressources multimédias dans les proportions appropriées pour votre emplacement publicitaire spécifique et l’affectation de texte aux éléments call-to-action et à la copie du corps. Vous pouvez ajouter des métadonnées informatives qui aident les utilisateurs à rechercher l’expérience après activation. Chaque emplacement de canal publicitaire spécifie des proportions valides pour les ressources visuelles incluses dans l’emplacement.

1. **Examinez et publiez votre expérience sur le canal cible**. Utilisez le panneau _Aperçu_ lors de la configuration de l’expérience pour évaluer votre choix d’emplacements publicitaires et d’éléments textuels avant de finaliser votre activation. Votre dernière révision avant publication a lieu dans l’application de gestion des publicités du canal de destination. Par exemple, après l’activation d’une expérience de métadonnées d’annonce dans GenStudio for Performance Marketing, vous devez vous connecter au gestionnaire de métadonnées d’annonce, passer en revue votre expérience d’annonce, puis sélectionner ses attributs spécifiques avant de la publier.

Une fois qu’une expérience publicitaire est en ligne sur son canal média payant cible, _[!DNL Insights]_&#x200B;pouvez suivre et analyser ses données de performances.

## Canaux pris en charge

Chaque canal média payant comporte un workflow d’activation unique. Sélectionnez le canal payant pour obtenir des instructions d’activation :

* [Meta](activate-meta-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
