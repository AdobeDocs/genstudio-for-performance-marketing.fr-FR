---
source-git-commit: f6a305c6a4e700525b570bbe280e5d1049d06537
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 6%

---
# Référence : création de notes de mise à jour

## Matière Première

La page active [](../../help/user-guide/release-notes.md) inclut des métadonnées Experience League au-delà d’un ensemble minimal (par exemple, `TQID`, `product_v2`, `feature_v2`, identifiants de taxonomie).

**Règles:**

- Lors de la modification du contenu de la note de mise à jour **corps**, **conservez les clés et valeurs existantes du front-issue**, sauf si la tâche demande explicitement de modifier les métadonnées.
- Ne supprimez pas la taxonomie ou les métadonnées de produit pour qu’elles correspondent à un modèle plus court.
- Les concepts requis pour les pages ExL incluent généralement `title`, `description` et `role` ; suivez les [conseils sur les métadonnées Experience League](https://experienceleague.adobe.com/en/docs/authoring-guide/using/authoring/using-metadata) pour les nouvelles pages.

## Sources internes (IT et wikis de version)

Utilisez ces champs **uniquement lors de la rédaction** ; les notes de mise à jour publiées ne doivent pas faire référence à des documents internes.

### Documents sur le transfert des connaissances (AC)

Extraire à partir de :

| champ | Utilisation |
|-------|-----|
| Description | Explication des fonctionnalités principales |
| Pas D&#39;Ascenseur | Proposition de valeur |
| Fonctionnalités diffusées | Comportement concret |
| Énoncé de problème | Point faible de l’utilisateur |
| Type de version et date | Planning |

### Pages du wiki de publication

Regrouper et définir la portée par :

| champ | Utilisation |
|-------|-----|
| Date De Publication (Version Corrigée) | Même date → même lot de notes de mise à jour |
| Initiative | Contexte uniquement ; ne pas lier en interne dans le texte public |
| PM présente la fonction à l&#39;aide de l&#39;AC | Des signaux plus détaillés en AC peuvent exister |

**Règle d’étendue :** les éléments qui partagent la même date de publication (version corrigée) appartiennent au même bloc de publication mensuel.

## Liaison de documentation

- Liez vers l’expression **la plus pertinente** (par exemple, liez « Ressources vidéo et d’image non prises en charge » à la section Formats publicitaires).
- Préférez `#anchor` liens vers la sous-section appropriée.
- Les pages d’aperçu sont acceptables lorsqu’il n’existe aucune ancre plus profonde.

## Chemins d’accès courants à la documentation

| Zone | Préfixe du chemin |
|------|-------------|
| Créer | `/help/user-guide/create/` |
| Contenu | `/help/user-guide/content/` |
| Activation | `/help/user-guide/activation/` |
| Validations | `/help/user-guide/approvals/` |
| Insights | `/help/user-guide/insights/` |
| Directives | `/help/user-guide/guidelines/` |
| Modèles | `/help/user-guide/templates/` |
| Campagnes | `/help/user-guide/campaigns/` |
| Extensibilité | `/help/extensibility/` |
