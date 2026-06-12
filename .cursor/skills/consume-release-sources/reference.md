---
source-git-commit: c3c6aa86f4f520d020f8928612d1be6be1599652
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 3%

---
# Référence : utiliser des sources de publication (MCP)

## Découverte de pages de cérémonie

| Motif | Exemple |
|---------|---------|
| Titre | `YYYY/MM Release Ceremony` dans l’espace **GenStudio** |
| Depuis Jira | Lien Wiki dans le ticket `description` (préféré) |
| Remplacement de SQL | `title ~ "2026/06 Release Ceremony" AND space = GenStudio` |

## Groupes de caractéristiques de la cérémonie

Les wikis de cérémonie de publication contiennent jusqu’à **deux** tableaux des fonctionnalités. Analysez les deux à partir d’HTML **storage**.

### Fonctionnalités de la version GA

- Titre de la section : `GA Release Features` (`<h2>`)
- Sous-titre : `Feature Group:` avec lien Floodgate facultatif
- Les colonnes du tableau incluent **Type** (`GA`, `Limited`, `EA`, `Beta` ou vide).
- **Documentation KT** colonne : `<ac:link><ri:page ri:content-title="..."/></ac:link>`

Par extrait de ligne :

| champ | Source |
|-------|--------|
| `featureDescription` | Première `<td>` dans la ligne de données |
| `type` | Saisir le texte de la cellule de la colonne |
| `ktPageTitle` | `ri:content-title` dans la colonne KT |
| `jiraKeys` | `ac:macro ac:name="jira"` → paramètre `key` (interne uniquement) |
| `releaseTier` | `ga` lorsque Type est `GA` ; hérite de Type pour les autres valeurs du tableau GA |

### Fonctionnalités de mise à jour de Beta

- Titre de la section : `Beta Release Features` (peut être **absent** certains mois)
- Deuxième tableau ; **pas de colonne Type** — chaque ligne est Beta
- Même extraction KT et Jira que la table GA
- Définissez `releaseTier: beta` et `requiresBetaBadge: true` sur chaque ligne de section Beta

Si la section Beta est manquante, consignez zéro ligne Beta et continuez.

### Modèles de stockage HTML

```html
<ac:link><ri:page ri:content-title="Translation on HZ Canvas" /></ac:link>
<ac:structured-macro ac:name="jira" ...><ac:parameter ac:name="key">GS-23218</ac:parameter></ac:structured-macro>
```

## Utilisation de l’outil MCP

| Étape | Outil | Paramètres |
|------|------|------------|
| Ticket | `jira_getIssue` | `issueKey`, `expand: renderedFields` facultative |
| Cérémonie | `confluence_getContent` | `contentId`, `bodyMode: storage` |
| Recherche KT | `confluence_searchContent` | `cql: title = "<KT title>" AND space = GenStudio` |
| Corps du KT | `confluence_getContent` | `contentId`, `bodyMode: text`, `maxBodyChars: 50000` |

**Ne pas utiliser** utilisez `bodyMode: text` pour les pages de cérémonie lors de l&#39;analyse des liens KT.

## Correspondance des champs KT (entrées de dessin)

Mappez-les dans generate-release-notes ; ne collez pas in extenso les notes de mise à jour publiques.

| Section AC | Utilisation |
|------------|-----|
| Description | Fonctionnalité principale |
| Pas de l&#39;ascenseur | Proposition de valeur |
| Fonctionnalité(s) fournie(s) | Comportement concret |
| Énoncé du problème | Douleur de l’utilisateur (contexte uniquement) |
| Type de version et date | GA / Beta / Limited (interne) ; prend la décision relative au badge |

## Filtres d’inclusion

Confirmer la portée avec l’utilisateur ou l’utilisatrice en cas de doute. Paramètres prédéfinis courants :

| Préréglage | Inclut |
|--------|----------|
| `ga_only` | Lignes du tableau GA où Type = `GA` |
| `ga_and_beta` | **Valeur par défaut recommandée pour les mois à venir** — Lignes GA où Type = `GA` **plus toutes** lignes du tableau Fonctionnalités de version de Beta |
| `ga_plus_empty` | Table GA : type = `GA` ou type vide |
| `all_except_pilot` | Lignes du tableau GA sauf `Limited` ; section plus Beta lors de l’utilisation de `ga_and_beta` |
| `all_with_badges` | Toutes les lignes du tableau GA ; les lignes de la section Beta reçoivent toujours le badge Beta |

## remise du badge Beta

| Condition | `requiresBetaBadge` |
|-----------|---------------------|
| Ligne du tableau **Fonctionnalités de version de** | `true` |
| Ligne du tableau GA avec Type = `Beta` | `true` |
| Ligne du tableau GA avec Type = `GA` | `false` |

En aval : [générer-des-notes de mise à jour des règles de décision](../generate-release-notes/SKILL.md#decision-rules) et [fragment de badge Beta](../generate-release-notes/SKILL.md#beta-badge).

## Payload de remise (informelle)

Transmettez à generate-Release-Notes en tant que liste d’éléments :

```yaml
- featureDescription: "YouTube Shorts"
  releaseTier: ga
  requiresBetaBadge: false
  ktPageTitle: "YouTube Shorts (Create + Activate)"
  # extracted KT fields: description, elevatorPitch, featuresDelivered, ...
```
