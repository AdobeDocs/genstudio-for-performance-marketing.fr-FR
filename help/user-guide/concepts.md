---
title: Concepts d’Adobe GenStudio for Performance Marketing
description: Découvrez les concepts et la terminologie d’Adobe GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
TQID: https://experienceleague.adobe.com/i3VF7S-ndAMDoF1akF3l20tStW-IPS--MSysxD-MArc
product_v2: id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2: id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7id: c5a86ad9-9158-4ab1-a7ea-9e29985087b8id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12id: c95c94c1-727b-457a-9184-a4dda4c95ab2id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3aid: f71bd2fc-e9ca-4cb6-8088-82e250211e32id: f912fa8d-7beb-4468-9ea7-1c0f198b59ef
subfeature_v2: id: a98e0185-3180-4e8c-8f31-f72af4cc21a2id: be495d08-ecd1-455f-951e-c22de504e667id: dd48f9df-f2e2-49fe-a918-332a8e240ffeid: e3878dde-4b87-4290-9e81-ed7ee6eb83feid: ec92a2bc-afe3-4ff0-a985-0c8ef22b4da0id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c7d04a2c-412a-4c9d-9d7a-4456eaa5adebid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eb30f47f-d87a-400f-8f78-63ce7979ff56
source-git-commit: e5011c95e9536d73b1f09d6bc76bb83f121573cd
workflow-type: tm+mt
source-wordcount: 754
ht-degree: 100%

---

# Concepts

GenStudio for Performance Marketing est un produit d’entreprise autonome qui incarne la chaîne d’approvisionnement de contenu d’Adobe afin de rationaliser les campagnes marketing. Il est difficile de créer du contenu personnalisé et approuvé par la marque à grande échelle, de surveiller l’efficacité et de s’adapter rapidement à un marché en constante évolution. GenStudio for Performance Marketing rassemble Creative Cloud et CX Enterprise dans une seule application qui utilise l’IA générative comme multiplicateur de performances pour les équipes marketing d’entreprise.

Avec GenStudio for Performance Marketing, vous pouvez :

* créer du contenu conforme à la marque à l’aide de prompts en langage naturel pour vos canaux numériques prioritaires, tels que les médias achetés, les e-mails et les publicités display ;

* collaborer avec les parties prenantes pour examiner et approuver le contenu généré ;
* enregistrer le contenu généré et approuvé pour pouvoir y accéder ultérieurement dans le cadre de futures campagnes marketing ;
* évaluer l’efficacité du contenu en analysant les performances des ressources et en identifiant les attributs clés du contenu le plus performant.

## Technologie d’IA générative

GenStudio for Performance Marketing exploite la puissance de l’IA générative pour accélérer le processus de création de contenu et assurer une génération de contenu de haute qualité. Le cycle de vie itératif de vos ressources de création permet d’obtenir un contenu de plus en plus précis et aligné sur la marque, qui trouve un écho auprès de votre audience cible.

Commencez par intégrer l’image de marque de votre entreprise, les profils de vos clientes et clients et les descriptions de vos produits grâce à la puissante fonctionnalité de gestion des directives de marque. Consultez la [vue d’ensemble des directives](../user-guide/guidelines/overview.md) pour savoir comment les préparer et les charger.

{{in-academy}}

### Grands modèles de langage

GenStudio for Performance Marketing exploite la plateforme d’IA générative d’Adobe, qui offre des services d’IA et de machine learning (ML) fondamentaux. Cette plateforme simplifie l’utilisation de grands modèles de langage (LLM), en optimisant les fonctionnalités GenAI d’Adobe pour créer des expériences attrayantes.

GenStudio for Performance Marketing utilise la série GPT de LLM tiers via Azure OpenAI.<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

Les _[!DNL Generative Actions]_, telles que définies dans la [description de produit Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/fr/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html), sont les unités quantifiant l’utilisation des fonctionnalités d’IA générative dans GenStudio for Performance Marketing.

<!-- 
Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not 
-->

### Taux

