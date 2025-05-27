---
title: Validation des marques dans Adobe GenStudio for Performance Marketing
description: Découvrez comment fonctionne le système de validation de marque intégré dans GenStudio for Performance Marketing.
feature: Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review, Generative AI
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
source-git-commit: 8f8d10db351f440ccd64f4ef5a54b6ace9f9db85
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 0%

---

# Validation de la marque

Dans GenStudio for Performance Marketing, la validation de marque est un composant essentiel qui fonctionne en collaboration avec les fonctionnalités et directives d’IA générative ([[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md) et [[!DNL Personas]](/help/user-guide/guidelines/personas.md)). Cela permet de s’assurer que tout votre contenu correspond à l’identité de votre marque, aux normes ADA et aux conseils relatifs aux plateformes de canaux individuelles.

GenStudio for Performance Marketing effectue la validation de la marque et d’autres contrôles de contenu sur divers aspects, notamment :

* Instructions d’[!DNL Brand] définies ou par défaut
* Instructions relatives à Platform
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->
* Normes de l’American with Disabilities Act (ADA)

## Résumé de la vérification du contenu

Un résumé de la validation de la marque et d’autres informations de vérification du contenu pour chaque élément de contenu généré est accessible via l’icône de résumé _Vérification de contenu_ pour chaque variante dans la zone de travail.

Le résumé de la _vérification de contenu_ affiche les éléments suivants :

* Pourcentage de conformité à votre [[!DNL Brand]](brands.md) calculé comme le nombre de [recommandations](overview.md) qui ont été validées par rapport au nombre de recommandations testées
* `Pass` ou `Fail` résultat pour les directives de la plateforme, telles que Meta ou LinkedIn
* `Pass` ou `Fail` résultat pour les normes d’accessibilité ADA

![Résumé de la vérification du contenu](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Cliquez sur le pourcentage pour voir dans quelle mesure la variante est conforme. Les scores sont automatiquement mis à jour lorsque vous apportez des modifications aux variantes ou à d’autres contenus. Vous pouvez cliquer sur _Afficher et résoudre les problèmes_ pour garantir une meilleure conformité.

Voir [Amélioration de l’alignement des marques](#improve-brand-alignment).

## Panneau de vérification du contenu

Le panneau _Vérification du contenu_ s’ouvre sur le côté droit de la zone de travail lorsque vous cliquez sur dans la barre d’actions de droite _ou_ à partir de l’icône de résumé [_Vérification du contenu_ ](#content-check-summary). Ce panneau fournit des informations détaillées sur la validation de la marque, les directives de la plateforme et les normes d’accessibilité, et met en évidence les possibilités d’amélioration.

![Panneau de vérification du contenu](/help/assets/content-check-panel.png){width="400" zoomable="yes"}

Le panneau _Vérification de contenu_ affiche des informations de validation et de [conformité](/help/user-guide/guidelines/overview.md#compliance) pour les sections d’images et de variantes :

* Représentation de la _vérification de contenu_ informations récapitulatives pour les [!DNL Brand], les directives de la plateforme et les normes d’accessibilité
* Section _À réviser_ indiquant le nombre d’instructions ayant échoué et des informations détaillées sur chaque instruction à réviser
* Section _Passed_ indiquant le nombre d’instructions transmises et des informations détaillées sur chaque instruction passée

Consultez [Améliorer l’alignement de la marque](#improve-brand-alignment) pour savoir comment améliorer les scores du panneau _Vérification de contenu_.

### Type de contenu

Dans le panneau _Vérification de contenu_ vous pouvez activer ou désactiver les contrôles des consignes et des normes d’accessibilité à effectuer. Cliquez sur l’icône _Type de contenu_ (icône de niveaux) en haut du panneau pour activer ou désactiver :

* **[!DNL Brand]** : effectue les vérifications associées aux directives [!DNL Brand].
* **Instructions relatives à Platform** : effectue les vérifications associées à la plateforme spécifique au canal, telle que Meta.
* **Accessibilité** : effectue les vérifications associées aux normes d&#39;accessibilité ADA.

Pour **définir le type de contenu** pour les vérifications à effectuer, cliquez sur pour activer ou désactiver les types disponibles, puis cliquez sur **Appliquer**.

## Améliorer l’alignement de la marque

Pour optimiser l’efficacité du contenu généré et maintenir une identité de marque cohérente, utilisez les panneaux [_Vérification de contenu_ Résumé](#content-check-summary) et [_Vérification de contenu_](#content-check-panel). Vous pouvez modifier manuellement des sections spécifiques pour les aligner sur vos [[!DNL Brand] directives](brands.md), les directives de la plateforme et les normes d’accessibilité.

**Pour améliorer l’alignement de la marque pour les variantes générées** :

1. Cliquez sur l’icône du panneau _Vérification de contenu_ dans la barre d’actions de droite pour afficher les informations de validation et d’accessibilité.

   Vous pouvez voir un résumé des contrôles _Révision des besoins_ et _Réussite_ pour voir ce qui doit être amélioré.

   >[!NOTE]
   >
   > La directive _voix de marque_ indiquée dans le panneau _Vérification de contenu_ s’applique à l’ensemble de la variante, et non à une section individuelle. L’ensemble de la variante de contenu est mis en surbrillance pour une amélioration suggérée.

1. Cliquez pour corriger les instructions qui ne sont pas actuellement conformes.
1. Cliquez pour développer et examiner chaque vérification qui doit être examinée dans les sections disponibles telles que _Titre_, _Couleur_ et _Voix de la marque_.

   Utilisez le raisonnement fourni pour chaque vérification afin de vous guider dans la révision des images et des variantes.

1. Après avoir effectué les révisions nécessaires, cliquez sur **[!UICONTROL Vérifier à nouveau le score]** pour revérifier et valider vos modifications afin de vous assurer qu’elles sont plus étroitement alignées sur l’identité de votre marque, les directives de la plateforme et les normes d’accessibilité.

   Le processus de vérification du contenu s’exécute à nouveau. Si les éléments modifiés sont validés, une bannière verte s’affiche au bas de la zone de travail pour confirmer que le score a été mis à jour. Si aucune modification n’a été apportée après une nouvelle vérification, la bannière confirme qu’aucune modification n’a été apportée au score. Le pourcentage de l’icône de résumé _Vérification de contenu_ pour la variante révisée indique également votre progression.

1. Continuez à réviser les sections pour vous assurer que la variante entière réussit la validation et les contrôles d’accessibilité. Parcourez chaque variante à l’aide des flèches adjacentes à une variante individuelle dans la zone de travail.
