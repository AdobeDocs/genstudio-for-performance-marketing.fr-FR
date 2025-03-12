---
title: Rôles utilisateur et autorisations Adobe GenStudio for Performance Marketing
description: Découvrez les rôles utilisateur et les autorisations de GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
exl-id: 33ebcf9c-e5f8-4011-b449-5f73d151f221
source-git-commit: de1c54ceb4402d98fd3ae9bd129b26d6b4919681
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 10%

---

# Rôles utilisateur et autorisations

La création et le déploiement de campagnes marketing modernes nécessitent une collaboration entre les parties prenantes ayant des responsabilités et des compétences variables. _Rôles utilisateur_ contrôlez l’accès des parties prenantes aux nombreuses fonctionnalités de GenStudio for Performance Marketing. Le rôle d’utilisateur affecté détermine les tâches que vous pouvez effectuer à l’aide de cette plateforme. Un administrateur système Adobe vous affecte un rôle dans le profil de produit GenStudio du Adobe Admin Console. L’e-mail de bienvenue identifie le rôle qui vous a été attribué.

>[!NOTE]
>
>Avant l’attribution des privilèges d’accès à ces rôles aux utilisateurs, un administrateur système Adobe doit être désigné dans Adobe Admin Console pour effectuer des tâches de configuration ponctuelles. Ce rôle d’administrateur Adobe ne fonctionne que dans le cadre de Adobe Admin Console. Il n’a aucun rôle dans l’interface de la plateforme GenStudio for Performance Marketing. Un administrateur système Adobe qui a besoin de droits de gestionnaire système doit se configurer en tant que gestionnaire système GenStudio dans Adobe Admin Console. Voir [Configuration de GenStudio for Performance Marketing](product-provisioning.md).

## Administrateur système Adobe vs gestionnaire système GenStudio

Ces titres de rôle d’utilisateur peuvent sembler similaires, mais ils identifient des rôles uniques qui fournissent des droits dans différents environnements.

**Les administrateurs système d’Adobe** disposent de droits d’utilisateur avancé dans Adobe Admin Console et effectuent toutes les tâches de gestion des utilisateurs, comme l’ajout ou la suppression d’utilisateurs. Ce rôle d’administrateur système ne fournit aucun privilège dans l’application GenStudio for Performance Marketing, ce qui explique pourquoi les administrateurs système Adobe n’ont pas besoin de licence pour GenStudio. Les administrateurs système d’Adobe utilisent généralement Admin Console pour ajouter et supprimer des comptes d’utilisateurs des déploiements de GenStudio et attribuer ou supprimer des droits, ou autorisations, d’utilisateurs individuels ou de groupes d’utilisateurs.

**Les gestionnaires système de GenStudio** sont des utilisateurs expérimentés de GenStudio for Performance Marketing mais n&#39;ont pas l&#39;autorisation d&#39;effectuer des tâches dans Adobe Admin Console. Ce rôle de gestionnaire système nécessite une licence de produit GenStudio et correspond à un utilisateur avancé dans la description du produit [Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html). Les gestionnaires système de GenStudio disposent de droits complets sur les fonctionnalités de GenStudio for Performance Marketing, notamment la création, la suppression, la mise à jour et la publication de [!DNL Brands], [!DNL Persona] et [!DNL Product]. [Description du produit Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) explique comment les rôles utilisateur de GenStudio sont liés aux licences de produit.

Voir [Rôles administratifs](https://helpx.adobe.com/enterprise/using/admin-roles.html#enterprise) dans le _guide d’administration d’entreprise et d’équipes_.

## Droits

_Droits_ accordez l’autorisation d’effectuer des tâches spécifiques et d’accéder à des ressources protégées. Les droits, ou autorisations, sont définis dans le rôle utilisateur au sein du profil de produit et les utilisateurs reçoivent ces droits lorsqu’ils sont affectés à ce rôle.

>[!IMPORTANT]
>
>N’ajoutez pas de nouveaux profils de produit, ni ne modifiez ou ne supprimez pas les profils existants. La modification des profils de produit par défaut peut perturber gravement votre déploiement GenStudio for Performance Marketing.

## Rôles d’utilisateur ou d’utilisatrice

Trois types de rôles utilisateur de GenStudio for Performance Marketing prennent en charge cette diversité de rôles organisationnels. Les droits sont adaptés à chacun de ces types d’utilisateurs et prennent en charge les responsabilités de chaque utilisateur dans l’organisation marketing. Ces trois types de rôles utilisateur sont les suivants :

* **Les éditeurs GenStudio** utilisent les fonctionnalités d’IA générative de GenStudio for Performance Marketing pour créer des ressources de campagne marketing, demander la révision et l’approbation du contenu et publier les brouillons approuvés de ce contenu. Tous les utilisateurs de GenStudio for Performance Marketing peuvent accéder à une ressource et l’utiliser une fois que son éditeur l’a enregistrée dans [!DNL Content]. Les éditeurs GenStudio sont des utilisateurs expérimentés dans GenStudio for Performance Marketing.

* Les **collaborateurs GenStudio** représentent le plus large éventail d&#39;utilisateurs de GenStudio for Performance Marketing. Les collaborateurs peuvent afficher et approuver du contenu. Ils constituent une partie essentielle du workflow pour s’assurer que le contenu que vous générez correspond aux besoins et aux normes de votre entreprise. Les collaborateurs GenStudio sont des _utilisateurs collaborateurs_ dans GenStudio for Performance Marketing.

* **Les gestionnaires système de GenStudio** disposent du jeu de droits ou d&#39;autorisations le plus large dans GenStudio for Performance Marketing. Les responsables système effectuent la tâche d’intégration essentielle consistant à établir les mécanismes de sécurisation fondamentaux pour la création et le déploiement des ressources de campagne. Les responsables système implémentent ces mécanismes de sécurisation en chargeant des informations spécifiques à la marque et à l’entreprise, telles que les [ directives relatives à la marque](./guidelines/overview.md). Les responsables système ont l’autorisation de créer et de publier des [!DNL Brands], mais n’ont aucun droit d’administration des utilisateurs. Les gestionnaires de système GenStudio sont des utilisateurs expérimentés dans GenStudio for Performance Marketing.

### Éditeurs GenStudio

Les _éditeurs_ ou les créateurs de contenu disposent des autorisations de base nécessaires pour créer des ressources GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] et [!DNL Content]. Ces utilisateurs expérimentés peuvent également modifier et supprimer les ressources qu’ils ont créées. GenStudio for Performance Marketing prend en charge la création rapide de centaines d’éléments de contenu. Ces utilisateurs et utilisatrices peuvent générer des fragments de contenu ou des expériences complètes qui orchestrent des éléments distincts de contenu approuvé pour répondre aux besoins de campagnes marketing spécifiques.