Vous recevez une allocation par défaut d’[!DNL Generative Actions], comme indiqué dans la [description de produit GenStudio for Performance Marketing](https://helpx.adobe.com/fr/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html).

>[!NOTE]
>
>Les quotas d’utilisation peuvent varier. Les plans sont susceptibles d’être modifiés. Voir la [description de produit Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/fr/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) pour obtenir des informations sur les quotas à jour.

Les fonctions suivantes consomment des [!DNL Generative Actions] selon le quota spécifié.

| Fonction | Quota d’actions génératives |
| -----------------------  | ------------------ |
| Créer un e-mail | 5 par génération |
| Créer des publicités paid media | 5 par génération |
| Créer des publicités display | 5 par génération |
| Régénérer des sections | 1 par génération |

<!-- 
| Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | 
-->

Les [!DNL Generative Actions] _ne sont pas_ consommées dans les cas suivants :

* Utilisation de la [validation de marque](/help/user-guide/guidelines/brand-validation.md) lors de la génération des variantes
* Extraction d’informations à partir des [directives chargées](/help/user-guide/guidelines/add-guidelines.md)
* [Revérification manuelle des variantes](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* Balisage automatique des ressources numériques avec des attributs ([[!DNL Insights]](/help/user-guide/insights/overview.md))

>[!TIP]
>
>Si vous dépassez votre quota d’[!DNL Generative Actions], vous pouvez en acheter davantage directement auprès du représentant ou de la représentante de votre compte.

## Gouvernance des données

Lorsque vous utilisez l’IA pour générer du contenu, il est essentiel de s’assurer que le résultat est sûr et inclusif pour l’ensemble des utilisateurs et utilisatrices. Cela nécessite une évaluation du contenu afin de détecter d’éventuels préjugés nuisibles, des discours haineux, des éléments offensants ou des propos injurieux. Adobe teste minutieusement la technologie de génération de contenu sous de multiples angles, effectue des évaluations éthiques approfondies et met en œuvre des plans d’atténuation efficaces afin d’empêcher la création de contenu préjudiciable dans les réponses.

Cette approche renforce la responsabilité sociale, réduit le risque relatif à la réputation et assure le respect des [politiques de confiance, de sécurité et d’éthique d’Adobe](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf).

GenStudio for Performance Marketing intègre des plans d’atténuation des risques afin d’empêcher l’utilisation de contenu préjudiciable ou biaisé identifié, conformément aux normes et politiques de gouvernance des données d’Adobe. Lorsqu’un tel contenu est détecté, le système vous en informe via un message « Génération impossible », indiquant que la génération de ressources est bloquée.

Lorsque ce message s’affiche, vous pouvez modifier le texte descriptif et réessayer _ou_ indiquer le contenu du prompt pour qu’il soit examiné par GenStudio for Performance Marketing. Les données du prompt relatives au contenu signalé pour révision sont collectées à des fins d’évaluation interne.

## Cycle de vie du contenu

La demande d’expériences de qualité sur plusieurs canaux est forte et nécessite une plus grande rapidité. GenStudio for Performance Marketing simplifie la chaîne d’approvisionnement de contenu en un processus bien organisé pour les spécialistes du marketing. GenStudio for Performance Marketing tire parti de toute la puissance de la technologie Adobe à chaque étape du cycle de vie.

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>Workflow et planification</strong></p>

    </td>

    <td>

        <p>Réfléchissez à des idées, définissez des consignes et créez une stratégie autour du contenu afin d’impliquer votre audience.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Création et production</strong></p>

    </td>

    <td>

        <p>Créez le contenu conformément au plan. Collaborez en temps réel, recevez des commentaires, apportez des modifications et approuvez du contenu.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Gestion de contenu</strong></p>

    </td>

    <td>

        <p>Stockez, partagez et recherchez des ressources de création dans le référentiel centralisé. Réutilisez et dynamisez le contenu en fonction des performances.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Diffusion et activation</strong></p>

    </td>

    <td>

        <p>Activez le contenu et publiez-le sur plusieurs canaux marketing.</P>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Rapports et insights</strong></p>

    </td>

    <td>

        <p>Collectez des données et tirez des enseignements pour optimiser les performances des ressources.</p>

    </td>

</tr>

</table>
