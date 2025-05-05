---
title: Gestion des données
description: Découvrez l’ingestion et le stockage de données pour  [!DNL Insights]  dans GenStudio for Performance Marketing.
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

GenStudio for Performance Marketing utilise Adobe Experience Platform (AEP) pour l’ingestion et le stockage des données des mesures et des métadonnées qui alimentent [!DNL Insights]. AEP utilise des _schémas_ pour définir les structures de données et des _jeux de données_ pour stocker et gérer les collections de données.

## Connexions de données

GenStudio for Performance Marketing utilise Customer Journey Analytics (CJA) pour agréger plusieurs sources de données en créant une connexion à un ou plusieurs jeux de données AEP. CJA utilise ces connexions de données pour créer des vues de données permettant d’analyser les mesures avec [!DNL Insights].

>[!BEGINSHADEBOX]

**Informations importantes sur les connexions de données**

Si vous êtes un [administrateur système Adobe](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), vous pouvez disposer de droits qui vous donnent accès à la gestion des sandbox AEP et aux composants du lac de données qui prennent en charge GenStudio for Performance Marketing.

>[!WARNING]
>
>La réinitialisation du sandbox de production dans AEP supprime toutes les connexions de données et [!DNL Insights] fait cesser de fonctionner.

Soyez prudent et ne supprimez pas les connexions de données suivantes, nécessaires au fonctionnement fiable de GenStudio for Performance Marketing :

- Jeux de données AEP dotés du préfixe `GS Insights`
- Schémas, classes et groupes de champs d’AEP précédés du préfixe `GS Insights`
- `timestamp for metadata` du groupe de champs personnalisé
- Connexions AEP : flux de données précédés du préfixe `GS Insights`
- AEP Connections : compte GS Insights

Voir [Implications de suppression](https://experienceleague.adobe.com/fr/docs/analytics-platform/using/technotes/deletion) dans le guide _Customer Journey Analytics_ avant de supprimer des composants de données dans AEP.

>[!ENDSHADEBOX]

## Politique de conservation des données

GenStudio for Performance Marketing conserve les données de canal pendant 13 mois. Cette politique de conservation comprend les 6 mois de données ingérées lors de la connexion initiale, ce qui garantit une analyse complète des données historiques et la création de rapports.

Voir [Connexion au compte publicitaire du canal](/help/user-guide/connectors/connect-channel.md).
