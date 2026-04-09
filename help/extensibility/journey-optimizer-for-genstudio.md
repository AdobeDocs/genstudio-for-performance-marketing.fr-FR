---
title: Journey Optimizer pour GenStudio
description: Installez et configurez l’application Journey Optimizer for GenStudio Adobe Exchange afin que votre entreprise puisse utiliser les modèles Adobe Journey Optimizer dans GenStudio for Performance Marketing.
feature: Extensibility
source-git-commit: fbec4567d960a6e3607c5e5e43057e2f22e9f6ea
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Journey Optimizer pour GenStudio

Les organisations qui utilisent [!DNL Adobe Journey Optimizer] (AJO) et [!DNL GenStudio for Performance Marketing] dans la même organisation [!DNL IMS] peuvent installer l’application **Journey Optimizer for GenStudio** à partir de [!DNL Adobe Exchange]. Une fois que l’administrateur système a validé l’application et terminé le déploiement, les auteurs peuvent choisir des modèles de contenu AJO lors de la création d’expériences e-mail dans GenStudio, en regard des modèles téléchargés directement dans [!DNL Content].

Cette rubrique est destinée aux **administrateurs et développeurs** qui installent l’application, créent des informations d’identification OAuth dans l’[!DNL Adobe Developer Console] et mappent des autorisations de compte technique dans [!DNL Adobe Experience Platform]. Pour connaître le fonctionnement de la syntaxe des modèles AJO et Marketo avec GenStudio, voir [Modèles AJO et Marketo](/help/user-guide/templates/use-templates.md#templates-from-ajo-and-marketo).

## Conditions préalables

* AJO doit être configuré dans l’organisation dans laquelle vous déployez l’extension.
* Les utilisateurs qui créent des modèles dans AJO doivent être autorisés à **créer et modifier** des modèles de contenu dans Journey Optimizer, selon la définition de votre entreprise.
* Les modèles d’e-mail dans AJO doivent inclure des espaces réservés de champ (barres de contrôle) où le contenu généré doit apparaître. Un modèle peut être sélectionné sans ces champs, mais **la génération de l’expérience échoue** si les espaces réservés attendus par [!DNL GenStudio for Performance Marketing] sont manquants. Voir [Personnalisation d’un modèle](/help/user-guide/templates/customize-template.md) et [Noms de champ reconnus](/help/user-guide/templates/customize-template.md#recognized-field-names).

## Installation de l’application à partir d’Adobe Exchange

>[!VIDEO](https://video.tv.adobe.com/v/3483287?learn=on)

1. Ouvrez [&#128279;](https://exchange.adobe.com) puis accédez à **[!UICONTROL Experience Cloud]**.
1. Ouvrez la liste [Journey Optimizer for GenStudio](https://exchange.adobe.com/apps/ec/abpopqqr1q/journey-optimizer-for-genstudio).
   ![Liste Journey Optimizer for GenStudio sur Adobe Exchange, y compris les conditions requises et l’installation gratuite](/help/extensibility/ajo-adobe-exchange.png){width="75%"}
1. Sélectionnez **[!UICONTROL Gratuit]** pour demander l’application pour votre organisation.
1. Une fois que votre organisation a **révisé et approuvé** la demande, continuez avec [Création des informations d’identification OAuth dans Adobe Developer Console](#create-oauth-credentials-in-adobe-developer-console) et [&#x200B; Déploiement de l’application à partir d’Exchange](#deploy-the-application-from-exchange).

## Création d’informations d’identification OAuth dans Adobe Developer Console

Créez un **projet** dans le [Adobe Developer Console](https://developer.adobe.com/console/) qui fournit des informations d’identification OAuth pour l’API Journey Optimizer. Vous aurez besoin de valeurs telles que **ID client**, **Secret client**, **ID d’organisation** et **Portée** lorsque vous configurez l’application dans Exchange.

1. Connectez-vous à Adobe Developer Console et créez un **projet**.
1. Ajoutez l’API **Adobe Journey Optimizer (AJO)** au projet en cliquant sur **[!UICONTROL Ajouter une API]** et en sélectionnant **[!UICONTROL Adobe Journey Optimizer]** dans la liste des API de produit **[!DNL Experience Cloud]**.
1. Générez des informations d’identification dans l’espace de travail du projet et copiez **ID client**, **Secret client**, **ID d’organisation**, **Portée** et toute autre valeur demandée par votre flux de déploiement. Conservez-les en lieu sûr pour la section suivante.

>[!NOTE]
>
>Lors de l’installation à partir d’Exchange, utilisez l’ID client **OAuth** si un ID client OAuth et un ID de compte technique sont affichés.

## Déployer l’application à partir d’Exchange

### Ouvrez l’application dans Gérer et ajoutez un environnement

1. Revenez à [&#128279;](https://exchange.adobe.com).
1. Sélectionnez **[!UICONTROL Gérer]** et ouvrez **[!UICONTROL les applications App Builder]** (ou le chemin d’accès de votre organisation aux applications gérées).
1. Sélectionnez **Journey Optimizer pour GenStudio** et vérifiez que l’application est **approuvée**.
1. Sous **[!UICONTROL Environnements]**, choisissez un environnement existant dans le menu déroulant **Environnements :** ou sélectionnez **[!UICONTROL Ajouter un environnement]** pour en créer un.
   ![Détails de l’application avec le statut Approuvé et Ajouter un environnement](/help/extensibility/ajo-config-002.png){width="50%"}
1. Dans l’environnement sélectionné, sélectionnez **[!UICONTROL Configuration]**.
1. Dans l’onglet **[!UICONTROL Configuration]**, recherchez **[!UICONTROL AJO Credentials]**.
   ![Configuration avec les informations d’identification AJO avant le déploiement (brouillon)](/help/extensibility/ajo-config-004.png){width="80%"}
1. Saisissez les informations d’identification du projet Developer Console auquel l’API Journey Optimizer a été ajoutée (par exemple, **[!UICONTROL l’ID client AJO]**, **[!UICONTROL le secret client AJO]** et **[!UICONTROL le point d’entrée du jeton AJO]** ainsi que tout autre champ obligatoire).
1. Saisissez le **nom du sandbox en minuscules** (par exemple, `prod`).
1. Cliquez sur **[!UICONTROL Déployer]**. Une fois le déploiement terminé, le statut indique comme déployé. Le texte du bouton devient **[!UICONTROL Annuler le déploiement]**.
   ![Application déployée avec l’option Annuler le déploiement disponible dans la vue des applications App Builder](/help/extensibility/ajo-config-005.png){width="80%"}

Après le déploiement, Adobe Developer Console inclut un nouveau projet généré automatiquement nommé **Journey Optimizer pour GenStudio &lt;Your_Environment_Name>** avec les API AJO et Adobe Runtime. Ce projet est en lecture seule et ne peut pas être modifié ni supprimé.
![Projet Developer Console généré automatiquement en lecture seule après le déploiement](/help/extensibility/ajo-auto-project.png){width="100%"}

### Mettre à jour la configuration

Pour modifier les variables de configuration d’un environnement, commencez par **[!UICONTROL Annuler le déploiement]**, mettez à jour les valeurs, puis **[!UICONTROL Déployer]** pour que les modifications prennent effet.

Vous pouvez créer **plusieurs environnements** dans Exchange (par exemple, un par sandbox). Chaque déploiement peut faire surface en tant qu’expérience distincte dans GenStudio lorsque votre organisation utilise plusieurs sandbox.

## Mapper les autorisations pour le compte technique

Les utilisateurs peuvent voir l’extension AJO dans GenStudio sans accès [!DNL Adobe Experience Platform] complet. Pour les appels d’API (par exemple, le chargement de modèles), le compte technique lié aux informations d’identification OAuth doit se voir accorder des autorisations Journey Optimizer dans **[!DNL Adobe Experience Platform]** > **[!UICONTROL Autorisations]**. Les noms de rôle et les jeux d’autorisations exacts dépendent de votre organisation.

Affichez l’extension sous **[!UICONTROL Administrateur de Parcours]** dans AJO **[!UICONTROL Autorisations]** > **[!UICONTROL Rôles]** et ajoutez les **Informations d’identification d’API** à partir du projet Developer Console, les mêmes informations d’identification que celles que vous avez utilisées lors d’un déploiement à partir d’Exchange.

![Informations d’identification d’API affectées au rôle Architecte AJO dans les autorisations Adobe Experience Platform](/help/extensibility/ajo-map-permissions.png){width="80%"}

**Voir aussi** (contrôle d’accès Journey Optimizer) :

* [Contrôle d’accès](https://experienceleague.adobe.com/fr/docs/journey-optimizer/using/access-control/access-control-landing-page)
* [Autorisations dans Journey Optimizer](https://experienceleague.adobe.com/fr/docs/journey-optimizer/using/access-control/permissions)
* [Prise en main pour les administrateurs système](https://experienceleague.adobe.com/fr/docs/journey-optimizer/using/get-started/quick-start/administrator)

## Accès aux modèles AJO dans GenStudio

Après le déploiement et le mappage des autorisations :
1. Ouvrez **[!UICONTROL Créer]** dans GenStudio for Performance Marketing et lancez une expérience **E-mail**.
1. Dans **[!UICONTROL Sélectionner un modèle]**, ouvrez l’onglet **[!UICONTROL Modèle AJO]** à côté de **[!UICONTROL Modèles chargés]** pour parcourir les modèles à partir de Journey Optimizer.

![Sélectionner un modèle avec l’onglet Modèle AJO et la galerie de modèles](/help/extensibility/ajo-template-tab.png){width="80%"}

## Dépannage

### L’onglet Modèles AJO n’est pas visible

* Vérifiez que les valeurs saisies dans Exchange **[!UICONTROL Configuration]** sont correctes, y compris **ID client**, **Secret client**, **Portée** et **Sandbox**.
* Assurez-vous que le **nom du sandbox est en minuscules** (par exemple, `prod`).
* Lors de l’installation à partir d’Exchange, utilisez l’**ID client** comme décrit dans [Création d’informations d’identification OAuth](#create-oauth-credentials-in-adobe-developer-console).

### L’onglet Modèles AJO est visible, mais aucun modèle n’apparaît

* Rechargez la page ou rouvrez l’onglet **[!UICONTROL Modèle]**.
* Dans les outils **[!UICONTROL Réseau]** du navigateur, examinez la requête **`get-templates`**. S’il renvoie **403 Interdit**, le compte technique n’est pas affecté à un rôle ou à un groupe avec les autorisations Journey Optimizer requises. Mettez à jour les mappages dans [!DNL Adobe Experience Platform] **[!UICONTROL Autorisations]** et dans AJO **[!UICONTROL Autorisations]** selon les besoins de votre organisation.
