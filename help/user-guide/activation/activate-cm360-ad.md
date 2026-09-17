---
title: Activer une publicité Google Campaign Manager 360
description: Découvrez comment activer une expérience Google Campaign Manager 360.
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 0%
---
# Activer une publicité Google Campaign Manager 360

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires dans Google Campaign Manager 360.

**Formats pris en charge** : affichage statique, affichage vidéo, affichage Zip HTML5.

L’activation d’une publicité Google Campaign Manager 360 suit les [mêmes étapes générales](create-activation.md) requises pour l’activation vers d’autres canaux de publicité payante. Cette page couvre les champs de configuration et de conditions préalables spécifiques à Google Campaign Manager 360. Après avoir activé une expérience dans GenStudio for Performance Marketing, utilisez Google Campaign Manager 360 pour passer en revue l’expérience et lancer la publicité.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Un compte Google Campaign Manager 360 avec accès à l’annonceur cible.
* Accès administrateur à l’annonceur, pour lire et écrire dans Campaign Manager 360.

Campaign Manager 360 organise des campagnes et des publicités au sein de différents annonceurs, chacun d’eux comprenant une bibliothèque de contenu créatif. L’annonceur cible doit déjà exister dans Campaign Manager 360 ; GenStudio for Performance Marketing publie les expériences publicitaires dans la bibliothèque de contenu publicitaire de cet annonceur, mais ne crée pas d’annonces.

## Connexion à votre compte Google Campaign Manager 360

Avant que votre entreprise puisse publier des ressources dans une bibliothèque de contenu créatif, un gestionnaire ou un éditeur du système GenStudio doit connecter votre compte Google Campaign Manager 360 à GenStudio for Performance Marketing. Vous devez disposer d’un accès administrateur à l’annonceur pour lire et écrire dans Campaign Manager 360. Voir [Connecter des comptes de médias achetés](/help/user-guide/connectors/connect-channel.md).

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés.

## Champs de configuration de Google Campaign Manager 360

Les ressources approuvées sont verrouillées et ne peuvent pas être modifiées lors de l’activation, car elles ont déjà fait l’objet d’une révision et d’une approbation en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : ID de suivi (utilisé comme nom du contenu créatif de la plateforme)
* **Champs de configuration de Platform** : annonceur

Votre expérience créative est diffusée à la bibliothèque créative de l’annonceur sélectionné dans Google Campaign Manager 360 une fois l’activation terminée.
