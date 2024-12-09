---
title: 'Connexion à un référentiel  [!DNL AEM Assets Content Hub] '
description: Découvrez comment connecter Adobe GenStudio for Performance Marketing à un référentiel Adobe Experience Manager (AEM) [!DNL Content Hub] et exploiter le contenu approuvé existant.
level: Experienced
feature: Assets, Content
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: abe1de42b81bff63d473a67632d27f96db7c1c7d
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Connexion à un référentiel [!DNL AEM Assets Content Hub]

Si vous disposez de ressources dans Adobe Experience Manager (AEM), vous pouvez suivre ces étapes pour les rendre accessibles dans GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Conditions préalables** :

Les étapes suivantes nécessitent un accès administratif à Admin Console et AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Étape 1 : Activer [!DNL AEM Assets Content Hub]

Suivez le processus **Déployer Content Hub** en libre-service pour activer [!DNL Content Hub] pour votre AEM Assets existant dans Cloud Manager. Voir [Déploiement [!DNL Content Hub]](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) dans la documentation _AEM as a Cloud Service_.

Après avoir activé [!DNL AEM Assets Content Hub], vous disposez d’une nouvelle instance avec le suffixe `contenthub` dans [!DNL AEM Assets as a Cloud Service] sur Admin Console.

>[!IMPORTANT]
>
>Les administrateurs doivent vérifier que le référentiel [!DNL AEM Assets Content Hub] se trouve dans la même organisation que GenStudio for Performance Marketing.

## Étape 2 : utilisateurs GenStudio intégrés

Dans le [!DNL Admin Console], ajoutez un utilisateur ou un groupe d’utilisateurs GenStudio for Performance Marketing au profil de produit [!DNL AEM Assets Content Hub]. Si un réviseur de contenu n’a pas accès à la même organisation que le référentiel [!DNL AEM Assets Content Hub], il peut rencontrer des difficultés pour vérifier et approuver le contenu.

- [Onboard [!DNL Content Hub] administrator](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Onboard [!DNL Content Hub] users](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Étape 3 : Approbation des ressources

Approuvez les ressources à utiliser dans [!DNL AEM Assets Content Hub], ce qui les rend disponibles dans GenStudio for Performance Marketing.

Voir [Approuver des ressources dans Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) dans la documentation _AEM as a Cloud Service_.

## Étape 4 : configuration de la visibilité des ressources

Dans les options de configuration _[!DNL AEM Assets Content Hub]_, passez en revue chaque ensemble d’options de configuration pour les filtres, les détails des ressources, la recherche et la valorisation de marque.

Voir [Configuration de l’interface utilisateur de Content Hub](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) dans la documentation _AEM as a Cloud Service_.

## Étape 5 : Vérification de la connexion

Dans le contenu GenStudio for Performance Marketing, la liste _[!UICONTROL Emplacement]_ est disponible au-dessus de la galerie sur le côté droit. La liste n’est pas disponible si vous n’avez pas accès ou si votre organisation n’a pas déployé et connecté de référentiel [!DNL AEM Assets Content Hub].

Voir [Emplacement Assets](manage-assets.md#assets-location) pour en savoir plus sur la liste Emplacement et la modification des référentiels.
