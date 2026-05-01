---
title: Connexion à Meta Ads
description: Connectez un compte Meta Ads pour activer et surveiller vos publicités et médias avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Admin, Developer
recommendations: noDisplay
feature: Reporting and Insights
exl-id: 78110edf-947b-4e05-a3f1-de4b1eabda44
TQID: https://experienceleague.adobe.com/egZtqgG24xRPuMu7QAnuo25ZgUr-q7hGL9-k1x-PCQ0
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: e0aa398c-6185-4e77-8cf7-2561c578c181
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: afce03c5167b728fe04e4722a1e4f39868d523df
workflow-type: tm+mt
source-wordcount: 875
ht-degree: 0%

---

# Connexion à Meta Ads

Cette page explique comment connecter et gérer votre compte de profil Meta Ads vers GenStudio for Performance Marketing afin de gérer les campagnes, d’exporter le contenu et d’accéder aux données publicitaires pour vos campagnes actives.

>[!BEGINSHADEBOX]

**Conditions préalables** :

- Une connexion Facebook/Meta qui peut accéder à tous les services Meta
- _Contrôle total_ sur Meta Business Portfolio et les comptes publicitaires, notamment :
   - Gestion des campagnes
   - Affichage des performances
   - Gestion des maquettes du Hub Creative
   - Analyses avancées
- Désactivez tous les bloqueurs de fenêtres contextuelles dans votre navigateur.
- Vérifiez les associations de pages de compte Instagram dans Meta Business Manager avant de tenter une connexion
- Confirmer l’accès administrateur à toutes les ressources connectées

>[!ENDSHADEBOX]

## Connexion à un compte Meta Ads

1. Cliquez sur **[!UICONTROL Plus]** > **[!UICONTROL Paramètres]**.

1. Dans la section _Connecteurs de données_, cliquez sur **[!UICONTROL Se connecter]** sur la carte _Meta Ads_.

1. Connectez-vous à votre compte Facebook.

   Vous devrez peut-être supprimer les bloqueurs de pop-up, puis utiliser **[!UICONTROL Actualiser]** pour réessayer.

1. Suivez les instructions d’authentification Facebook, vérifiez les informations du compte, puis cliquez sur **[!UICONTROL Continuer comme ...]**

1. Dans _[!UICONTROL Facebook Login for Business]_ (symbole Meta vers Adobe), parcourez les sélections suivantes pour accorder l’accès à GenStudio for Performance Marketing :

   - Sélectionnez un ou plusieurs profils Meta Business et cliquez sur **[!UICONTROL Continuer]**
   - Sélectionnez une ou plusieurs pages Meta, puis cliquez sur **[!UICONTROL Continuer]**
   - Sélectionnez un ou plusieurs comptes Instagram et cliquez sur **[!UICONTROL Continuer]**
   - Vérifiez les sélections et cliquez sur **[!UICONTROL Enregistrer]**

     ![Vérifier sélections](/help/assets/meta/meta-review-selections.png "Vérifier sélections"){width="400" zoomable="yes"}

1. Une fois que vous avez reçu la vérification que votre compte est connecté, cliquez sur **[!UICONTROL Compris]**.

   Cette étape permet à GenStudio for Performance Marketing d’accéder à toutes les publicités, métadonnées et mesures pour des performances optimales.

1. Dans _[!UICONTROL Meta Ads]_, sélectionnez un ou plusieurs comptes à inclure dans [!DNL Insights] et cliquez sur **[!UICONTROL Sélectionner]**.

