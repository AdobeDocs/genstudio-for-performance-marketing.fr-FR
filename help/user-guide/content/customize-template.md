---
title: Personnaliser un modèle
description: Découvrez comment personnaliser votre modèle HTML à l’aide d’espaces réservés de contenu reconnus par l’IA générative d’Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
source-git-commit: 04bb7adcc9ce7eaeca2ea1f3ef39882f8e43ff6d
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# Personnalisation d’un modèle

Vous pouvez personnaliser un modèle à utiliser dans GenStudio for Performance Marketing en insérant des espaces réservés de contenu, ou des champs, que l’IA générative utilise pour insérer du contenu.

Les sections suivantes expliquent comment adapter vos modèles HTML pour GenStudio for Performance Marketing à l’aide du langage de modèle _[!DNL Handlebars]_. La syntaxe [!DNL Handlebars] utilise du texte normal avec des accolades doubles comme espaces réservés de contenu. Voir [Qu’est-ce que  [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) dans le_ guide du langage Handlebars _pour savoir comment préparer votre modèle.

Une fois votre modèle prêt, vous pouvez [le charger dans GenStudio for Performance Marketing](use-templates.md#upload-a-template) et commencer à générer des e-mails personnalisés en fonction de votre modèle personnalisé.

>[!TIP]
>
>Suivez les [directives d’accessibilité](accessibility-for-templates.md) et [bonnes pratiques](/help/user-guide/content/best-practices-for-templates.md) afin de toucher davantage d’audiences et d’offrir une expérience optimale.

## Espaces réservés de contenu

GenStudio for Performance Marketing reconnaît certains [éléments](use-templates.md#template-elements) dans un modèle, mais uniquement si vous les identifiez avec un [nom de champ reconnu](#recognized-field-names).

Dans l’en-tête ou le corps d’un modèle HTML, vous pouvez utiliser la syntaxe [!DNL Handlebars] pour insérer un espace réservé de contenu dans lequel vous avez besoin que GenStudio for Performance Marketing renseigne le modèle avec du contenu réel. GenStudio for Performance Marketing reconnaît et interprète les espaces réservés de contenu en fonction du [nom _champ_ reconnu](#recognized-field-names).

Par exemple, vous pouvez utiliser `{{headline}}` avec la syntaxe [!DNL Handlebars] pour indiquer où le titre de l’e-mail doit être placé. GenStudio reconnaît ce champ, génère un titre approprié en fonction de vos directives et critères d’invite, et insère le titre à cet emplacement :

```handlebars
<div>{{headline}}</div>
```

### Noms de champs reconnus

Le tableau suivant répertorie les noms de champ reconnus par GenStudio for Performance Marketing pour l’ajout d’un espace réservé dans un modèle. Ajoutez ces noms de champ en utilisant la syntaxe [!DNL Handlebars] à votre modèle dans lequel vous avez besoin de GenStudio for Performance Marketing pour générer un certain type de contenu.

| champ | Rôle | Modèle de canal |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Pré-titre | email |
| `{{headline}}` | Titre | e-mail <br>Méta-annonce <br>bannière et publicité display <br>publicité LinkedIn |
| `{{sub_headline}}` | Sous-Titre | e-mail<br>bannière et publicité display |
| `{{introductory_text}}` | Texte d’introduction | Annonce LinkedIn |
| `{{body}}` | Copie du corps | e-mail <br>Méta-annonce <br>bannière et publicité display |
| `{{cta}}` | Call to action<br>Voir [Appels à l’action](#calls-to-action) | e-mail <br>Méta-annonce <br>bannière et publicité display <br>publicité LinkedIn |
| `{{image}}` | Image : sélection à partir de l&#39;[!DNL Content] | e-mail <br>Méta-annonce <br>bannière et publicité display <br>publicité LinkedIn |
| `{{on_image_text}}` | Dans le texte de l’image<br>voir [Dans le texte de l’image](#on-image-text). | Méta-publicité <br>publicité LinkedIn |
| `{{link}}` | Call to action sur l’image<br>voir [Lien sur l’image](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing génère automatiquement certains champs dans les modèles suivants :

- **Modèle d’e-mail** ne nécessite pas que vous identifiiez le champ `subject`
- **Modèle de méta-annonce** ne nécessite pas que vous identifiiez les champs `headline`, `body` et `CTA`
- **Modèle de bannière et d’affichage publicitaire** ne nécessite pas que vous identifiiez le champ `CTA`
- **Modèle d’annonce LinkedIn** ne nécessite pas que vous identifiiez les champs `headline`, `introductory_text` et `CTA`

>[!WARNING]
>
>Pour les publicités Instagram, le titre généré n’apparaît pas dans l’expérience finale.

Le nombre de champs est limité à 20 lors du chargement d’un modèle vers GenStudio for Performance Marketing. Le champ `subject` étant généré automatiquement dans un e-mail, il est comptabilisé comme un seul champ. Cela signifie que 19 champs sont autorisés dans un modèle d’e-mail.

>[!TIP]
>
>Vous pouvez vérifier votre modèle à l’aide de l’aperçu du [modèle](#template-preview) dans GenStudio for Performance Marketing.

### Appels à l’action

Un Call to action (CTA) comprend une expression et un lien. Pour que les fonctionnalités _[!UICONTROL Reformuler]_ et _[!UICONTROL Ajouter un lien]_ fonctionnent correctement pendant le processus de génération de la variante, vous devez inclure des espaces réservés pour le lien et l’expression dans votre modèle.

Suivez les instructions ci-dessous pour configurer les espaces réservés CTA :

- La rephrase CTA est disponible et le lien est modifiable.

  ```html
  <a class="button" href="{{pod1_link}}" >{{cta}}</a>
  ```

- La rephrase CTA est disponible, mais le lien n’est **modifiable** car le lien réel est fourni dans le modèle

  ```html
  <a align="center" href="https://link">{{cta}}</a>
  ```

- Le lien CTA est modifiable, mais la reformulation n’est **pas** disponible, car l’expression est fournie dans le modèle

  ```html
  <a class="button" href="{{pod1_link}}" >Register now</a>
  ```

GenStudio for Performance Marketing peut également fournir des variantes d’expressions d’appel à l’action. Voir [Révision de l’appel à l’action](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Lien sur l’image

Vous pouvez personnaliser votre modèle d’e-mail pour permettre aux créatifs d’ajouter un lien à une image. Comme pour le lien CTA, suivez les instructions ci-après pour appliquer un espace réservé `link` à une balise d’image :

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

Dans cet exemple :

- `{{link}}` est un espace réservé pour l’URL réelle.
- `src="image-source.jpg"` doit être remplacé par l’URL source de l’image réelle.
- `{{imageDescription}}` est un nom de champ défini par l’utilisateur qui fournit un espace réservé pour le texte secondaire de l’image, ce qui s’avère utile pour l’accessibilité et l’optimisation du moteur de recherche.

### Texte secondaire

Utilisez un nom de champ défini par l’utilisateur comme espace réservé pour générer une description de texte secondaire (attribut HTML `alt="text"`) pour une image. L’espace réservé `{{imageDescription}}` suivant est utilisé avec le champ `{{image}}` dans la même balise `<img>`, en veillant à ce que la relation entre l’image et sa description persiste.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

Dans cet exemple :

- `{{image}}` est l’espace réservé de l’URL source de l’image.
- `{{imageDescription}}` est l’espace réservé du texte secondaire, qui fournit une description de l’image à des fins d’accessibilité et d’optimisation du moteur de recherche (SEO).

### Texte sur l’image

L’espace réservé `{{on_image_text}}` est utilisé pour spécifier une superposition de texte de messages à impact court, placés directement sur l’image dans une expérience.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- this field does not work in Create canvas 2025/03

### Brand logo field name

At this time, you cannot select the brand logo for the template upload. The following examples demonstrate two methods that conditionally render the brand logo. Each method verifies the source, provides a default or alternative image in case the brand logo is not available, and applies a style:

**Example 1**: Using [!DNL Handlebars] Built-in Helpers condition directly in the HTML `img src` attribute:

```html
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default-image>{{/if}}" alt="img alt text" style="max-width: 88px; margin: 10px auto; display: block;">
```

**Example 2**: Using [!DNL Handlebars] Built-in condition statement to wrap the HTML `img` tag:

```html
{{#if brand_logo}}
    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
    {{else}}
    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">
{{/if}}
```

-->

### Noms de champs manuels

Tous les autres noms de champ sont définis par l’utilisateur et traités comme des champs renseignés manuellement. Par exemple, vous pouvez réserver une section au contenu du pied de page.

Pour créer une section modifiable, ajoutez des crochets doubles autour du nom de la section :

```html
<tbody>
    <tr>
        <td>
            <p><span class="footer-text">{{footerLegal}}</span></p>
        </td>
    </tr>
</tbody>
```

## Sections ou groupes

_Sections_ indiquez à GenStudio for Performance Marketing que les champs de cette section nécessitent un haut degré de cohérence. L’établissement de cette relation permet à l’IA de générer du contenu correspondant aux éléments créatifs de la section .

Utilisez un préfixe de votre choix dans le nom du champ pour indiquer qu’un champ fait partie d’une section ou d’un groupe. Utilisez un nom de champ (tel que `headline`, `body`, `image` ou `cta`) après le trait de soulignement (`_`).

- _Correct_ (👍) : `pod1_body`
- _Incorrect_ (❌) : `pod1body`

Chaque section ne peut utiliser qu’un seul de chaque type de champ. Par exemple, les champs suivants appartiennent à la section `pod1` :

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Pour cette raison, les sections ne peuvent pas être imbriquées.

Chaque type de modèle, tel qu’un e-mail ou une méta-annonce, présente des contraintes spécifiques au canal quant à l’utilisation des sections. Consultez les [instructions spécifiques aux canaux](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates#follow-channel-specific-template-guidelines) dans la rubrique _Bonnes pratiques relatives à l’utilisation des modèles_.

Par exemple, un modèle d’e-mail peut inclure jusqu’à trois sections. Par conséquent, vous pouvez avoir trois sections de titre et de corps :


- `pre_header`
- `pod1_headline`
- `pod1_body`
- `pod2_headline`
- `pod2_body`
- `pod3_headline`
- `pod3_body`
- `cta`

GenStudio for Performance Marketing comprend que `pod1_headline` est plus étroitement lié à `pod1_body` qu’à `pod2_body`.

>[!TIP]
>
>Consultez [Invites structurées](/help/user-guide/effective-prompts.md#structured-prompts) pour savoir comment concevoir une invite qui génère un contenu variable pour chaque section dans un e-mail à plusieurs sections.

## Aperçu du modèle

Lorsque vous [téléchargez un modèle](use-templates.md#upload-a-template), GenStudio for Performance Marketing analyse le fichier HTML à la recherche de champs reconnus. Utilisez l’aperçu pour passer en revue vos [éléments de modèle](use-templates.md#template-elements) et confirmer que vous les avez correctement identifiés avec les [noms de champ reconnus](#recognized-field-names).

Exemple de prévisualisation pour un modèle d’e-mail :

![Prévisualisation des champs détectés](/help/assets/template-detected-fields.png "Vérification des champs détectés"){zoomable="yes"}

Voir [Éditeur de code de modèle](/help/user-guide/content/code-editor.md).

### Prévisualisation du contrôle

Vous pouvez contrôler la visibilité du contenu spécial à l’aide des assistants intégrés (expressions spéciales du langage de modèle [!DNL Handlebars] qui effectuent certaines actions). Par exemple, vous pouvez ajouter une instruction conditionnelle qui ajoute des paramètres de suivi aux liens du modèle exporté tout en préservant les liens d’aperçu.

La valeur `_genStudio.browser` est définie lors du rendu d’un modèle et la valeur `genStudio.export` est définie lors de l’exportation d’un modèle. Vous pouvez décider d’inclure certains contenus en haut d’un e-mail à l’aide d’un wrapper conditionnel, par exemple lorsque le modèle est utilisé pour l’exportation :

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un autre exemple peut être d’empêcher l’utilisation des codes de suivi lors de la prévisualisation d’un modèle dans GenStudio for Performance Marketing. L’exemple suivant montre comment ajouter des paramètres de tracking aux liens dans le modèle exporté, tout en préservant les liens d’aperçu :

```html
<a class="button" {{#if _genStudio.browser }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Contenu statique

Les modèles E-mail et Métadonnées sont souvent associés à des images et des fichiers CSS hébergés sur d’autres domaines. Lorsque GenStudio for Performance Marketing génère des miniatures pour les aperçus de modèle ou les expériences qui en sont dérivées, il valide la source de contenu et incorpore une copie à des fins d’aperçu.

Les fichiers externes sont temporairement incorporés uniquement dans le but de créer l’aperçu du modèle, ce qui garantit que l’aperçu reflète précisément le contenu tel qu’il apparaît au moment de la création. Ces fichiers externes ne sont **pas** stockés de manière permanente dans GenStudio for Performance Marketing. Une fois l’aperçu du modèle créé, GenStudio for Performance Marketing continue à référencer le lien source d’origine fourni dans le modèle.

### Actualiser le contenu

Si la source change après la création de l’aperçu initial, utilisez la fonction [refresh](/help/user-guide/content/use-templates.md#refresh-template) pour mettre à jour l’aperçu du modèle avec la version la plus récente du contenu provenant des sources externes.

## Exemples de modèles

+++Exemple : modèle d’e-mail avec une section

Voici un exemple de base de modèle HTML pour un e-mail contenant une section. L’en-tête contient un CSS simple et intégré pour le style. Le corps contient un `pre_header`, un `headline` et `image` [espace réservé](#content-placeholders) que GenStudio for Performance Marketing peut utiliser pour injecter du contenu pendant le processus de génération d’e-mail.

```html {line-numbers="true" highlight="13"}
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p><a href="{{link}}">
            <img alt="{{headline}}"
                    src="{{image}}"
                    width="600" height="600"
                    border="0"/></a></p>
            <p>{{body}}</p>
        </div>
    </body>
</html>
```

+++

+++Exemple : modèle d’e-mail avec plusieurs sections

Vous trouverez ci-dessous le même modèle HTML dans l’exemple ci-dessus, mais avec deux sections supplémentaires. L’en-tête contient un CSS intégré pour la mise en forme d’un groupe. Le corps utilise deux groupes avec des [espaces réservés de contenu](#content-placeholders) utilisant un préfixe.

```html
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
    <body>{{pre_header}}
        <div class="container">
            <h1>{{headline}}</h1>
            <p>{{body}}</p>
            <!-- Pod1 -->
            <div class="pod">
                <h2>{{pod1_headline}}</h2>
                <p><img alt="{{ headline }}" src="{{pod1_image}}" width="200" height="200" border="0"></p>
                <p>{{pod1_body}}</p>
            </div>
            <!-- End of Pod1 -->
            <!-- Pod2 -->
            <div class="pod">
                <h2>{{pod2_headline}}</h2>
                <p><img alt="{{headline}}" src="{{pod2_image}}" width="200" height="200" border="0"></p>
                <p>{{pod2_body}}</p>
            </div>
            <!-- End of Pod2 -->
        </div>
    </body>
</html>
```

+++

+++Exemple : modèle de méta-annonce

Voici un exemple de base de modèle de métadonnées. L’en-tête contient le CSS intégré pour la mise en forme. Le corps utilise des [espaces réservés de contenu](#content-placeholders) tels que `image` et `on_image_text`, pour indiquer où GenStudio for Performance Marketing peut générer du contenu.

```html {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <title>Adobe</title>
        <style>
            .ad-container {
            font-family: Helvetica, sans-serif;
            position: relative;
            text-align: center;
            height: 100%;
            }
            .ad-image {
            width: 100%;
            height: 100%;
            object-fit: cover;
            }
            .ad-text {
            position: absolute;
            top: 0;
            left: 0;
            margin: 1em;
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            padding: 1em;
            font-size: 75px;
            }
        </style>
    </head>
    <body>
        <div class="ad-container">
            <img src="{{image}}" alt="Ad Image" class="ad-image" />
            <div class="ad-text">{{on_image_text}}</div>
        </div>
    </body>
</html>
```

+++
