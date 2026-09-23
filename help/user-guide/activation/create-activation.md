---
title: Workflow d’activation
description: Découvrez le workflow d’activation des expériences publicitaires.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: db0cebfe795569d9913757d190db853097a00405
workflow-type: tm+mt
source-wordcount: '1233'
ht-degree: 4%
---
# Workflow d’activation

[!DNL Activate] active les expériences publiées sur ses plateformes de publicités payantes. Une expérience GenStudio for Performance Marketing est un composant de campagne marketing, tel qu’une publicité, préparé pour une audience spécifique sur une plateforme de publicités payantes. Les expériences d’activation contiennent trois composants principaux :

* **Ressources multimédias** : images ou vidéo dans votre expérience publicitaire, dans des types de fichiers et des proportions qui varient selon la plateforme et le format.

* **Texte** : toutes les copies incluses dans votre publicité, y compris les titres, le corps du texte et les éléments call-to-action.

* **Métadonnées** : attributs définis par l’utilisateur, généralement non visibles pour l’audience de l’annonce, qui améliorent l’analyse, le filtrage et le suivi des performances.

Vous préparez et approuvez ces composants dans [!DNL Content] avant l’activation. [!DNL Activate] ne crée ni ne modifie les ressources, les titres ou le corps du texte approuvés. Il applique uniquement la configuration dont chaque plateforme a besoin, puis publie l’expérience.

Un seul tableau d’activation peut inclure des expériences pour plusieurs plateformes et formats d’annonces publicitaires payantes.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## Connecter les comptes de votre plateforme

Un gestionnaire ou un éditeur de système GenStudio doit connecter les comptes publicitaires de chaque plateforme publicitaire payante avant que vous puissiez activer une expérience sur cette plateforme. Pour connaître les étapes de ce processus, voir [Connecter des comptes de médias achetés](/help/user-guide/connectors/connect-channel.md).

## Démarrer une activation

Démarrez une activation à partir de l’un des deux points d’entrée suivants :

* **Dans[!DNL Content]** : filtrer les expériences, sélectionnez une ou plusieurs expériences publiées, puis cliquez sur **[!UICONTROL Activer]** dans la barre d’actions supérieure.

  ![Sélection des expériences publiées dans le contenu et clic sur Activer pour démarrer une activation](./images/content-select-activate.png)

* **De[!DNL Activate]** : sur la page de destination [!DNL Activate], cliquez sur **[!UICONTROL + Nouvelle activation]**. Cette action ouvre la même galerie d’expériences, où vous sélectionnez des expériences à activer.

Dans les deux cas, recherchez les expériences par nom d’expérience ou filtrez selon plusieurs canaux pour trouver les expériences souhaitées.

Si votre sélection comprend des expériences de format d’affichage, spécifiez la plateforme d’affichage à utiliser : Google Campaign Manager 360, Innovid, Amazon Ads ou The Trade Desk. Cliquez ensuite sur **[!UICONTROL Démarrer l’activation]**. Pour d’autres formats, tels que Meta, LinkedIn, TikTok, YouTube et ChatGPT, [!DNL Activate] déduit la plateforme du canal de l’expérience et ignore cette étape.

[!DNL Activate] génère ensuite un tableau d’activation répertoriant toutes les expériences sélectionnées.

![Une table d’activation nouvellement générée, regroupée en sous-tables Meta et LinkedIn, avec chaque annonce marquée comme nécessitant une attention particulière jusqu’à ce que ses champs soient terminés](./images/activation-table.png)

[!DNL Activate] organise le tableau en sous-tableaux par format et plateforme publicitaires, par exemple Meta single image ou LinkedIn single image. Chaque ligne représente une annonce publicitaire. Pour la plupart des plateformes, telles que LinkedIn, TikTok et d’affichage, une expérience avec plusieurs proportions génère une ligne par proportion d’aspect ; supprimez toutes les lignes dont vous n’avez pas besoin. Meta est l’exception. Une publicité Meta peut inclure plusieurs proportions dans une même publicité, de sorte qu’une expérience Meta à proportions multiples ne génère toujours qu’une seule ligne.

