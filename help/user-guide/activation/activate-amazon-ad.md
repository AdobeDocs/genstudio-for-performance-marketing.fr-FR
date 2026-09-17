---
title: Activer Amazon Ads
description: Découvrez comment activer les expériences Amazon Ads.
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%
---
# Activer Amazon Ads

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires sur les publicités Amazon.

**Formats pris en charge** : affichage statique.

L’activation d’une expérience Amazon Ads suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux de publicités payantes. Cette page couvre les champs de configuration et les conditions préalables spécifiques à Amazon Ads. Après avoir activé une expérience dans GenStudio for Performance Marketing, utilisez Amazon Ads pour passer en revue l’expérience et lancer l’annonce.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Accès au compte Amazon Ads cible.
* Accès administrateur à ce compte, pour lire et écrire dans Amazon Ads.

Amazon Ads organise les campagnes et les annonces dans différents comptes, chacun d’eux comprenant une bibliothèque de contenu créatif. Le compte cible doit déjà exister dans Amazon Ads ; GenStudio for Performance Marketing publie les expériences publicitaires dans la bibliothèque de contenu publicitaire de ce compte, mais ne crée pas de comptes.

## Connecter votre compte Amazon Ads

Avant que votre entreprise puisse publier des ressources dans une bibliothèque de contenu créatif, un responsable système GenStudio doit connecter votre compte Amazon Ads à GenStudio for Performance Marketing. Vous devez disposer d’un accès administrateur à ce compte pour pouvoir lire et écrire dans Amazon Ads. Voir [Connecter des comptes de médias achetés](/help/user-guide/connectors/connect-channel.md).

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés.

## Champs de configuration des publicités Amazon

Les ressources approuvées sont verrouillées et ne peuvent pas être modifiées lors de l’activation, car elles ont déjà fait l’objet d’une révision et d’une approbation en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : ID de suivi (utilisé comme nom du contenu créatif de la plateforme)
* **Champs de configuration de Platform** : compte

Votre expérience créative est diffusée à la bibliothèque créative du compte sélectionné dans Amazon Ads une fois l’activation terminée.
