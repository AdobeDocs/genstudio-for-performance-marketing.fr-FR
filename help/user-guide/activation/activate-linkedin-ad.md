---
title: Activer une publicité LinkedIn
description: Découvrez comment activer une expérience publicitaire LinkedIn.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
source-git-commit: 0ccdeb2b3375e9ee72bfc4458eeaff11709768cb
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# Activer une publicité LinkedIn

Adobe GenStudio for Performance Marketing prend en charge l’activation des expériences LinkedIn avec des ressources uniques sur les pages [Gestionnaire de campagne LinkedIn](https://business.linkedin.com/marketing-solutions) et LinkedIn.

Vous pouvez [créer une expérience LinkedIn](/help/user-guide/create/create-linkedin.md) dans GenStudio for Performance Marketing et la sélectionner pour activation, ou créer une expérience à partir de ressources approuvées dans [!DNL Activate].

L’activation d’une publicité LinkedIn suit les [mêmes étapes générales](create-activation.md) requises pour l’activation sur d’autres canaux payants. Le processus d’activation prend en charge la préparation de votre expérience publicitaire aux exigences spécifiques de LinkedIn. Après avoir activé une expérience LinkedIn dans GenStudio for Performance Marketing, utilisez LinkedIn Campaign Manager pour affiner l’expérience pour des emplacements d’annonces LinkedIn spécifiques avant la publication finale.

Les gestionnaires de système et les éditeurs de GenStudio peuvent activer les expériences publicitaires.

## Étape 1 : Configurer vos comptes LinkedIn

Avant de lancer une activation, [connectez-vous à](https://www.linkedin.com/campaignmanager/login) votre compte LinkedIn Campaign Manager.

>[!BEGINSHADEBOX]

**Conditions préalables** :

* Un compte LinkedIn Campaign Manager avec l’autorisation complète de gérer les groupes de campagnes, les campagnes et les annonces. Ce compte doit contenir des groupes de campagnes et des campagnes.

* Comptes publicitaires LinkedIn avec l’autorisation complète de créer des annonces et de publier du contenu sur des pages LinkedIn.

>[!ENDSHADEBOX]

## Étape 2 : Connexion à vos comptes LinkedIn

Avant que votre entreprise puisse activer des expériences, un responsable système GenStudio doit connecter vos comptes LinkedIn à GenStudio for Performance Marketing. Cette connexion permet aux données de circuler entre GenStudio et les outils marketing externes tels que LinkedIn, ce qui active le processus d’activation.

Une fois la synchronisation terminée, vous pouvez afficher les comptes ajoutés. La synchronisation de grandes quantités de données prend plus de temps.

## Étape 3 : préparer votre expérience

Vous pouvez lancer une activation en sélectionnant une ou plusieurs expériences approuvées avec des paramètres prédéfinis depuis [!DNL Content].

La vue _Configuration de l’expérience_ est un espace de travail permettant de peaufiner et de passer en revue les expériences avant activation. Si vous sélectionnez plusieurs expériences à activer, cette vue comprend une barre latérale gauche qui affiche des miniatures de toutes les expériences sélectionnées. Utilisez cette barre latérale gauche pour placer le focus de la vue _Configuration de l’expérience_ sur les détails de l’expérience sélectionnée.

Le _panneau d’aperçu_ prend en charge une vue interactive de votre texte et de vos ressources dans le contexte d’un emplacement publicitaire spécifique. Utilisez le menu déroulant _Sélectionner l’emplacement_ pour basculer entre les emplacements publicitaires pris en charge. Les aperçus permettent de finaliser les décisions concernant les éléments publicitaires pour des emplacements spécifiques. Lorsque vous sélectionnez un emplacement dans le panneau _Aperçu_, seule votre vue de l’annonce est affectée. Votre sélection d’emplacement dans le panneau _Aperçu_ n’est pas enregistrée.

### Activer une expérience approuvée à partir du contenu

Vous pouvez sélectionner une ou plusieurs expériences à activer sur un seul canal payant. Les expériences ne peuvent contenir qu’une seule ressource. Les détails sont chargés à partir des expériences approuvées sélectionnées.

Les détails de l’expérience modifiables sont les suivants :

* Texte de call-to-action (CTA)
* URL du site web
* Afficher le lien

**Pour sélectionner des expériences** :

1. Utilisez les outils de recherche et de filtrage de la galerie de [!DNL Content] pour identifier l’expérience à activer, puis cliquez sur **[!UICONTROL Activer]**. Vous pouvez également sélectionner une expérience et sélectionner **[!UICONTROL Activer]** dans le menu Plus (...).

   La page LinkedIn ads _configuration de l’expérience_ s’ouvre pour cette expérience. Il est prérempli avec des détails de l’expérience sélectionnée. Il peut vous être demandé de sélectionner une plateforme avant de poursuivre l’activation.

1. (Facultatif) Modifiez les valeurs dans les champs modifiables (**[!UICONTROL Call to action]**, **[!UICONTROL URL du site Web]**, *[!UICONTROL Afficher le lien]**).

1. (Facultatif) Cliquez sur **[!UICONTROL Ajouter une expérience]** pour ajouter des expériences à ce groupe d’activation.

1. Cliquez sur **[!UICONTROL Suivant]** pour confirmer la configuration de votre expérience.

## Étape 4 : confirmer la configuration du compte LinkedIn

Après avoir préparé vos expériences publicitaires, vous devez confirmer les informations de votre compte LinkedIn. La vue _Configuration de l’annonce LinkedIn_ est renseignée avec des options dérivées des comptes LinkedIn configurés.

_Les groupes Campaign_ sont un composant essentiel du gestionnaire de campagne LinkedIn. Les groupes de campagnes organisent des campagnes discrètes sous un objectif partagé. Les campagnes peuvent hériter des limites budgétaires, des objectifs et des plannings du groupe de campagnes auquel elles appartiennent.

**Pour confirmer la configuration de votre compte** :

1. Sélectionnez un compte dans le menu déroulant **[!UICONTROL Compte]**. Les options sont les comptes LinkedIn qui ont été connectés à GenStudio for Performance Marketing.

1. Sélectionnez un groupe de campagnes dans le menu déroulant **[!UICONTROL Groupe de campagnes]**. Il s’agit du groupe de campagnes LinkedIn dans lequel l’expérience est publiée.

1. Sélectionnez une campagne dans le menu déroulant **[!UICONTROL Campagnes]**. Il s’agit de la campagne LinkedIn à laquelle l’expérience publicitaire est diffusée.

1. Saisissez un nom d’annonce publicitaire dans le champ **[!UICONTROL Nom de l’annonce]** pour chaque expérience. LinkedIn Campaign Manager identifie l&#39;expérience sous ce nom.

1. Cliquez sur **[!UICONTROL Suivant]** pour confirmer la configuration de vos publicités LinkedIn.

## Étape 5 : Prévisualiser et activer votre publicité

La page _Réviser_ vous offre une dernière occasion de passer en revue votre activation avant la publication.

**Pour passer en revue et publier votre expérience** :

1. (Facultatif) Cliquez sur **[!UICONTROL Modifier la section]** en regard des détails de l’expérience ou de la plateforme à modifier.
Selon la section que vous avez sélectionnée, la vue _Configuration des expériences_ ou _Configuration de Platform_ s’ouvre.

1. (Facultatif) Modifiez les détails, puis cliquez sur **[!UICONTROL Suivant]** pour revenir à la vue _Réviser_.

1. Cliquez sur **[!UICONTROL Publier]**.

   L’expérience publicitaire LinkedIn complète et ses métadonnées associées sont directement transmises à la campagne désignée du gestionnaire de campagnes LinkedIn. Les expériences sont diffusées dans un état inactif. À partir du gestionnaire de campagne LinkedIn, vous pouvez gérer les dernières étapes de déploiement de l’expérience publicitaire et de la campagne LinkedIn.

## Étape 6 : terminer la publication de votre expérience publicitaire

1. [Connectez-vous à](https://www.linkedin.com/campaignmanager/login) votre compte LinkedIn Campaign Manager pour passer en revue votre expérience publicitaire et finaliser la publication sur des pages LinkedIn spécifiques.
