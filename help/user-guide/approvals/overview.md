---
title: Révisions et approbations Adobe GenStudio for Performance Marketing
description: Découvrez le processus de révision et d’approbation de GenStudio for Performance Marketing.
feature: Approval
exl-id: c83f47c0-e8ae-4c54-84b3-c50f67d6b3c2
source-git-commit: 478815d74a742cdc05d3f1faebf27d5adc04d417
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# Révisions et approbations Adobe GenStudio for Performance Marketing

Le processus d’examen et d’approbation garantit que toutes les parties prenantes, des équipes créatives aux experts juridiques, peuvent examiner et approuver efficacement les ressources et les expériences de campagne, y compris les ressources de marque générées par l’IA.

## Avantages du workflow [!DNL Review and Approval]

* **Prise en charge de la création de contenu d’IA itérative et robuste**. La création et le déploiement de contenu aligné sur la marque dans une entreprise est un processus hautement itératif. Les fonctionnalités d’IA générative de GenStudio for Performance Marketing prennent en charge la création rapide de centaines de variantes de ressources. Chaque réviseur peut demander plusieurs modifications à un brouillon de ressource avant de l’approuver. Plus les réviseurs sont nombreux, plus le nombre d&#39;itérations potentielles est élevé avant que toutes les parties prenantes ne s&#39;accordent sur une variante finale.

* **Prise en charge de l’intégrité créative**. Les approbations protègent l’intégrité créative des ressources de marque en maintenant les créateurs de contenu impliqués dans le processus d’approbation. En impliquant les parties prenantes créatives (par exemple, les créateurs de contenu et les directeurs créatifs) dans le processus de révision et d’approbation, vous vous assurez que la sortie finale s’aligne sur votre vision et votre identité de marque.

* **Respect des objectifs de Campaign et des exigences légales**. Le processus d’approbation permet de vérifier que le contenu prend en charge les objectifs de la campagne. Elle garantit que tous les supports marketing sont conformes aux normes légales et réglementaires, ce qui réduit les risques et les problèmes juridiques potentiels.

## Cycle de vie de révision et d’approbation

Les phases principales du workflow de révision et d’approbation sont les suivantes :

* [ Demandez la révision et l&#39;approbation du contenu que vous avez créé ](./request-review.md)
* [Réviser et modifier du contenu](./review-and-edit.md)
* [Approuver le contenu](./approve-content.md)
* [Publier le contenu](./publish-content.md)

## Qui peut demander une révision ou approuver un contenu ?

Si vous avez créé une ressource ou une expérience, vous pouvez demander à d’autres personnes de la chaîne d’approbation de votre organisation de passer en revue et de commenter officiellement votre travail. Bien que tout membre de l’organisation GenStudio for Performance Marketing puisse réviser un brouillon, seuls les approbateurs désignés peuvent commenter ou approuver un brouillon.

## À propos de [!DNL Content] brouillons

_Les brouillons_ sont des versions préliminaires de ressources ou d’expériences qui n’ont pas subi le processus de révision et d’approbation. L’état Version préliminaire identifie l’emplacement du brouillon dans le processus de révision et d’approbation. Un ID de brouillon unique identifie chaque brouillon. L’ID est valide jusqu’à ce qu’un brouillon soit approuvé et publié sur [!DNL Content]. Les commentaires de révision et les approbations pour un brouillon sont associés à cet ID de brouillon individuel.

Lorsqu’un brouillon termine le processus de révision et d’approbation et est publié sur [!DNL Content], l’ID de brouillon expire et GenStudio for Performance Marketing n’enregistre pas les commentaires et les états d’approbation associés. L’URL du brouillon n’est plus valide.

L’état Version préliminaire capture l’état du brouillon de contenu au fur et à mesure qu’il passe par le processus de révision et d’approbation. L’éditeur de contenu GenStudio for Performance Marketing qui a créé la ressource en cours de révision est informé de toute modification requise du brouillon ou des approbations. Les approbateurs modifient le statut du brouillon pour indiquer si un brouillon doit être révisé plus avant ou s’il peut être approuvé. Tous les approbateurs désignés doivent approuver une ressource ou une expérience avant qu’elle ne puisse être publiée.

Statuts de brouillon disponibles :

**Notifié** : l’éditeur de contenu a démarré le processus de révision et d’approbation en informant les approbateurs qu’un brouillon est prêt pour révision.
**Travail nécessaire** : indique qu’un ou plusieurs approbateurs ont demandé des modifications au brouillon de contenu. Le contenu de cet état ne peut pas être enregistré dans [!DNL Content].
**Approuvé** : tous les approbateurs désignés ont approuvé la ressource ou l’expérience. L’éditeur de contenu peut désormais ajouter des métadonnées à la ressource ou à l’expérience et les enregistrer dans [!DNL Content].

## Notifications

Les notifications internes aux produits GenStudio for Performance Marketing mettent à jour les approbateurs et les éditeurs de contenu en temps réel des modifications d’état des ressources et des commentaires `@mention`. Les notifications prennent en charge l’itération rapide par le biais de plusieurs cycles de révision, de modification et d’approbation.

Les éditeurs et les approbateurs de contenu peuvent s’inscrire pour recevoir ces notifications dans Slack. Voir [Abonnement aux services en Experience Cloud](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences#slack).

Les actions entreprises par les participants à l’approbation déclenchent des notifications internes et des notifications électroniques automatiques. Lorsque vous lancez un processus d’approbation, les approbateurs désignés reçoivent des notifications par courrier électronique et des notifications internes au produit. Vous êtes tenu dans la boucle avec des notifications internes et par e-mail chaque fois qu’un approbateur ajoute `@mention` commentaires ou prend une décision. Les notifications comprennent des liens vers le brouillon de contenu.

Si vous avez lancé le processus de révision et d’approbation du contenu, vous êtes informé de toutes les approbations et de tous les commentaires de révision. Cependant, les approbateurs sont avertis uniquement des commentaires qui les incluent avec un `@mention`.
