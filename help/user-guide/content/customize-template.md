---
title: Personnaliser un modèle
description: Découvrez comment personnaliser et optimiser votre modèle pour Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Templates, Content
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: e9c398cc81413fc22746d85abd6444c6bd42efe4
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# Personnalisation d’un modèle

Vous pouvez personnaliser un modèle à utiliser dans GenStudio for Performance Marketing en insérant des espaces réservés de contenu, ou des champs, que l’IA générative utilise pour insérer du contenu.

Les sections suivantes expliquent comment adapter vos modèles d’HTML à GenStudio for Performance Marketing à l’aide du langage de modèle _Handlebars_. La syntaxe [!DNL Handlebars] utilise du texte normal avec des accolades doubles comme espaces réservés de contenu. Voir [Qu’est-ce que  [!DNL Handlebars] ?](https://handlebarsjs.com/guide/#what-is-handlebars) dans le guide de langue _Handlebars_ pour savoir comment préparer votre modèle.


Une fois votre modèle prêt, vous pouvez [le charger dans GenStudio for Performance Marketing](use-templates.md#upload-a-template) et commencer à générer des e-mails personnalisés en fonction de votre modèle personnalisé.

>[!TIP]
>
>Suivez les [directives d’accessibilité](accessibility-for-templates.md) et [bonnes pratiques](/help/user-guide/content/best-practices-for-templates.md) afin de toucher davantage d’audiences et d’offrir une expérience optimale.

## Espaces réservés de contenu

GenStudio for Performance Marketing reconnaît certains [éléments](use-templates.md#template-elements) dans un modèle, mais uniquement si vous les identifiez avec un nom de champ reconnu.

Dans l’en-tête ou le corps d’un modèle, vous pouvez utiliser la syntaxe [!DNL Handlebars] comme espace réservé du contenu dans lequel vous avez besoin de GenStudio for Performance Marketing pour remplir le modèle avec du contenu réel. GenStudio for Performance Marketing reconnaît et interprète les espaces réservés de contenu en fonction du [nom _champ_ reconnu](#recognized-field-names).

Par exemple, vous pouvez utiliser `{{ headline }}` avec la syntaxe [!DNL Handlebars] pour indiquer où le titre de l’e-mail doit être placé :

```handlebars
<div>{{headline}}</div>
```

### Noms de champs reconnus

Le tableau suivant répertorie les noms de champ reconnus par GenStudio for Performance Marketing pour le remplissage en modèles. Ajoutez ces noms de champ en utilisant la syntaxe [!DNL Handlebars] à votre modèle dans lequel vous avez besoin de GenStudio for Performance Marketing pour générer du contenu.

| champ | Rôle | Modèle de canal |
| ------------------ | ---------------------- | -------------------------------- |
| `{{pre_header}}` | Pré-en-tête | email |
| `{{headline}}` | Titre | e-mail <br>Méta-annonce <br>Afficher l’annonce |
| `{{body}}` | Copie du corps | e-mail <br>Méta-annonce <br>Afficher l’annonce |
| `{{cta}}` | Appel à l’action | e-mail <br>Méta-annonce <br>Afficher l’annonce |
| `{{on_image_text}}` | Texte sur l’image | Méta-annonce |
| `{{image}}` | Image : sélectionnez à partir du contenu. | e-mail <br>Méta-annonce <br>Afficher l’annonce |
| `{{brand_logo}}` | Logo de la marque sélectionnée <br>voir [nom du champ du logo de la marque](#brand-logo-field-name) pour une utilisation recommandée. | email<br>Meta ad |

GenStudio for Performance Marketing renseigne automatiquement certains champs dans les modèles suivants :

- **Modèle d’e-mail** ne nécessite pas que vous identifiiez le champ `subject`
- **Modèle de métadonnées publicitaires** ne nécessite pas que vous identifiiez les champs `headline`, `body` et `CTA`
- **Modèle Afficher les publicités** ne nécessite pas que vous identifiiez le champ `CTA`

>[!WARNING]
>
>Pour les publicités Instagram, le titre généré n’apparaît pas dans l’expérience finale.

Le nombre de champs est limité à 20 lors du chargement d’un modèle vers GenStudio for Performance Marketing. Le champ `subject` étant généré automatiquement dans un e-mail, il est comptabilisé comme un seul champ. Cela signifie que 19 champs sont autorisés dans un modèle d’e-mail.

>[!TIP]
>
>Vous pouvez vérifier votre modèle à l’aide de l’aperçu du [modèle](#template-preview) dans GenStudio for Performance Marketing.

#### Nom du champ du logo de la marque

Actuellement, vous ne pouvez pas sélectionner le logo de la marque pour le chargement du modèle. Les exemples suivants présentent deux méthodes qui effectuent le rendu conditionnel du logo de la marque. Chaque méthode vérifie la source, fournit une image par défaut ou alternative au cas où le logo de la marque ne serait pas disponible, et applique un style :

**Exemple 1** : utilisation de [!DNL Handlebars] condition d’assistance intégrée directement dans l’attribut de `img src` d’HTML :

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Exemple 2** : utilisation de [!DNL Handlebars]’instruction de condition intégrée pour encapsuler la balise de `img` d’HTML :

```handlebars
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

#### Noms de champs manuels

Tous les autres noms de champ sont traités comme des champs remplis manuellement.

Pour créer une section modifiable, ajoutez des crochets doubles autour du nom de la section :

```handlebars
{{customVariable}}
```

### Sections ou groupes

_Sections_ indiquez à GenStudio for Performance Marketing que les champs de cette section nécessitent un haut degré de cohérence. L’établissement de cette relation permet à l’IA de générer du contenu correspondant aux éléments créatifs de la section .

Utilisez un préfixe de votre choix dans le nom du champ pour indiquer qu’un champ fait partie d’une section ou d’un groupe. Utilisez un nom de champ (`headline`, `body`, `image` ou `cta`) après le trait de soulignement (`_`). Par exemple, le titre et le corps suivants appartiennent à la section `pod1` :

- `pod1_headline`
- `pod1_body`

Chaque section ne peut utiliser qu’un seul de chaque type de champ. Dans l’exemple ci-dessus, la section `pod1` ne peut utiliser qu’un seul champ de `pod1_headline`. Pour cette raison, les sections ne peuvent pas être imbriquées.

Un modèle d’e-mail peut inclure jusqu’à trois sections. Par exemple, la liste suivante comporte trois sections de titre et de corps :

- `pre-header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing comprend que `pod1_headline` est plus étroitement lié à `pod1_body` qu’à `pod2_body`.

Consultez [Invites structurées](/help/user-guide/effective-prompts.md#structured-prompts) pour savoir comment concevoir une invite qui génère un contenu variable pour chaque section d’un e-mail.

## Aperçu du modèle

Lorsque vous [téléchargez un modèle](use-templates.md#upload-a-template), GenStudio for Performance Marketing recherche les champs reconnus dans le fichier d’HTML. Utilisez l’aperçu pour passer en revue vos [éléments de modèle](use-templates.md#template-elements) et confirmer que vous les avez correctement identifiés avec les [noms de champ reconnus](#recognized-field-names).

Exemple de prévisualisation pour un modèle d’e-mail :

![Champs de prévisualisation détectés](/help/assets/template-detected-fields.png){width="650"}

### Prévisualisation du contrôle

Vous pouvez contrôler la visibilité du contenu spécial à l’aide des assistants intégrés (expressions spéciales du langage de modèle [!DNL Handlebars] qui effectuent certaines actions). Par exemple, vous pouvez ajouter une instruction conditionnelle qui ajoute des paramètres de suivi aux liens du modèle exporté tout en préservant les liens d’aperçu.

La valeur `_genStudio.browser` est définie lors du rendu d’un modèle et la valeur `genStudio.export` est définie lors de l’exportation d’un modèle. Vous pouvez décider d’inclure certains contenus en haut d’un e-mail à l’aide d’un wrapper conditionnel, par exemple lorsque le modèle est utilisé pour l’exportation :

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un autre exemple peut être d’empêcher l’utilisation des codes de suivi lors de la prévisualisation d’un modèle dans GenStudio for Performance Marketing. L’exemple suivant montre comment ajouter des paramètres de tracking aux liens dans le modèle exporté, tout en préservant les liens d’aperçu :

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Contenu statique

Les modèles E-mail et Métadonnées sont souvent associés à des images et des fichiers CSS hébergés en dehors de GenStudio for Performance Marketing. Lorsque GenStudio for Performance Marketing génère des miniatures pour ces modèles ou les expériences qui en sont dérivées, il est possible qu’il ignore ces ressources externes si elles ne disposent pas des en-têtes CORS (Cross-Origin Resource Sharing) appropriés.

Pour vous assurer que ces ressources sont disponibles pendant le processus de génération de miniatures, considérez deux options :

1. **Utiliser des en-têtes CORS** : le serveur hôte doit envoyer des réponses avec un en-tête `Access-Control-Allow-Origin` défini sur `https://experience.adobe.com` valeur pour les environnements de production. Cette méthode permet à GenStudio for Performance Marketing d’accéder aux ressources et de les inclure.

1. **Utiliser des URL de données** : incorporez les ressources externes directement dans le modèle à l’aide des URL de données. Cette méthode contourne les restrictions CORS et garantit que les ressources sont disponibles pendant la génération des miniatures.

>[!TIP]
>
>Utilisez [actualiser](/help/user-guide/content/use-templates.md#refresh-template) pour mettre à jour l’aperçu du modèle avec le contenu statique le plus récent.

## Exemples de modèles

+++Exemple : modèle d’e-mail avec une section

Voici un exemple de base de modèle d’HTML pour un e-mail contenant une section. L’en-tête contient un CSS simple et intégré pour le style. Le corps contient un `pre-header`, un `headline` et `image` [espace réservé](#content-placeholders) que GenStudio for Performance Marketing peut utiliser pour injecter du contenu pendant le processus de génération d’e-mail.

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

+++Exemple : modèle d’e-mail avec plusieurs sections

Vous trouverez ci-dessous le même modèle d’HTML dans l’exemple ci-dessus, mais avec deux sections supplémentaires. L’en-tête contient un CSS intégré pour la mise en forme d’un groupe. Le corps utilise deux groupes avec des [espaces réservés de contenu](#content-placeholders) utilisant un préfixe.

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

+++Exemple : modèle de méta-annonce

Voici un exemple de base de modèle de métadonnées. L’en-tête contient le CSS intégré pour la mise en forme. Le corps utilise des [espaces réservés de contenu](#content-placeholders) précédés d’un préfixe.

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