## Gérer votre table d’activation

Votre tableau d’activation est enregistré automatiquement en tant que brouillon lorsqu’il s’ouvre. Vous pouvez quitter et reprendre le brouillon à tout moment avant de le publier.

Pour ajouter d’autres expériences à un tableau d’activation que vous avez déjà ouvert, cliquez sur **[!UICONTROL Ajouter d’autres expériences]** en haut à droite du tableau. La galerie d’expériences s’ouvre à nouveau, vous pouvez ainsi sélectionner d’autres expériences et les ajouter [!DNL Activate] au tableau existant.

**[!UICONTROL Ajouter plus d’expériences]** permet également d’activer plusieurs plateformes d’affichage dans le même tableau. Les expériences de format d’affichage vous demandent de choisir une plateforme d’affichage unique en premier, mais vous pouvez cliquer sur **[!UICONTROL Ajouter d’autres expériences]**, sélectionner d’autres expériences de format d’affichage et choisir une plateforme d’affichage différente de celle déjà présente dans votre tableau. Par exemple, vous pouvez ajouter les annonces The Trade Desk à un tableau qui contient déjà les annonces Innovid.

Une fois que votre tableau propose les expériences appropriées, configurez ensuite les champs de chaque annonce publicitaire.

## Configurer des détails de configuration de la publicité et de la plateforme

Modifiez les champs intégrés par ligne ou sélectionnez plusieurs lignes dans le même tableau de format et cliquez sur **[!UICONTROL Modifier les détails]** dans la barre d’outils qui s’affiche pour modifier ces champs en bloc en même temps.

![Sélection de plusieurs publicités dans un tableau d’activation pour modifier en masse les détails ou les paramètres de la plateforme](./images/bulk-edit-action-bar.png)

Les ressources, titres et corps de texte approuvés sont verrouillés et ne peuvent pas être modifiés dans le tableau d’activation, puisqu’ils ont déjà été examinés et approuvés en [!DNL Content]. Les champs restants peuvent être modifiés et varient selon la plateforme. [!DNL Activate] affiche uniquement les colonnes relatives aux plateformes et formats que vous avez sélectionnés. Utilisez le tableau ci-dessous comme référence pour connaître les éléments modifiables par plateforme.

**Champs modifiables par plateforme**

| Plateforme | Formats pris en charge | Copie verrouillée | Champs de texte modifiables | Champs de configuration de plateforme modifiables |
|---|---|---|---|---|
| Meta | Image, Vidéo, Carrousel | Titre, corps | Description, Call-to-action, URL de destination, Paramètres d’URL, ID de suivi | Compte Publicitaire, Page Facebook, Profil Instagram, Meta Campaign, Ensemble Publicitaire Meta |
| LinkedIn | Image unique, vidéo unique | Titre, Texte D’Introduction | Description, Call-to-action, URL de destination, Paramètres d’URL, ID de suivi | Compte Publicitaire, Campagne, Ensemble Publicitaire |
| Google Campaign Manager 360 | Affichage statique, affichage vidéo, affichage Zip HTML5 | s.o. | Identifiant de tracking | Annonceur |
| Amazon Ads | Affichage statique | s.o. | Identifiant de tracking | Compte |
| Innovid | Affichage statique, affichage Zip HTML5 | s.o. | Identifiant de tracking | Compte, Bibliothèque Creative, Nom Du Concept |
| TikTok | Publicités vidéo intégrées au flux | Texte du Principal | Call-to-action, URL de destination, ID de tracking | Compte publicitaire, campagne, groupe publicitaire |
| YouTube | Shorts dans les campagnes de génération de la demande Google Ads | Description | Call-to-action, nom de l’entreprise, URL de destination, paramètres d’URL, ID de suivi | Compte, Campagne, Groupe Publicitaire, Logo |
| ChatGPT | Cartes de conversation | Titre, corps | URL de la cible, ID de tracking | Compte publicitaire OpenAI, campagne OpenAI, groupe publicitaire OpenAI |
| Le Trade Desk | Affichage statique | s.o. | Identifiant de tracking | Compte, Campagne |

