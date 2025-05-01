---
title: Création d’une application App Builder pour étendre GenStudio for Performance Marketing
description: Commencez à créer une application ou un module complémentaire.
feature: Extensibility
exl-id: 4e757dd4-a02d-472c-bc13-6f27dffa48f2
source-git-commit: 89b7f477310326755a6b34cb97d5ad5664e98dec
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Développement d’une application App Builder

Les développeurs qui étendent les fonctionnalités natives de GenStudio for Performance Marketing utilisent [Adobe App Builder](https://developer.adobe.com/app-builder/) pour créer, envoyer et déployer leurs applications extensibles, ou modules complémentaires.

>[!BEGINSHADEBOX]

**Conditions préalables** :

* Node.js (version 20.x ou ultérieure)

* npm (package avec Node.js)

* Interface de ligne de commande (CLI) Adobe Developer. A installer : `npm install -g @adobe/aio-cli`

>[!ENDSHADEBOX]

## Structure de l’application

Les modules complémentaires GenStudio for Performance Marketing sont des applications App Builder et contiennent les mêmes composants de base que les autres applications App Builder.

### Fichiers de build et de configuration

Les composants principaux des applications App Builder incluent ces fichiers de build et de configuration. Cette liste ne comprend pas tous les fichiers de version et de configuration.

* `README.md` : contient des informations générales sur l’application.

* Fichiers d’application TS :

   * `package.json`
   * `package-lock.json`
   * `eslint`
   * `tsconfig`
   * `jest test up`

* Fichiers de configuration App Builder :

   * `app.config.yaml`
   * `ext.config.yaml` : fichier de configuration pour le module complémentaire
   * `app.config.yaml` : fichier de configuration pour le module complémentaire (y compris la définition de votre application en tant que module complémentaire GenStudio for Performance Marketing)
   * `.aio`
   * `.env` : ne pas valider le fichier `.env` dans le contrôle de code source

### code Source

```
- src/
    - genstudiopem/
        - web-src/
            - src/
                - components/
                - utils/
                - Constants.ts
                - index.tsx
                - index.css
                - utils.ts
        - index.html
```

### Composants de code Source

* `ExtensionRegistration.tsx` : définit les API nécessaires dont l’application hôte (GenStudio for Performance Marketing) a besoin pour charger et afficher le module complémentaire.

* `App.tsx` : composant d’application principal qui définit le routage vers d’autres composants.

* `AdditionalContextDialog.tsx` : composant de boîte de dialogue pour afficher des modules complémentaires contextuels supplémentaires.

* `RightPanel.tsx` : composant de boîte de dialogue pour un module complémentaire de validation.

* Composants `Helper` : inclut les `ClaimsChecker`.

## Création d’une application App Builder à partir d’une application existante

Vous pouvez utiliser un exemple d’application pour démarrer rapidement la création de votre module complémentaire.

**Pour créer une application App Builder à partir d’une application existante** :

1. Téléchargez un exemple d’application à partir du référentiel [Exemples UIX de GenStudio](https://github.com/adobe/genstudio-uix-examples).

1. Dans l’espace de travail Projet App Builder sur [Adobe Developer Console](https://developer.adobe.com/console/), sélectionnez **[!UICONTROL Tout télécharger]** pour télécharger les détails du projet.

1. Ouvrez votre exemple d’application localement dans l’environnement de développement intégré (IDE) de votre choix.

1. Authentifiez-vous avec l’interface de ligne de commande Adobe Developer :

   ```bash
   aio login
   ```

1. Téléchargez votre fichier JSON, puis créez votre application :

   ```bash
   aio app use '/path/to/your/downloaded/app-builder/project/details/config.json'
   ```

## Ajout de code personnalisé à votre module complémentaire

Vous définissez le code du module complémentaire dans les fichiers `AdditionalContextDialog.tsx` et `RightPanel.tsx`. Ces deux fichiers définissent l’aspect et le comportement des fenêtres contextuelles lorsque les utilisateurs accèdent au module complémentaire.

* `AdditionalContextDialog.tsx` : définissez ce composant si vous prévoyez d’utiliser le module complémentaire _Ajouter du contexte_. Les utilisateurs interagissent avec ce composant lorsqu’ils cliquent sur _Modules complémentaires_ dans le tiroir d’invite de [!DNL Create].

* `RightPanel.tsx` : définissez ce composant si vous prévoyez d’utiliser le module complémentaire _Panneau de droite_ (validation de l’expérience). Les utilisateurs interagissent avec ce composant lorsqu’ils cliquent sur le module complémentaire de validation dans le panneau de droite d’un brouillon d’expérience [!DNL Create].

Vous êtes maintenant prêt à [déployer votre application](deploy-app.md)

## Bonnes pratiques de développement d’applications

La maintenance de votre environnement de développement peut vous aider à éviter les erreurs de développement et de déploiement d’applications :

* Si vous utilisez une ancienne version d’un exemple d’application, mettez à niveau les dépendances en les réinstallant :

  ```bash
  rm -rf node_modules package-lock.json && npm i
  ```

* Mettez à niveau le SDK UIX de GenStudio. Vérifiez que vous utilisez la version la plus récente de [GenStudio UIX SDK](https://github.com/adobe/genstudio-uix-sdk). Reportez-vous au [Référentiel d’exemples de l’UIX de GenStudio](https://github.com/adobe/genstudio-uix-examples) pour savoir comment utiliser les modifications SDK les plus récentes.
