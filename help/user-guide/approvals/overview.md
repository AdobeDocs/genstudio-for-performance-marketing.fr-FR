---
title: Examens et approbations Adobe GenStudio for Performance Marketing
description: Découvrez le processus de révision et d’approbation de GenStudio for Performance Marketing.
level: Beginner
feature: Content Review, Content Management
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 7955796949c17f7cd877b115cba45c58cdd614a7
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Examens et approbations Adobe GenStudio for Performance Marketing

Le workflow de révision et d’approbation garantit que toutes les parties prenantes, des équipes créatives aux experts juridiques, peuvent examiner et approuver efficacement les ressources et les expériences de campagne, y compris les ressources de marque générées par l’IA.

>[!NOTE]
>
> Cette fonctionnalité est également disponible en tant qu’[intégration à Adobe Workfront Proof](/help/user-guide/approvals/proof-integration.md). Cette intégration fournit des fonctionnalités de BAT dans la zone de travail GenStudio for Performance Marketing. Grâce à l’intégration de Workfront Proof, GenStudio for Performance Marketing bénéficie d’un processus d’examen plus structuré, transparent et collaboratif, ce qui permet aux équipes de passer de la version préliminaire à la version finale avec plus de confiance et de clarté.

## Avantages des workflows de révision et d’approbation

* **Prise en charge d’une création de contenu IA robuste et itérative**. La création et le déploiement de contenu aligné sur la marque dans une organisation sont un processus hautement itératif. Les fonctionnalités d’IA générative de GenStudio for Performance Marketing prennent en charge la création rapide de centaines de variantes de ressources. Chaque réviseur ou réviseuse peut demander plusieurs modifications à un brouillon de ressource avant de l’approuver. Plus il y a de réviseurs, plus il y a d’itérations potentielles avant que toutes les parties prenantes ne s’accordent sur une variante finale.

* **Prise en charge de l’intégrité créative**. Les approbations protègent l’intégrité créative de vos ressources de marque en maintenant les créateurs de contenu impliqués dans le processus d’approbation. En impliquant les parties prenantes de la création (par exemple, les créateurs de contenu et les directeurs créatifs) dans le processus de révision et d’approbation, vous vous assurez que le résultat final correspond à votre vision et à votre identité de marque.

* **Respect des objectifs de la campagne et des exigences légales**. Le processus de validation permet de vérifier que le contenu prend en charge les objectifs de la campagne. Elle garantit que tous les documents de marketing sont conformes aux normes juridiques et réglementaires, ce qui réduit les risques et les problèmes juridiques potentiels.

* **Intégration à Adobe Workfront Proof**. Les utilisateurs et utilisatrices peuvent accéder à des fonctionnalités de révision et d’approbation robustes de Workfront Proof depuis GenStudio for Performance Marketing. Le contenu révisé dans GenStudio for Performance Marketing se synchronise avec Workfront Proof et les commentaires et le statut de révision sont conservés. [Les points forts de l’intégration](/help/user-guide/approvals/proof-integration.md) identifie comment Proof étend le workflow d’approbation de GenStudio for Performance Marketing.

## Cycle de vie de la révision et de l’approbation

Les principales phases du workflow de révision et d’approbation sont les suivantes :

* [Demander la révision et l’approbation du contenu que vous avez créé](/help/user-guide/approvals/request-review.md). GenStudio for Performance Marketing simplifie le processus de demande des approbations et de gestion des approbateurs. Les modèles d’approbation Workfront Proof peuvent simplifier encore plus cette tâche.

* [Examen et modification du contenu](/help/user-guide/approvals/review-and-edit.md). Les notifications permettent de tenir les créateurs de contenu informés des modifications et approbations demandées. La révision du contenu déclenche un nouveau cycle d’approbation automatique.

* [Approuver le contenu](/help/user-guide/approvals/approve-content.md). Les approbateurs désignés marquent le contenu comme approuvé ou prêt à être publié.

* [Publier le contenu](/help/user-guide/approvals/publish-content.md). La publication de contenu approuvé sur [!DNL Content] le rend disponible pour référence ou à l’usage d’autres membres de votre organisation.

