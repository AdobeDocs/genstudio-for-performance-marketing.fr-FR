---
title: Notes de mise à jour d’Adobe GenStudio for Performance Marketing Beta
description: Découvrez les dernières fonctionnalités et améliorations apportées à Adobe GenStudio for Performance Marketing.
hidefromtoc: true
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 9b5e8b37ba988c3dd4a1e5a828487997375474ac
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Notes de mise à jour d’Adobe GenStudio for Performance Marketing Beta

Ces notes mettent en évidence d’importants correctifs et améliorations d’Adobe GenStudio for Performance Marketing pour la semaine se terminant le 4 octobre.

## Nouvelles fonctionnalités et améliorations

* La fonctionnalité de filtrage sur l’ensemble du produit a été améliorée. Les problèmes de filtrage par âge et par sexe dans [!DNL Insights] ont été résolus.  <!-- GS-1198 -->

* Vous pouvez modifier des ressources d’image (JPG ou PNG) directement à l’aide d’Adobe Express. Les éditeurs de contenu peuvent utiliser le canevas _[!UICONTROL Powered by Adobe Express]_ pour supprimer les arrière-plans, appliquer des remplissages génératifs, ajuster les effets et recadrer les images sans quitter GenStudio for Performance Marketing. <!-- GS-4615 -->

* Amélioration de l’expérience de chargement progressif pour les variantes générées, le courrier électronique généré et la messagerie contextuelle. <!-- GS-4651 3062-->

* Les éditeurs de contenu peuvent désormais utiliser la fonction d’ajustement de recadrage pour recadrer les images rendues dans des variantes. <!-- GS-2342 -->

* Les problèmes de redimensionnement et de duplication des modèles ont été résolus. <!-- GS-4895 -->

* La validation de marque explique désormais la cause des échecs qui se produisent lors de la validation.

* Les aperçus de modèle affichent désormais le texte sur l’image comme prévu. <!-- GS-5917 -->

## Améliorations supplémentaires et problèmes résolus

* Le canevas [!DNL Create] effectue désormais le rendu des polices personnalisées à partir des modèles comme prévu. <!-- GS-3415 -->

* La police correcte est désormais appliquée lors de l’exportation des métadonnées publicitaires. <!-- GS-5875 -->

* Les problèmes liés au chargement de modèles qui ont abouti à un chargement réussi mais à une invisibilité de l’interface du produit ont été résolus. <!-- GS-4815 5650-->

* Les utilisateurs peuvent désormais recadrer manuellement les métadonnées publicitaires après les avoir redimensionnées. <!-- GS-5871 -->

* Les utilisateurs n’ont plus besoin de se connecter deux fois à un compte Métadonnées de canal lorsqu’ils sont également connectés à Facebook. <!-- GS-3009 -->

* La vue Canevas des ressources et des expériences reste maintenant cohérente dans tout le processus de création, de révision et d’approbation de contenu. <!-- GS-5877 -->

* Le canevas affiche désormais uniquement quatre variantes lors de la régénération après une opération de redimensionnement. <!-- GS-5869 -->

* La vérification orthographique basée sur le navigateur fonctionne désormais comme prévu dans la zone de travail [!DNL Create]. <!-- GS-5760 -->

* Les publicités affichées sont désormais exportées en tant que fichiers PNG lorsque l’option **[!UICONTROL Exporter en tant que PNG]** est sélectionnée. Auparavant, les publicités affichées étaient exportées en tant que JPEG lorsque le format PNG était sélectionné. <!-- GS-5545 -->

* La marge intérieure a été augmentée entre le bouton **[!UICONTROL Recadrage manuel]** et le bouton **[!UICONTROL Générer]**. Auparavant, le bouton **[!UICONTROL Recadrage manuel]** était partiellement masqué. <!-- GS-6084 -->

* Les aperçus de modèle affichent désormais les polices Google comme prévu. <!-- GS-5946 -->

* Les polices TypeKit et Google importées sont désormais chargées comme prévu lors de l’exportation. <!-- GS-5948 -->

* Résolution de problèmes liés à la génération de contenu avec des modèles personnalisés. Auparavant, lorsqu’un éditeur de contenu tentait de générer une ressource à l’aide d’un modèle personnalisé, la fenêtre contextuelle de génération ne s’affichait pas et la console affichait des erreurs. <!-- GS-5262 -->

* Le brouillon de la zone de travail DisplayAds conserve désormais sa position lorsqu’un utilisateur clique avec le bouton droit sur la zone de travail avant de cliquer à gauche dans le menu contextuel. Auparavant, le Canevas se déplaçait lorsque l’utilisateur cliquait à gauche, ce qui rendait le contenu du brouillon partiellement inaccessible.  <!-- GS-5687 -->

* Le chargement des effets de fusion persiste maintenant jusqu’à ce que la régénération de l’image soit terminée.  <!-- GS-5811 -->

* Les scores de validation de marque ne sont plus invalidés une fois qu’un utilisateur a apporté des modifications à des e-mails, des métadonnées publicitaires ou des publicités affichées. Auparavant, ce score était masqué. <!-- GS-5379 -->

* Les modèles dont les styles CSS sont associés à leur élément `body` sont désormais utilisés comme prévu lors de l’exportation d’expériences. <!-- GS-5947 -->

* Correction de problèmes liés au recadrage manuel d’images de dimension volumineuses. <!-- GS-6039 -->

* Un seul message contextuel s’affiche désormais lorsqu’un utilisateur ajoute une nouvelle ressource dans [!DNL Content]. <!-- GS-5020 -->

* Amélioration des performances de la zone de travail lors de la modification de texte.  <!-- GS-5118 -->

* Ajout d’espaces manquants entre les chaînes sur l’e-mail [!DNL Create] ou la zone de travail des métadonnées. <!-- GS-5019 -->

* Les éditeurs peuvent désormais enregistrer un fichier dont les noms contiennent des caractères spéciaux après modification dans Express. <!-- GS-6131 -->

### Localisation

Cette version comprend des améliorations de la localisation dans l’interface du produit, notamment dans les zones suivantes :

* URL de la destination de l’option **[!UICONTROL En savoir plus]** dans le menu d’invite [!DNL Create]. <!-- GS-5029 -->

* Formats des nombres adjacents aux champs de saisie de recherche [!DNL Insights] > [!DNL Experience]. <!-- GS-4494 -->

## Problème connu

* Les fragments d&#39;email régénérés n&#39;apparaissent pas dans la variante après sélection. (Cependant, les variantes apparaissent une fois le brouillon rouvert ouvert.) <!-- GS-5913 -->
