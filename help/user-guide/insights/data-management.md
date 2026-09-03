---
title: Gestion des données
description: Découvrez l’ingestion et le stockage de données pour  [!DNL Insights]  dans GenStudio for Performance Marketing.
feature: Reporting and Insights
level: Experienced
role: Admin, Developer
last-substantial-update: 2025-1-7
exl-id: a5ab44d6-75c0-405b-82ad-9c65f6094bd6
TQID: https://experienceleague.adobe.com/HM2e0Yq2uwTpKtK-z8gHs0hDFrsJS6koQBqoNoKJK0Y
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: e0aa398c-6185-4e77-8cf7-2561c578c181
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: d3cdead0-685a-4489-9250-4bb709942f66id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 249
ht-degree: 2%

---

# Gestion des données

GenStudio for Performance Marketing utilise Adobe Experience Platform (AEP) pour l’ingestion et le stockage des données des mesures et des métadonnées qui alimentent [!DNL Insights]. AEP utilise des _schémas_ pour définir les structures de données et des _jeux de données_ pour stocker et gérer les collections de données.

## Connexions de données

GenStudio for Performance Marketing utilise Customer Journey Analytics (CJA) pour agréger plusieurs sources de données en créant une connexion à un ou plusieurs jeux de données AEP. CJA utilise ces connexions de données pour créer des vues de données permettant d’analyser les mesures avec [!DNL Insights].

>[!BEGINSHADEBOX]

**Informations importantes sur les connexions de données**

Si vous êtes un [administrateur système ](/help/user-guide/user-roles.md#adobe-system-administrator-vs-genstudio-system-manager), vous pouvez disposer de droits qui vous donnent accès à la gestion des sandbox AEP et aux composants du lac de données qui prennent en charge GenStudio for Performance Marketing.

>[!WARNING]
>
>La réinitialisation du sandbox de production dans AEP supprime toutes les connexions de données et [!DNL Insights] fait cesser de fonctionner.

Soyez prudent et ne supprimez pas les connexions de données suivantes, nécessaires au fonctionnement fiable de GenStudio for Performance Marketing :

- Jeux de données AEP dotés du préfixe `GS Insights`
- Schémas, classes et groupes de champs d’AEP précédés du préfixe `GS Insights`
- `timestamp for metadata` du groupe de champs personnalisé
- Connexions AEP : flux de données précédés du préfixe `GS Insights`
- AEP Connections : compte GS Insights

Voir [Implications de suppression](https://experienceleague.adobe.com/en/docs/analytics-platform/using/technotes/deletion) dans le guide _Customer Journey Analytics_ avant de supprimer des composants de données dans AEP.

>[!ENDSHADEBOX]

## Politique de conservation des données

GenStudio for Performance Marketing conserve les données de canal pendant 13 mois. Cette politique de conservation comprend les 6 mois de données ingérées lors de la connexion initiale, ce qui garantit une analyse complète des données historiques et la création de rapports.

Consultez [Connecter un compte de média acheté](/help/user-guide/connectors/connect-channel.md).