Les éditeurs interagissent avec les technologies d’IA génératives de GenStudio for Performance Marketing via _invite_. Le tiroir d’invites de la zone de travail fournit des outils permettant de placer des invites dans le contexte des directives d’une campagne spécifique. Par conséquent, la qualité et le succès du contenu généré dépendent en partie de la qualité des directives de marque que votre organisation a chargées et de la spécificité de votre invite. Voir [Rédiger des invites efficaces](effective-prompts.md).

Le tableau suivant affiche les autorisations d’éditeur par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | non | non | non | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Create] | oui | oui | oui | oui |
| [!DNL Insights] | configuration des connecteurs uniquement |    |     | oui |
| [!DNL Personas] | oui | oui* | oui* | oui |
| [!DNL Products] | oui | oui* | oui* | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |
| [!DNL Templates] | non | non | non | oui |

Les éditeurs et éditrices peuvent modifier et supprimer les [!DNL Personas] et [!DNL Products] qu’ils ont créés.

Les responsables système de GenStudio peuvent autoriser les éditeurs à modifier et supprimer un [!DNL Brand].

### Collaborateurs GenStudio

Les _collaborateurs_ peuvent afficher des ressources dans GenStudio for Performance Marketing, mais ne peuvent ni les créer, ni les modifier, ni les supprimer. Par exemple, les collaborateurs voient un message « *Vous n’avez pas accès à ce contenu* » lorsqu’ils tentent d’accéder à [[!DNL Create]](/help/user-guide/create/overview.md).

Les collaborateurs incluent les parties prenantes qui sont essentielles au succès du processus de révision et d’approbation du contenu, mais qui n’ont pas besoin de créer ou de modifier directement le contenu. Les experts juridiques et les gestionnaires de contenu créatif sont des exemples de collaborateurs potentiels. Les collaborateurs GenStudio for Performance Marketing peuvent être autorisés à créer et afficher des ressources dans d’autres produits Creative Cloud.

Le tableau suivant affiche les autorisations de collaborateur par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | non | non | non | oui |
| [!DNL Campaigns] | non | non | non | oui |
| [!DNL Content] | non | non | non | oui |
| [!DNL Create] | non | non | non | oui |
| [!DNL Insights] | non | non | non | oui |
| [!DNL Personas] | non | non | non | oui |
| [!DNL Products] | non | non | non | oui |
| [!DNL Reviews and approvals] | non | non | non | oui |
| [!DNL Templates] | non | non | non | oui |

### Gestionnaires système de GenStudio

_Les gestionnaires système de GenStudio_ disposent de l&#39;ensemble d&#39;autorisations le plus puissant de GenStudio for Performance Marketing. Ces utilisateurs avancés effectuent la tâche d’intégration essentielle consistant à établir les mécanismes de sécurisation fondamentaux pour la création et le déploiement de ressources de campagne. Les responsables système implémentent ces mécanismes de sécurisation en chargeant des informations spécifiques à la marque et à l’entreprise, telles que les [ directives relatives à la marque](./guidelines/overview.md). Les responsables système ont l’autorisation de créer et de publier des [!DNL Brands], mais n’ont aucun droit d’administration des utilisateurs.

Le tableau suivant affiche les autorisations de gestionnaire système par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | oui | oui | oui | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Insights] | oui | oui | oui | oui |
| [!DNL Personas] | oui | oui | oui | oui |
| [!DNL Products] | oui | oui | oui | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |
| [!DNL Templates] | oui | oui | oui | oui |

Les responsables système peuvent également charger des modèles.

Consultez [Prise en main d’Adobe GenStudio for Performance Marketing](get-started.md) pour obtenir un aperçu des tâches de configuration préliminaire.