Pour configurer les champs de configuration de la plateforme pour un groupe de formats d’annonce publicitaire, cliquez sur **[!UICONTROL Gérer les paramètres de la plateforme]** et modifiez les champs dans la boîte de dialogue qui s’affiche.

![Boîte de dialogue Gérer les paramètres de plateforme permettant de choisir un compte publicitaire, une campagne et une visionneuse d’annonces Meta](./images/manage-platform-settings.png)

Chaque champ **[!UICONTROL ID de suivi]** est prérempli avec le nom de l’expérience : la plateforme publicitaire utilise cette valeur comme nom de l’annonce publicitaire ou nom du contenu créatif pour le compte rendu des performances et la résolution des problèmes. Modifiez la valeur sur place si vous souhaitez utiliser autre chose.

![Modification d’un champ Identifiant de tracking sur la ligne dans la table d’activation](./images/tracking-id-edit.png)

Pour passer plus rapidement d’un champ **[!UICONTROL ID de tracking]** à l’autre, utilisez les raccourcis clavier suivants :

* Appuyez sur **Entrée** pour ouvrir le champ de modification de l’**[!UICONTROL ID de suivi]** sélectionné.
* Appuyez sur la touche fléchée **Haut** ou **Bas** pour accéder au champ **[!UICONTROL ID de suivi]** précédent ou suivant de cette colonne.
* Appuyez à nouveau sur **Entrée** pour enregistrer vos modifications.

## Examinez et publiez vos expériences sur leurs plateformes publicitaires

Vérifiez que chaque ligne indique [!UICONTROL Prêt pour activation]. [!DNL Activate] signale les champs manquants ou non valides, les appels à l’action incompatibles et duplique les identifiants de tracking comme [!UICONTROL Attention requise]. Lorsque chaque ligne est prête, cliquez sur **[!UICONTROL Envoyer aux plateformes]** et confirmez dans la boîte de dialogue de publication.

![Tableau d’activation dans lequel chaque ligne indique Prêt pour l’activation, ce qui active Envoyer aux plateformes](./images/ready-to-activate.png)

[!DNL Activate] signale le statut de chaque publicité en temps quasi réel : En attente, puis Envoyée aux plateformes ou En échec. Si une publicité échoue, passez la souris sur son statut pour afficher l’erreur de la plateforme. Vous pouvez réessayer toutes les annonces ayant échoué dans le tableau en même temps en cliquant sur **[!UICONTROL Réessayer]**, plutôt que de réessayer individuellement. Les lignes déjà envoyées aux plateformes sont bloquées en cas de nouvel envoi et incluent un lien profond vers la publicité dans le gestionnaire de publicités natif de la plateforme de destination. Votre dernière révision avant publication et le lancement des annonces se font dans le propre gestionnaire d’annonces de la plateforme de destination : [!DNL Activate] diffuse toujours les annonces dans un état inactif.

![Tableau d’activation présentant un mélange des statuts En attente et Envoyé aux plateformes après publication](./images/activation-status-pending.png)

Vos tableaux d’activation s’affichent sur la page de destination [!DNL Activate].

## Plateformes prises en charge

Chaque plateforme de publicités payantes comporte des champs de configuration et des conditions préalables spécifiques. Sélectionnez la plateforme de publicités payantes pour obtenir des instructions d’activation :

* [Meta](activate-meta-ad.md)
* [ LinkedIn ](activate-linkedin-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
* [Amazon Ads](activate-amazon-ad.md)
* [Innovid](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [ChatGPT](activate-chatgpt-ad.md)
* [The Trade Desk](activate-trade-desk-ad.md)
