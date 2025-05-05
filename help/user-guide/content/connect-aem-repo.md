---
title: 'Connexion à un référentiel  [!DNL AEM Assets Content Hub] '
description: Découvrez comment connecter Adobe GenStudio for Performance Marketing à un référentiel Adobe Experience Manager (AEM) [!DNL Content Hub]  et exploiter le contenu approuvé existant.
level: Experienced
role: Admin, Data Engineer
feature: Content Management
recommendations: noDisplay
exl-id: abb587fd-593c-4b9f-baad-993d92400d9b
source-git-commit: 85948ccd9b6d198a2064d95639f96a045ea61743
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Connexion à un référentiel [!DNL AEM Assets Content Hub]

Si vous disposez de ressources dans Adobe Experience Manager (AEM), vous pouvez suivre les étapes suivantes pour les rendre accessibles dans GenStudio for Performance Marketing.

>[!BEGINSHADEBOX]

**Conditions préalables** :

Les étapes suivantes nécessitent un accès administratif à Admin Console et AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Étape 1 : Activer [!DNL AEM Assets Content Hub]

Suivez le processus en libre-service **Déployer Content Hub** pour activer le [!DNL Content Hub] pour votre AEM Assets existant dans Cloud Manager. Voir [Déployer [!DNL Content Hub]](https://experienceleague.adobe.com/fr/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) dans la documentation d’_AEM as a Cloud Service_.

Après avoir activé [!DNL AEM Assets Content Hub], vous disposez d’une nouvelle instance avec le suffixe `contenthub` dans [!DNL AEM Assets as a Cloud Service] sur Admin Console.

>[!IMPORTANT]
>
>Les administrateurs doivent vérifier que le référentiel [!DNL AEM Assets Content Hub] se trouve dans la même organisation que GenStudio for Performance Marketing.

## Étape 2 : intégration des utilisateurs GenStudio

Dans le [!DNL Admin Console], ajoutez un utilisateur ou un groupe d’utilisateurs GenStudio for Performance Marketing au profil de produit [!DNL AEM Assets Content Hub]. Si un réviseur ou une réviseuse de contenu n’a pas accès à la même organisation que le référentiel [!DNL AEM Assets Content Hub], il ou elle peut rencontrer des difficultés pour réviser et approuver le contenu.

- [Intégration [!DNL Content Hub] administrateur](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Intégration [!DNL Content Hub] utilisateurs](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Étape 3 : Approuver les ressources

Approuver les ressources à utiliser dans [!DNL AEM Assets Content Hub], ce qui les rend disponibles dans GenStudio for Performance Marketing.

Voir [Approbation de ressources dans Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) dans la documentation d’_AEM as a Cloud Service_.

## Étape 4 : configurer la visibilité des ressources

Dans _[!DNL AEM Assets Content Hub]_&#x200B;options de configuration, passez en revue chaque jeu d’options de configuration pour les filtres, les détails de la ressource, la recherche et le branding.

Voir [Configuration de l’interface utilisateur de Content Hub](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) dans la documentation d’_AEM as a Cloud Service_.

## Étape 5 : vérifier la connexion

Dans Contenu GenStudio for Performance Marketing, la liste _[!UICONTROL Emplacement]_ est disponible au-dessus de la galerie sur le côté droit. La liste n’est pas disponible si vous n’y avez pas accès ou si votre organisation n’a pas déployé et connecté un référentiel [!DNL AEM Assets Content Hub].

Voir [Emplacement Assets](manage-assets.md#assets-location) pour en savoir plus sur la liste Emplacement et la modification des référentiels.
