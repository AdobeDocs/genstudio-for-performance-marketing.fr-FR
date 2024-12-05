---
title: Personnalisation d’un modèle
description: Découvrez comment personnaliser et optimiser votre modèle pour Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 088bc6df481fb1e961a7df3c79515642ec39767d
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 0%

---

# Personnalisation d’un modèle

Adaptez vos modèles d’HTML pour Adobe GenStudio for Performance Marketing à l’aide du langage de modèle _Handlebars_. La syntaxe [!DNL Handlebars] utilise du texte normal avec des accolades doubles comme espaces réservés au contenu. Voir [`What is [!DNL Handlebars]?`](https://handlebarsjs.com/guide/#what-is-handlebars) dans le _guide de langue Handlebars_ pour apprendre à préparer votre modèle.

Les sections suivantes expliquent comment ajouter des espaces réservés de contenu, masquer les éléments superflus de l’aperçu et gérer les liens vers du contenu statique. Une fois votre modèle prêt, vous pouvez [le charger vers GenStudio for Performance Marketing](use-templates.md#upload-a-template) et commencer à générer des emails personnalisés basés sur votre modèle personnalisé.

## Espaces réservés de contenu

GenStudio for Performance Marketing reconnaît certains [éléments](use-templates.md#template-elements) dans un modèle, mais seulement si vous les identifiez avec un nom de champ reconnu.

Dans l’en-tête ou le corps d’un modèle, vous pouvez utiliser la syntaxe [!DNL Handlebars] comme espace réservé de contenu dans lequel vous avez besoin de GenStudio for Performance Marketing pour remplir le modèle avec du contenu réel. GenStudio for Performance Marketing reconnaît et interprète les espaces réservés de contenu en fonction du [nom _champ_ reconnu](#recognized-field-names).

Par exemple, vous pouvez utiliser `{{ headline }}` avec la syntaxe [!DNL Handlebars] pour indiquer où le titre de l&#39;email doit être placé :

```handlebars
<div>{{headline}}</div>
```

### Noms de champ reconnus

Le tableau suivant répertorie les noms de champ reconnus par GenStudio for Performance Marketing pour la population dans les modèles. Ajoutez ces noms de champ en utilisant la syntaxe [!DNL Handlebars] à votre modèle pour lequel vous avez besoin de GenStudio for Performance Marketing pour générer du contenu.

| champ | Rôle | Modèle de canal |
| -------------- | ---------------------- | ------------------------------ |
| `pre_header` | En-tête pre | email |
| `headline` | Titre | email <br>Métadonnées |
| `body` | Copie de contenu | email <br>Métadonnées |
| `cta` | Appel à l’action | email <br>Métadonnées |
| `on_image_text` | Sur le texte de l’image | Métadonnées |
| `image` | Image | email <br>Métadonnées |
| `brand_logo` | Logo de la marque sélectionnée <br>Voir [Nom du champ de logo de la marque](#brand-logo-field-name) pour une utilisation recommandée. | email<br>Métadonnées |

GenStudio for Performance Marketing renseigne automatiquement certains champs dans les modèles suivants :

- **Modèle d’email** ne vous oblige pas à identifier le champ `subject`
- **Modèle de métadonnées publicitaires** ne nécessite pas que vous identifiiez les champs `headline`, `body` et `CTA`
- **Le modèle Afficher les publicités** ne nécessite pas que vous identifiiez le champ `CTA`

>[!WARNING]
>
>Pour les annonces Instagram, le titre généré n’apparaît pas dans l’expérience finale.

La limite est de 20 champs lors du téléchargement d’un modèle vers GenStudio for Performance Marketing. Comme le champ `subject` est généré automatiquement dans un email, il est compté comme un champ. Un modèle d&#39;email peut donc contenir 19 champs.

>[!TIP]
>
>Vous pouvez vérifier votre modèle à l’aide de l’ [aperçu de modèle](#template-preview) dans GenStudio for Performance Marketing.

#### Nom du champ du logo de la marque

Actuellement, vous ne pouvez pas sélectionner le logo de la marque pour le téléchargement du modèle. Les exemples suivants montrent deux méthodes qui rendent de manière conditionnelle le logo de la marque. Chaque méthode vérifie la source, fournit une image par défaut ou alternative si le logo de la marque n’est pas disponible et applique un style :

**Exemple 1** : utilisation de la condition [!DNL Handlebars] d’assistance intégrée directement dans l’attribut d’HTML `img src` :

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Exemple 2** : utilisation de l’instruction de condition intégrée [!DNL Handlebars] pour encapsuler la balise d’HTML `img` :

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Noms de champ manuels

Tous les autres noms de champ sont traités comme des champs renseignés manuellement.

Pour créer une section modifiable, ajoutez des crochets doubles autour du nom de la section :

```handlebars
{{customVariable}}
```

### Sections ou groupes

Les _sections_ informent GenStudio for Performance Marketing que les champs de cette section nécessitent un haut degré de cohérence. L’établissement de cette relation permet à l’IA de générer du contenu correspondant aux éléments créatifs de la section .

Utilisez un préfixe de votre choix dans le nom du champ pour indiquer qu’un champ fait partie d’une section ou d’un groupe. Par exemple, vous pouvez mettre en évidence le contenu qui s’affiche dans une zone mise en surbrillance :

- `pod1_headline`
- `pod1_body`

Chaque section ne peut utiliser qu’un seul type de champ. Dans l’exemple ci-dessus, la section `pod1` ne peut utiliser qu’un seul champ `pod1_headline`.

Un modèle peut comporter trois sections au maximum :

- `headline`
- `body`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`

GenStudio for Performance Marketing comprend que `pod1_headline` est plus étroitement lié à `pod1_body` qu’à `pod2_body`.

## Aperçu du modèle

Lorsque vous [ chargez un modèle](use-templates.md#upload-a-template), GenStudio for Performance Marketing recherche les champs reconnus dans le fichier d’HTML. Utilisez l’aperçu pour passer en revue vos [éléments de modèle](use-templates.md#template-elements) et confirmer que vous les avez correctement identifiés avec les [ noms de champ reconnus](#recognized-field-names).

Exemple d&#39;aperçu pour un modèle de courrier électronique :

![Champs d’aperçu détectés](../../assets/template-detected-fields.png){width="650"}

### Aperçu du contrôle

Vous pouvez contrôler la visibilité du contenu spécial à l’aide des assistants intégrés (expressions spéciales dans le langage de modèle [!DNL Handlebars] qui effectuent certaines actions). Par exemple, vous pouvez ajouter une instruction conditionnelle qui ajoute des paramètres de suivi aux liens dans le modèle exporté tout en prévisualisant les liens propres.

La valeur `_genStudio.browser` est définie lors du rendu d’un modèle et la valeur `genStudio.export` est définie lors de l’exportation d’un modèle. Vous pouvez décider d’inclure certains contenus en haut d’un email à l’aide d’un wrapper conditionnel, par exemple, lorsque le modèle est utilisé pour l’exportation :

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un autre exemple peut être d’empêcher l’utilisation des codes de suivi lors de la prévisualisation d’un modèle dans GenStudio for Performance Marketing. L’exemple suivant montre comment ajouter des paramètres de suivi aux liens dans le modèle exporté, tout en conservant les liens d’aperçu propres :

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenu statique

Les modèles de courrier électronique et de métadonnées sont souvent liés à des images et à des fichiers CSS hébergés en dehors de GenStudio for Performance Marketing. Lorsque GenStudio for Performance Marketing génère des miniatures pour ces modèles ou les expériences qui en découlent, il se peut qu’il ignore ces ressources externes si elles ne comportent pas les en-têtes CORS (Cross-Origin Resource Sharing) corrects.

Pour vous assurer que ces ressources sont disponibles pendant le processus de génération de miniatures, envisagez deux options :

1. **Utiliser les en-têtes CORS** : le serveur hôte doit envoyer des réponses avec un en-tête `Access-Control-Allow-Origin` défini sur la valeur `https://experience.adobe.com` pour les environnements de production. Cette méthode permet à GenStudio for Performance Marketing d’accéder aux ressources et de les inclure.

1. **Utiliser des URL de données** : incorporez les ressources externes directement dans le modèle à l’aide des URL de données. Cette méthode contourne les restrictions CORS et garantit que les ressources sont disponibles pendant la génération des miniatures.

## Exemples de modèles

+++Exemple : modèle d&#39;email avec une section

Voici un exemple de base d&#39;un modèle d&#39;HTML pour un email contenant une section. L’en-tête contient une feuille CSS simple et intégrée pour la mise en forme. Le corps contient un `pre-header`, un `headline` et un `image` [espace réservé](#content-placeholders) à utiliser par GenStudio for Performance Marketing pour injecter du contenu pendant le processus de génération de courrier électronique.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Exemple : modèle d&#39;email avec plusieurs sections

L’exemple ci-dessous présente le même modèle d’HTML que celui illustré ci-dessus, mais avec deux sections supplémentaires. L’en-tête contient des CSS intégrés pour le style d’un groupe. Le corps utilise deux groupes avec des [espaces réservés de contenu](#content-placeholders) à l’aide d’un préfixe.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    <!-- Pod1 -->
        <div class="pod">
            <h2>{{ pod1_header }}</h2>
            <p>{{ pod1_body }}</p>
        </div>
        <!-- End of Pod1 -->
    <!-- Pod2 -->
        <div class="pod">
            <h2>{{ pod2_header }}</h2>
            <p>{{ pod2_body }}</p>
        </div>
        <!-- End of Pod2 -->
    </div>
</body>
</html>
```

+++

+++Exemple : modèle de métadonnées publicitaires

Voici un exemple de base d’un modèle de métadonnées publicitaires. L’en-tête contient des CSS intégrés pour la mise en forme. Le corps utilise des [espaces réservés de contenu](#content-placeholders) à l’aide d’un préfixe.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>
</body>
</html>
```

+++
