---
title: Connecter un assistant d’IA
description: Découvrez comment connecter un assistant d’IA pris en charge à [!DNL GenStudio for Performance Marketing] et vérifier l’accès aux outils disponibles.
role: User
source-git-commit: 6fb7ddb7549ea6bcd66b6139fbde9ebe12ddaa22
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---

# Connecter un assistant d’IA

Connectez un assistant d’IA pris en charge à [!DNL GenStudio for Performance Marketing] avant d’interroger les données de performances, d’assembler des brouillons ou de publier des publicités approuvées. Les options de connexion varient selon l’assistant IA et l’organisation.

## Conditions préalables

Avant de vous connecter, vérifiez que vous disposez des éléments suivants :

- Un compte Adobe actif ayant accès à [!DNL GenStudio for Performance Marketing].
- Un plan pris en charge qui autorise les connexions MCP à distance lorsque vous utilisez Claude, ChatGPT ou Microsoft Copilot. Reportez-vous à la documentation de l’assistant AI pour obtenir des instructions spécifiques sur la configuration manuelle des connexions MCP.

## Connecter Adobe CX Enterprise Coworker

[!DNL GenStudio for Performance Marketing] outils sont gérés en tant que connexion native dans Adobe CX Enterprise Coworker. Votre organisation contrôle la disponibilité. Vous ne devez donc pas saisir l’URL directe du serveur MCP.

Démarrez une nouvelle conversation et [vérifiez la connexion](#verify-the-connection). Si les outils n’apparaissent pas, contactez l’administrateur ou administratrice de votre organisation ou le représentant ou représentante Adobe.

## Connect Claude

Claude a besoin d&#39;un plan Pro, Max, Équipe ou Entreprise. Le même connecteur distant fonctionne dans Claude sur le web et dans l&#39;application de bureau.

1. Pour Claude, sélectionnez **[!UICONTROL Personnaliser]** dans la barre latérale gauche.
1. Sélectionnez **[!UICONTROL Connecteurs]**, puis sélectionnez l’icône d’ajout.
1. Sélectionnez **[!UICONTROL Ajouter un connecteur personnalisé]**.
1. Saisissez `https://genstudio-services.adobe.io/mcp` comme URL du serveur MCP.
1. Connectez-vous avec votre Adobe ID.
1. Sélectionnez l’organisation IMS ayant accès à [!DNL GenStudio for Performance Marketing].

> [!NOTE]
> Dans une formule Équipe ou Entreprise, un propriétaire d’organisation peut avoir besoin d’ajouter d’abord le connecteur. Si le connecteur est déjà disponible, sélectionnez **[!UICONTROL Se connecter]** à la place.

## Connexion à ChatGPT

ChatGPT nécessite un compte Plus, Pro, Business, Enterprise ou Education. Les connexions MCP personnalisées sont disponibles sur le Web via le mode Développeur.

1. Connectez-vous à [ChatGPT](https://chatgpt.com) dans un navigateur web.
1. Ouvrez **[!UICONTROL Paramètres]**, puis activez **[!UICONTROL mode Développeur]**.
1. Dans **[!UICONTROL Paramètres]**, ouvrez la zone pour les applications ou les connecteurs.
1. Ajoutez une connexion MCP personnalisée nommée `GenStudio`.
1. Saisissez `https://genstudio-services.adobe.io/mcp` comme URL du serveur MCP.
1. Conservez **[!UICONTROL OAuth]** comme méthode d’authentification.
1. Connectez-vous avec votre Adobe ID.
1. Sélectionnez l’organisation IMS ayant accès à [!DNL GenStudio for Performance Marketing].

> [!NOTE]
> ChatGPT peut modifier l&#39;emplacement des paramètres du développeur et du connecteur. Si ces libellés diffèrent dans votre compte, suivez les instructions OpenAI actuelles pour ajouter un connecteur MCP distant.

## Connect Codex

Le Codex requiert l’interface de ligne de commande du Codex et un compte Codex authentifié.

1. Ouvrez `~/.codex/config.toml` pour tous les projets ou `.codex/config.toml` pour un seul projet.
1. Ajoutez la configuration suivante :

   ```toml
   [mcp_servers.genstudio]
   url = "https://genstudio-services.adobe.io/mcp"
   auth = "oauth"
   ```

1. Exécutez `codex mcp login genstudio`.
1. Connectez-vous avec votre Adobe ID dans la fenêtre du navigateur qui s’ouvre.
1. Sélectionnez l’organisation IMS ayant accès à [!DNL GenStudio for Performance Marketing].

## Connect Writer

Writer requiert l’accès à AI Studio.

1. Dans Writer, ouvrez ****.
1. Sélectionnez **[!UICONTROL Connecteurs et outils]**.
1. Sélectionnez **[!UICONTROL Créer un connecteur personnalisé]**.
1. Sélectionnez **[!UICONTROL Serveur MCP]** comme type de connecteur.
1. Saisissez un nom et une description pour le connecteur.
1. Saisissez `https://genstudio-services.adobe.io/mcp` comme URL du serveur MCP.
1. Définissez l’accès de l’équipe au connecteur.
1. Sélectionnez **[!UICONTROL OAuth 2.0 (niveau utilisateur)]** comme méthode d’authentification.
1. Connectez-vous avec votre Adobe ID.
1. Sélectionnez **[!UICONTROL Enregistrer]**.

[!DNL GenStudio for Performance Marketing] outils s’affichent dans la bibliothèque d’outils AI Studio. Chaque utilisateur Writer se connecte avec une Adobe ID individuelle.

## Connecter le copilote Microsoft

Microsoft contrôle le flux de configuration des connexions MCP personnalisées dans Copilot. Suivez la [documentation Microsoft Copilot en cours](https://learn.microsoft.com/en-us/copilot/) pour ajouter un serveur MCP distant, puis utilisez `https://genstudio-services.adobe.io/mcp` comme URL du serveur.

Lorsque vous y êtes invité, connectez-vous avec votre Adobe ID et sélectionnez l’organisation IMS qui a accès à [!DNL GenStudio for Performance Marketing].

## Vérifier la connexion

Après la configuration, vérifiez que les outils sont disponibles.

1. Commencez une nouvelle conversation dans votre assistant d’IA.
1. Demandez à l&#39;assistant quels outils [!DNL GenStudio for Performance Marketing] il peut accéder.
1. Vérifiez que la réponse répertorie les outils dans Insights, Créer et Activer.
1. Demandez un résumé des performances pour un canal média payant connecté.

L’assistant renvoie les données de performances disponibles ou explique pourquoi aucune donnée ne correspond à la requête.

> [!TIP]
> Si l’authentification échoue, reconnectez-vous et confirmez que vous avez sélectionné l’organisation IMS appropriée. Si aucun outil n’apparaît, vérifiez que votre compte a accès à [!DNL GenStudio for Performance Marketing].

## Fonctionnalités connexes

- [Présentation des assistants d’IA](overview.md)
- [Utilisation des assistants d’IA](use-ai-assistants.md)
- [Référence des outils de l’assistant d’IA](tools-reference.md)
