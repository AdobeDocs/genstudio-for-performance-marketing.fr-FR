---
title: MFE du sélecteur d’expérience GenStudio
description: Découvrez et implémentez le microfront-end du sélecteur d’expérience pour vos applications et modules complémentaires GenStudio.
feature: Extensibility, Extensions, Experiences
source-git-commit: e30e43bd8d226628b425c341d19195f7f860e560
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 6%

---

# MFE du sélecteur d’expérience GenStudio

Le sélecteur d’expérience est un micro front-end (MFE) qui fournit un composant `ExperienceSelectorDialog` pour sélectionner des expériences GenStudio. Utilisez le composant dans votre application en important la fonction `renderExperienceSelectorWithSUSI` à partir du lot JavaScript autonome, qui charge automatiquement le dernier micro front-end déployé et présente une interface de composant naturelle.

Le MFE Sélecteur d’expérience GenStudio permet aux utilisateurs et utilisatrices de :

- Parcourir et sélectionner des expériences GenStudio
- Filtrage des expériences selon divers critères
- Prise en charge des modes de sélection unique et multiple
- Gérer l’authentification via l’intégration SUSI (Sign-In)
- Fournir une interface utilisateur cohérente dans différents frameworks

## Options d’intégration

L’EFM peut être intégrée selon deux approches différentes :

### ESM (modules ES) - Recommandé

```javascript
import { renderExperienceSelectorWithSUSI } from 'https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/esm/standalone.js';
```

### UMD (Universal Module Definition)

```html
<script src="https://experience-stage.adobe.com/solutions/GenStudio-experience-selector-mfe/static-assets/resources/@genstudio/experience-selector/umd/standalone.js"></script>
```

## Propriétés de configuration

La fonction `renderExperienceSelectorWithSUSI` accepte un objet de configuration avec les propriétés suivantes :

| Propriété | Type | Requis | Description |
|----------|------|----------|-------------|
| `apiKey` | chaîne | Oui | Clé API pour les services GenStudio |
| `imsOrg` | chaîne | Oui | Identifiant de l’organisation IMS |
| `env` | chaîne | Oui | Environnement (`stage`, `prod`) |
| `susiConfig` | object | Oui | [Configuration de l’authentification SUSI](#susi-configuration) |
| `onSelectionConfirmed` | fonction | Oui | Rappel lorsque la sélection est confirmée |
| `onDismiss` | fonction | Oui | Rappel lorsque la boîte de dialogue est fermée |
| `locale` | chaîne | Non | Paramètres régionaux de la langue (par exemple, `en-US`) |
| `isOpen` | booléen | Non | État initial de la boîte de dialogue |
| `selectionType` | chaîne | Non | Le mode de sélection (`single` ou `multiple`) |
| `customFilters` | Tableau | Non | Critères de filtre personnalisés |
| `dialogTitle` | chaîne | Non | Titre de la boîte de dialogue personnalisée |

### Configuration SUSI

L’objet `susiConfig` peut inclure :

```javascript
{
  clientId: 'genstudio',
  environment: 'stg1', // or 'prod'
  scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
  locale: 'en_US',
  modalSettings: {
    width: 500,
    height: 700
  }
}
```

## Démarrage rapide

1. **Choisissez votre framework** à partir des exemples disponibles ci-dessous
1. **Accédez au répertoire d’exemple**
1. **Installer des dépendances** (pour les exemples React/Vue)
1. **Mettez à jour la configuration** avec vos clés API et votre organisation IMS :

   ```javascript
   const experienceSelectorProps = {
     locale: 'en-US',
     apiKey: 'exc_app',           
     imsOrg: 'your-ims-org@AdobeOrg',  // Replace with your IMS Org
     env: 'stage', // or 'prod'
     susiConfig: {
        clientId: 'genstudio',
        environment: 'stg1', // or 'prod'
        scope: 'additional_info.projectedProductContext,additional_info.ownerOrg,AdobeID,openid,session,read_organizations,ab.manage',
        locale: 'en_US',
        modalSettings: {
          width: 500,
          height: 700,
        },
     },
     customFilters: ['genstudio-channel:email'],
     selectionType: 'single', // or 'multiple'
     dialogTitle: 'Select Email Templates'
   };
   ```

1. **Exécuter le serveur de développement**

### Exemples d’implémentation

Ce référentiel comprend des exemples de travail pour différents frameworks :

- [Application React **complète** démontrant l’intégration au système de création Vite](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/react-js).

- [Application **Vue 3** avec intégration de l’API Composition](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vue-js).

- [Deux **implémentations de Vanilla JavaScript**](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js) :

   - [Cette version **Vanilla ESM** utilise des modules ES6 et des JavaScript modernes](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-esm).

   - [Cette version **Vanilla UMD** utilise un lot UMD chargé via une balise de script](https://github.com/adobe/genstudio-extensibility-examples/tree/main/genstudio-experience-selector-mfe/vanilla-js/vanilla-umd-global-var).

## Flux d’authentification

Le sélecteur d’expérience gère automatiquement l’authentification via SUSI :

1. Lorsque la boîte de dialogue s’ouvre, elle vérifie l’authentification existante.
1. S’il n’est pas authentifié, il ouvre un flux de connexion SUSI.
1. Une fois l’authentification réussie, le sélecteur d’expérience s’affiche.
1. Les utilisateurs peuvent parcourir et sélectionner des expériences.
1. Les expériences sélectionnées sont renvoyées par le biais du rappel `onSelectionConfirmed`.
