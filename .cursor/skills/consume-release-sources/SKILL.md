---
name: consume-release-sources
description: ""
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---


# Consommer des sources de libération (Jira + Confluence MCP)

**Rédaction en aval :** [generate-release-notes](../generate-release-notes/SKILL.md) → facultatif [polish-release-notes](../polish-release-notes/SKILL.md)

**Référence d’analyse :** [reference.md](reference.md)

**Fichier de sortie cible (en aval uniquement) :** [help/user-guide/release-notes.md](../../help/user-guide/release-notes.md)

## Conditions préalables

- **Jira MCP** (`jira_getIssue`, `jira_searchIssues`) authentifié
- **Confluence MCP** (`confluence_getContent`, `confluence_searchContent`) authentifié
- Clé de ticket Jira à partir du nom de branche (`GS-#####`), de l’entrée utilisateur ou de la description du ticket

## Liste de contrôle des workflows

1. [ ] **Résoudre le ticket Jira** — `jira_getIssue` avec `issueKey`. Lisez `description` pour le lien du wiki de la cérémonie et le mois de publication.
2. [ ] **Localiser la page de cérémonie** — utiliser l’URL du wiki du ticket ; CQL de secours : `title ~ "YYYY/MM Release Ceremony" AND space = GenStudio`.
3. [ ] **Récupérer le corps de la cérémonie** — `confluence_getContent` avec `bodyMode: storage` (obligatoire ; `text` perd les liens KT et la structure du tableau).
4. [ ] **Analyser les groupes de fonctionnalités** — extraire des lignes des **fonctions de version GA** et des **fonctions de version Beta** (voir [référence.md](reference.md#ceremony-feature-groups)).
5. [ ] **Appliquer le filtre d’inclusion** — par portée d’utilisateur (voir [référence.md](reference.md#inclusion-filters)) ; confirmer le nombre de lignes Beta (peut être égal à zéro).
6. [ ] **Résoudre les pages d&#39;AC** — `confluence_searchContent` par titre d&#39;AC ; `confluence_getContent` avec `bodyMode: text`.
7. [ ] **Extraire les champs KT** — Description, Pas d&#39;ascenseur, Fonctionnalité(s) fournie(s), Énoncé du problème, Type et date de publication.
8. [ ] **Définir les indicateurs Beta** — `requiresBetaBadge: true` pour les lignes de section Beta ou les lignes du tableau GA avec le type `Beta`.
9. [ ] **Transmettre** à [générer-des-notes de mise à jour](../generate-release-notes/SKILL.md) avec une liste de lignes structurée (aucune référence wiki/Jira dans la copie envoyée).

## Étiquetage du Beta (transfert pour générer des compétences)

Lorsqu’elle est `requiresBetaBadge: true`, la section de `###` en aval doit inclure immédiatement sous l’en-tête :

```markdown
[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}
```

N’ajoutez pas de clauses de non-responsabilité de planification en italique pour Beta. Le badge est le modèle pris en charge.

## Interdit dans les notes de mise à jour expédiées

Les identifiants internes, les URL wiki, les citations KT et les clés Jira restent uniquement dans cette phase d’ingestion. Résumez les résultats visibles par l’utilisateur dans la page publique par [générer-du-contenu interdit de notes de mise à jour](../generate-release-notes/SKILL.md#prohibited-content).

## Secours

Si les appels MCP échouent, demandez à l’utilisateur de coller le contenu de la cérémonie et de l’KT, puis continuez avec les notes de mise à jour générées à l’aide du mappage de champs [reference.md KT](../generate-release-notes/reference.md#internal-sources-kt-and-release-wikis).

## Ressources supplémentaires

- [reference.md](reference.md) — analyse de cérémonie, CQL, filtres d’inclusion, paramètres MCP
- [generate-release-notes](../generate-release-notes/SKILL.md) — archive, brouillon, liens, contrôles qualité
- [polish-release-notes](../polish-release-notes/SKILL.md) — passe éditoriale sur les nouvelles `###` sous `{#latest}`
