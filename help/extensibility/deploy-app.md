---
title: Déploiement de l’application App Builder
description: Déployez votre application App Builder, ou module complémentaire, pour GenStudio for Performance Marketing.
feature: Extensibility
exl-id: 51888ab7-7772-4ac8-838d-26db3019e9b0
source-git-commit: 6fef5933421a56cf9f77c19bc198f017ee6c117e
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---

# Déploiement de l’application

L’exécution de votre application fournit un instantané préliminaire de votre comportement de module complémentaire avant son déploiement. Ces informations peuvent faciliter le débogage. Vous pouvez forcer la création et le déploiement d&#39;une application déployée sans la soumettre à nouveau pour approbation.

**Pour exécuter l’application** :

Exécutez l’application dans `https://localhost:9080` :

```bash
aio app run
```

**Pour déployer l’application** :

1. Accédez à l’espace de travail Déploiement . Par exemple, pour accéder à l’espace de travail de production :

   ```bash
   aio app use -w Production
   ```

1. Déployez l’application :

   ```bash
   aio app deploy
   ```

**Pour forcer le redéploiement** :

>[!NOTE]
>
>Le fait de forcer la création et le déploiement remplace votre déploiement existant. Testez d’abord minutieusement votre application dans un environnement de test.

```bash
aio app build --force-build
```

```bash
aio app deploy --force-deploy
```

**Pour créer et déployer simultanément** :

```bash
aio app deploy --force-build --force-deploy
```

**Pour afficher l’application** :

Après le déploiement, vous pouvez afficher l’application dans GenStudio for Performance Marketing en ajoutant un paramètre `query` à l’URL de GenStudio for Performance Marketing :

`https://experience.adobe.com/?ext=https://<my-deployed-add-on>.adobeio-static.net/index.html#/@<ims-org>/genstudio/create`

Si vous êtes satisfait de votre module complémentaire, vous êtes prêt à le distribuer sans le paramètre `query` .

Vous pouvez maintenant [distribuer votre application](distribute-app.md).
