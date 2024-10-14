---
title: Rôles utilisateur et autorisations Adobe GenStudio for Performance Marketing
description: Découvrez les rôles utilisateur et les autorisations de GenStudio for Performance Marketing.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 3e9a2a4f42ba79389691705c571bf6bbd0b990c5
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 12%

---

# Rôles utilisateur et autorisations

La création et le déploiement de campagnes marketing modernes nécessitent une collaboration entre les parties prenantes avec des responsabilités et des compétences variables. _Les rôles utilisateur_ contrôlent l’accès des parties prenantes aux nombreuses fonctionnalités de GenStudio for Performance Marketing. Le rôle utilisateur qui vous est attribué détermine les tâches que vous pouvez effectuer à l’aide de cette plateforme. Un administrateur système Adobe vous affecte un rôle dans le profil de produit GenStudio dans Adobe Admin Console. Votre e-mail de bienvenue identifie votre rôle attribué.

>[!NOTE]
>
>Avant que des utilisateurs ne soient configurés dans ces rôles, un administrateur système Adobe doit être désigné dans Adobe Admin Console pour effectuer des tâches de configuration uniques. Ce rôle d’administrateur d’Adobe fonctionne uniquement dans le contexte de Adobe Admin Console. Il n’a aucun rôle dans l’interface de la plateforme GenStudio for Performance Marketing. Un administrateur système Adobe ayant besoin des droits de gestionnaire système doit se configurer en tant que gestionnaire système GenStudio dans Adobe Admin Console. Voir [Configuration de GenStudio for Performance Marketing](product-provisioning.md).

## Droits

_Les droits_ accordent l’autorisation d’effectuer des tâches spécifiques et d’accéder à des ressources protégées. Les droits sont définis dans le rôle utilisateur au sein du profil de produit et les utilisateurs reçoivent ces droits lorsqu’ils sont affectés à ce rôle.

## Rôles d’utilisateur ou d’utilisatrice

Trois types de rôles utilisateur GenStudio for Performance Marketing prennent en charge cette diversité de rôles d’organisation. Les autorisations sont adaptées à chacun de ces types d’utilisateurs et prennent en charge les responsabilités de chaque utilisateur au sein de l’organisation marketing. Ces trois types de rôles utilisateur sont les suivants :

* Les **éditeurs GenStudio** utilisent les fonctionnalités d’IA générative de GenStudio for Performance Marketing pour créer des ressources de campagne marketing, demander l’approbation et la révision du contenu et publier des brouillons approuvés de ce contenu. Tous les utilisateurs de GenStudio for Performance Marketing peuvent accéder à une ressource et l’utiliser une fois que son éditeur l’a enregistrée sur [!DNL Content].

* **Les collaborateurs de GenStudio** sont le plus large éventail d’utilisateurs de GenStudio for Performance Marketing. Les collaborateurs peuvent visualiser et approuver le contenu. Ils constituent une partie essentielle du workflow, qui permet de s’assurer que le contenu que vous générez correspond aux exigences et aux normes de votre entreprise.

* Les **gestionnaires de système GenStudio** ont le plus grand ensemble d’autorisations dans GenStudio for Performance Marketing. Les gestionnaires de système effectuent la tâche essentielle d’intégration pour établir les barrières de sécurité fondamentales pour la création et le déploiement des ressources de campagne. Les gestionnaires système implémentent ces barrières de sécurité en chargeant des informations spécifiques à la marque et à l’entreprise, telles que les [directives sur la marque](./guidelines/overview.md). Les gestionnaires système sont autorisés à créer et publier [!DNL Brands], mais ne disposent pas de privilèges d’administration des utilisateurs.

### Éditeurs GenStudio

Les _éditeurs_, ou créateurs de contenu, disposent des autorisations de base nécessaires pour créer des ressources GenStudio for Performance Marketing [!DNL Brands], [!DNL Campaigns] et [!DNL Content]. Ils peuvent également modifier et supprimer les ressources qu’ils ont créées. GenStudio for Performance Marketing prend en charge la création rapide de centaines de fragments de contenu. Ces utilisateurs peuvent générer des fragments de contenu ou des expériences complètes qui orchestrent des éléments distincts de contenu approuvé pour répondre aux besoins de campagnes marketing spécifiques.

Les éditeurs interagissent avec les technologies GenStudio for Performance Marketing Generative AI via _l’invite_. Le tiroir d’invite du canevas fournit des outils pour placer des invites dans le contexte des instructions d’une campagne spécifique. Par conséquent, la qualité et le succès du contenu généré dépendent partiellement de la qualité des directives de marque que votre entreprise a chargées et de la spécificité de votre invite. Voir [Écrire des invites efficaces](effective-prompts.md).

Le tableau suivant affiche les autorisations de l’éditeur par défaut :

| Fonctionnalité | Créer | Mettre à jour | Supprimer | Afficher |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | non | non | non | oui |
| [!DNL Campaigns] | oui | oui | oui | oui |
| [!DNL Content] | oui | oui | oui | oui |
| [!DNL Create] | oui | oui | oui | oui |
| [!DNL Insights] | peut configurer les connecteurs d’annonces uniquement. |    |     | oui |
| [!DNL Personas] | oui | oui* | oui* | oui |
| [!DNL Products] | oui | oui* | oui* | oui |
| [!DNL Reviews and approvals] | oui | oui | oui | oui |

Les éditeurs peuvent modifier et supprimer [!DNL Personas] et [!DNL Products] qu’ils ont créés.

Les gestionnaires de système GenStudio peuvent autoriser les éditeurs à modifier et supprimer un [!DNL Brand].

### Collaborateurs GenStudio

_Les collaborateurs_ peuvent afficher des ressources dans GenStudio for Performance Marketing, mais pas créer, modifier ou supprimer ces ressources. Les collaborateurs incluent les parties prenantes qui sont essentielles au succès du processus de révision et d’approbation du contenu, mais qui n’ont pas besoin de créer ou de modifier directement le contenu. Les experts juridiques et les gestionnaires de créatifs sont des exemples de collaborateurs potentiels. Les collaborateurs de GenStudio for Performance Marketing peuvent être autorisés à créer et afficher des ressources dans d’autres produits de Creative Cloud.

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

### Gestionnaire de système GenStudio

_Les gestionnaires de système GenStudio_ disposent de l’ensemble d’autorisations le plus puissant de GenStudio for Performance Marketing. Les gestionnaires de système effectuent la tâche essentielle d’intégration pour établir les barrières de sécurité fondamentales pour la création et le déploiement des ressources de campagne. Les gestionnaires système implémentent ces barrières de sécurité en chargeant des informations spécifiques à la marque et à l’entreprise, telles que les [directives sur la marque](./guidelines/overview.md). Les gestionnaires système sont autorisés à créer et publier [!DNL Brands], mais ne disposent pas de privilèges d’administration des utilisateurs.

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

Voir [Prise en main d’Adobe GenStudio for Performance Marketing](get-started.md) pour une présentation des tâches de configuration préliminaires.
