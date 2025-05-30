---
title: Instructions relatives aux modèles d’e-mail
description: Appliquez les bonnes pratiques lorsque vous utilisez des modèles d’e-mail avec Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
source-git-commit: d9d774f727b69b18af6114965fdb8ffb450f797b
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Instructions relatives aux modèles d’e-mail

Un modèle d’e-mail marketing sert de base pour des campagnes par e-mail attrayantes et réactives sur le plan visuel. En règle générale, les modèles HTML vous permettent de contrôler la mise en page, la typographie, les couleurs et l’imagerie pour vous aligner sur les directives de votre marque. Lorsque vous préparez votre modèle à utiliser dans GenStudio for Performance Marketing, utilisez la sémantique HTML et le CSS intégré pour le style et évitez les scripts ou les dépendances externes. Des modèles HTML bien structurés peuvent améliorer l’expérience du ou de la destinataire ainsi que la délivrabilité et les taux d’engagement.

Suivez ces bonnes pratiques de conception lors de la personnalisation de modèles d’e-mail pour travailler avec GenStudio for Performance Marketing :

- Utilisation des polices Adobe ou Google
- Utilisation d’HTML et de CSS intégré propres et réactifs
- N’utilisez **&#x200B;**&#x200B;JavaScript
- N **utilisez pas** largeur fixe dans le corps ou le conteneur
- N’utilisez **pas** codage base64 pour les images, car il peut augmenter considérablement la taille du modèle
- La taille maximale du fichier HTML est de 102 Ko

## Noms de champs reconnus

GenStudio for Performance Marketing génère automatiquement le champ `subject` pour les e-mails. Lorsque vous personnalisez votre modèle, utilisez des espaces réservés de contenu pour les champs obligatoires suivants :

- `pre_header` (texte enrichi non activé)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (sélectionné parmi Content JPEG, PNG ou GIF)

Le nombre maximal de champs autorisés dans un modèle est de 20. Voir [Espaces réservés de contenu](/help/user-guide/content/customize-template.md#content-placeholders) pour en savoir plus sur l’utilisation de noms de champ dans les modèles.

## E-mail à plusieurs sections

Les _sections_ vous permettent d’organiser le contenu en groupes distincts, ce qui rend les dispositions plus complexes. Dans Genstudio pour le marketing de performance, vous pouvez définir chaque section à l’aide d’une convention de nommage de groupe. Voir [Personnaliser les sections de modèle](/help/user-guide/content/customize-template.md#sections-or-groups).

Les modèles à plusieurs sections peuvent comporter 0, 2 ou 3 sections :

- Un modèle de base (zéro section) peut générer un seul ensemble d’éléments de modèle, ce qui ne nécessite pas la convention d’affectation des noms de groupe.
- Un modèle complexe (plusieurs sections) peut générer jusqu’à trois ensembles d’éléments de modèle, ce qui nécessite de respecter la convention de dénomination des groupes : (`groupname_fieldname`)

Exemples de noms de champ pour deux sections :

- `pod1_headline`, `pod1_body`, `pod1_cta`
- `pod2_headline`, `pod2_body`, `pod2_cta`

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
