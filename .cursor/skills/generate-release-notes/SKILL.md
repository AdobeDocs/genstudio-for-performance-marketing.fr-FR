---
name: generate-release-notes
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


# Générer des notes de mise à jour GenStudio

**Fichier cible canonique :** [help/user-guide/release-notes.md](help/user-guide/release-notes.md)

**Exemples complets :** [exemples.md](examples.md)

**Mappage des champs KT/wiki et chemins de document :** [reference.md](reference.md)

## Édition de l’étendue (stricte)

Lors de l’utilisation de cette compétence, **le seul endroit** vous pouvez **ajouter** ou **modifier** le contenu du corps de la note de mise à jour est la section intitulée avec **`## … {#latest}`** (le bloc unique qui porte l’ancrage `{#latest}`).

- **Ne modifiez pas** **Notes de mise à jour antérieures** (tout bloc `+++Notes from YYYY.MM.DD+++` réductible) ou **tout** toute ancienne section mensuelle `##` qui n’a plus de `{#latest}`, même si la rubrique semble liée, si un lien semble erroné ou si une copie semble y être dupliquée ou obsolète.
- **Ne retouchez pas** les sous-sections, les puces, les liens ou les libellés des `###` précédents en dehors du bloc de `{#latest}` actuel, sauf si l’utilisateur ou l’utilisatrice donne une requête **explicite, distincte** qui n’est pas couverte par cette compétence.
- **Exception :** [Archiver la version précédente au plus tard](#archive-previous-latest) lors de l’introduction d’un **nouveau** bloc de `{#latest}` supérieur : **déplacer** l’ensemble de la section `{#latest}` précédente dans un **nouveau** réductible sous **Notes de mise à jour antérieures** comme décrit ci-dessous. Au cours de cette passe, **ne pas** réécrire ou ajouter à d’**autres blocs d’archives plus anciens**.

Si de nouvelles informations appartiennent au document, placez-les sous l’en-tête **`{#latest}`** actuel (ou archivez-les d’abord, puis ajoutez-les uniquement sous le nouveau `{#latest}`).

## Liste de contrôle des workflows

Travaillez dans cet ordre. Copiez la liste de contrôle et suivez la progression pour les modifications à plusieurs étapes.

0. [ ] Si **Jira** et **Confluence** MCP sont disponibles, exécutez [consume-release-sources](../consume-release-sources/SKILL.md) d’abord pour ingérer le ticket de travail, le wiki de cérémonie (groupes de fonctionnalités GA et Beta) et les pages KT. Si MCP n’est pas disponible, utilisez le contenu KT/wiki collé et le mappage de champ [reference.md](reference.md#internal-sources-kt-and-release-wikis).
1. [ ] Ouvrir le `help/user-guide/release-notes.md` et lire le bloc de `## YYYY.MM {#latest}` actif. Traitez les **notes de mise à jour antérieures** comme du contexte **lecture seule** sauf si vous effectuez l’étape d’archivage de l’étape 2.
2. [ ] Si vous ajoutez une **nouvelle** version mensuelle : archivez la dernière version (voir [Archiver la dernière version précédente](#archive-previous-latest)).
3. [ ] Ajouter ou modifier **uniquement** la section des `## YYYY.MM {#latest}` principaux (le mois le plus récent en haut de la liste des versions).
4. [ ] Pour chaque élément, appliquez [Règles de décision](#decision-rules) (`###` des fonctionnalités par rapport à **Correctifs et améliorations**, badge Beta ou non).
5. [ ] Ajoutez ou vérifiez des liens vers la documentation relative à l’expression la plus pertinente (voir [reference.md](reference.md#documentation-linking)).
6. [ ] Exécutez [contrôles qualité](#quality-checks) avant de terminer.
7. [ ] Conserver [frontMATTER](reference.md#frontmatter) sur la page sauf si la tâche met explicitement à jour les métadonnées.

## Règles de décision

Utilisez ces règles if/then pour que le contenu arrive au bon endroit :

| Si | Alors |
|----|------|
| Cette fonctionnalité est nouvelle et disponible dans Beta | Ajoutez la ligne de badge Beta immédiatement sous l’en-tête `###` (voir [exemples.md](examples.md)). |
| Les ressources Source étiquettent explicitement l’élément comme **correctif** ou **amélioration** | Mettez-le sous `### Fixes and enhancements` avec `*` balles seulement. |
| L’élément est une nouvelle fonctionnalité ou une nouvelle fonctionnalité | Utilisez une section `###` avec 1 à 3 phrases (et non la liste des correctifs). |
| Vous ne savez pas si quelque chose est un correctif ou une fonctionnalité | Par défaut, utilisez une section de fonctionnalité `###`, sauf si la source indique clairement correctif/amélioration. |

**Règle de section des correctifs :** n’ajoutez pas de puces aux **Correctifs et améliorations**, sauf si la source est explicitement étiquetée comme correctif ou amélioration.

## Archiver la dernière version précédente

Lors de l’introduction d’un nouveau `## YYYY.MM {#latest}` :

1. Coupez l’ensemble de la section `## YYYY.MM {#latest}` précédente (de son en-tête à la fin du contenu de cette version, avant la `##` suivante ou **Notes de mise à jour précédentes**).
2. Collez-le dans **Notes de mise à jour antérieures**, dans un bloc **nouveau** réductible.
3. Remplacez l’ancien en-tête par : `+++Notes from YYYY.MM.DD+++` (utilisez la date de publication réelle ; mettez-la au format des notes existantes dans le fichier).
4. Supprimez le `{#latest}` de l’en-tête archivé ; la nouvelle section supérieure est la seule avec `{#latest}`.
5. Conservez l’ordre chronologique à l’intérieur **Notes de mise à jour antérieures** (les blocs archivés les plus récents sont placés en haut, sauf si le fichier utilise déjà un ordre différent, **correspondent au fichier existant**).

Ne modifiez **pas** le corps des blocs de `+++Notes from …+++` **préexistants** lors de l’exécution de cette archive. Insérez uniquement le bloc nouvellement archivé et conservez les anciennes archives en l’état.

## Structure requise

### Titre de la page et introduction

Après le front-match, utiliser :

```markdown
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.
```

Si le fichier utilise déjà une phrase d’introduction légèrement différente (par exemple, « fournit » au lieu de « détails »), conservez la cohérence avec le reste de la page.

### En-tête de la dernière version

- Format : `## YYYY.MM {#latest}` pour le bloc de version le plus récent.
- Une seule ancre de `{#latest}` sur la page.

### Sections de caractéristiques

- Utilisez `###` pour les principales catégories de fonctionnalités.
- Présentez du contenu, 1 à 3 phrases, expliquez clairement pourquoi et pourquoi, et les actions de l’utilisateur s’avèrent utiles.
- Noms de produits : `[!DNL Create]`, `[!DNL Content]`, `[!DNL Insights]`, etc.
- Interface utilisateur : `[!UICONTROL Control Name]` le cas échéant.
- Accent : `_italics_` pour les zones/sections de l’interface utilisateur ; `**bold**` pour les termes clés avec parcimonie.

### Badge Beta

Utilisez exactement :

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

### Liens vers la documentation

- Modèle : `[link text](/help/user-guide/section/page.md#anchor)`
- Préférez les ancres ; liez l’expression qui intéresse les utilisateurs et non « cliquez ici ».

### Correctifs et améliorations

- Les puces utilisent `*`.
- Seuls les éléments explicitement étiquetés comme correctifs/améliorations dans le matériau source.
- Mêmes conventions de terminologie et de liens que les fonctionnalités.

## Contenu interdit

- N’incluez **pas** les clés Jira, les numéros de problème internes, les URL internes uniquement ou les liens de wiki d’entreprise dans les notes de mise à jour publiées.
- N **utilisez pas** documents de transfert de connaissances, des tickets ou des outils internes comme preuves - résumez uniquement les résultats visibles par les utilisateurs.
- Ne **dupliquez pas** `{#latest}` sur plusieurs sections.

## Contrôles de qualité

Avant d’effectuer la tâche :

- [ ] **Portée :** seul le bloc `## … {#latest}` a été ajouté ou modifié ; **Notes de mise à jour antérieures** et les anciennes sections mensuelles n’ont pas été modifiées, à l’exception de la [Archiver la dernière version](#archive-previous-latest) qui a été coupée/collée de l’ancienne `{#latest}` dans un bloc **new**.
- [ ] Tous les liens relatifs, nouveaux ou modifiés, sont résolus sur des chemins réels sous `help/`, dans la mesure du possible.
- [ ] fonctionnalités de Beta incluent le fragment de code Beta si nécessaire.
- [ ] terminologie correspond aux notes de mise à jour existantes (`[!DNL …]`, `[!UICONTROL …]`).
- [ ] rechercher des ID internes accidentels (`[A-Z]+-\d+`), des URL de wiki ou un langage « See Jira » dans le brouillon ; supprimez-les.
- [ ] **correctifs et améliorations** contient uniquement des correctifs/améliorations explicitement étiquetés.
- [ ] Dernière section précédente archivée correctement lorsqu’un nouveau mois a été ajouté.

## Sources de contenu (résumé)

Lorsque **Jira/Confluence MCP** est disponible, commencez par [consume-release-sources](../consume-release-sources/SKILL.md) (wiki de cérémonie → pages KT → remise structurée). Sinon, mappez les champs wiki de transfert de connaissances collés ou de publication comme décrit dans [reference.md](reference.md#internal-sources-kt-and-release-wikis). La page fournie doit être lue en tant que documentation utilisateur autonome.

## Facultatif : publiez de nouvelles sous-sections

Après avoir ajouté du nouveau contenu `###` sous `{#latest}`, exécutez [notes de mise à jour polonaises](../polish-release-notes/SKILL.md) pour une passe de style copyeditor (tonalité de transfert d’avantages, **2-3 phrases par paragraphe**, pas de procédure à suivre) **uniquement** sur ces **nouvelles** sous-sections—**not** sur les notes de mise à jour précédentes ou le texte préexistant, sauf demande explicite.

## Ressources supplémentaires

- [exemples.md](examples.md) — exemples prêts pour le collage (fonctionnalités, correctifs, bloc d&#39;archivage).
- [reference.md](reference.md) — notes frontMATTER, chemins de documents, stratégie de liaison.
- [Notes de mise à jour polonaises](../polish-release-notes/SKILL.md) — laissez-passer éditorial facultatif pour les nouveaux `###` ajoutés sous `{#latest}`.
