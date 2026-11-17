---
title: Gérer les activations
description: Découvrez comment gérer les expériences activées avec Adobe GenStudio for Performance Marketing.
feature: Ad Activation
exl-id: 7cf340d4-37ab-4906-9aad-088a26db0818
TQID: 'https://experienceleague.adobe.com/ird0IiW8L5Axjj2FmEjlUcD1sPaNCNfxj9XNqGfQWiI'
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
source-git-commit: 7863995df08681a8a427277121a5fbeca131c6a9
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%
---
# Gérer les activations

Vos tableaux d’activation apparaissent sur la page de destination [!DNL Activate]. Chaque tableau répertorie ses publicités, ainsi que leur statut :

| Statut | Signification |
|---|---|
| [!UICONTROL Attention Requise] | Au moins une annonce publicitaire de la table d’activation comporte un champ manquant ou non valide, tel qu’un call to action incompatible, ou un identifiant de suivi en double. |
| [!UICONTROL Prêt pour activation] | Toutes les publicités du tableau d’activation sont validées et prêtes à être publiées. |
| [!UICONTROL En attente] | La table d&#39;activation entière a été envoyée et est en cours de traitement par la plateforme de destination. |
| [!UICONTROL Publié] | L’intégralité du tableau d’activation a été publiée. |
| [!UICONTROL Échec] | La plateforme de destination a rejeté au moins une des publicités du tableau. Pointez sur l’info-bulle d’état pour afficher le message d’erreur de la plateforme. |

Vous pouvez automatiquement réessayer les activations ayant échoué en cliquant sur **[!UICONTROL Réessayer]** en haut à droite.

Les lignes publiées sont verrouillées contre toute nouvelle soumission et incluent un lien profond vers la publicité dans le gestionnaire de publicités natif de la plateforme de destination, de sorte que vous puissiez y accéder directement pour la réviser ou la lancer.

## Générer des noms d’annonces publicitaires

Utilisez la convention de nommage de votre organisation pour générer des noms d’annonces publicitaires cohérents à partir des informations d’expérience. Vous pouvez vérifier, modifier ou remplacer des noms avant d’envoyer des annonces aux plateformes. Voir [Générer des noms d’annonces publicitaires](generate-ad-names.md).

## Vue Détails

Cliquez sur une ligne d’annonce pour ouvrir une vue ciblée de ses détails d’activation. La vue Détails en lecture seule capture les détails déterminants d’une publicité activée, y compris les activations ayant échoué, avec des informations provenant à la fois de GenStudio for Performance Marketing et de la plateforme de destination :

* **Heure et date de publication** : heure et date de publication à partir de la plateforme de destination
* **ID de publicité** : ID attribué par la plateforme de destination et utilisé pour le suivi, avec un lien profond vers l’annonce publiée dans le gestionnaire d’annonces natif de la plateforme
* **Détails de l’annonce publicitaire** : ressources, copie et métadonnées approuvées utilisées pour l’annonce publicitaire
* **Configuration de la plateforme** : le compte, la campagne et les autres champs de configuration de la plateforme utilisés pour activer la publicité

La vue des détails d’une activation ayant échoué indique la raison de l’échec.
