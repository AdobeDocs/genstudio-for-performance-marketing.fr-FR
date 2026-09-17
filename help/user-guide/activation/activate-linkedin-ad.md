---
title: Activer une publicité LinkedIn
description: Découvrez comment activer une expérience publicitaire LinkedIn.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%
---
# Activer une publicité LinkedIn

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences publicitaires LinkedIn sur [LinkedIn Campaign Manager](https://business.linkedin.com/marketing-solutions).

**Formats pris en charge** : Image unique, Vidéo unique.

Vous pouvez [créer une expérience LinkedIn](/help/user-guide/create/create-linkedin.md) dans GenStudio for Performance Marketing, puis la sélectionner pour activation.

L’activation d’une publicité LinkedIn suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux de publicité payante. Cette page couvre les champs de configuration et les conditions préalables spécifiques à LinkedIn. Après avoir activé une expérience LinkedIn dans GenStudio for Performance Marketing, utilisez LinkedIn Campaign Manager pour passer en revue l’expérience et lancer la publicité.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Conditions préalables

* Un compte LinkedIn Campaign Manager avec l’autorisation complète de gérer les campagnes et les annonces. Ce compte doit contenir des campagnes existantes.
* Comptes publicitaires LinkedIn avec l’autorisation complète de créer des annonces et de publier du contenu sur des pages LinkedIn.

La campagne et le jeu d&#39;annonces LinkedIn cible doivent déjà exister dans LinkedIn Campaign Manager. GenStudio for Performance Marketing ne crée pas de campagnes ni de visionneuses d’annonces.

>[!NOTE]
>
>LinkedIn a renommé sa hiérarchie de campagnes : ce que LinkedIn Campaign Manager appelait auparavant un **groupe de campagnes** s’appelle désormais une **campagne** et ce qu’il appelait auparavant une **campagne** s’appelle désormais un **ensemble d’annonces**. Les champs de configuration **[!UICONTROL Campagne LinkedIn]** et **[!UICONTROL Visionneuse d’annonces LinkedIn]** dans [!DNL Activate] utilisent cette terminologie actuelle.

GenStudio for Performance Marketing prend actuellement en charge les annonces LinkedIn à une seule image et à une seule vidéo, qui ne comportent chacune qu’une seule image ou vidéo par publication. Si votre expérience comprend plusieurs proportions, [!DNL Activate] génère une ligne distincte par proportion dans le tableau d’activation afin que chacune d’elles puisse s’exécuter en tant que propre annonce ; supprimez toutes les lignes dont vous n’avez pas besoin.

## Connecter vos comptes LinkedIn

Avant que votre entreprise puisse activer des expériences, un gestionnaire ou un éditeur du système GenStudio doit connecter vos comptes publicitaires LinkedIn à GenStudio for Performance Marketing. Vous devez disposer d’un accès administrateur complet au compte publicitaire et à la page de profil LinkedIn pour vous connecter. Vous ne devez connecter un compte publicitaire qu’une seule fois dans **[!UICONTROL Paramètres]**. Ensuite, elle est accessible à toute personne pouvant accéder à cette instance.

Cette connexion permet aux données de circuler entre GenStudio for Performance Marketing et LinkedIn, ce qui active le processus d’activation.

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés. La synchronisation de grandes quantités de données prend plus de temps.

## Champs de configuration LinkedIn

Les ressources approuvées, les titres et le texte d’introduction sont verrouillés et ne peuvent pas être modifiés pendant l’activation, car ils ont déjà été examinés et approuvés en [!DNL Content]. Vous pouvez modifier les éléments suivants :

* **Champs de texte** : description, Call-to-action, URL de destination, paramètres d’URL, ID de suivi (utilisé comme nom de publicité pour la plateforme)
* **Champs de configuration de Platform** : compte publicitaire LinkedIn, campagne LinkedIn, jeu publicitaire LinkedIn
