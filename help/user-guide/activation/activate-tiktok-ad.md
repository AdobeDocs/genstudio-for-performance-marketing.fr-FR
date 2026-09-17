---
title: Activation d’une publicité TikTok
description: Découvrez comment activer une expérience publicitaire vidéo intégrée à TikTok.
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
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
source-wordcount: '294'
ht-degree: 1%
---
# Activer une publicité TikTok

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires TikTok.

**Formats pris en charge** : publicités vidéo intégrées.

Vous pouvez [créer une expérience TikTok](/help/user-guide/create/tiktok-experiences.md) dans GenStudio for Performance Marketing, puis la sélectionner pour activation.

L’activation d’une publicité TikTok suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux de publicité payante. Cette page couvre les champs de configuration et les conditions préalables spécifiques à TikTok. Après avoir activé une expérience TikTok dans GenStudio for Performance Marketing, utilisez le gestionnaire de publicités TikTok pour effectuer les vérifications finales et lancer la publicité.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Compte TikTok Ads avec accès Opérateur ou Administrateur.
* Au moins un compte publicitaire TikTok activé pour l’utilisation, connecté par un gestionnaire système ou un éditeur GenStudio.
* La campagne TikTok cible doit déjà exister dans TikTok Ads Manager. TikTok Ads Manager, et non GenStudio for Performance Marketing, définit le budget, les enchères, l’optimisation et le ciblage du groupe publicitaire.

## Connexion à votre compte TikTok

Avant que votre entreprise puisse activer des expériences, un responsable système GenStudio doit connecter votre compte TikTok Ads à GenStudio for Performance Marketing :

1. Accédez à **[!UICONTROL Paramètres]** > **[!UICONTROL TikTok]** > **[!UICONTROL Se connecter]**.
1. Connectez-vous à votre compte TikTok Ads Manager dans la fenêtre qui s’ouvre et terminez la connexion OAuth. Votre compte doit disposer d’un accès opérateur ou administrateur au compte publicitaire.

Une fois la connexion établie, vérifiez qu’au moins un compte publicitaire TikTok est activé pour être utilisé.

## Champs de configuration de TikTok

Les ressources approuvées et le texte principal sont verrouillés et ne peuvent pas être modifiés pendant l’activation, car ils ont déjà été examinés et approuvés en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : Call-to-action, URL de destination, ID de tracking (utilisé comme nom de publicité pour la plateforme)
* **Champs de configuration de Platform** : compte TikTok Ads, campagne, groupe publicitaire
