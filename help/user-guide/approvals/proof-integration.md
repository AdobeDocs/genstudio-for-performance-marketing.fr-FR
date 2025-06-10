---
title: Intégration de Workfront Proof à la révision et aux approbations
description: Intégration de Workfront Proof à Adobe GenStudio for Performance Marketing.
feature: Content Review, Content Management
source-git-commit: f8508ee9440714137141e933cfe0f5761a510c7a
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Intégration de Workfront Proof à GenStudio for Performance Marketing

L’intégration à Workfront Proof améliore le cycle de vie de révision et d’approbation de GenStudio for Performance Marketing grâce à des fonctionnalités avancées, notamment des modèles d’approbation, des workflows à plusieurs étapes et la possibilité de [comparer des versions de BAT](https://experienceleague.adobe.com/fr/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs). Ce contrôle de version structuré garantit la transparence, la responsabilité et une collaboration rationalisée tout au long du cycle de vie de la révision du contenu.

>[!BEGINSHADEBOX]

**Conditions préalables** :

Installez l’extension [Visionneuse web Adobe Workfront](https://experienceleague.adobe.com/fr/docs/workfront/using/review-and-approve-work/proofing/review-proofs-in-workfront/review-a-proof/review-proof-in-web-viewer-extension)

>[!ENDSHADEBOX]

L’[!DNL Proofing Viewer] de Workfront Proof est un espace de travail riche permettant d’afficher, de commenter et de comparer des épreuves. De [!DNL Proofing Viewer], vous pouvez :

* Comparer différentes versions du contenu
* Ajout de commentaires et de balises de dessin à une épreuve
* Valider le BAT

[!DNL Proofing Viewer] se charge lorsque vous cliquez sur l’URL du bat dans l’e-mail de demande d’approbation ou la notification intégrée au produit. La vue [!DNL Proofing Viewer] _Ma nouvelle approbation_ s’ouvre. Dans cette vue, vous pouvez réviser le contenu et fournir des commentaires à l’aide des principaux outils d’annotation [!DNL Proofing Viewer].

Pour quitter [!DNL Proofing Viewer], cliquez sur **[!UICONTROL Revenir à GenStudio]**.

## Genstudio pour Performance Marketing et Workfront Proof : comparaison des fonctionnalités

Le tableau ci-dessous compare les fonctions de révision et d’approbation standard de GenStudio for Performance Marketing aux fonctionnalités plus avancées disponibles via l’intégration de Workfront Proof.

| Fonctionnalité        | GenStudio for Performance Marketing                                                                 | Workfront Proof                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| **Cycle de vie des brouillons/épreuves**        | Le contenu du brouillon expire lors de la publication. | Chaînes d’approbation à plusieurs étapes basées sur les rôles avec journaux persistants et horodatés.<br> Toutes les versions sont conservées indéfiniment. |
| **Commentaires**                | Les commentaires sont liés à l’ID de brouillon et ignorés après publication.                                           | Les commentaires et annotations persistants sont conservés à des fins d’audit et de conformité.     |
| **Versions**           | Les brouillons sont traités comme des instances uniques.<br>Aucune comparaison côte à côte.                                      | Contrôle de version complet avec des outils de comparaison côte à côte et de recouvrement.        |
| **Gestion de projet** | Gestion de base des campagnes. | Gestion complète du cycle de vie des campagnes, avec personnalisation, modèles, rapports et audits détaillés. |

### Licences et rôles utilisateur

Les licences identifient l’ensemble des droits d’utilisateur au sein d’un produit. Workfront Proof fournit plus de types de licence ou de rôles utilisateur que GenStudio for Performance Marketing. [Présentation des rôles dans l’épreuve](https://experienceleague.adobe.com/fr/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles) introduit les rôles utilisateur associés au workflow de révision et d’approbation de Workfront Proof.

| Licence GenStudio for Performance Marketing       | Licence Workfront                 | Description                                                                                                                                                      |
|---------------------------------------------------|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| GenStudio System Manager                          | Administrateur Workfront/Utilisateur expérimenté | Accès complet aux fonctionnalités GenStudio Performance Marketing telles que la gestion des marques, des rôles et des produits. Gère les workflows et les paramètres. Crée des modèles d&#39;approbation. |
| Créateur et éditeur de contenu (licence utilisateur avancé)   | Créateur d&#39;épreuve (licence standard)  | Génère et envoie des brouillons de contenu. Dans la visionneuse de relecture, charge des ressources et lance des épreuves. Nécessite une licence Workfront Proof.                              |
| Réviseur/approbateur (licence collaborateur)        | Réviseur/approbateur                 | participe à des révisions en plusieurs étapes, ajoute des commentaires et approuve ou rejette le contenu ;                                                                             |

Les administrateurs système d’Adobe gèrent l’approvisionnement des utilisateurs et les droits pour les deux produits dans Adobe Admin Console.

>[!NOTE]
>
> Workfront Proof fournit des [rôles utilisateur supplémentaires](https://experienceleague.adobe.com/fr/docs/workfront/using/review-and-approve-work/proofing/proofing-overview/proof-roles). Tous les rôles ne sont pas visibles dans Performance Marketing. Cependant, le système honore tout jeu de rôles au sein d’un modèle Workfront Proof.

### Brouillons et épreuves

Workfront [!DNL Proofing Viewer] étend le processus de révision et d’approbation de base de GenStudio for Performance Marketing avec des fonctionnalités de révision et d’approbation plus structurées. Les épreuves examinées dans cette intégration sont limitées aux formats pris en charge par GenStudio for Performance Marketing.

### Gestion des versions

GenStudio for Performance Marketing ne prend pas en charge les modèles de validation, contrairement à Workfront Proof. Les fonctionnalités de contrôle de version de Proof améliorent considérablement le processus de révision et d’approbation du contenu de GenStudio. Chaque envoi dans le workflow de l’épreuve est traité comme une version distincte du brouillon de contenu ou de l’_épreuve_. Les épreuves sont automatiquement enregistrées et peuvent être comparées côte à côte aux itérations précédentes. Les parties prenantes peuvent suivre les modifications, fournir des commentaires précis et maintenir l’alignement tout au long du cycle d’examen. Proof conserve un historique complet de tous les commentaires, décisions et versions, prenant en charge la préparation à l’audit et les exigences de conformité. Chaque version prend également en charge des workflows d’approbation basés sur les rôles et à plusieurs étapes, chaque action (approbation, rejet ou commentaire) étant clairement consignée et horodatée.

### Modèles de validation

Les modèles d’approbation Workfront Proof fournissent des étapes préformatées qui peuvent rationaliser le workflow d’approbation des épreuves. Ces modèles incluent les réviseurs et approbateurs sélectionnés, les rôles de BAT et les échéances, assurant ainsi la cohérence et l’efficacité. Les créateurs et créatrices de contenu qui lancent une révision peuvent choisir parmi un ensemble de modèles prédéfinis pour les workflows d’approbation à une ou plusieurs phases.

Chaque étape du modèle de workflow identifie les validants affectés. Toutes les mises à jour de statut et tous les commentaires du workflow Workfront Proof sont visibles dans le lecteur de vérification, ce qui accroît la transparence et la collaboration.

Les modèles d’approbation prennent en charge les approbations à plusieurs étapes, ce qui permet la coordination des examens de différents groupes d’intervenants.

### Commentaires

Les réviseurs peuvent cliquer directement sur des zones spécifiques du BAT pour laisser des commentaires précis et contextuels. Tous les commentaires sont horodatés et enregistrés dans l’historique des versions de l’épreuve. L’historique des commentaires n’est pas disponible dans GenStudio for Performance Marketing.

Vous pouvez [comparer deux versions d’une épreuve](https://experienceleague.adobe.com/fr/docs/workfront/using/workfront-proof/work-with-proofs-in-wf-proof/review-proofs-web-proofing-viewer/compare-proofs) pour évaluer les commentaires et le contenu de la révision.

## Notifications et rappels

Les réviseurs et les approbateurs reçoivent des notifications par e-mail lorsqu’une nouvelle épreuve est disponible pour révision ou lorsqu’une révision en cours a changé de statut.
Les [notifications et rappels relatifs aux épreuves](https://experienceleague.adobe.com/fr/docs/workfront/using/workfront-proof/proof-notifications-and-reminders/proof-notifications-and-reminders/proof-notifications-and-reminders) comprennent un lien personnalisé vers l’épreuve, des détails sur l’épreuve et sa progression tout au long du processus d’approbation, ainsi que des informations de contrôle de version.
