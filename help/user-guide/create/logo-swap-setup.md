---
title: Configurer la permutation de logo dans les modèles
description: Configurez les espaces réservés au logo de la marque dans les modèles pour permettre le remplacement du logo [!DNL GenStudio for Performance Marketing].
feature: Create Canvas
role: User
level: Intermediate
source-git-commit: 98cb7ba338878495e6d7b68f3b8c620abae10127
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 2%

---

# Configurer la permutation de logo dans les modèles

Ce guide explique comment configurer des espaces réservés de logo de marque dans vos modèles afin d’activer la fonctionnalité [remplacement de logo](/help/user-guide/create/logo-swap.md) dans [!DNL GenStudio for Performance Marketing]. Appliquez ces instructions pour vous assurer que l’espace réservé s’affiche correctement dans différentes tailles d’image et proportions.

## Configuration rapide

Utilisez le code de modèle de base suivant pour votre image de logo :

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="my-logo"
>
```

Obligatoire :

- `src="{{brand_logo}}"` : active la fonctionnalité de permutation de logo.
- `style="{{defaultLogo}}"` : applique le style de bordure de l&#39;espace réservé.

Facultatif :

- `class="my-logo"` : classe CSS personnalisée pour le dimensionnement et le style.

## Comprendre la bordure de l’espace réservé

Si aucun logo n’est sélectionné, `{{brand_logo}}` contient une image transparente de 1×1 pixel. Le style `{{defaultLogo}}` applique automatiquement un contour pour que l’espace réservé soit visible :

```css
outline: clamp(1px, 0.1em, 5px) dashed #FFF;
```

Comportement de la bordure :

- S’affiche lorsque l’espace réservé par défaut est affiché.
- Disparaît automatiquement après le remplacement d&#39;un logo.
- Mise à l’échelle en fonction de la taille de la police parente.

### Dimensionnement de la bordure

La fonction `clamp()` adapte l&#39;épaisseur du contour à la taille du modèle :

| Taille de police du parent | Taille de la composition |
| --- | --- |
| 10px | 1 px (min) |
| 16px | 1.6px |
| 24px | 2.4px |
| 32px | 3.2px |
| 50px+ | 5 px (max.) |

Formule : `0.1em` est égal à 10 % de la taille de police héritée, comprise entre `1px` et `5px`.

## Personnalisation de la bordure de l’espace réservé

Vous pouvez remplacer la composition par défaut à l’aide de classes CSS. Le style `{{defaultLogo}}` applique le contour de base et votre classe peut personnaliser la couleur, la largeur et le style.

HTML modèle :

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-custom-border"
>
```

Modèle CSS :

```css
.logo-custom-border {
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: dotted !important;
}
```

>[!NOTE]
>Les styles de contour personnalisés n’affectent que l’espace réservé. Une fois qu’un logo est permuté, tous les styles de contour sont automatiquement supprimés.

## Définir le dimensionnement recommandé du logo

Pour vous assurer que l’espace réservé est visible et empêche les changements de disposition, définissez un dimensionnement explicite dans votre classe CSS :

HTML modèle :

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-standard"
>
```

Modèle CSS :

```css
.logo-standard {
  width: 120px;
  height: 60px;
}
```

## Contrôle du positionnement du logo

Utilisez `object-fit` et `object-position` pour contrôler la mise à l’échelle du logo dans son conteneur.

### Logo centré (le plus souvent)

Le logo s’adapte à une taille de 150×80 pixels, centré horizontalement et verticalement.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-centered"
>
```

```css
.logo-centered {
  width: 150px;
  height: 80px;
  object-fit: contain;
  object-position: center center;
}
```

### Logo aligné à gauche

Le logo est dimensionné pour s’adapter, aligné sur le bord gauche et centré verticalement.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-left"
>
```

```css
.logo-left {
  width: 200px;
  height: 60px;
  object-fit: contain;
  object-position: left center;
}
```

### Logo dans le coin supérieur droit

Le logo s’adapte à vos besoins, positionné dans le coin supérieur droit.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-top-right"
>
```

```css
.logo-top-right {
  width: 100px;
  height: 100px;
  object-fit: contain;
  object-position: right top;
}
```

## Exemples complets

### Configuration minimale

```html
<img src="{{brand_logo}}" style="{{defaultLogo}}">
```

>[!NOTE]
>Cette configuration fonctionne, mais l’espace réservé peut être presque invisible, car l’image transparente de 1×1 pixel retombe à sa taille naturelle. Utilisez une classe CSS avec `width` et `height` pour un espace réservé visible.

