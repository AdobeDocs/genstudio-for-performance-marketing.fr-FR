---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
role: User
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
source-git-commit: 015f2f14edfb05cab11a66a8e5bc9b357f2e3ab9
workflow-type: tm+mt
source-wordcount: '3763'
ht-degree: 0%

---

# Notes de mise à jour de GenStudio for Performance Marketing

Ces informations de mise à jour fournissent les dernières mises à jour de l’application GenStudio for Performance Marketing.

## 2025.10.16 {#latest}

### Nouveaux plug-ins GenStudio pour Photoshop et Figma

* Créez des annonces sur la marque et personnalisées directement à l’aide des nouveaux plug-ins GenStudio pour les outils de conception Adobe Photoshop et Figma.

### Fonctionnalités vidéo étendues

* Les marketeurs peuvent désormais facilement ajouter des clips d’introduction et de sortie pour cadrer les publicités vidéo avec des messages ou des marques préproduits.
* Ajoutez des superpositions d’images, de texte et de logo tout au long de la vidéo

### Informations étendues pour LinkedIn, Meta et TikTok

* GenStudio Insights comprend désormais le compte rendu des performances des publicités LinkedIn, qui permet aux marketeurs d’afficher et d’analyser les performances de leurs campagnes et publicités directement dans la plateforme pour :
   * LinkedIn Ads
   * Meta Ads
   * TikTok Ads

### Activation d’Amazon Ads

* GenStudio prend désormais en charge l’activation des publicités display directement dans la plateforme Amazon Ads.

### Activation Flashtalking

* GenStudio prend désormais en charge l’activation des publicités display directement dans la plateforme de diffusion de publicités Flashtalking (Innovid).
* Les utilisateurs doivent configurer manuellement leur jeton API Flashtalking en coordination avec l’équipe d’ingénierie Activate. La configuration de jeton en libre-service sera ajoutée dans une version ultérieure.

### Intégration à Adobe Campaign V8

* GenStudio for Performance Marketing s’intègre désormais à Adobe Campaign V8, ce qui permet aux marketeurs d’exploiter en toute transparence la création de contenu optimisée par l’IA ainsi que les fonctionnalités avancées d’orchestration de Campaign.

### Lecture automatique de vidéo

* Les vidéos sont désormais automatiquement lues sur les modules [!DNL Create], [!DNL Content] et [!DNL Insights], offrant ainsi des expériences d’aperçu transparentes.

### Import de modèles d’e-mail tiers

* GenStudio for Performance Marketing prend désormais en charge l’intégration transparente à des systèmes de conception d’e-mail tiers grâce à un framework d’extensibilité. Les principales fonctionnalités sont les suivantes :

   * Importer automatiquement des modèles provenant de systèmes de conception d’e-mails tiers lors de la création de contenu
   * Ajout de métadonnées de modèle avec les modèles importés
   * Maintenir une source unique de vérité en se connectant directement à des systèmes tiers
   * SDK et exemple d’application fournis pour créer des intégrations personnalisées


## Notes de mise à jour antérieures

+++Notes de la version 2025.09.11

### Nouvelle fonctionnalité Generative Expand AI pour les médias achetés

La nouvelle fonctionnalité GenExpand permet aux marketeurs d’adapter dynamiquement leurs ressources créatives afin de prendre en charge différents proportions sur les canaux de médias achetés tels que Meta, LinkedIn, Display Ads et Banners. Lorsqu’une image ne correspond pas aux proportions prévues, par exemple en ajoutant une image étroite à une disposition large, vous pouvez utiliser GenExpand pour réviser l’image afin qu’elle s’adapte.

