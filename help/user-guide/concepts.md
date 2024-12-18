---
title: Concepts d’Adobe GenStudio for Performance Marketing
description: Découvrez les concepts et la terminologie d’Adobe GenStudio for Performance Marketing.
feature: Workflow, Generative AI
exl-id: 7dd00b4c-f429-499b-851d-3606c82c09dc
source-git-commit: bfe961a06f62e55f3207088f6f390204b12e7142
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Concepts

GenStudio for Performance Marketing est un produit d’entreprise autonome qui incarne la chaîne d’approvisionnement de contenu d’Adobe afin de rationaliser les campagnes marketing. Il est difficile de créer du contenu personnalisé et approuvé par la marque à grande échelle, de surveiller l’efficacité et de s’adapter rapidement à un marché en constante évolution. GenStudio for Performance Marketing rassemble Creative Cloud et Experience Cloud dans une seule application qui utilise l’IA générative comme multiplicateur de performances pour les équipes marketing d’entreprise.

Avec GenStudio for Performance Marketing, vous pouvez :

* Créez du contenu intégré à la marque à l’aide d’invites en langage naturel pour vos canaux numériques prioritaires, tels que les médias achetés, les e-mails et les publicités display

* Collaborer avec les parties prenantes pour examiner et approuver le contenu généré
* Enregistrer le contenu généré et approuvé pour y accéder pour les prochaines campagnes marketing
* Évaluez l’efficacité du contenu en analysant les performances des ressources et en identifiant les attributs clés du contenu le plus performant.

## Technologie IA générative

GenStudio for Performance Marketing exploite la puissance de l’IA générative pour accélérer le processus de création de contenu et assurer une génération de contenu de haute qualité. Le cycle de vie itératif de vos ressources de création permet d’obtenir du contenu de plus en plus précis et aligné sur la marque qui trouve un écho auprès de votre audience cible.

Commencez par intégrer l’image de marque de votre entreprise, les personnages clients et les descriptions de produits grâce à la puissante fonctionnalité directives sur la marque. Consultez la [présentation des instructions](../user-guide/guidelines/overview.md) pour savoir comment préparer et télécharger ces instructions.

{{in-academy}}

## Modèles de langue volumineux

GenStudio for Performance Marketing exploite la plateforme d’IA générative d’Adobe, qui offre des services d’IA et de machine learning (ML) fondamentaux. Cette plateforme simplifie l’utilisation de grands modèles de langage (LLM), alimentant les fonctionnalités GenAI d’Adobe pour créer des expériences attrayantes.

GenStudio for Performance Marketing utilise la série GPT de LLM tiers via Azure OpenAI.<!-- Claude, and Gemini models. -->

## [!DNL Generative Actions]

_[!DNL Generative Actions]_, telles que définies dans la description du produit [Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html), sont les unités quantifiant l’utilisation des fonctionnalités d’IA générative dans GenStudio for Performance Marketing.

<!-- Add example about usage mode?
Where users check how many generative actions they have left
How they re-up their genactions
If genactions roll over month to month or not -->

### Taux

Vous recevez une allocation par défaut de [!DNL Generative Actions] comme indiqué dans la description du produit [GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html).

>[!NOTE]
>
>Les taux d’utilisation peuvent varier. Les plans peuvent faire l&#39;objet de modifications. Voir la description du produit [Adobe GenStudio for Performance Marketing](https://helpx.adobe.com/legal/product-descriptions/adobe-genstudio-for-performance-marketing---product-description.html) pour obtenir des informations à jour sur les taux.

Les fonctions suivantes consomment du [!DNL Generative Actions] à la vitesse spécifiée.

| Fonction | Taux d’actions génératives |
| -----------------------  | ------------------ |
| Créer un e-mail | 5 par génération |
| Création d’annonces publicitaires média payantes | 5 par génération |
| Créer des publicités display | 5 par génération |
| Régénération des sections | 1 par génération |

<!-- | Generate on-brand images | 1 per prompt  |
| Translation              | 1 per prompt  |
| Video: ADLS              | 1 per prompt  |
| Video: TTS + Avatar      | 1 per prompt  | -->

[!DNL Generative Actions] _ne sont pas_ consommés lorsque :

* Utilisation de la [validation de marque](/help/user-guide/guidelines/brand-validation.md) lors de la génération des variantes
* Extraction d’informations à partir de [directives téléchargées](/help/user-guide/guidelines/add-guidelines.md)
* [revérification manuelle des variantes](/help/user-guide/guidelines/brand-validation.md#improve-brand-alignment)
* Les ressources numériques sont automatiquement balisées avec des attributs ([[!DNL Insights]](/help/user-guide/insights/overview.md))

>[!TIP]
>
>Si vous dépassez votre droit de [!DNL Generative Actions], vous pouvez acheter plus directement auprès de votre représentant de compte.

## Gouvernance des données

Lorsque vous utilisez l’IA pour générer du contenu, il est essentiel de s’assurer que la sortie est sécurisée et inclusive pour tous les utilisateurs et utilisatrices. Cela nécessite une évaluation du contenu à la recherche de préjugés potentiellement nuisibles, de discours de haine, de matériel offensant ou de blasphèmes. Adobe teste minutieusement la technologie de génération de contenu sous plusieurs angles, effectue des examens éthiques complets et met en œuvre des plans d’atténuation efficaces pour empêcher l’émergence de contenu préjudiciable dans les sorties.

Cette approche renforce la responsabilité sociale, minimise le risque de réputation et assure le respect des politiques de confiance, de sécurité et d&#39;éthique de [Adobe ](https://www.adobe.com/content/dam/cc/en/ai-ethics/pdfs/Adobe-AI-Ethics-Principles.pdf).

GenStudio for Performance Marketing intègre des plans de réduction des risques pour empêcher l’utilisation de contenu préjudiciable ou biaisé identifié, conformément aux normes et politiques de gouvernance des données de l’Adobe. Lorsqu’un tel contenu est détecté, vous êtes averti que la génération de ressources est bloquée avec un message « Impossible de générer ».

Lorsque ce message s’affiche, vous pouvez modifier l’invite et réessayer _ou_ marquer le contenu de l’invite pour révision par GenStudio for Performance Marketing. Les données d’invite pour le contenu marqué pour révision sont collectées à des fins de révision interne.

## Cycle de vie du contenu

La demande d’expériences de qualité sur plusieurs canaux est élevée et plus rapide. GenStudio for Performance Marketing simplifie la chaîne d’approvisionnement du contenu en un workflow bien organisé pour les marketeurs. GenStudio for Performance Marketing exploite la technologie d’Adobe à chaque étape du cycle de vie.

<table style="table-layout:auto">

<tr style="border: 0;">

    <td>

       <p><strong>Workflow et planification</strong></p>

    </td>

    <td>

        <p>Réfléchissez à des idées, définissez des directives et élaborez une stratégie autour du contenu afin d’impliquer votre audience.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Création et production</strong></p>

    </td>

    <td>

        <p>Produisez le contenu en fonction du plan. Collaborez en temps réel, recevez des commentaires, apportez des modifications et approuvez du contenu.</p>

    </td>

</tr>

<tr style="border: 0;">

    <td>

        <p><strong>Gestion de contenu</strong></p>

    </td>

    <td>

        <p>Stockez, partagez et recherchez des ressources de création dans le référentiel centralisé. Réutilisez et revitalisez le contenu en fonction des performances.</p>

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

        <p><strong>Rapports et informations</strong></p>

    </td>

    <td>

        <p>Collectez des données et obtenez des informations pour optimiser les performances des ressources.</p>

    </td>

</tr>

</table>
