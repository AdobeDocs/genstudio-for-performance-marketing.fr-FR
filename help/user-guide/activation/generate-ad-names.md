---
title: Générer des noms d’annonces publicitaires
description: Découvrez comment configurer des modèles de dénomination, générer des noms d’annonce cohérents et réviser ou personnaliser les noms avant d’envoyer des annonces à vos plateformes d’activation prises en charge.
role: User
source-git-commit: 7863995df08681a8a427277121a5fbeca131c6a9
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 1%
---

# Générer des noms d’annonces publicitaires

L’affectation de noms d’annonce automatisée dans [!DNL GenStudio for Performance Marketing] vous permet de respecter les conventions de dénomination de votre organisation lorsque vous activez des annonces. Les noms cohérents prennent en charge le reporting des performances, l’attribution et la réconciliation des dépenses.

Chargez votre convention d’affectation des noms pour créer un modèle, puis utilisez-la pour générer des noms à partir des métadonnées d’expérience. Examinez les résultats et apportez les corrections nécessaires avant d&#39;envoyer des annonces à vos plateformes.

## Avant de commencer

La configuration des modèles est une tâche unique. Si un modèle est déjà affecté à votre plateforme dans votre projet actuel, passez à [Générer des noms pour une activation](#generate-names-for-an-activation).

Pour la configuration du modèle, préparez un fichier Excel ne dépassant pas 3 Mo, avec une seule feuille. Les fichiers CSV ne sont pas pris en charge Décrivez la convention d’affectation des noms pour les annonces individuelles, et non pour les campagnes ou les groupes d’annonces.

Incluez les champs dans l’ordre requis, les valeurs autorisées, les codes correspondants et les instructions pour choisir les valeurs. Par exemple, la sélection de `Image` pour le champ `format` peut générer `IMG` dans le nom.

Téléchargez l’[exemple de convention de nommage WKND Meta (Excel)](assets/wknd-meta-naming-convention.xlsx) pour explorer un exemple de structure. Elle comprend des définitions de champ et des exemples de valeurs pour l’année, le trimestre, la marque, le produit, la campagne, la plateforme, le format, la version créative, le persona, le marché, la langue et le CTA.

Remplacez les exemples de valeurs et de règles par la convention de votre organisation avant d’utiliser le fichier pour vos propres activations. Les valeurs de plateforme de l’exemple illustrent les choix de dénomination, et non une liste de destinations d’activation prises en charge.

Un responsable système doit affecter le modèle à vos plateformes. Différents projets peuvent utiliser différents modèles par défaut pour la même plateforme.

## Création d’un modèle de dénomination

Créez un modèle à partir de votre fichier de convention de nommage existant, puis passez en revue la structure extraite avant de l’utiliser.

1. Ouvrez le projet dans lequel vous souhaitez utiliser le modèle.
1. Accédez à **[!UICONTROL Plus]** > **[!UICONTROL Paramètres]**.
1. Sélectionnez **[!UICONTROL Configurer]** en regard de **[!UICONTROL Modèle de nom d&#39;annonce]**.

   Si des modèles existent déjà, ouvrez le **[!UICONTROL modèle de nom d&#39;annonce publicitaire]**, puis sélectionnez **[!UICONTROL Créer un modèle]**.

1. Sélectionnez **[!UICONTROL Sélectionner le fichier]** dans la boîte de dialogue **[!UICONTROL Télécharger le fichier]**.
1. Choisissez votre fichier Excel.

   Vous pouvez également faire glisser le fichier dans la zone de chargement. Lors de l’analyse de **[!UICONTROL votre feuille de calcul...]** apparaît, les champs et les valeurs sont mappés à votre modèle. Cela peut prendre quelques minutes.

1. Passez en revue les champs, les valeurs autorisées et l’aperçu du nom de l’annonce **[!UICONTROL 1.]**

   L’aperçu utilise des exemples de valeurs, et non les détails d’une annonce publicitaire spécifique.

1. Sélectionnez **[!UICONTROL Enregistrer]**.

Les fichiers de plus de 3 Mo, les types de fichiers non pris en charge et les fichiers vides affichent une erreur sans modifier les modèles existants ou les affectations de plateforme.

## Personnalisation d’un modèle

Modifiez un modèle enregistré pour ajuster son nom, ses champs, son séparateur ou ses règles.

1. Accédez à **[!UICONTROL Plus]** > **[!UICONTROL Paramètres]** > **[!UICONTROL Modèle de nom publicitaire]**.
1. Ouvrez le menu à trois points en regard de votre modèle.
1. Sélectionnez **[!UICONTROL Modifier]**.
1. Sélectionnez l’icône en forme de crayon à côté du titre pour renommer le modèle.
1. Définissez le séparateur de champs **** en fonction de votre convention.
1. Faites glisser les champs dans l’ordre requis.

   Utilisez **[!UICONTROL Ajouter un champ]** ou l’icône de corbeille d’un champ si vous devez modifier les champs inclus.

1. Sélectionnez l’icône en forme de crayon d’un champ pour ouvrir ses paramètres.
1. Vérifiez **[!UICONTROL Type]** et **[!UICONTROL Name]** dans la boîte de dialogue **[!UICONTROL Modifier un champ]**.

   Utilisez **[!UICONTROL Liste déroulante]** pour un champ avec des choix prédéfinis ou **[!UICONTROL Texte libre]** pour une valeur que vous saisissez.

1. Pour un champ de liste déroulante, passez en revue les **[!UICONTROL options]** et le **[!UICONTROL code]**.

   **[!UICONTROL Options]** contient les choix lisibles. **[!UICONTROL Code]** contient les valeurs correspondantes utilisées dans le nom de la publicité. Par exemple, l’option `Image` utilise le code `IMG`.

   Utilisez l&#39;option **[!UICONTROL Ajouter]** pour ajouter un choix ou l&#39;icône moins à côté d&#39;un choix pour le supprimer. Les valeurs en double dans un champ ne sont pas autorisées.

1. Saisissez les **[!UICONTROL règles de champ]** nécessaires pour choisir ou formater la valeur de ce champ.

   Pour le champ de texte libre `creativeVersion` de l’exemple, vous pouvez saisir `Use the experience name as a starting value, with spaces removed.`

1. Sélectionnez **[!UICONTROL Enregistrer]** dans la boîte de dialogue du champ.

   Répétez la vérification des champs pour tous les autres champs qui nécessitent des modifications.

1. Saisissez les **[!UICONTROL règles de modèle]** qui s’appliquent à l’ensemble du nom.

   Par exemple, saisissez `Remove spaces from Product and Campaign values.`

1. Sélectionnez **[!UICONTROL Enregistrer]** en haut de la page.

L’aperçu reflète l’ordre et le séparateur des champs mis à jour. Rouvrez le modèle pour vérifier vos modifications enregistrées.

L’éditeur de champ indique comment les options lisibles correspondent aux codes inclus dans les noms générés :

![Modifiez une boîte de dialogue de champ avec les options de format Image, Vidéo, Carrousel et HTML5 et leurs codes correspondants.](images/ad-name-field-options-codes.png)

## Affectation d’un modèle à des plateformes

Les responsables système définissent le modèle par défaut pour chaque plateforme au sein d’un projet. Si vous n&#39;êtes pas un responsable système, demandez-lui d&#39;effectuer cette procédure.

1. Ouvrez le projet dont vous souhaitez définir les paramètres par défaut de la plateforme.
1. Accédez à **[!UICONTROL Plus]** > **[!UICONTROL Paramètres]** > **[!UICONTROL Modèle de nom publicitaire]**.
1. Ouvrez le menu à trois points en regard de votre modèle.
1. Sélectionnez **[!UICONTROL Modifier]**.
1. Sélectionnez une ou plusieurs plateformes sous **[!UICONTROL Plateformes préférées]** au bas de l’éditeur.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

Chaque plateforme comporte un modèle par défaut par projet. Vous pouvez attribuer le même modèle à plusieurs plateformes.

Vous pouvez afficher et modifier des modèles dans plusieurs projets, mais vous ne pouvez modifier les affectations que pour le projet dans lequel vous vous trouvez actuellement.

Le remplacement des valeurs par défaut d&#39;une plateforme ne supprime pas le modèle précédent et ne modifie pas les affectations d&#39;autres projets.

L’exemple ci-dessous montre l’aperçu du modèle, l’ordre des champs, les règles et **[!UICONTROL les plateformes préférées]** avec Meta Ads sélectionnées :

![Éditeur de modèles WKND avec un séparateur de traits de soulignement, 12 champs de nom d’annonce, des règles de modèle et des annonces Meta sélectionnés sous Plateformes préférées.](images/ad-name-template-editor.png)

## Générer des noms pour une activation

Générez des noms après avoir préparé votre activation et examiné les métadonnées d’expérience dont votre modèle a besoin, telles que la campagne, le produit ou la personne.

1. Ouvrez **[!UICONTROL Activer]** dans le projet prévu.
1. Ajoutez vos expériences à une activation.
1. Terminez la configuration de la plateforme et toutes les informations requises, y compris la copie, call-to-action (CTA) et l’URL du site web.
1. Vérifiez que les expériences disposent des métadonnées nécessaires à votre convention d’affectation de noms.
1. Sélectionnez **[!UICONTROL Générer le nom de l’annonce publicitaire]** au-dessus du tableau d’activation.

   Attendez que **[!UICONTROL Génération des noms d&#39;annonces]** soit terminée avant de consulter les résultats.

1. Vérifiez la colonne **[!UICONTROL Nom de l’annonce publicitaire]**.

La génération s’applique à toutes les annonces sur les plateformes auxquelles un modèle est affecté, à l’exception des annonces dont les remplacements sont activés. Les noms ne sont pas générés automatiquement lorsque vous ouvrez le tableau.

Au départ, chaque publicité utilise le nom de son expérience. Si aucun modèle n’est affecté à une plateforme, la génération laisse ses noms inchangés et vous pouvez les modifier manuellement.

Si aucun modèle n’est affecté à aucune plateforme, aucun nom n’est généré.

## Corriger un nom d’annonce publicitaire individuel

Consultez les noms générés avant d’envoyer vos publicités. Les valeurs manquantes apparaissent comme des espaces réservés de champ mis en surbrillance, tels que `[market]`, et les publicités affectées affichent **[!UICONTROL Besoin d’attention]**.

Le tableau d’activation signale les noms dont les valeurs sont manquantes afin que vous puissiez les rechercher et les corriger :

![Tableau d’activation avec un avertissement de valeurs manquantes, des espaces réservés de marché mis en surbrillance dans la colonne Nom de l’annonce et des statuts Attention requise.](images/ad-names-missing-values.png)

1. Sélectionnez la ligne de l’annonce publicitaire dans le tableau d’activation.
1. Sélectionnez **[!UICONTROL Modifier le nom de l’annonce publicitaire]**.
1. Mettez à jour les listes déroulantes ou les champs de texte appropriés.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

Par exemple, si `market` n’a pas de valeur, saisissez ou sélectionnez le marché approprié pour remplacer `[market]` dans le nom.

Vérifiez le nom mis à jour par rapport à votre convention.

## Résoudre les noms potentiellement en double

Les noms d’annonces publicitaires identiques sur la même plateforme sont marqués comme doublons potentiels.

1. Sélectionnez l’une des publicités concernées.
1. Sélectionnez **[!UICONTROL Modifier le nom de l’annonce publicitaire]**.
1. Modifiez le nom afin que les deux noms soient différents.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

L’avertissement de doublon potentiel disparaît après modification des noms.

## Modifier plusieurs noms d’annonces publicitaires à la fois

Utilisez la modification en masse pour appliquer une correction partagée sans remplacer les valeurs qui doivent rester différentes pour chaque publicité.

1. Sélectionnez les annonces à l’aide des cases à cocher de leur ligne.
1. Sélectionnez **[!UICONTROL Modifier le nom de l’annonce publicitaire]** dans la barre d’outils de sélection.
1. Modifiez uniquement les champs qui doivent avoir la même valeur pour les annonces sélectionnées.

   **[!UICONTROL Valeurs mixtes]** signifie que les publicités sélectionnées ont actuellement des valeurs différentes pour un champ. Ne modifiez pas ce champ pour conserver la valeur de chaque annonce publicitaire.

1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Vérifiez les noms mis à jour pour en vérifier l’exactitude et les doublons potentiels.

Seules les publicités sélectionnées sont mises à jour. Les publicités non sélectionnées restent inchangées.

L’éditeur en masse affiche **[!UICONTROL Valeurs mixtes]** pour les champs qui diffèrent selon les publicités sélectionnées :

![Détail de la boîte de dialogue Modifier 4 noms d&#39;annonces affichant des valeurs mixtes pour le produit, la campagne, creativeVersion et persona.](images/ad-names-bulk-edit.png)

Par exemple, le fait de modifier uniquement le persona de `OutdoorBeginners` à `Adventurers` conserve les différents produits. Ces noms raccourcis illustrent la modification :

| Avant | Après |
| --- | --- |
| `WKND_TrailBag_OutdoorBeginners` | `WKND_TrailBag_Adventurers` |
| `WKND_RiosShirt_OutdoorBeginners` | `WKND_RiosShirt_Adventurers` |

## Utiliser un nom d’annonce publicitaire personnalisé

Remplacer un nom généré lorsqu’une publicité nécessite un nom personnalisé complet.

1. Sélectionnez la ligne de l’annonce.
1. Sélectionnez **[!UICONTROL Modifier le nom de l’annonce publicitaire]**.
1. Activez **[!UICONTROL Remplacer les noms d&#39;annonces]**.
1. Saisissez le nom personnalisé.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

Le nom personnalisé reste inchangé lorsque vous générez à nouveau des noms.

Lorsque le remplacement est activé, vous pouvez modifier le nom complet au lieu de ses champs de modèle individuels :

![Boîte de dialogue Modifier le nom de l’annonce publicitaire avec l’option Remplacer les noms d’annonce activée et le nom complet de l’annonce WKND disponible pour modification.](images/ad-name-override.png)

Pour revenir à l’affectation de nom basée sur un modèle, procédez comme suit :

1. Ouvrez **[!UICONTROL Modifier le nom de l’annonce publicitaire]**.
1. Désactivez **[!UICONTROL Remplacer les noms d&#39;annonces]**.
1. Sélectionnez **[!UICONTROL Enregistrer]**.
1. Sélectionnez **[!UICONTROL Générer le nom de l’annonce publicitaire]** au-dessus du tableau d’activation.

Cette action de génération s’applique également aux autres annonces éligibles dans le tableau.

## Répondre aux modifications du modèle

Lorsque vous modifiez une table d&#39;activation, un avertissement s&#39;affiche si un modèle qu&#39;elle utilise a été modifié ou supprimé.

Si le modèle a été modifié, passez en revue le modèle mis à jour avant de régénérer les noms. Sélectionnez **[!UICONTROL Générer le nom de l’annonce]** pour l’appliquer.

Si le modèle a été supprimé ou si vous avez besoin d’un remplacement, procédez comme suit :

1. Demandez à un responsable système d&#39;affecter un modèle de remplacement à la plateforme concernée dans le même projet.
1. Revenez à la table d’activation.
1. Sélectionnez **[!UICONTROL Générer le nom de l’annonce publicitaire]**.
1. Passez en revue les noms mis à jour.

Les noms dont les remplacements sont activés restent inchangés pendant la régénération.

## Envoyer des publicités aux plateformes

Passez en revue vos noms et adresses définitifs de champs non résolus, de doublons potentiels et d&#39;autres **[!UICONTROL problèmes nécessitant votre attention]** avant d&#39;envoyer des publicités.

Lorsque l’activation est prête, sélectionnez **[!UICONTROL Envoyer aux plateformes]**.

Les noms publiés correspondent exactement aux noms finaux dans [!DNL GenStudio for Performance Marketing], y compris les noms générés, les noms modifiés par le biais de champs de modèle et les noms remplacés.

Pour les destinations d’affichage telles qu’Innovid, les noms apparaissent comme des noms créatifs.