Cette fonctionnalité simplifie le processus d’édition et de redimensionnement d’images directement dans GenStudio for Performance Marketing. Consultez [Fonctionnalités Generative Expand AI](/help/user-guide/create/manage-variants.md#use-generative-expand) pour plus d’informations.

+++

+++Notes de la version 2025.08.15

### Informations pour les attributs de texte

Dans Adobe GenStudio, les informations sur les attributs de texte analysent le ton émotionnel, les techniques de persuasion et le style narratif utilisés dans la copie publicitaire. Une fois qu’une campagne est active, GenStudio effectue le suivi de la corrélation entre ces attributs de texte et des mesures de performances clés telles que le taux de clics, le CPA, le CPC, les impressions et les dépenses.

Actuellement, cette fonctionnalité est disponible uniquement pour les publicités en anglais. Voir [Fonctions de texte](/help/user-guide/insights/text-features.md) pour plus d’informations.

### Améliorations du modèle Insights

* La carte Aperçu de l’annonce publicitaire comprend désormais une option « En savoir plus » pour le texte.
* Nouveaux modèles pour les cartes de maçonnerie de page de publicités.

### Génération de contenu multilingue avec validation de marque

Le nouveau sélecteur Langue dans le tiroir d’invite prend en charge la création de contenu multilingue, ce qui permet aux marketeurs régionaux de développer du contenu de marque pour leurs audiences locales. Cette fonctionnalité prend actuellement en charge 12 langues.

### Prise en charge des ressources vidéo sur les modèles

* Il est possible d’ajouter des ressources vidéo sur des modèles Meta et LinkedIn.

### Activer les améliorations de l’expérience

* Nouvelle fonctionnalité pour enregistrer les brouillons des activations.
* Nouvelle fonctionnalité permettant de réessayer les activations ayant échoué.

### Utiliser le même rôle dans plusieurs champs de texte

Plusieurs champs de texte avec le même rôle sont désormais pris en charge (par exemple, « body », « cta », « on image text », etc.) pour les modèles clients complexes.

Explorez les détails dans [les conseils pour l’éditeur de code de modèle](/help/user-guide/content/code-editor.md).

### Nouveaux modèles de génération d’images Firefly pris en charge

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Adobe GenStudio for Performance Marketing prend désormais en charge la dernière suite Firefly Image Model 4, y compris deux variantes puissantes :

**Firefly Image 4** : optimisé pour la vitesse et la simplicité, idéal pour générer des illustrations, des icônes, des photos d&#39;objets de base et des portraits sur un seul sujet, couvrant 90 % des besoins créatifs quotidiens.

**Firefly Image 4 Ultra** : Privilégie le photoréalisme et la précision, excellant dans le rendu de portraits humains, de groupes de taille moyenne et de scènes complexes pour des tâches créatives haut de gamme.

Consultez [Générer des ressources](/help/user-guide/create/generate-assets.md) pour obtenir des informations détaillées sur l’utilisation de ces nouveaux modèles de génération d’images.

### Traduction d&#39;email prête à l&#39;emploi

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Adobe GenStudio for Performance Marketing propose désormais des fonctionnalités de traduction d’e-mail intégrées qui permettent aux spécialistes marketing de mettre à l’échelle efficacement leurs campagnes par e-mail à l’échelle mondiale. Cette fonctionnalité vous permet de prendre une expérience d’e-mail approuvée et de la traduire dans plusieurs langues cibles à l’aide des services de traduction Azure Open AI.

+++

+++Notes de la version 2025.07.25

### Filtre des ressources compatibles

Un nouveau filtre dans le module [!DNL Insights] masque automatiquement les [ressources d’image et vidéo non prises en charge](/help/user-guide/insights/ads.md#ad-formats) des aperçus des publicités, éliminant ainsi l’encombrement visuel et les mosaïques endommagées. Cette amélioration garantit que les utilisateurs ne voient que les médias réellement disponibles et prêts à l’emploi, ce qui crée une expérience plus épurée et plus fiable. Le filtre fonctionne avec le filtre Annonces de compatibilité existant.

### Multi-Asset Activation for Meta

L’activation d’images à proportions multiples pour les méta-publicités permet aux annonceurs de charger et d’activer plusieurs ressources d’images dans différentes proportions sous une seule publicité créative. Cette fonctionnalité permet à une annonce publicitaire de présenter l’élément créatif approprié pour différents emplacements de Meta tels que les flux, les histoires et les rouleaux. Les annonceurs peuvent prévisualiser la manière dont chaque image sera rendue à différents emplacements et publier toutes les versions dans les métadonnées dans un seul appel API.

### Mise en forme de texte enrichi dans les variantes

[Modifiez les champs de texte dans les variantes générées avec une mise en forme de texte enrichi](/help/user-guide/create/manage-variants.md#manually-edit-text) des options telles que le gras, l’italique, le soulignement, l’alignement du texte, les listes, la couleur du texte, la taille du texte et les liens. Vous pouvez ainsi affiner le texte et les expressions de votre audience et appliquer une mise en forme pour répondre aux exigences de mise en page.

### Libellés d’accessibilité des images et des liens

Ajoutez des libellés d’accessibilité (Aria-labels) aux images et aux liens call-to-action dans vos variantes pour fournir des noms accessibles qui aident les utilisateurs à comprendre l’objectif des éléments interactifs. Voir [Gérer les variantes](/help/user-guide/create/manage-variants.md) pour obtenir des instructions détaillées.

### Génération de contenu non anglais

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Le nouveau menu déroulant Sélecteur de langue dans le tiroir de l’invite prend en charge la création de contenu multilingue, ce qui permet aux spécialistes du marketing régional de développer du contenu de marque pour leurs audiences locales. Cette fonctionnalité prend actuellement en charge 12 langues GA et 5 langues Beta. La liste des langues fournit un workflow défini et une directive de langue claire au LLM pour des sorties plus cohérentes.

### Sélection de modèle facultative pour les publicités Meta

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

La sélection de modèles est désormais facultative avec les méta-annonces, ce qui permet aux utilisateurs de créer des annonces sans avoir besoin de texte et de logo en haut du média. Cette amélioration autorise d’autres types de médias, tels que les GIF animés et les vidéos, qui ne nécessitent pas de superpositions de texte ni d’emplacement du logo.

+++

+++Notes de la version 2025.06.15

### Modèles de démarrage disponibles

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Les [modèles de démarrage](/help/user-guide/templates/starter-templates.md) permettent de relancer le processus de création. Vous pouvez désormais effectuer une sélection à partir d’un modèle de démarrage d’annonce publicitaire Meta ou LinkedIn.

### Fonctionnalité Generative Expand AI

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Désormais, dans GenStudio for Performance Marketing [!DNL Create], vous pouvez utiliser les [fonctionnalités Generative Expand AI](/help/user-guide/create/manage-variants.md#use-generative-expand) pour étendre les dimensions des images et ajouter du contenu génératif pour adapter vos modèles d’annonce publicitaire dans des variantes de médias achetés.

### Ajout de vidéos aux publicités

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Avec le contenu de l’image, vous pouvez désormais ajouter des vidéos aux publicités [LinkedIn](/help/user-guide/create/create-linkedin.md#manage-videos) et [Meta](/help/user-guide/create/create-meta-ad.md#manage-videos). Consultez les aperçus de lecture automatique des vidéos directement dans GenStudio for Performance Marketing au fur et à mesure que vous choisissez et ajoutez des vidéos à vos variantes.

### Correctifs et améliorations

* Ajout de la prise en charge de la [publication d’expériences publicitaires](/help/user-guide/activation/activate-linkedin-ad.md) de GenStudio for Performance Marketing vers LinkedIn Campaign Manager. [!DNL Activate] prend en charge les aperçus d’annonces publicitaires LinkedIn détaillés avant la publication sur LinkedIn Campaign Manager.

* L&#39;intégration de [Workfront Proof](/help/user-guide/approvals/overview.md) apporte les fonctionnalités robustes de révision et d&#39;approbation de Proof à GenStudio for Performance Marketing. Le contenu révisé dans GenStudio for Performance Marketing se synchronise avec Workfront Proof et les commentaires et le statut de révision sont conservés.

* Possibilité de [fournir des noms accessibles pour les images et les liens call-to-action](/help/user-guide/create/manage-variants.md#add-accessibility-labels) dans vos variantes en ajoutant des libellés d’accessibilité (libellés Aria).

* Lors de l’ajout ou de la révision de [directives relatives aux marques](/help/user-guide/guidelines/brands.md) dans une langue autre que l’anglais, GenStudio for Performance Marketing affiche ces directives dans la même langue.

* Après avoir ajouté manuellement une [!DNL Brand] ou créé un [!DNL Brand] à partir d’une extraction manuelle à partir d’un document, vous pouvez [modifier ou ajouter des images miniatures de marque](/help/user-guide/guidelines/add-guidelines.md#change-brand-thumbnail) pour vous assurer que chaque marque est facilement identifiable dans votre liste de [!DNL Brands].

* Vous pouvez désormais [utiliser la mise en forme d’édition de texte enrichi pour le texte](/help/user-guide/create/manage-variants.md#manually-edit-text) dans vos variantes générées. Testez une myriade d’options de mise en forme pour le texte de variante, telles que la couleur, la taille, les listes, etc.

* Vous pouvez désormais [créer une visionneuse d’annonces](/help/user-guide/activation/activate-meta-ad.md#create-a-new-ad-set) lors de la configuration de la plateforme en clonant une visionneuse d’annonces existante. Les ensembles de métadonnées publicitaires définissent le timing, les détails du canal et l’audience d’une publicité spécifique. Une méta-campagne peut contenir plusieurs visionneuses d’annonces, mais une visionneuse d’annonces est exclusivement associée à une campagne.

* Vous pouvez désormais exporter les détails de la campagne pour les rendre accessibles en externe sous forme de résumés de campagne dans Word ou PDF. Sélectionnez une campagne, puis cliquez sur **[!UICONTROL Exporter]** (coin supérieur droit).

+++

+++Notes de la version 2025.05.15

### Correctifs et améliorations

* Activation de la fonctionnalité [ajout d’un texte secondaire (alt)](/help/user-guide/create/manage-variants.md#add-alt-text-for-images) à une image pour une variante individuelle.
* Ajout d’un [nouveau format Meta](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) —Paysage 1,19 :1 (largeur de 1 080 pixels).
* Vous pouvez désormais choisir plusieurs expériences à exporter ou télécharger. Voir [Exporter des expériences](/help/user-guide/content/manage-assets.md#export-experiences).
<!-- * Added support for [publishing ad experiences](/help/user-guide/activation/activate-meta-ad.md) directly from _[!DNL Content]_ [into Google Campaign Manager 360 and Meta Ads Manager](/help/user-guide/activation/activate-cm360-ad.md). -->

+++

+++Notes de la version 2025.04.15

### Correctifs et améliorations

* Nouvelles options de filtre pour les modèles ! Vous pouvez maintenant affiner votre liste _[!UICONTROL Sélectionner des modèles]_ dans [!DNL Create] et dans _[!UICONTROL Contenu]_ > _[!UICONTROL Modèles]_. Voir [Modèles de recherche](/help/user-guide/content/use-templates.md#search-templates). Assurez-vous que les modèles sont correctement balisés avec des métadonnées pour les rendre détectables via ces filtres.
* Activation de la fonctionnalité [affichage et sélection de calques individuels](/help/user-guide/create/manage-variants.md#view-layers) tels que des champs de texte modifiables ou des images modifiables) d’une expérience afin de les mettre en surbrillance pour les révisions, telles que la régénération de contenu ou le recadrage d’images.
* Ajout d’un [nouveau champ de modèle](/help/user-guide/content/use-templates.md#template-elements), `sub-headline`, pour du texte supplémentaire dans les expériences afin de capter l’attention de l’audience et de mettre en évidence les messages marketing.
* Ajout de la prise en charge de la [publication d’expériences publicitaires](/help/user-guide/activation/overview.md) depuis GenStudio for Performance Marketing dans Google Campaign Manager 360. Activer prend en charge les aperçus détaillés des annonces Google Campaign Manager 360 avant leur publication sur un annonceur Campaign Manager 360. Les publicités publiées via Activer sont automatiquement extraites dans Insights une fois en ligne, ce qui permet aux utilisateurs et utilisatrices de suivre et de générer des rapports sur les performances des publicités.

+++

+++Notes de la version 2025.03.13

### Activer les métadonnées

Les marketeurs peuvent désormais [publier des expériences publicitaires](/help/user-guide/activation/overview.md) de GenStudio for Performance Marketing dans le Gestionnaire de métadonnées publicitaires. [!DNL Activate] prend en charge les prévisualisations détaillées des métadonnées de publicité avant le déploiement. Les publicités Meta publiées via [!DNL Activate] sont automatiquement extraites dans le [!DNL Insights] une fois en ligne, ce qui permet aux utilisateurs et utilisatrices de suivre et de générer des rapports sur les performances des publicités.

### Création d’expériences LinkedIn

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Ajout de la prise en charge de la [ création d’expériences LinkedIn ](/help/user-guide/create/create-linkedin.md). Consultez l’onglet [Annonce publicitaire LinkedIn](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) dans les instructions spécifiques aux canaux.

### Créer des expériences de bannière

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Ajout de la prise en charge de la [création d’expériences de bannière](/help/user-guide/create/create-banner-experience.md). Consultez l’onglet [Bannière](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) dans les instructions spécifiques aux canaux.

### Conformité

Dans le cadre du processus de validation de la marque, des [normes de conformité](/help/user-guide/guidelines/overview.md) ont été introduites dans les [contrôles de contenu](/help/user-guide/guidelines/brand-validation.md). Ces contrôles examinent chaque variante d’une expérience par rapport aux directives [!DNL Brand], aux directives de plateforme (telles que pour Meta) et aux normes ADA. Ce processus fournit un résumé complet des lignes directrices et des normes qui doivent être révisées pour une meilleure conformité.

### Extensibilité

Le nouveau GenStudio for Performance Marketing [framework d’extensibilité](/help/extensibility/setup.md) fournit aux entreprises des outils leur permettant d’incorporer leurs propres protocoles de conformité aux réclamations dans le workflow de création de contenu et la validation par le biais de modules complémentaires, ou applications extensibles.

### Modèles

* **Éditeur de code de modèle** : le nouvel [Éditeur de code de modèle](/help/user-guide/content/code-editor.md) vous permet de vérifier et d’affiner votre modèle pour une utilisation optimale lors de la génération de nouvelles expériences avec GenStudio for Performance Marketing.

  ![Affichage de l’éditeur de code](/help/assets/template-detected-fields.png "Vérification des champs détectés"){width="500" zoomable="yes"}

* **Liens sur l’image** : personnalisez votre modèle d’e-mail en activant les liens d’image. Voir [Personnaliser un modèle : lien sur une image](/help/user-guide/content/customize-template.md#link-on-image).
* **Modèles AJO et Marketo**—Téléchargez un modèle que vous avez créé dans Adobe Journey Optimizer (AJO) ou Marketo. Voir [ Utilisation de modèles provenant d’AJO et de Marketo](/help/user-guide/content/use-templates.md#templates-from-ajo-and-marketo).

### Correctifs et améliorations

* Activation de la fonctionnalité pour les instructions [canal par défaut](/help/user-guide/guidelines/brands.md#channel-guidelines), [image](/help/user-guide/guidelines/brands.md#image-guidelines), [logo](/help/user-guide/guidelines/brands.md#logos) et [couleur](/help/user-guide/guidelines/brands.md#colors) pour [[!DNL Brands]](/help/user-guide/guidelines/brands.md).
* Possibilité d’[ajouter des liens à des images](/help/user-guide/create/manage-variants.md#add-image-link) dans une variante.
* Déplacement de la fonctionnalité [Vérification de contenu](/help/user-guide/guidelines/brand-validation.md) et Révision et approbation vers la nouvelle barre d’actions de droite pour optimiser l’espace sur la zone de travail et améliorer l’expérience utilisateur.
* Simplification du flux [chargement ou ajout manuel d’une marque](/help/user-guide/guidelines/add-guidelines.md#add-brands).
* Ajout de la possibilité d’[ajouter ou de permuter des ressources d’image dans une variante](/help/user-guide/create/manage-variants.md#swap-image) sur la zone de travail.
* Amélioration de l’expérience utilisateur et de la visibilité des catégories de canal [sur la page d’accueil Créer](/help/user-guide/create/overview.md) en les séparant en sections Média détenu, Média payant et Contenu .
* Amélioration du filtrage dans les vues Tableau et Galerie [!DNL Insights].

+++

+++Notes de la version 2025.02.13

### Améliorations des pages de destination pour [!DNL Create]

La page de destination [!DNL Create] de GenStudio for Performance Marketing comprend des améliorations de l’interface utilisateur qui améliorent l’expérience utilisateur. La section _Travail récent_ est affinée et configurée avec la vue Liste comme vue par défaut. Le remplissage et d’autres améliorations visuelles rationalisent l’aspect de la zone de travail [!DNL Create].

### Exportation des informations au format CSV

Vous pouvez désormais télécharger le tableau affichable à partir de n’importe quelle vue [!DNL Insights] dans un fichier CSV. Cette fonctionnalité vous permet d’exporter et d’analyser des données provenant de diverses vues de [!DNL Insights], ce qui facilite l’analyse des données et les options de rapports.

+++

+++Notes de la version 2025.01.16

### Intégration à Adobe Workfront Proof

[!BADGE Beta]{type=Informative tooltip="Cette fonctionnalité est actuellement disponible dans Beta, de sorte que certaines d’entre elles peuvent être limitées ou susceptibles d’être modifiées."}

Le programme Beta d’intégration des épreuves GenStudio for Performance Marketing et Adobe Workfront est lancé ce mois-ci. Workfront Proof stimule le cycle de vie de la création et de l’activation de contenu avec des modèles d’approbation, des workflows en plusieurs étapes et des annotations. Les utilisateurs de GenStudio for Performance Marketing disposant de droits Workfront Proof peuvent utiliser les fonctionnalités avancées de Proof dans GenStudio for Performance Marketing pour examiner et commenter le contenu généré par GenStudio.

Les programmes Beta permettent de façonner le développement de produits et de déterminer leur disponibilité générale.

### Générer de nouveaux appels à l’action

Vous pouvez désormais générer de nouvelles expressions call-to-action (CTA) lors de la gestion des variantes. Utilisez les nouvelles options _Reformuler_ et _Ajouter un lien_ pour générer de nouvelles expressions et modifier le lien CTA. Votre modèle doit être correctement configuré pour que ces nouvelles fonctions CTA fonctionnent. Suivez les instructions de la section _Personnaliser un modèle_ : [Appels à l’action](/help/user-guide/content/customize-template.md#calls-to-action). Pour obtenir des instructions sur la gestion des CTA dans les variantes, voir [Revise Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action). <!-- GS-6676 -->

### Correctifs et améliorations

* Le nombre de caractères est désormais affiché dans tous les champs générés et manuels des publicités affichées. Voir _Nombre de caractères_ dans [Méta-expériences](/help/user-guide/create/meta-experiences.md#character-counts). <!-- GS-7732 -->

* Les _collaborateurs_ peuvent désormais afficher les ressources, mais ne peuvent pas les créer, les modifier ni les supprimer. Auparavant, les droits des collaborateurs n’étaient pas appliqués comme prévu dans [!DNL Create]. <!-- GS-7614 -->

* Les éditeurs de contenu peuvent désormais modifier les métadonnées des ressources, des expériences et des modèles. <!-- GS-4905 -->

* Les tailles d’image personnalisées dans les métamodèles et les modèles sont désormais prises en charge. <!-- GS-7512 -->

* Les sélections de personnes, de marques et de produits sont désormais préchargées lors de la génération du modèle. <!-- GS-8069 -->

* Le lien call-to-action d’e-mail n’est plus un champ obligatoire. <!-- GS-8103 -->

* Le menu déroulant du sélecteur de [!DNL Brand] fonctionne désormais comme prévu pour les modèles. Auparavant, le sélecteur ne se chargeait pas correctement pour certains modèles. <!-- GS-8908 -->

* Les éditeurs et éditrices peuvent désormais sélectionner un maximum de quatre images pour les e-mails à pod unique et les publicités Meta. <!-- GS-2631 -->

* La valeur d’année du champ `Created by` d’une expérience approuvée reste désormais cohérente comme prévu une fois les métadonnées de l’expérience modifiées. <!-- GS-8344 -->

* Les éditeurs de contenu peuvent désormais sélectionner un modèle dans [!DNL Create]. Auparavant, l’application générait une erreur de console lorsqu’un éditeur sélectionnait un modèle.  <!-- GS-8798 -->

* Les problèmes liés aux opérations de redimensionnement et de régénération des publicités Meta ont été résolus. <!-- GS-8900 -->

* Le bouton **[!UICONTROL Précédent]** renvoie désormais les utilisateurs à la page précédente ou à la page de destination [!DNL Create] comme prévu. <!-- GS-8622 -->

+++

+++Notes de la version 2024.12.12

### Nouvelles fonctionnalités

Les éditeurs peuvent désormais effectuer les tâches liées aux métadonnées suivantes :

* Modifiez les métadonnées de la ressource, de l’expérience et du modèle. Voir [Détails de la ressource](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* Affichez les balises générées par une ressource dans la vue _Détails_ de toute expérience qui utilise la ressource. Voir _Balises générées_ dans [Détails de la ressource](/help/user-guide/content/asset-details.md#generated-tags). <!-- GS-3705 -->

Les éditeurs peuvent désormais spécifier des valeurs personnalisées pour ces aspects des variantes générées :

* Largeur et hauteur des bannières web dans les modèles d’affichage publicitaire. Ces valeurs sont désormais enregistrées en tant que métadonnées de modèle. <!-- GS-6735 -->

* Dimensions des images dans les expériences d’affichage et de publicité lors du chargement des images.<!-- GS-7166 -->

* Consultez les instructions spécifiques aux canaux dans la section [Bonnes pratiques pour les modèles](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

Les options d’exportation incluent désormais :

* Exportez les publicités display et les publicités Meta sous la forme HTML, JPEG ou PNG. Voir [Créer une expérience d’affichage publicitaire](/help/user-guide/create/create-display-ad.md) et [Créer une expérience de méta-annonce](/help/user-guide/create/create-meta-ad.md). <!-- GS-7093 6655 5152-->

De nouvelles fonctionnalités supplémentaires permettent aux éditeurs de :

* Utilisez le bouton **[!UICONTROL Actualiser]** sur la vue Modèle de [!DNL Content] _Détails de la ressource_ pour actualiser le modèle sélectionné. <!-- GS-7102 -->

* Régénérer les sections des variantes d’annonces publicitaires et d’emails. Voir [Créer une expérience d’affichage d’annonce publicitaire](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) et [Créer une expérience d’e-mail](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Dupliquez les marques existantes. Voir [Gérer les marques](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

### Correctifs et améliorations

* Les titres des publicités display sont désormais enregistrés dans [!DNL Content] comme prévu. <!-- GS-7239 -->

* Le tiroir d’invite ne se ferme plus lorsqu’un éditeur clique en dehors du menu déroulant du tiroir. <!-- GS-7275 -->

* Le menu déroulant [!DNL Create] [!DNL Persona]/[!DNL Product] se charge désormais comme prévu lorsqu’une erreur de service d’URL de miniature se produit. <!-- GS-7277 -->

* Les publicités display qui contiennent des éléments qui recouvrent des fragments sont désormais modifiables. <!-- GS-7186 -->

* Le bouton Zone de travail **[!UICONTROL Marque]** est désormais désactivé lorsque les scores de la marque ne sont pas générés pour une expérience. <!-- GS-6429 -->

* La zone de travail affiche désormais les expériences redimensionnées dans un ordre cohérent. <!-- GS-7123 -->

* Le recadrage manuel utilise désormais les dimensions d’image, et non celles du modèle, lors de la modification des publicités. Auparavant, lorsqu’une image était plus petite que les dimensions spécifiées dans l’affichage et le modèle, le cadre de sélection utilisait les dimensions du modèle, et non les dimensions de l’image. <!-- GS-7315 -->

* Les éditeurs et éditrices peuvent désormais sélectionner jusqu’à quatre images lors de la création d’une publicité display. <!-- GS-7189 -->

* Les brouillons Afficher l’annonce et Méta-annonce se chargent désormais comme prévu lorsqu’ils sont redimensionnés sur un autre navigateur. <!-- GS-7204 -->

* Les champs de modèle inutilisés ne s’affichent plus dans le contenu généré.  <!-- GS-5670 -->

* Les éditeurs peuvent désormais cliquer une seule fois sur les liens pour les modifier comme prévu dans les variantes générées. <!-- GS-7423 -->

* [!DNL Create] respecte désormais correctement les privilèges des collaborateurs. <!-- GS-7614 -->

* Le bouton Zone de travail **[!UICONTROL Redimensionner]** est désormais désactivé une fois toutes les options de redimensionnement sélectionnées et rendues. <!-- GS-5940 -->

* Les réviseurs et réviseuses disposant d’un accès en lecture seule peuvent désormais effectuer un zoom avant ou arrière sur les variantes lors des révisions. <!-- GS-7371 -->

* La sélection au clavier a été ajoutée uniquement aux boutons exploitables dans la vue [!DNL Create] _Travail récent_. <!-- GS-4060 -->

* Le message **Enregistrement en cours** affiché pendant les opérations d’enregistrement de fragment d’e-mail s’affiche désormais uniquement pendant l’opération d’enregistrement. Auparavant, la zone de travail affichait ce message indéfiniment. <!-- GS-6964 -->

* Les éditeurs voient désormais un message d’erreur comme prévu lorsqu’un brouillon ne parvient pas à se charger dans la zone [!DNL Create] _Travail récent_.  <!-- GS-8081 -->

* La zone de travail affiche désormais les méta-annonces redimensionnées et les annonces dans le bon ordre.  <!-- GS-7375 -->

* Les éditeurs peuvent désormais cliquer simultanément dans les champs de l’e-mail et afficher des publicités. <!-- GS-6297 -->

* La fonctionnalité de modification de fragment pour les e-mails et les méta-annonces est désormais déclenchée comme prévu par un seul clic. <!-- GS-8081 -->

* Amélioration des performances du bouton [!DNL Create] **[!UICONTROL Précédent]**. <!-- GS-6767 -->

+++

+++Notes de la version 2024.11.14

### Nouvelles fonctionnalités

Ajout de la prise en charge de l’affichage de contenu statique hébergé sur des domaines externes. GenStudio for Performance Marketing valide la source de contenu définie dans le modèle et incorpore une copie pour produire l’aperçu du modèle. Voir [Contenu statique](/help/user-guide/content/customize-template.md#static-content). <!-- GS-6107 -->

### Correctifs et améliorations

* Lorsqu’ils sont redimensionnés dans un navigateur autre que celui utilisé pour générer le contenu initial, les brouillons se chargent désormais comme prévu. <!-- GS-7204 -->

* Tous les caractères sont désormais correctement représentés dans HTML exporté. <!-- GS-7246 -->

* Les boutons de la fenêtre contextuelle [!DNL Content] _Expériences_ **[!UICONTROL Exporter]** ne sont plus tronqués dans certaines langues. <!-- GS-6873 -->

* Les publicités display créées avec des modèles dimensionnés à 50x50 sont désormais exportées dans la taille d’image attendue. Auparavant, les fichiers PNG étaient exportés à des dimensions deux fois supérieures à celles attendues. <!-- GS-7192 -->

* Les erreurs de modèle qui se sont produites lorsque les publicités display ont été redimensionnées sont désormais résolues. <!-- GS-7322 -->

### Localisation

Cette version comprend des améliorations de la localisation dans toute l’interface utilisateur, notamment :

* Toutes les chaînes de la fenêtre contextuelle [!DNL Content] _Charger une ressource_ sont désormais correctement localisées. <!-- GS-6872 6770 -->
* Toutes les info-bulles du champ [!DNL Content] _Assets_ view **[!UICONTROL Search]** sont localisées. <!-- GS-6879 -->
* Lors du remplacement d’une image existante dans une variante d’e-mail sur la zone de travail [!DNL Create], la vue _Sélectionner à partir du contenu_ est désormais localisée. <!-- GS-6906 -->

+++

+++Notes de la version 2024.11.07

### Correctifs et améliorations

* L’icône _Enregistrement en cours_ ne s’affiche plus lorsqu’un utilisateur clique sur **[!UICONTROL Charger une nouvelle image]** puis annule l’opération avant la fin du chargement. <!-- GS-6780 -->

* Les titres des expériences sont désormais créés correctement lors de la régénération des expériences. <!-- GS-7006 -->

* Les problèmes liés au scintillement des barres de défilement lors du chargement du brouillon ont été résolus. <!-- GS-5587 -->

* Le lien `View documentation` dans la fenêtre contextuelle [!DNL Content] _Ajouter votre modèle approuvé_ fonctionne désormais comme prévu. <!-- GS-6881 -->

* La suppression d’une image du tiroir d’invite lors d’une opération de redimensionnement n’entraîne plus d’erreur. <!-- GS-7115 7009 -->

* Sélectionnez **[!UICONTROL Supprimer]** dans le menu d’actions [!DNL Create] (...) pour continuer. <!-- GS-6871 -->

* Les utilisateurs peuvent désormais contrôler tous les éléments interactifs Meta et de modèle uniquement à l’aide du clavier. <!-- GS-4066 -->

* Ajout de l’extraction des dimensions d’image des champs d’image de modèle aux modèles d’affichage publicitaire. Les demandes de recadrage intelligent sont désormais envoyées pour la dimension réelle de l’image et non pour le modèle entier. <!-- GS-6926 -->

* Chaîne de `Zoom to fit to screen` localisée dans l’e-mail généré et les métadonnées publicitaires. <!-- GS-5063 -->

* Le tiroir d’invite [!DNL Create] se ferme désormais comme prévu lorsqu’un utilisateur clique dessus. <!-- GS-5254 -->

* L’exportation des publicités Meta inclut désormais le libellé call-to-action sélectionné comme prévu. <!-- GS-6504 -->

* Le score de la marque est maintenant mis à jour et conservé comme prévu pour les expériences régénérées. <!-- GS-6535 -->

* L’exportation HTML des publicités Meta et des publicités display n’inclut plus de `div` wrapper et d’éléments `chrome`. <!-- GS-7116 -->

* Les problèmes de rendu des brouillons d’e-mails lors de la publication sont désormais résolus. <!-- GS-6394 -->

* Le bouton Zone de travail **[!UICONTROL Marque]** est désormais désactivé lorsqu’un score de marque n’est pas généré. <!-- GS-6429 -->

* Le bouton (bascule) Facebook/Instagram de la barre d’actions Zone de travail met désormais à jour les rendus d’expérience comme prévu lorsque le paramètre Zone de travail `ReadOnly` est activé. <!-- GS-7039 -->

#### Régénération de l&#39;image

* Le redimensionnement de plusieurs variantes Meta et fonctionne désormais comme prévu. Auparavant, la zone de travail n’affichait pas les variantes régénérées, mais restait vide. <!-- GS-7010 -->

* La régénération de fragment fonctionne désormais comme prévu pour les expériences redimensionnées. <!-- GS-6836 -->

* La régénération des images Meta et des publicités après leur redimensionnement n’entraîne plus d’erreur. Auparavant, le redimensionnement des images avant la régénération modifiait les métadonnées du canal de `meta` en `facebook`. <!-- GS-7042 -->

+++

+++Notes de la version 2024.10.31

### Nouvelles fonctionnalités

* Le filtre de recherche **[!DNL Content]** prend désormais en charge la recherche par balise de couleur. <!-- GS-5501 -->

* La zone de travail **[!DNL Create]** affiche désormais le nombre de caractères des fragments d’e-mail. <!-- GS-5819 -->

### Correctifs et améliorations

* Des libellés de lecteur d’écran manquants ont été ajoutés aux éléments de `view` mobiles et de bureau. <!-- GS-5624 4729 -->

* Les zones d’objet et de texte pré-en-tête de l’e-mail **[!DNL Create]** Canvas sont désormais dynamiques en hauteur. <!-- GS-6258 -->

* Les problèmes de disposition liés aux bordures des emails ont été résolus. <!-- GS-6631 -->

* Le focus au clavier fonctionne désormais comme prévu sur le bouton **[!DNL Content]** **[!UICONTROL Supprimer]**. Auparavant, les utilisateurs ne pouvaient pas accéder à ce bouton à l’aide du clavier.  <!-- GS-4065 -->

+++

+++Notes relatives à la version 2024.10.14 Disponibilité générale

Cette version présente Adobe GenStudio for Performance Marketing, une application générative basée sur l’IA qui accélère la planification, le développement et l’analyse des campagnes marketing. GenStudio for Performance Marketing permet aux équipes marketing de créer du contenu multicanal sur la marque pour les publicités, les e-mails et les campagnes, tout en fournissant des informations en temps réel pour optimiser les performances du contenu.

### Fonctionnalités

Les principales fonctionnalités du produit sont les suivantes :

**[!DNL Create]** présente la zone de travail, qui offre une expérience d’invite structurée qui permet aux éditeurs de contenu de générer rapidement du contenu et des variantes. Les responsables système forment le produit aux directives de la marque de l’entreprise. [!DNL Create] garantit que tout le contenu généré par l’IA s’aligne sur les directives de votre marque (marque, personnages clients et descriptions de produits) et rationalise la production de contenu marketing à fort impact et cohérent avec la marque.

**[!DNL Content]** stocke des ressources et des expériences approuvées organisées et conformes à la marque. Les utilisateurs de GenStudio for Performance Marketing peuvent facilement rechercher, modifier, réutiliser et partager des ressources approuvées, ce qui réduit la nécessité de recréer du contenu pour chaque campagne.

**[!DNL Reviews and Approvals]** établit un cadre permettant aux parties prenantes d’examiner et d’approuver les variantes générées avant de les enregistrer pour **[!DNL Content]** ou l’exportation.

**[!DNL Campaigns]** organise et gère les campagnes marketing, assurant ainsi une exécution et un tracking rationalisés. Les collaborateurs peuvent visualiser, planifier et suivre les campagnes afin de gérer plusieurs initiatives efficacement et d’assurer une diffusion rapide.

**[!DNL Insights]** permet d’évaluer en temps réel les performances du contenu, ce qui aide les spécialistes marketing à optimiser leurs stratégies et à prendre des décisions éclairées.

GenStudio for Performance Marketing s’intègre à d’autres produits Adobe Experience Cloud, notamment Adobe Express et Adobe AEM Assets.

+++
