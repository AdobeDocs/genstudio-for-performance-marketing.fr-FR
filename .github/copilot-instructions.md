---
source-git-commit: 8ed1e6853c9f844c72431dc692b556ece9c215a8
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---
## Objectif

Aidez les assistants de codage de l’IA à apporter de petites modifications sécurisées au référentiel de documentation de GenStudio for Performance Marketing.

## Architecture de haut niveau (courte)
- Ce référentiel est un site de documentation composé de Markdown sous `help/` avec des inclusions partagées dans `help/_includes/` et des images sélectionnées sous `help/_includes/assets/`.
- Notes de mise à jour, guide de l’utilisateur et contenu d’extensibilité en direct sous `help/`. Les modifications de contenu importantes doivent préserver le frontdomain et la structure d’en-tête existante.
- Le site est créé à l’aide de Jekyll et hébergé sur des pages GitHub. Le processus de création utilise les conventions Jekyll standard avec certains modules externes personnalisés.

## Conventions spécifiques au projet
- Règles de curseur : l’automatisation et le guidage personnalisés se trouvent dans `.cursor/rules/*.mdc`. Exemples : `.cursor/rules/docs-lint.mdc` (processus de lint), `.cursor/rules/generate-release-notes.mdc` (format des notes de mise à jour). Suivez ces instructions pour les tâches automatisées.
- Noms de fichiers et frontend :
   - Les notes de mise à jour nécessitent un front-issue spécifique (voir `.cursor/rules/generate-release-notes.mdc`).
   - Utilisez la casse kebab pour les fichiers de règle et l’extension de `.mdc`.
- Conventions de formatage : les documents utilisent le Markdown parfumé GitHub. Les en-têtes suivent généralement la casse des phrases et les paragraphes courts. Préférez les puces `*` pour les listes dans les notes de mise à jour et les `###` pour les sections de fonctionnalités.

## Instructions de style de documentation
- Suivez le [Guide de style d’écriture Microsoft](https://learn.microsoft.com/en-us/style-guide/) pour connaître les bonnes pratiques en matière de documentation technique :
   - Écrire des phrases claires et concises axées sur les actions des utilisateurs et utilisatrices
   - Utiliser la voix active et le présent
   - Diviser le texte en blocs courts et analysables
   - Gardez un ton chaud et direct tout en conservant la précision technique
- Création Markdown :
   - Utiliser la casse des phrases pour les en-têtes (avec une majuscule en début de texte uniquement)
   - Conserver les paragraphes courts (2 à 3 phrases) pour plus de lisibilité
   - Ajouter des lignes vides avant et après les en-têtes et les listes
   - Utiliser des accents graves pour les éléments de l’interface utilisateur, les chemins d’accès aux fichiers et le code
   - Inclure le texte secondaire pour toutes les images
   - Lien vers des sections spécifiques à l’aide de texte descriptif

## Règles de sécurité pour les modifications (ce que l’IA doit faire)
- N’ajoutez jamais d’ID Jira, de liens internes ou de références d’entreprise uniquement aux documents publics. Voir `generate-release-notes.mdc` section « Suivi des problèmes ».
- Conservez le code YAML du front-end exactement lors de la modification des fichiers qui l’incluent. De nombreux modèles et notes de mise à jour reposent sur des clés fixes (titre, description, rôle, exl-id).
- Pour les corrections de ligne, préférez les modifications automatisées et idempotentes à partir de `.cursor/rules/docs-lint.mdc` (supprimez les espaces de fin, assurez-vous de la dernière nouvelle ligne). Exemples de commandes utilisées par des humains :

```sh
sed -i '' 's/ $//' <file>
sed -i '' '$ { /^$/d; }' <file> && echo "" >> <file>
```

## Exemples (que modifier et comment)
- Correctifs pour petites copies : mettez à jour le texte dans `help/` fichiers Markdown, en conservant les en-têtes et les ancres intacts.
- Mises à jour des images : images de référence sous `help/_includes/assets/`. Ne déplacez pas et ne renommez pas les images sans mettre à jour toutes les références.

## Où chercher en premier
- `help/_includes/` : fragments et images partagés.
- `.cursor/rules/` — automatisation et conseils de liaison ; utilisez-les comme règles faisant autorité pour le formatage et les processus.
- `markdownlint_custom.json` — remplacements markdownlint locaux.
- `.github/pull_request_template.md` — attentes en matière de relations publiques.

## Quand demander à l&#39;humain
- Si une modification nécessite l’exécution ou la modification d’un outil basé sur Docker (la règle de ligne mentionne Docker) ou affecte les pipelines de création de site.
- Si un fichier fait référence à une configuration externe inconnue (par exemple, `markdownlint.json` est manquant) — demandez s’il faut créer ou ignorer.

## Commandes minimales pour les humains

```sh
# Install linter (if not present)
npm install -g markdownlint-cli

# Run lint locally using project config
markdownlint --config markdownlint_custom.json "help/**/*.md"

# Project lint via yarn (preferred if available in environment)
yarn lint
```

---
Si vous le souhaitez, je peux le fusionner en `.github/copilot-instructions.md` dans le référentiel (ou ajuster le libellé/la longueur). Que dois-je modifier ou ajouter ?
