---
title: Distribuer votre application
description: Distribuez votre application ou module complémentaire pour GenStudio for Performance Marketing.
exl-id: 4935356b-08df-402c-b1a2-b89627afc188
source-git-commit: 8884f3438a0010119f578ca9a3b7158e2e01cfa3
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Distribuer votre application

La distribution de votre module complémentaire le rend disponible pour une utilisation par votre organisation et potentiellement par d’autres organisations.

La distribution privée limite le déploiement de votre module complémentaire à l’organisation identifiée par l’organisation IMS pour laquelle vous avez développé votre module complémentaire. La distribution publique rend le module complémentaire disponible sous la forme d’une application sur Adobe Exchange. Votre workflow de distribution dépend de si votre module complémentaire est destiné à une distribution publique ou privée.

Cette rubrique traite de la distribution privée. [Distribution publique](https://developer.adobe.com/app-builder/docs/guides/distribution/public/) dans la documentation du développeur _App Builder_, explique comment rendre votre application disponible pour toute organisation Adobe.

>[!BEGINSHADEBOX]

**Conditions préalables** :

Vérifiez que vous disposez des autorisations suivantes :

* Autorisations de développeur dans l’organisation à partir de laquelle vous soumettez l’application à approbation

* Autorisations de l’administrateur système pour approuver l’application

Votre application App Builder doit être déployée dans un projet App Builder.

>[!ENDSHADEBOX]

**Pour distribuer votre application de manière privée** :

La distribution privée met votre application à disposition uniquement des membres de votre organisation.

1. Dans [Adobe Developer Console](https://developer.adobe.com/console/), sélectionnez l&#39;organisation, le projet et l&#39;espace de travail dans lesquels l&#39;application est déployée.

1. Sélectionnez **[!UICONTROL Approbation]** dans la zone de présentation de Workspace __. Le volet _Approbation de l’application_ s’ouvre.

1. Dans la zone _Détails des envois d’application_, ajoutez des informations détaillées sur votre module complémentaire. Les détails incluent le nom de l’application, la description et l’adresse e-mail du contact.

1. Une fois tous les champs renseignés, cliquez sur **[!UICONTROL Envoyer]**.

1. Connectez-vous à [Adobe Exchange](https://exchange.adobe.com/) en utilisant la même Adobe ID que celle utilisée pour vous connecter à Developer Console. Si vous ne disposez pas des autorisations d’administrateur système dans cette organisation, demandez l’approbation d’un administrateur système d’organisation.

1. Sélectionnez **[!UICONTROL Gérer]** > **[!UICONTROL Applications App Builder]** pour accéder à une demande de révision de l’application.

1. Après avoir examiné l’application, sélectionnez **[!UICONTROL Approuver]**. Vous pouvez éventuellement ajouter des notes informatives.

Votre module complémentaire est maintenant visible dans l’instance GenStudio for Performance Marketing de votre organisation.