## À propos des brouillons de contenu

Les _brouillons_ sont des versions préliminaires de ressources ou d’expériences qui n’ont pas terminé le processus de révision et d’approbation. Le statut de brouillon identifie où se trouve le brouillon dans le processus d’examen et d’approbation. Un ID de brouillon unique identifie chaque brouillon. Cet identifiant est valide jusqu’à ce qu’un brouillon soit approuvé et publié sur [!DNL Content]. Les commentaires de révision et les approbations d’un brouillon sont associés à cet ID de brouillon individuel. Il n’existe aucun contrôle de version pour les brouillons de contenu GenStudio.

Lorsqu’un brouillon termine le processus de révision et d’approbation et est publié sur [!DNL Content], l’ID du brouillon expire. GenStudio for Performance Marketing n’enregistre pas les commentaires associés ni le statut d’approbation. L’URL du brouillon n’est plus valide.

Le statut de brouillon capture l’état du brouillon de contenu au fur et à mesure qu’il passe par le processus de révision et d’approbation. L’éditeur de contenu GenStudio for Performance Marketing qui a créé la ressource en cours de révision est informé de toute modification demandée concernant le brouillon ou les approbations. Les approbateurs modifient le statut du brouillon pour indiquer s’il doit être révisé davantage ou s’il peut être approuvé. Tous les approbateurs désignés doivent approuver une ressource ou une expérience avant de pouvoir la publier.

Statuts de brouillon disponibles :

**Notifié** : l’éditeur de contenu a lancé le processus de révision et d’approbation en informant les approbateurs qu’un brouillon est prêt pour la révision.
**Travail nécessaire** : indique qu&#39;un ou plusieurs approbateurs ont demandé des modifications pour le brouillon de contenu. Le contenu avec ce statut ne peut pas être enregistré dans [!DNL Content].
**Approuvé** : tous les approbateurs désignés ont approuvé la ressource ou l’expérience. L’éditeur de contenu peut désormais ajouter des métadonnées à la ressource ou à l’expérience et les enregistrer dans [!DNL Content].

>[!NOTE]
>
> Les brouillons correspondent aux _BAT_ pour les utilisateurs de l’intégration Workfront Proof. [Les brouillons et les épreuves](/help/user-guide/approvals/proof-integration.md#drafts-and-proofs) diffèrent en termes de persistance et de contrôle de version.

## Rôles d&#39;approbation

_Les réviseurs et réviseuses_ peuvent ajouter des commentaires, mais ne peuvent pas approuver le contenu. La participation des réviseurs est utile, mais pas essentielle. _Les approbateurs_ doivent approuver le contenu avant qu’il ne puisse progresser dans le processus d’approbation. L’intégration de Workfront Proof prend en charge un plus large éventail de rôles utilisateur.

## Notifications

Les notifications intégrées au produit GenStudio for Performance Marketing mettent à jour les approbateurs et les éditeurs de contenu en temps réel des changements de statut des ressources et des commentaires `@mention`. Les notifications prennent en charge une itération rapide tout au long des multiples cycles de révision, de modification et d’approbation.

Les éditeurs et approbateurs de contenu peuvent s’inscrire pour recevoir ces notifications dans Slack. Voir [S’abonner à des services dans Experience Cloud](https://experienceleague.adobe.com/en/docs/core-services/interface/services/customer-attributes/subscription).

Les actions entreprises par les participants à l’approbation déclenchent des notifications automatiques internes au produit et des notifications par e-mail. Lorsque vous lancez un processus d’approbation, les approbateurs désignés reçoivent des notifications par e-mail et internes au produit. Vous êtes tenu au courant grâce aux notifications intégrées au produit et aux notifications par e-mail chaque fois qu’un approbateur ajoute `@mention` commentaires ou prend une décision. Les notifications incluent des liens vers le brouillon de contenu.

Si vous avez lancé le processus de révision et d’approbation du contenu, vous êtes informé de toutes les approbations et de tous les commentaires de révision. Toutefois, les approbateurs ne sont avertis que des commentaires qui les incluent avec une `@mention`.
