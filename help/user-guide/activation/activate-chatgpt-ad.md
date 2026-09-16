---
title: Activer une annonce publicitaire ChatGPT
description: Découvrez comment activer une expérience publicitaire ChatGPT.
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
source-wordcount: '272'
ht-degree: 0%
---
# Activer une annonce ChatGPT

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires ChatGPT.

**Formats pris en charge** : cartes de conversation.

Vous pouvez [créer une expérience ChatGPT](/help/user-guide/create/create-chatgpt-ad.md) dans GenStudio for Performance Marketing, puis la sélectionner pour activation.

L’activation d’une publicité ChatGPT suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux de publicité payante. Cette page couvre les champs de configuration et les conditions préalables spécifiques à ChatGPT. Après avoir activé une expérience ChatGPT dans GenStudio for Performance Marketing, utilisez OpenAI Ads Manager pour effectuer les vérifications finales et lancer la publicité.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Un compte OpenAI Ads et une clé API provenant de ce compte.
* La campagne ChatGPT cible et le groupe publicitaire doivent déjà exister dans OpenAI Ads Manager. GenStudio for Performance Marketing ne crée pas de campagnes ni de groupes publicitaires.

## Connecter votre compte ChatGPT

Avant que votre entreprise puisse activer des expériences, un responsable système GenStudio doit connecter votre compte OpenAI Ads à GenStudio for Performance Marketing :

1. Dans OpenAI Ads Manager, accédez à **[!UICONTROL Paramètres]** > **[!UICONTROL Clés API]** > **[!UICONTROL Créer une clé]**.
1. Dans GenStudio for Performance Marketing, accédez à **[!UICONTROL Plus]** > **[!UICONTROL Paramètres]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Se connecter]** > **[!UICONTROL Ajouter un compte]**.
1. Saisissez le nom de votre compte OpenAI Ads, collez votre clé API, puis cliquez sur **[!UICONTROL Ajouter un compte]**.

## Champs de configuration GPT de conversation

Les ressources approuvées, les titres (titre) et la copie du corps sont verrouillés et ne peuvent pas être modifiés pendant l’activation, car ils ont déjà été examinés et approuvés en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : URL cible, ID de tracking (utilisé comme nom de publicité pour la plateforme)
* **Champs de configuration de Platform** : compte OpenAI Ads, campagne OpenAI, groupe publicitaire OpenAI

L’URL cible doit utiliser un format de `https://` valide, par exemple `https://www.example.com`.
