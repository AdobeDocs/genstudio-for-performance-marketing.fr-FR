---
title: Marketo pour GenStudio
description: Installez et configurez l’application Marketo for GenStudio Adobe Exchange afin que votre entreprise puisse utiliser les modèles Marketo Engage dans GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: c9bfee479a433a1303a66a66917b0bbe60f24a74
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 0%

---

# Marketo pour GenStudio

Les organisations qui utilisent [!DNL Marketo Engage] et [!DNL GenStudio for Performance Marketing] dans la même organisation [!DNL IMS] peuvent installer l’application **Marketo for GenStudio** à partir de [!DNL Adobe Exchange]. Une fois que l’administrateur système a validé l’application et terminé le déploiement, les auteurs peuvent choisir des modèles Marketo lors de la création d’expériences d’e-mail dans GenStudio, en regard des modèles téléchargés directement dans [!DNL Content].

Cette rubrique est destinée aux **administrateurs** qui installent l’application, collectent les informations d’identification de Marketo et déploient l’application dans Exchange. Pour connaître le fonctionnement de la syntaxe des modèles AJO et Marketo avec GenStudio, voir [Modèles AJO et Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Conditions préalables

* [!DNL Marketo Engage] doit être configuré dans l’organisation dans laquelle vous déployez l’extension.
* Les utilisateurs qui déploient l’application ont besoin de **informations d’identification**. Pour créer et récupérer ces informations d’identification, vous devez disposer d’un accès d’administrateur de produit **** (la zone **[!UICONTROL Admin]** doit être disponible lorsque vous ouvrez Marketo).

## Installation de l’application à partir d’Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483299?learn=on)

1. Ouvrez [](https://exchange.adobe.com) puis accédez à **[!UICONTROL Experience Cloud]**.
1. Ouvrez la liste [Marketo for GenStudio](https://exchange.adobe.com/apps/ec/ab6p21vo8r/marketo-for-genstudio).
   Liste de ![Marketo for GenStudio sur Adobe Exchange](/help/extensibility/marketo-adobe-exchange.png){width="75%"}
1. Sélectionnez **[!UICONTROL Gratuit]** pour demander l’application pour votre organisation.
1. Une fois que votre organisation a **révisé et approuvé** la demande, continuez avec [Obtention des informations d’identification Marketo](#get-marketo-credentials) et [ Déploiement de l’application à partir d’Exchange](#deploy-the-application-from-exchange).

## Obtention des informations d’identification Marketo

Vous utilisez les informations d’identification de votre instance **** (et non de Adobe Developer Console). Collectez les informations d’identification suivantes en suivant les étapes ci-dessous avant de procéder au déploiement dans Exchange.

>[!NOTE]
>
>Pour générer et récupérer les informations d’identification Marketo, vous devez disposer d’un accès d’administrateur de produit Marketo. Dans le cas contraire, l’onglet Administrateur n’est pas visible dans Marketo.

### Créer un utilisateur API uniquement (facultatif si vous réutilisez un utilisateur API existant)

1. Dans Marketo, accédez à **[!UICONTROL Admin]**.
   ![Onglet Administrateur ](/help/extensibility/marketo-admin-global.png){width="80%"}
1. Sous **[!UICONTROL Sécurité]**, ouvrez **[!UICONTROL Utilisateurs et rôles]** et accédez à l’onglet **[!UICONTROL Rôles]**.
1. Créez un nouveau rôle ou modifiez un rôle existant, en y ajoutant les autorisations suivantes : _API Access_ et _Access Design Studio_.
1. Pour un nouvel utilisateur d’API, cliquez sur **[!UICONTROL Créer un utilisateur d’API uniquement]** (utilisez un e-mail unique pour chaque utilisateur d’API).
1. Cochez la case correspondant aux rôles et affectez le nouveau rôle que vous avez créé. Si vous souhaitez déjà utiliser un utilisateur d’API, passez à [Créer ou sélectionner un service LaunchPoint](#create-or-select-a-launchpoint-service).

![Utilisateurs et rôles avec des rôles d’utilisateur et d’API uniquement](/help/extensibility/marketo-users-roles-api-user.png){width="80%"}

### Créer ou sélectionner un service LaunchPoint

1. Dans **[!UICONTROL Admin]**, sous **[!UICONTROL Intégration]**, ouvrez **[!UICONTROL LaunchPoint]**.
1. Cliquez sur **[!UICONTROL Créer]** pour créer un service (ou utiliser un service personnalisé existant).
   ![Service personnalisé LaunchPoint](/help/extensibility/marketo-launchpoint-custom-service.png){width="80%"}
1. Pour votre service, cliquez sur **[!UICONTROL Afficher les détails]** et copiez les **[!UICONTROL ID client]** et **[!UICONTROL Secret client]**. Vous les entrerez dans Adobe Exchange **[!UICONTROL Configuration]**.

### Notez l’URL de base de l’API REST Marketo

1. Dans **[!UICONTROL Admin]**, sous **[!UICONTROL Intégration]**, ouvrez **[!UICONTROL Web Services]**.
1. Recherchez le point d’entrée **[!UICONTROL API REST]**. Copiez uniquement l’**URL de base** (hôte), dans le `https://###-XXX-###.mktorest.com` de formulaire. N’incluez **** de segments de chemin tels que `/rest` ou `/identity`. Cette valeur est unique par instance Marketo.

![URL de base du point d’entrée de l’API REST des services web](/help/extensibility/marketo-web-services-rest-endpoint.png){width="80%"}

Vous aurez également besoin de l’**[!UICONTROL URL d’identité]** demandée par votre écran de déploiement Exchange, ainsi que de l’URL de base REST et de l’ID client et du secret client de LaunchPoint.

## Déployer l’application à partir d’Exchange

Pour rendre l’extension disponible dans GenStudio, déployez l’application à partir d’Adobe Exchange.

1. Revenez à [](https://exchange.adobe.com).
1. Sélectionnez **[!UICONTROL Gérer]** et ouvrez l’application **Marketo for GenStudio** (par exemple sous **[!UICONTROL Applications App Builder]** ou les applications gérées de votre organisation).
1. Sous **[!UICONTROL Environnements]**, choisissez un environnement existant dans la liste déroulante ou sélectionnez **[!UICONTROL Ajouter un environnement]** pour en créer un.
1. Ouvrez **[!UICONTROL Configuration]** pour l’environnement sélectionné.
1. Saisissez l’**[!UICONTROL ID client]** et le **[!UICONTROL Secret client]** à partir de [LaunchPoint](#create-or-select-a-launchpoint-service), l’**[!UICONTROL URL d’identité Marketo Engage]** et l’**[!UICONTROL URL de base de l’API REST Marketo Engage]** (l’hôte de base à partir de [Web Services](#note-your-marketo-rest-api-base-url)) pour l’URL d’identité Marketo Engage &#x200B;et l’URL de base de l’API REST Marketo Engage.
1. Cliquez sur **[!UICONTROL Déployer]**. Lorsque le déploiement réussit, l’action devient **[!UICONTROL Annuler le déploiement]**.

### Mettre à jour la configuration

Pour modifier les valeurs de configuration d’un environnement, commencez par **[!UICONTROL Annuler le déploiement]**, mettez à jour les champs, puis **[!UICONTROL Déployer]**.

### Configuration de Workspace (facultatif)

Vous pouvez ignorer cette étape si vous envisagez d’utiliser l’espace de travail par défaut. Par défaut, les champs **Workspace ID** et **Taille de page de la liste des modèles** sont préconfigurés.

Cependant, si vous devez récupérer des modèles à partir d’un autre espace de travail :

1. Dans Marketo, accédez à **[!UICONTROL Admin]** → **[!UICONTROL Sécurité]** → **[!UICONTROL Espaces de travail et partitions]**.
1. La colonne **Workspace ID** est masquée par défaut. Pour l’activer, cliquez avec le bouton droit de la souris sur la ligne d’en-tête (où les noms des colonnes sont affichés).
1. Sélectionnez **[!UICONTROL Colonnes]**.
1. Activez **[!UICONTROL ID]** à partir de la liste.
   ![Espaces de travail et partitions avec la colonne Workspace ID activée](/help/extensibility/marketo-workspace-id.png){width="80%"}

Une fois visible, utilisez l’identifiant Workspace **approprié** pour votre configuration.

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

### Erreur « Aucun modèle trouvé »

Si l’extension s’installe correctement et que l’onglet Modèles Marketo est visible mais affiche « Aucun modèle trouvé », le problème peut être dû au fait que l’application a dépassé les limites de taille lors du rendu des modèles, ce qui entraîne un blocage.
Pour résoudre ce problème :

1. Annulez le déploiement de l’application à partir d’Exchange.
1. Réduisez la taille de la page de la liste de modèles (par exemple, définissez-la sur 1 ou 2).
1. Redéployez l’application.
