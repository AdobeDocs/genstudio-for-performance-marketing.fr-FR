---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
hidefromtoc: true
hide: true
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: c0f45fb0ffc61d20611693498f1b12d3946ca6ca
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# Notes de mise à jour d’Adobe GenStudio for Performance Marketing Beta

Ces notes mettent en évidence les correctifs et améliorations importants apportés à Adobe GenStudio for Performance Marketing pour la semaine se terminant le 4 octobre.

## Nouvelles fonctionnalités et améliorations

* La fonctionnalité de filtrage sur l’ensemble du produit a été améliorée. Les problèmes de filtrage par âge et par sexe dans [!DNL Insights] ont été résolus.  <!-- GS-1198 -->

* Vous pouvez modifier des ressources d’image (JPG ou PNG) directement dans Adobe Express. Les éditeurs de contenu peuvent utiliser la zone de travail _[!UICONTROL Optimisée par Adobe Express]_ pour supprimer des arrière-plans, appliquer des remplissages génératifs, ajuster des effets et recadrer des images sans quitter GenStudio for Performance Marketing. <!-- GS-4615 -->

* Amélioration de l’expérience de chargement progressif pour les variantes générées, les e-mails générés et les messages contextuels. <!-- GS-4651 3062-->

* Les éditeurs de contenu peuvent désormais utiliser la fonction d’ajustement du recadrage pour recadrer les images rendues dans les variantes. <!-- GS-2342 -->

* Les problèmes de redimensionnement et de duplication des modèles ont été résolus. <!-- GS-4895 -->

* La validation de la marque explique désormais la cause des échecs qui se produisent pendant la validation.

* Les aperçus de modèles affichent désormais le texte sur l’image comme prévu. <!-- GS-5917 -->

## Améliorations supplémentaires et problèmes résolus

* La zone de travail [!DNL Create] effectue désormais le rendu des polices personnalisées à partir de modèles comme prévu. <!-- GS-3415 -->

* La police correcte est désormais appliquée lors de l’exportation de publicités Meta. <!-- GS-5875 -->

* Les problèmes de chargement du modèle qui entraînaient la réussite du chargement, mais un manque de visibilité dans l’interface du produit ont été résolus. <!-- GS-4815 5650-->

* Les utilisateurs peuvent désormais recadrer manuellement les annonces Meta après les avoir redimensionnées. <!-- GS-5871 -->

* Les utilisateurs n’ont plus besoin de se connecter deux fois à un compte Meta Ads lorsqu’ils sont également connectés à Facebook. <!-- GS-3009 -->

* La vue Zone de travail des ressources et des expériences reste désormais cohérente tout au long du processus de création, de révision et d’approbation de contenu. <!-- GS-5877 -->

* La zone de travail n’affiche désormais que quatre variantes lors de la régénération après une opération de redimensionnement. <!-- GS-5869 -->

* La vérification orthographique basée sur le navigateur fonctionne désormais comme prévu dans la zone de travail [!DNL Create]. <!-- GS-5760 -->

* Les publicités display sont désormais exportées sous forme de fichiers PNG lorsque l’option **[!UICONTROL Exporter au format PNG]** est sélectionnée. Auparavant, les publicités display étaient exportées en tant que JPEG lorsque le format PNG était sélectionné. <!-- GS-5545 -->

* La marge intérieure a été augmentée entre le bouton **[!UICONTROL Recadrage manuel]** et le bouton **[!UICONTROL Générer]**. Auparavant, le bouton **[!UICONTROL Recadrage manuel]** était partiellement masqué. <!-- GS-6084 -->

* Les aperçus de modèles affichent désormais les polices Google comme prévu. <!-- GS-5946 -->

* Les polices TypeKit et Google importées sont désormais chargées comme prévu lors de l’exportation. <!-- GS-5948 -->

* Résolution de problèmes liés à la génération de contenu avec des modèles personnalisés. Auparavant, lorsqu’un éditeur de contenu tentait de générer une ressource à l’aide d’un modèle personnalisé, la fenêtre contextuelle de génération n’était pas affichée et la console affichait des erreurs. <!-- GS-5262 -->

* Le brouillon de zone de travail DisplayAds conserve désormais sa position lorsqu’un utilisateur clique avec le bouton droit sur la zone de travail avant de cliquer avec le bouton gauche en dehors du menu contextuel. Auparavant, la zone de travail se déplaçait lorsque l’utilisateur cliquait avec le bouton gauche de la souris, ce qui rendait le contenu du brouillon partiellement inaccessible.  <!-- GS-5687 -->

* Le chargement des effets de scintillement persiste jusqu’à ce que la régénération de l’image soit terminée.  <!-- GS-5811 -->

* Les scores de validation de marque ne sont plus invalidés lorsqu’un utilisateur apporte des modifications à des e-mails générés, à des publicités Meta ou à des publicités display. Auparavant, ce score était masqué. <!-- GS-5379 -->

* Les modèles auxquels des styles CSS sont associés à leur élément `body` sont désormais utilisés comme prévu lors de l’exportation d’expériences. <!-- GS-5947 -->

* Correction de problèmes liés au recadrage manuel d’images de grandes dimensions. <!-- GS-6039 -->

* Un seul message pop-up s’affiche désormais lorsqu’un utilisateur ajoute une nouvelle ressource dans [!DNL Content]. <!-- GS-5020 -->

* Amélioration des performances de la zone de travail lors de la modification de texte.  <!-- GS-5118 -->

* Ajout d’espaces manquants entre les chaînes de l’e-mail [!DNL Create] ou de la zone de travail de publicité Meta. <!-- GS-5019 -->

* Les éditeurs peuvent désormais enregistrer un fichier dont les noms contiennent des caractères spéciaux après modification dans Express. <!-- GS-6131 -->

### Localisation

Cette version comprend des améliorations de la localisation dans l’interface du produit, notamment dans les domaines suivants :

* L’URL de la destination de l’option **[!UICONTROL En savoir plus]** dans le menu d’invite du [!DNL Create]. <!-- GS-5029 -->

* Formats des nombres adjacents aux champs de saisie de recherche [!DNL Insights] > [!DNL Experience]. <!-- GS-4494 -->

## Problème connu

* Les fragments d’e-mail régénérés n’apparaissent pas dans la variante après la sélection. (Cependant, des variantes apparaissent après la réouverture du brouillon.) <!-- GS-5913 -->
