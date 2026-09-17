---
title: Activer une publicité Innovid
description: Découvrez comment activer une expérience Innovid.
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%
---
# Activer une annonce Innovid

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires sur Innovid.

**Formats pris en charge** : affichage statique, affichage Zip HTML5.

L’activation d’une expérience Innovid suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux publicitaires payants. Cette page couvre les champs prérequis et configuration spécifiques à Innovid. Après avoir activé une expérience dans GenStudio for Performance Marketing, utilisez Innovid pour passer en revue l’expérience et lancer la publicité.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Accès au compte Innovid cible.
* Accès administrateur à ce compte, pour lire et écrire dans Innovid.

Innovid organise des campagnes et des publicités dans différents comptes, chacun disposant d’une bibliothèque de contenu créatif. La bibliothèque de contenu créatif cible doit déjà exister dans Innovid ; GenStudio for Performance Marketing publie les expériences publicitaires dans cette bibliothèque de contenu créatif, mais ne crée pas de comptes ni de bibliothèques de contenu créatif.

## Connecter votre compte Innovid

Avant que votre entreprise puisse publier des ressources dans une bibliothèque de contenu créatif, un responsable système GenStudio doit connecter votre compte Innovid à GenStudio for Performance Marketing. Vous devez disposer d’un accès administrateur à ce compte pour pouvoir lire et écrire dans Innovid. Voir [Connecter des comptes de médias achetés](/help/user-guide/connectors/connect-channel.md).

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés.

## Champs de configuration non valides

Les ressources approuvées sont verrouillées et ne peuvent pas être modifiées lors de l’activation, car elles ont déjà fait l’objet d’une révision et d’une approbation en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : ID de suivi (utilisé comme nom du contenu créatif de la plateforme)
* **Champs de configuration de Platform** : compte, bibliothèque Creative, nom du concept

Votre expérience créative est diffusée à la bibliothèque créative sélectionnée dans Innovid une fois l’activation terminée.
