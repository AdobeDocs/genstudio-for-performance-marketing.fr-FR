---
title: Gestion des données
description: Découvrez l’ingestion et le stockage des données dans [!DNL Insights] GenStudio pour le marketing à la performance.
feature: Reporting and Insights
level: Experienced
role: Admin, Data Architect
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
source-git-commit: 8e61fa5c08102c5dd9905e693d7f129105d9f633
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Gestion des données

GenStudio for Performance Marketing utilise Adobe Experience Platform (AEP) pour l’ingestion et le stockage des données et des métadonnées qui alimentent [!DNL Insights]. AEP utilise _des_ schémas pour définir les structures de données et _les ensembles de_ données pour le stockage et la gestion des collections de données.

## Connexions de données

GenStudio for Performance Marketing utilise Customer Journey Analytics (CJA) pour agréger plusieurs sources de données en créant une connexion à un ou plusieurs ensembles de données AEP. CJA utilise ces connexions de données pour créer des vues de données afin d’analyser les mesures avec [!DNL Insights].

>[!BEGINSHADEBOX]

**Informations importantes sur la connexion aux données**

Si vous êtes un [administrateur](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager) système Adobe, vous pouvez avoir des droits qui permettent d’accéder à la gestion des sandbox AEP et aux composants du lac de données qui prennent en charge GenStudio for Performance Marketing.

>[!WARNING]
>
>La réinitialisation du sandbox de production dans AEP supprime toutes les connexions de données et provoque [!DNL Insights] l’arrêt du fonctionnement.

Soyez prudent et ne supprimez pas les connexions de données suivantes requises pour que GenStudio for Performance Marketing fonctionne de manière fiable :

- Jeux de données AEP dont le préfixe est `GS Insights`
- Les schémas, classes et groupes de champs AEP dont le préfixe est `GS Insights`
- Groupe de champs personnalisé `timestamp for metadata`
- Connexions AEP : flux de données dont le préfixe est `GS Insights`
- Connexions AEP : compte Insights GS

Voir [Supprimer les implications](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) dans le guide d’Customer Journey Analytics __ avant de supprimer des composants de données dans AEP.

>[!ENDSHADEBOX]

## Politique de conservation des données

GenStudio for Performance Marketing conserve les données de canal pendant 13 mois. Cette politique de rétention inclut les 6 mois de données ingérées lors de la connexion initiale, garantissant une analyse et un reporting complets des données historiques.

Consultez la section [Connecter le compte](/help/user-guide/connectors/connect-channel.md) publicitaire de canal.
