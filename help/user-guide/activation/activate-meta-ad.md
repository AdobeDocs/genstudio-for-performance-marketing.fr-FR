---
title: Activation d’une publicité Meta
description: Découvrez comment activer une expérience publicitaire Meta.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%
---
# Activer une publicité Meta

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires Meta sur Instagram et Facebook.

**Formats pris en charge** : image, vidéo, carrousel.

[Créez une expérience Meta](/help/user-guide/create/create-meta-ad.md) dans GenStudio for Performance Marketing, puis sélectionnez-la pour activation.

L’activation d’une publicité Meta suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux de publicité payante. Cette page couvre les champs de configuration et les conditions préalables spécifiques à Meta. Après avoir activé une expérience Meta dans GenStudio for Performance Marketing, utilisez [Meta Ads Manager](https://adsmanager.facebook.com/) pour passer en revue l’expérience et lancer l’annonce.

Contrairement à d’autres canaux, une publicité Meta peut inclure plusieurs proportions dans une seule publicité. Si votre expérience comporte plusieurs proportions, [!DNL Activate] génère toujours une seule ligne pour celle-ci, et non une par proportion.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

Vérifiez que vos comptes publicitaires Meta connectés disposent des autorisations complètes de gestion des publicités dans ces composants de la plateforme publicitaire Meta :

* Compte publicitaire Meta
* Page Facebook
* Campagne Meta
* Visionneuse publicitaire Meta
* Profil Instagram (facultatif)

La campagne Meta et le jeu d’annonces cibles doivent déjà exister dans Meta Ads Manager. GenStudio for Performance Marketing ne crée actuellement aucune campagne ni aucune visionneuse d’annonces.

## Connexion de vos comptes Meta

Avant que votre entreprise puisse activer des expériences, un responsable système GenStudio doit connecter vos comptes Meta à GenStudio for Performance Marketing. Cette connexion permet aux données de circuler entre GenStudio for Performance Marketing et Meta, ce qui active le processus d’activation. Voir [Connexion à Meta Ads](/help/user-guide/connectors/meta-ads.md).

Pour sélectionner un compte Instagram, assurez-vous dans Meta Business Manager que [le compte Instagram que vous souhaitez utiliser est connecté au même compte publicitaire](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account) sélectionné lors de l’intégration. Si cette connexion est manquante, le compte Instagram peut ne pas apparaître dans le menu déroulant **[!UICONTROL Profil Instagram]** lors de l’activation.

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés. La synchronisation de grandes quantités de données prend plus de temps.

## Champs de configuration de Meta

Les ressources, titres et corps de texte approuvés sont verrouillés et ne peuvent pas être modifiés pendant l’activation, car ils ont déjà fait l’objet d’une révision et d’une approbation en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : description, Call-to-action, URL de destination, paramètres d’URL, ID de suivi (utilisé comme nom de publicité Meta)
* **Champs de configuration de Platform** : compte publicitaire, page Facebook, profil Instagram, campagne Meta, jeu de publicités Meta
