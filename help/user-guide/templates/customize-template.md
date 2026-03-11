---
title: Personnaliser un modèle
description: Découvrez comment personnaliser votre modèle HTML à l’aide d’espaces réservés de contenu reconnus par l’IA générative d’Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation, Generative AI
exl-id: 292c1689-1b12-405d-951e-14ee6aebc75a
TQID: https://experienceleague.adobe.com/6gHxPvfz-30X3w2MYIc2Aj5SiGZokzOqSvOHYTQ-u7I
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: e8e0898054576454bad9ecdbd1a48b17f955e138
workflow-type: tm+mt
source-wordcount: 1646
ht-degree: 0%

---

# Personnalisation d’un modèle

Vous pouvez personnaliser un modèle à utiliser dans GenStudio for Performance Marketing en insérant des espaces réservés de contenu, ou des champs, que l’IA générative utilise pour insérer du contenu.

Les sections suivantes expliquent comment adapter vos modèles HTML pour GenStudio for Performance Marketing à l’aide du langage de modèle _[!DNL Handlebars]_. La syntaxe [!DNL Handlebars] utilise du texte normal avec des accolades doubles comme espaces réservés de contenu. Voir [Qu’est-ce que  [!DNL Handlebars]](https://handlebarsjs.com/guide/#what-is-handlebars) dans le_ guide du langage Handlebars _pour savoir comment préparer votre modèle.

Une fois votre modèle prêt, vous pouvez [le charger dans GenStudio for Performance Marketing](use-templates.md#upload-a-template) et commencer à générer des e-mails personnalisés en fonction de votre modèle personnalisé.

Suivez les [directives d’accessibilité](accessibility-for-templates.md) et [bonnes pratiques](/help/user-guide/templates/best-practices-for-templates.md) afin de toucher davantage d’audiences et d’offrir une expérience optimale.

## Espaces réservés de contenu

>[!TIP]
>
>Les espaces réservés de contenu sont **différents** texte d’espace réservé dans le contenu destiné à être rempli ultérieurement par un utilisateur. En savoir plus sur l’[utilisation de texte d’espace réservé dans les modèles](/help/user-guide/templates/best-practices-for-templates.md#using-placeholder-text-in-templates).

GenStudio for Performance Marketing reconnaît certains types de contenu ou [éléments](use-templates.md#template-elements) dans un modèle, mais uniquement si vous les identifiez avec un [nom de champ reconnu](#recognized-field-names).

Dans l’en-tête ou le corps d’un modèle HTML, vous pouvez utiliser la syntaxe [!DNL Handlebars] pour insérer un espace réservé de contenu dans lequel vous avez besoin que GenStudio for Performance Marketing renseigne le modèle avec du contenu réel. GenStudio for Performance Marketing reconnaît et interprète ces espaces réservés en fonction du [nom _champ_ reconnu](#recognized-field-names). Chaque nom de champ est associé à des règles et comportements spécifiques qui déterminent la manière dont le contenu est généré et inséré dans votre modèle.

Par exemple, vous pouvez utiliser `{{headline}}` avec la syntaxe [!DNL Handlebars] pour indiquer où le titre de l’e-mail doit être placé. GenStudio reconnaît ce champ, génère un titre approprié en fonction de vos directives et critères d’invite, et insère le titre à cet emplacement :

```handlebars
<div>{{headline}}</div>
```

### Noms de champs reconnus

Le tableau suivant répertorie les noms de champ reconnus par GenStudio for Performance Marketing pour l’ajout d’un espace réservé dans un modèle. Chaque champ suit des instructions de canal spécifiques, des instructions LLM et des règles basées sur les rôles. Ajoutez ces noms de champ en utilisant la syntaxe [!DNL Handlebars] à votre modèle dans lequel vous avez besoin de GenStudio for Performance Marketing pour générer un certain type de contenu.

| champ | Rôle | Modèle de canal |
| ----------------------- | ------------------------- | ------------------------------------------------ |
| `{{pre_header}}` | Pré-titre | email |
| `{{headline}}` | Titre | e-mail <br>Annonce Meta <br>bannière et publicité display <br>annonce LinkedIn |
| `{{sub_headline}}` | Sous-Titre | e-mail<br>bannière et publicité display |
| `{{introductory_text}}` | Texte d’introduction | Annonce LinkedIn |
| `{{body}}` | Copie du corps | e-mail <br>Annonce Meta <br>bannière et publicité display |
| `{{cta}}` | Call to action<br>Voir [Appels à l’action](#calls-to-action) | e-mail <br>Annonce Meta <br>bannière et publicité display <br>annonce LinkedIn |
| `{{image}}` | Image : sélection à partir de l&#39;[!DNL Content] | e-mail <br>Annonce Meta <br>bannière et publicité display <br>annonce LinkedIn |
| `{{on_image_text}}` | Dans le texte de l’image<br>voir [Dans le texte de l’image](#on-image-text). | Annonce Meta <br>Annonce LinkedIn |
| `{{link}}` | Call to action sur l’image<br>voir [Lien sur l’image](#link-on-image). | email |

<!-- | `{{brand_logo}}`        | Logo of selected brand<br>See [Brand logo field name](#brand-logo-field-name). | email<br>Meta ad <br>LinkedIn ad | -->

GenStudio for Performance Marketing génère automatiquement certains champs dans les modèles suivants :

- **Modèle d’e-mail** ne nécessite pas que vous identifiiez le champ `subject`
- **Le modèle de publicité Meta** ne nécessite pas que vous identifiiez les champs `headline`, `body` et `CTA`
- **Modèle de bannière et d’annonce publicitaire d’affichage** ne nécessite pas que vous identifiiez le champ `CTA`
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

GenStudio for Performance Marketing peut également fournir des variantes d’expressions d’appel à l’action. Voir [Révision de Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action).

### Lien sur l’image

Vous pouvez personnaliser votre modèle d’e-mail pour permettre aux créatifs d’ajouter un lien à une image. Comme pour le lien CTA, suivez les instructions ci-après pour appliquer un espace réservé `link` à une balise d’image :

```html
<a href="{{link}}"><img src="image-source.jpg" alt="{{imageDescription}}"></a>
```

Dans cet exemple :

- `{{link}}` est un espace réservé pour l’URL réelle.
- `src="image-source.jpg"` doit être remplacé par l’URL source de l’image réelle.
- `{{imageDescription}}` est un nom de champ défini par l’utilisateur qui fournit un espace réservé pour le texte secondaire de l’image, ce qui s’avère utile pour l’accessibilité et l’optimisation du moteur de recherche.

### Texte secondaire

Utilisez un nom de champ défini par l’utilisateur comme espace réservé pour générer une description de texte secondaire (attribut HTML `alt="text"`) pour une image. L’espace réservé `{{imageDescription}}` suivant est utilisé avec le champ `{{image}}` dans la même balise `<img>`, en veillant à ce que la relation entre l’image et sa description persiste.

```html
<img src="{{image}}" alt="{{imageDescription}}">
```

Dans cet exemple :

- `{{image}}` est l’espace réservé de l’URL source de l’image.
- `{{imageDescription}}` est l’espace réservé du texte secondaire, qui fournit une description de l’image à des fins d’accessibilité et d’optimisation du moteur de recherche (SEO).

### Libellé d’accessibilité

L’attribut `aria-label` est utilisé pour définir un nom accessible pour les éléments qui n’ont pas de libellés visibles. Cet attribut est particulièrement utile dans les modèles où il est important de fournir un contexte pour les éléments interactifs, tels qu’un bouton CTA.

```html
<a class="button" href="{{link}}" aria-label="{{CTAAriaLabel}}">{{cta}}</a>
```

### Texte sur l’image

L’espace réservé `{{on_image_text}}` est utilisé pour spécifier une superposition de texte de messages à impact court, placés directement sur l’image dans une expérience.

```html
<div class="image-text">{{on_image_text}}</div>
```

<!-- 
this field does not work in Create canvas 2025/03

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

### Modification de texte enrichi

Améliorez votre contenu créatif pendant le processus de [!DNL Create] avec la modification de texte enrichi. La zone de travail détermine la fonctionnalité de texte enrichi en fonction de l’emplacement de l’espace réservé de contenu. La fonctionnalité de texte enrichi est disponible uniquement lorsque vous utilisez des espaces réservés de contenu en tant qu’éléments autonomes ou dans des balises HTML au niveau du bloc, telles que `<p>`, `<div>` ou `<span>`.

La modification de texte enrichi est disponible pour le contenu autonome d’un paragraphe :

```html
<p>{{body}}</p>
```

Si vous utilisez un espace réservé de contenu dans un attribut HTML (tel que `alt`, `href` ou `src`), la modification de texte enrichi n’est pas prise en charge pour ce champ.

La modification de texte enrichi n’est **pas** disponible pour le contenu `alt` :

```html
<img src="image.jpg" alt="{{image_description}}">
```

Si un champ apparaît plusieurs fois, la fonctionnalité de texte enrichi est déterminée en fonction de son utilisation ou non comme attribut HTML dans l’une des instances. Par exemple, lorsque le titre est utilisé comme titre et comme texte secondaire pour une image, la balise `alt` est prioritaire.

La modification de texte enrichi n’est **pas** disponible pour les `headline`, car elle est utilisée comme contenu `alt` :

```html
<h1>{{headline}}</h1>
<img src="image.jpg" alt="{{headline}}">
```

L’édition de texte enrichi peut être disponible pour certains champs dans des canaux spécifiques, tels que les `on_image_text` dans les canaux sociaux (Meta, LinkedIn).

## Sections ou groupes

Si votre modèle d’e-mail nécessite plusieurs zones de contenu, telles que plusieurs offres ou histoires, vous pouvez les organiser à l’aide de sections ou de groupes. _Sections_ informez GenStudio for Performance Marketing que les champs de cette section nécessitent un haut degré de cohérence. L’établissement de cette relation permet à l’IA de générer du contenu correspondant aux éléments créatifs de la section .

Utilisez le nom d’un groupe de votre choix comme préfixe pour indiquer qu’un champ fait partie d’une section ou d’un groupe. Utilisez un nom de champ (tel que `headline`, `body`, `image` ou `cta`) après le trait de soulignement (`_`).

Syntaxe : `groupname_fieldname`

- _Correct_ (👍) : `pod1_body`
- _Incorrect_ (❌) : `pod1body`

Chaque section ne peut utiliser qu’un seul de chaque type de champ. Par exemple, les champs suivants appartiennent à la section `pod1` :

- `pod1_headline`
- `pod1_body`
- `pod1_image`
- `pod1_cta`

Pour cette raison, les sections ne peuvent pas être imbriquées.

Chaque type de modèle, tel qu’une publicité par e-mail ou Meta, présente des contraintes spécifiques au canal quant à l’utilisation des sections. Consultez les [instructions spécifiques aux canaux](/help/user-guide/templates/best-practices-for-templates.md) dans la rubrique _Bonnes pratiques relatives à l’utilisation des modèles_.

Par exemple, un modèle d’e-mail peut inclure jusqu’à trois sections. Par conséquent, vous pouvez avoir trois sections de titre et de corps :

- `pre_header`
- `pod1_headline`, `pod1_body`
- `pod2_headline`, `pod2_body`
- `pod3_headline`, `pod3_body`
- `cta`

GenStudio for Performance Marketing comprend que `pod1_headline` est plus étroitement lié à `pod1_body` qu’à `pod2_body`.

>[!TIP]
>
>Consultez [Invites structurées](/help/user-guide/effective-prompts.md#structured-prompts) pour savoir comment concevoir une invite qui génère un contenu variable pour chaque section dans un e-mail à plusieurs sections.

## Aperçu du modèle

Lorsque vous [téléchargez un modèle](use-templates.md#upload-a-template), GenStudio for Performance Marketing analyse le fichier HTML à la recherche de champs reconnus. Utilisez l’aperçu pour passer en revue vos [éléments de modèle](use-templates.md#template-elements) et confirmer que vous les avez correctement identifiés avec les [noms de champ reconnus](#recognized-field-names).

Exemple de prévisualisation pour un modèle d’e-mail :

![Prévisualisation des champs détectés](/help/assets/template-detected-fields.png "Vérification des champs détectés"){zoomable="yes"}

Voir [Éditeur de code de modèle](/help/user-guide/templates/code-editor.md).

### Prévisualisation du contrôle

Vous pouvez contrôler la visibilité du contenu spécial à l’aide des assistants intégrés (expressions spéciales du langage de modèle [!DNL Handlebars] qui effectuent certaines actions). Par exemple, vous pouvez ajouter une instruction conditionnelle qui ajoute des paramètres de suivi aux liens du modèle exporté tout en préservant les liens d’aperçu.

La valeur `_genStudio.canvas` est définie lors du rendu d’un modèle et la valeur `genStudio.export` est définie lors de l’exportation d’un modèle. Vous pouvez décider d’inclure certains contenus en haut d’un e-mail à l’aide d’un wrapper conditionnel, par exemple lorsque le modèle est utilisé pour l’exportation :

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Un autre exemple peut être d’empêcher l’utilisation des codes de suivi lors de la prévisualisation d’un modèle dans GenStudio for Performance Marketing. L’exemple suivant montre comment ajouter des paramètres de tracking aux liens dans le modèle exporté, tout en préservant les liens d’aperçu :

```html
<a class="button" {{#if _genStudio.canvas }}
   href="{{link}}"{{/if}}{{#if _genStudio.export }}
   href="{{link}}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{cta}}</a>
```

## Contenu statique

Les modèles d’e-mail et de Meta sont souvent associés à des images et des fichiers CSS hébergés sur d’autres domaines. Lorsque GenStudio for Performance Marketing génère des miniatures pour les aperçus de modèle ou les expériences qui en sont dérivées, il valide la source de contenu et incorpore une copie à des fins d’aperçu.

Les fichiers externes sont temporairement incorporés uniquement dans le but de créer l’aperçu du modèle, ce qui garantit que l’aperçu reflète précisément le contenu tel qu’il apparaît au moment de la création. Ces fichiers externes ne sont **pas** stockés de manière permanente dans GenStudio for Performance Marketing. Une fois l’aperçu du modèle créé, GenStudio for Performance Marketing continue à référencer le lien source d’origine fourni dans le modèle.

### Actualiser le contenu

Si la source change après la création de l’aperçu initial, utilisez la fonction [refresh](/help/user-guide/templates/use-templates.md#refresh-template) pour mettre à jour l’aperçu du modèle avec la version la plus récente du contenu provenant des sources externes.