1. Une fois que vous avez reçu une confirmation _Connecté à Platform_, cliquez sur **[!UICONTROL Afficher les comptes]**.

   La vue _[!UICONTROL Comptes Meta Ads]_ répertorie les `Account name`, `Added by`, `Date added` et `Status`.

   ![Liste &#x200B;](/help/assets/meta/meta-accounts-list.png " comptes MetaListe des comptes Meta connectés"){zoomable="yes"}

Utilisez **[!UICONTROL Ajouter un compte]** pour ajouter d’autres comptes à la liste. Le flux d’autorisation peut différer légèrement lorsque vous ajoutez des comptes liés au même profil Meta Business. Vous sélectionnez uniquement les nouveaux comptes Meta Ads pendant le processus de connexion.

## Connexion à un compte Instagram

>[!IMPORTANT]
>
>Avant d’activer une publicité Meta, assurez-vous dans Meta Business Manager que le compte Instagram que vous souhaitez utiliser est connecté au même compte publicitaire sélectionné lors de l’intégration. Si cette connexion est manquante, le compte Instagram peut ne pas apparaître dans le menu déroulant [!DNL GenStudio for Performance Marketing] _Compte Instagram_ lors de l’activation.

**Pour vérifier ou mettre à jour la connexion au compte Instagram dans Meta Business Manager** :

1. Accédez à **[!UICONTROL Paramètres]**.
1. Sous _Comptes_, sélectionnez **[!UICONTROL Comptes Instagram]**.
1. Choisissez le compte Instagram que vous souhaitez utiliser.
1. Cliquez sur **[!UICONTROL Ressources connectées]**.
1. Sous _Comptes publicitaires_, vérifiez que le compte publicitaire utilisé lors de l’intégration est répertorié.
1. S’il n’est pas répertorié, cliquez sur **[!UICONTROL Connecter des ressources]** et ajoutez le compte publicitaire approprié.

Une fois le compte publicitaire connecté, revenez à [!DNL GenStudio for Performance Marketing] et poursuivez le flux d’activation.

## Bonnes pratiques relatives à la connexion

Pour éviter toute erreur, tenez compte des bonnes pratiques suivantes lors de la configuration des connexions :

- [ ] Commencez par la sélection minimale de ressources (une seule page uniquement) pour la connexion initiale
- [ ] Ajouter des comptes Instagram uniquement après avoir confirmé que l’accès à la page fonctionne
- [ ] Assurez-vous que les comptes Instagram sont correctement associés à la page Facebook sélectionnée dans Meta Business Manager
- [ ] Utiliser une approche par phases : établir d’abord une connexion de base, puis développer les ressources
- [ ] Vérifier les autorisations d’administrateur pour toutes les ressources avant de tenter une connexion

## Déconnexion et dépannage d’une intégration Meta Ads

Il arrive qu’une instance GenStudio for Performance Marketing ne soit pas correctement connectée à un compte Meta Ads. Les configurations les plus courantes pouvant entraîner des problèmes sont les suivantes :

- Un compte Instagram est sélectionné sans sélectionner sa page Facebook associée
- Autorisations révoquées pour un utilisateur qui a effectué la connexion initiale

Dans ce cas, il est préférable de reconnecter le compte publicitaire Meta à l’instance GenStudio for Performance Marketing. Tout d’abord, l’utilisateur doit supprimer l’intégration de l’application directement depuis son Meta Business Manager, ce qui permet de réinitialiser les autorisations. Pour ce faire, un accès administrateur à Meta Business Manager est nécessaire.

Ces étapes effacent les autorisations mises en cache et réinitialisent le flux d’intégration :

1. Accédez à [Meta Business Manager](https://business.facebook.com) en consultant le site web Facebook.
1. Connectez-vous avec votre compte. Le compte doit avoir un accès administrateur au Business Manager.
1. Cliquez sur l’icône représentant un engrenage **[!UICONTROL Paramètres]** dans le coin inférieur gauche pour accéder aux paramètres de Business Portfolio.
1. Dans le menu de gauche, cliquez sur **[!UICONTROL Intégrations]**.
1. Sélectionnez **[!UICONTROL Applications connectées]**. Adobe GenStudio apparaît dans la liste des applications connectées .
   ![Meta Business Manager Connected Apps](./meta-connected-apps.png "Volet Meta Business Manager Connected Apps")
1. Cliquez sur le nom de l’application.
1. Cliquez sur **[!UICONTROL Supprimer]**.
1. Confirmez la suppression lorsque vous y êtes invité.

Vous pouvez maintenant reconnecter vos comptes publicitaires Meta, profils Instagram et pages Facebook.

## Problèmes de connexion au compte Instagram

Des problèmes peuvent survenir lorsque des comptes Instagram sont sélectionnés sans connecter une page Facebook associée pendant la configuration de la connexion. Cela peut entraîner des erreurs telles que :

- « Impossible de se connecter à {Page_Name} » ou échecs de connexion génériques.
- Délais d’expiration de la connexion pendant la connexion Facebook au flux métier.
- Échecs silencieux lorsque plusieurs ressources sont sélectionnées.
- La connexion échoue lors de la sélection simultanée d&#39;Instagram, de Page et de Compte publicitaire.

### Étapes de résolution :

1. Accédez à [Meta Business Manager](https://business.facebook.com) > Intégrations > Applications connectées.
1. Supprimez l’intégration « Adobe GenStudio » existante, le cas échéant. Cliquez sur **Supprimer**.
1. Revenez à GenStudio et relancez le processus de connexion.
1. Sélectionnez UNIQUEMENT la page Facebook cible lors de la connexion initiale.
1. NE PAS sélectionner le compte Instagram lors de la première tentative de connexion.
1. Vérifiez que la connexion est établie avant d’ajouter d’autres ressources.
1. Une fois la connexion à la page stable, ajoutez les comptes Instagram séparément.
