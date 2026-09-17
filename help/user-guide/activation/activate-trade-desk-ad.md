---
title: Activer une annonce publicitaire sur The Trade Desk
description: Découvrez comment activer un affichage statique et une expérience dans The Trade Desk.
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
source-wordcount: '461'
ht-degree: 0%
---
# Activer une annonce publicitaire sur The Trade Desk

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires sur The Trade Desk.

**Formats pris en charge** : affichage statique (pour une seule ressource uniquement).

L&#39;activation d&#39;une annonce dans The Trade Desk suit les [mêmes étapes générales](create-activation.md) requises pour l&#39;activation vers d&#39;autres canaux d&#39;annonces payantes, à une différence près. Trade Desk est un service d’entreprise géré, et non une plateforme publicitaire en libre-service. Par conséquent, l’accès au compte fonctionne différemment des autres canaux. Cette page répertorie ces différences, ainsi que les conditions préalables et les champs de configuration spécifiques à The Trade Desk.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Un compte Trade Desk actif existant. Configurez-le directement avec The Trade Desk avant de le connecter à GenStudio for Performance Marketing.
* Accès à l’API activé par votre équipe de compte Trade Desk. Pour The Trade Desk, votre équipe de compte active cet accès en votre nom à l&#39;aide d&#39;un jeton API, plutôt que de la connexion OAuth utilisée par d&#39;autres canaux publicitaires payants.
* Annonceur, siège et autorisations appropriés activés par The Trade Desk pour l’intégration de GenStudio for Performance Marketing.
* Jeton API ou informations d’identification de l’équipe chargée de votre compte Trade Desk, avec les autorisations de publier des contenus publicitaires sur le compte de l’annonceur cible.
* Une campagne de destination qui existe déjà dans The Trade Desk. GenStudio for Performance Marketing active les publicités dans cette campagne existante.

## Connecter votre compte The Trade Desk

Avant que votre entreprise puisse activer des expériences, collaborez avec l’équipe chargée de votre compte Trade Desk pour activer l’accès à l’API, puis un responsable système GenStudio connecte le compte à GenStudio for Performance Marketing :

1. Contactez votre équipe de compte The Trade Desk et demandez l’accès pour publier des contenus publicitaires de GenStudio for Performance Marketing dans votre compte The Trade Desk. Vérifiez l’ID de l’annonceur, le siège ou les détails du partenaire à utiliser pour l’activation.
1. Obtenez le jeton API ou les informations d’identification auprès de l’équipe du compte Trade Desk et vérifiez que le jeton prend en charge les autorisations de publication créative pour le compte de l’annonceur cible.
1. Dans GenStudio for Performance Marketing, accédez à **[!UICONTROL Paramètres]** > **[!UICONTROL Canaux]**, puis cliquez sur **[!UICONTROL Se connecter]** sur la mosaïque **[!UICONTROL The Trade Desk]**. Saisissez le nom du compte, l’ID publicitaire et le jeton API ou les informations d’identification, puis enregistrez la connexion.

Si la connexion échoue, vérifiez auprès de l’équipe du compte Trade Desk que l’accès à l’API a été activé et que le jeton dispose des autorisations d’annonceur et de siège appropriées.

## Champs de configuration de Trade Desk

Les ressources approuvées sont verrouillées et ne peuvent pas être modifiées lors de l’activation, car elles ont déjà fait l’objet d’une révision et d’une approbation en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : ID de suivi (utilisé comme nom du contenu créatif de la plateforme)
* **Champs de configuration de Platform** : compte, campagne

Actuellement, l’activation vers The Trade Desk prend uniquement en charge les annonces d’affichage statique à ressource unique.
