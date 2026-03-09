---
title: Optimisation de votre activation
description: Découvrez comment optimiser les activations sur les canaux publicitaires payants tiers.
level: Intermediate
feature: Ad Activation
exl-id: 5bc624c2-d064-4190-8761-ed05d0629d1f
TQID: https://experienceleague.adobe.com/-D3DGxTpZ-0J-grE5-jKPrptf4C1Z-OE1t0DCoqhRLQ
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 466
ht-degree: 1%

---

# Optimiser les activations

L’activation d’une expérience publicitaire pour les canaux de publicités payantes comprend deux phases principales :

* Préparation de votre expérience pour l’activation

* Publier votre expérience sur ses responsables publicitaires de canaux payants désignés

Le respect des bonnes pratiques lors de la création et de l’activation de votre expérience publicitaire peut contribuer à réduire les complications ou erreurs potentielles lors de la diffusion aux canaux cibles.

## Bonnes pratiques

Voici quelques bonnes pratiques courantes et les erreurs qu’elles peuvent éviter.

* **Utiliser des URL de destination valides et complètes**

  Les URL non valides peuvent déclencher des erreurs. Exemple d’erreur : _L’URL que vous avez saisie ne dirige pas vers un site web. Veuillez saisir une URL valide et réessayer. (100)_

* **Vérifiez que votre application gère correctement l’expiration des jetons**

  Les applications doivent demander de nouveaux jetons si nécessaire. Si nécessaire, réauthentifiez-vous et obtenez un nouveau jeton d’accès en vous connectant à nouveau ou en actualisant la session. Exemple d’erreur : _Erreur de validation du jeton d’accès : la session a été invalidée car l’utilisateur a modifié son mot de passe ou Facebook a modifié la session pour des raisons de sécurité. (190)_

* **Vérifiez votre jeu d’annonces et assurez-vous qu’une seule annonce est active à la fois**

  Si vous devez activer plusieurs publicités Meta, créez une visionneuse de publicités Dynamic Creative distincte pour chacune d’elles. Exemple d’erreur : _la visionneuse d’annonces Dynamic Creative autorise au plus une annonce active. Les utilisateurs ne sont pas autorisés à créer plusieurs annonces dans la même visionneuse d’annonces Dynamic Creative. (100)_

* **Faire correspondre le nombre de règles appliquées avec le montant spécifié par la plateforme**

  Les canaux payants s’attendent à ce que le nombre de règles appliquées corresponde à leur format spécifié.  Si nécessaire, ajustez le nombre de règles pour qu’il corresponde à la valeur spécifiée par la plateforme. Exemple d’erreur : _L’annonce AssetFeed comporte X règle(s) cible(s) pour le format : nom du format, mais exactement X règle cible pour ce format est attendue. (100)_

* **Choisissez un call-to-action (CTA) compatible avec votre objectif de jeu d’annonces**

  Les appels à l’action incompatibles avec l’objectif dans les visionneuses d’annonces Dynamic Creative déclenchent une erreur. Exemple d’erreur : _Le type de call to action X n’est pas pris en charge pour l’objectif Y dans la visionneuse d’annonces Dynamic Creative. (100)_

* **Assurez-vous que la limite de l’ensemble d’annonces cible prend en charge le nombre d’expériences publicitaires**

  Vérifiez que la limite d’annonces publicitaires de l’ensemble d’annonces cible peut s’adapter à vos expériences publicitaires activées. Si nécessaire, supprimez toutes les annonces inutiles ou inactives du jeu d’annonces afin de respecter cette limite. Vous pouvez également créer un nouveau jeu d’annonces pour activer des annonces supplémentaires. Exemple d’erreur : _Vous avez atteint les limites de la campagne, du jeu d’annonces publicitaires ou des annonces publicitaires par compte publicitaire. Chaque jeu de publicités peut contenir un maximum de 50 publicités. Cela inclut les annonces en pause/inactives/désactivées. (100)_

* **Assurez-vous que la plateforme prend en charge le type CTA sélectionné**

  Vérifiez que votre expérience comprend un type CTA pris en charge. Exemple d’erreur : _(#100) type call to action non valide (100)_