### Configuration recommandée

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="brand-logo"
>
```

```css
.brand-logo {
  width: 120px;
  height: 60px;
  object-fit: contain;
  object-position: center center;
}
```

### Configuration avancée avec une bordure personnalisée

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="sponsor-logo"
>
```

```css
.sponsor-logo {
  width: 180px;
  height: 90px;
  object-fit: contain;
  object-position: left center;
  outline-color: #0066CC !important;
  outline-width: 2px !important;
  outline-style: solid !important;
}
```

### Configuration flexible avec des limites de taille

Utilisez les propriétés `min-*` et `max-*` pour les modèles réactifs ou des tailles de logo variables.

```html
<img
  src="{{brand_logo}}"
  style="{{defaultLogo}}"
  class="logo-flexible"
>
```

```css
.logo-flexible {
  min-width: 20px;
  min-height: 20px;
  max-width: 200px;
  max-height: 100px;
  object-fit: contain;
  object-position: center center;
}
```

Fonctionnement :

- `min-width` et `min-height` l’espace réservé visible.
- `max-width` et `max-height` empêchent les logos surdimensionnés de rompre la mise en page.
- Le logo se met à l’échelle proportionnellement à l’intérieur de ces limites.

## Référence des propriétés CSS

| Catégorie | Propriété | Valeur | Objectif |
| --- | --- | --- | --- |
| Obligatoire (HTML) | `src` | `{{brand_logo}}` | Active la fonctionnalité de permutation de logo. |
| Obligatoire (HTML) | `style` | `{{defaultLogo}}` | Applique le contour de l’espace réservé. |
| Recommandé (classe CSS) | `width` | `120px` | Définit la largeur maximale du logo. |
| Recommandé (classe CSS) | `height` | `60px` | Définit la hauteur maximale du logo. |
| Recommandé (classe CSS) | `object-fit` | `contain` | Met le logo à l’échelle sans le recadrer. |
| Recommandé (classe CSS) | `object-position` | `center center` | Contrôle l’alignement du logo. |
| Facultatif (classe CSS) | `outline-color` | `#FF0000` | Modifie la couleur du contour. |
| Facultatif (classe CSS) | `outline-width` | `3px` | Modifie l’épaisseur du contour. |
| Facultatif (classe CSS) | `outline-style` | `solid` | Modifie le style de contour. |
| Dimensionnement flexible (classe CSS) | `min-width` | `20px` | Permet d’assurer la visibilité de l’espace réservé. |
| Dimensionnement flexible (classe CSS) | `min-height` | `20px` | Permet d’assurer la visibilité de l’espace réservé. |
| Dimensionnement flexible (classe CSS) | `max-width` | `200px` | Empêche le débordement. |
| Dimensionnement flexible (classe CSS) | `max-height` | `100px` | Contrôle les limites de la disposition. |

## Bonnes pratiques

Faire :

- Toujours inclure les `{{brand_logo}}` et les `{{defaultLogo}}`.
- Définissez des `width` et des `height` afin que l’espace réservé soit visible.
- Utilisez des classes CSS pour le dimensionnement et la personnalisation de la composition.
- Utilisez `object-fit: contain` pour conserver les proportions du logo.
- Testez avec des logos de différentes tailles et proportions.

Ne pas :

- Utilisez `border` au lieu de `outline` (la bordure ne se masque pas automatiquement).
- Définissez les propriétés de dimensionnement dans les styles intégrés.
- Omettez les contraintes de taille (l’espace réservé est rendu sur 1×1 pixel).
- Utilisez `object-fit: cover` (il peut recadrer les logos).

## Dépannage

Bordure non visible :

- Assurez-vous que `style="{{defaultLogo}}"` est inclus.
- Vérifiez que `width` et `height` sont définis dans votre classe CSS.

L’espace réservé est trop petit (1 px) :

- Ajoutez des `width` et des `height` explicites à votre classe CSS.

La bordure ne disparaît pas après l’échange :

- Utilisez les propriétés de contour dans votre classe CSS, et non `border`.

Logo recadré :

- Utilisez `object-fit: contain` au lieu de `cover`.

Logo trop petit ou trop grand :

- Ajustez les `width` et les `height` dans votre classe CSS.

La bordure personnalisée n’affiche pas :

- Confirmez `{{defaultLogo}}` se trouve dans l’attribut `style`.
- Placez les propriétés de `outline-*` personnalisées dans la classe CSS.
