---
title: Marketo pour GenStudio
description: Installez et configurez l’application Marketo for GenStudio Adobe Exchange afin que votre entreprise puisse utiliser les modèles Marketo Engage dans GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: 4118624b479905cd2f2193d542c000678daaf4b8
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Marketo pour GenStudio

Les organisations qui utilisent [!DNL Marketo Engage] et [!DNL GenStudio for Performance Marketing] dans la même organisation [!DNL IMS] peuvent installer l’application **Marketo for GenStudio** à partir de [!DNL Adobe Exchange]. Une fois que l’administrateur système a validé l’application et terminé le déploiement, les auteurs peuvent choisir des modèles Marketo lors de la création d’expériences d’e-mail dans GenStudio, en regard des modèles téléchargés directement dans [!DNL Content].

Cette rubrique est destinée aux **administrateurs** qui installent l’application, collectent les informations d’identification de Marketo et déploient l’application dans Exchange. Pour connaître le fonctionnement de la syntaxe des modèles AJO et Marketo avec GenStudio, voir [Modèles AJO et Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Conditions préalables

* [!DNL Marketo Engage] doit être configuré dans l’organisation dans laquelle vous déployez l’extension.
* Les utilisateurs qui déploient l’application ont besoin de **informations d’identification**. Pour créer et récupérer ces informations d’identification, vous devez disposer d’un accès d’administrateur de produit **&#x200B;**&#x200B;(la zone **[!UICONTROL Admin]** doit être disponible lorsque vous ouvrez Marketo).

## Installation de l’application à partir d’Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483313?captions=fre_fr&learn=on)

1. Ouvrez [&#128279;](https://exchange.adobe.com) puis accédez à **[!UICONTROL Experience Cloud]**.
1. Ouvrez la liste [Marketo for GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio).
   Liste de ![Marketo for GenStudio sur Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Sélectionnez **[!UICONTROL Gratuit]** pour demander l’application pour votre organisation.
1. Une fois que votre organisation a **révisé et approuvé** la demande, continuez avec [Obtention des informations d’identification Marketo](#get-marketo-credentials) et [&#x200B; Déploiement de l’application à partir d’Exchange](#deploy-the-application-from-exchange).

## Obtention des informations d’identification Marketo

Vous utilisez les informations d’identification de votre instance **&#x200B;**&#x200B;(et non de Adobe Developer Console). Collectez les éléments suivants avant de procéder au déploiement dans Exchange.

### Créer un utilisateur API uniquement (facultatif si vous réutilisez un utilisateur API existant)

1. Dans Marketo, accédez à **[!UICONTROL Admin]**.
1. Sous **[!UICONTROL Sécurité]**, ouvrez **[!UICONTROL Utilisateurs et rôles]**.
1. Pour un nouvel utilisateur d’API, cliquez sur **[!UICONTROL Créer un utilisateur d’API uniquement]** (utilisez un e-mail unique pour chaque utilisateur d’API). Attribuez le rôle **[!UICONTROL Rôles d’API (tous les espaces de travail)]** (ou les rôles requis par votre organisation). Si vous souhaitez déjà utiliser un utilisateur d’API, passez à [Créer ou sélectionner un service LaunchPoint](#create-or-select-a-launchpoint-service).

![Utilisateurs et rôles avec des rôles d’utilisateur et d’API uniquement](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### Créer ou sélectionner un service LaunchPoint

1. Dans **[!UICONTROL Admin]**, sous **[!UICONTROL Intégration]**, ouvrez **[!UICONTROL LaunchPoint]**.
1. Cliquez sur **[!UICONTROL Créer]** pour créer un service (ou utiliser un service personnalisé existant).
   ![Service personnalisé LaunchPoint](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. Pour votre service, cliquez sur **[!UICONTROL Afficher les détails]** et copiez les **[!UICONTROL ID client]** et **[!UICONTROL Secret client]**. Vous les entrerez dans Adobe Exchange **[!UICONTROL Configuration]**.

### Notez l’URL de base de l’API REST Marketo

1. Dans **[!UICONTROL Admin]**, sous **[!UICONTROL Intégration]**, ouvrez **[!UICONTROL Web Services]**.
1. Recherchez le point d’entrée **[!UICONTROL API REST]**. Copiez uniquement l’**URL de base** (hôte), dans le `https://###-XXX-###.mktorest.com` de formulaire. N’incluez **&#x200B;**&#x200B;de segments de chemin tels que `/rest` ou `/identity`. Cette valeur est unique par instance Marketo.

![URL de base du point d’entrée de l’API REST des services web](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

Vous aurez également besoin de l’**[!UICONTROL URL d’identité]** demandée par votre écran de déploiement Exchange, ainsi que de l’URL de base REST et de l’ID client et du secret client de LaunchPoint.

## Déployer l’application à partir d’Exchange

Pour rendre l’extension disponible dans GenStudio, déployez l’application à partir d’Adobe Exchange.

1. Revenez à [&#128279;](https://exchange.adobe.com).
1. Sélectionnez **[!UICONTROL Gérer]** et ouvrez l’application **Marketo for GenStudio** (par exemple sous **[!UICONTROL Applications App Builder]** ou les applications gérées de votre organisation).
1. Sous **[!UICONTROL Environnements]**, choisissez un environnement existant dans la liste déroulante ou sélectionnez **[!UICONTROL Ajouter un environnement]** pour en créer un.
1. Ouvrez **[!UICONTROL Configuration]** pour l’environnement sélectionné.
1. Saisissez l’**[!UICONTROL ID client]** et le **[!UICONTROL Secret client]** à partir de [LaunchPoint](#create-or-select-a-launchpoint-service), l’**[!UICONTROL URL d’identité Marketo Engage]** et l’**[!UICONTROL URL de base de l’API REST Marketo Engage]** (hôte de base à partir de [Services web](#note-your-marketo-rest-api-base-url)).
1. Cliquez sur **[!UICONTROL Déployer]**. Lorsque le déploiement réussit, l’action devient **[!UICONTROL Annuler le déploiement]**.

### Mettre à jour la configuration

Pour modifier les valeurs de configuration d’un environnement, commencez par **[!UICONTROL Annuler le déploiement]**, mettez à jour les champs, puis **[!UICONTROL Déployer]**.

## Accès aux modèles Marketo dans GenStudio

Une fois Marketo for GenStudio installé et configuré, un onglet **[!UICONTROL Modèles Marketo]** s’affiche lorsque vous créez une expérience **E-mail** dans GenStudio. Utilisez cet onglet pour parcourir les modèles à partir de Marketo Engage.

>[!IMPORTANT]
>
>Créez des e-mails sous le flux d’expérience **e-mail standard** dans GenStudio for Performance Marketing. Cette intégration ne prend PAS en charge les e-mails créés avec la nouvelle expérience de l&#39;éditeur d&#39;e-mail.

![Configuration d’Exchange avec des informations d’identification Marketo](/help/extensibility/marketo-exchange-configuration.png){width="80%"}

## Dépannage

### L’onglet Modèles Marketo n’est pas visible

* Vérifiez que l’application est **approuvée** dans Exchange et que l’environnement est **déployé** avec un ID client, un secret client et des URL de base Marketo valides.
* Demandez à votre administrateur de vérifier que l&#39;accès **Administrateur de produit** a été utilisé lors de la création des informations d&#39;identification.

### Modèles non chargés

* Rechargez la page ou déconnectez-vous et reconnectez-vous à GenStudio.
* Dans le panneau des outils de développement du navigateur **[!UICONTROL Réseau]**, recherchez les appels d’API ayant échoué vers votre instance Marketo et vérifiez que l’URL de base REST correspond à **[!UICONTROL Services web]** dans Marketo (aucun chemin supplémentaire après l’hôte).
