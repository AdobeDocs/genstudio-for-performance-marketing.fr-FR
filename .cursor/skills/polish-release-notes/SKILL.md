---
name: polish-release-notes
description: ""
notes: refines only newly added
source-git-commit: ee2875f35035e23e2577adbde5f408702b77d233
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---


# Notes de mise à jour de la version polonaise de GenStudio

**Fichier cible canonique :** [help/user-guide/release-notes.md](../../../help/user-guide/release-notes.md)

**Exemples:** [exemples.md](examples.md)

**Workflow de rédaction (amont) :** [generate-release-notes](../generate-release-notes/SKILL.md)

## Portée (obligatoire)

Contenu polonais **uniquement** que l’utilisateur identifie comme **nouvellement ajouté** ce cycle :

- **Dans le fichier :** `###` sous l’en-tête unique `## YYYY.MM {#latest}` dans `help/user-guide/release-notes.md`.
- **Ne modifiez pas** le titre de la page, le paragraphe d’introduction, le sujet principal ou tout texte sous **Notes de mise à jour antérieures** (blocs de `+++` réductibles).
- **Ne modifiez pas** sauf si l’utilisateur le demande **explicitement**, les blocs mensuels `##` précédents ou les `###` préexistants dans la même section de `{#latest}`.
- Si les nouveaux `###` ne sont pas clairs, **demandez** ou utilisez **git diff**/edit context avant de changer de prose.
- **Contenu collé :** l’utilisateur ne colle le markdown que lorsqu’il confirme qu’il correspond à ces **mêmes** nouvelles sous-sections (ne traitez pas un collage sans rapport comme étant inclus dans la portée).

Conserver les différences **minimales** : le libellé et les sauts de paragraphe uniquement, sans refactorisation dynamique ailleurs dans le fichier.

## Voix et tonalité

- Écrivez en tant que **rédacteur** pour les notes de mise à jour des produits : **concis**, **scannable** et **énergisé** sur la **nouvelle valeur**—dirigez avec des résultats et « qu’avez-vous à y gagner », utilisez des verbes forts et un langage clair et net.
- **Restez précis :** aucune revendication au-delà de ce que la fonctionnalité offre ; collez au ton d’Experience League/Adobe (confiant et clair, pas sensationnaliste).
- **Générer de l’excitation** avec des avantages et des différences **spécifiques** (ce que les professionnels du marketing peuvent faire maintenant, quelle friction est supprimée), et non du battage publicitaire ou des superlatifs non corroborés.

## Règles de paragraphe

- Chaque paragraphe : **2-3 phrases**. **Jamais plus de trois phrases** dans un paragraphe ; si vous en avez besoin, commencez un **nouveau paragraphe**.
- Facultatif : si un paragraphe s’exécute toujours sur plus de **à 3 lignes** dans les documents rendus à une longueur de ligne standard, fractionnez davantage.

## Ne pas ajouter

- **Procédure à suivre»** contenu : étapes numérotées, « cliquez sur **[!UICONTROL ...]** puis... », explications complètes de l’interface utilisateur ou expressions du tutoriel. Les notes de mise à jour résument **ce qui a été livré** et **pourquoi c’est important**, pas des leçons pratiques.
- Contenu enfreignant la [Contenu interdit](../generate-release-notes/SKILL.md#prohibited-content) sur la compétence générée (pas de clés Jira, URL internes uniquement, wiki-as-proof, etc.).

## Supprimer pendant le polissage (planification des versions)

Les brouillons comprennent parfois des lignes **en italique** (`_…_` ou `*…*`) sur la **disponibilité**, par exemple la publication limitée, le timing du Summit, la disponibilité générale, le déploiement étendu ou Beta **fenêtres**. Ce langage est adapté à la **gestion de version**, et non aux notes affinées destinées aux clients et clientes de cette page.

- **Supprimez entièrement** ces **lignes italiques** ou **clauses italiques de fin** lorsque leur **objectif principal** est la planification ou le statut de déploiement (y compris **GA**, **limited release**, **Summit** ou similaire).
- **Ne supprimez pas** les phrases ordinaires (non italiques) qui décrivent le comportement du produit, mais uniquement la copie de planification définie en **italiques** comme clause de non-responsabilité.
- **Conserver** le bloc **[!BADGE Beta]** lorsque la fonctionnalité est Beta ; le badge est le modèle pris en charge pour Beta, et non une ligne de planification italique distincte.
- Après la suppression, **resserrez la prose environnante** si un paragraphe commence ou se termine mal ; ne remplacez pas l’italique supprimé par de nouvelles phrases de planification, sauf si l’utilisateur le demande explicitement.

## Conserver (ne pas supprimer ni réécrire structurellement)

- `[!DNL …]`, `[!UICONTROL …]`, `[!BADGE …]` et autres codes courts ExL.
- Liens de documentation **relatifs** et modèles d’ancrage existants : `[phrase](/help/...)` sur un texte d’ancrage significatif.
- Le badge Beta se bloque exactement comme utilisé dans les exemples [generate-release-notes](../generate-release-notes/examples.md).

## Liste de contrôle des workflows

1. [ ] Confirmez **&#x200B;**&#x200B;quels `###` en cours de `## … {#latest}` sont concernés (nouveaux pour ce cycle).
2. [ ] Pour chaque `###` de la portée, resserrez le texte par [règles de voix et de ton](#voice-and-tone) et [&#x200B; règles de paragraphe](#paragraph-rules).
3. [ ] supprimer ou raccourcir toute **procédure** instructions ; conserver **les résultats pour l’utilisateur**.
4. [ ]Supprimez les lignes **planification et disponibilité en italique (ou en style italique)** par [Supprimez-les lors du polissage (planification des versions)](#remove-during-polish-release-scheduling).
5. [ ] Vérifiez que les liens et les numéros courts sont toujours valides. Exécutez une analyse rapide pour rechercher les identifiants internes ou les modèles interdits par [Contrôles qualité](#quality-checks).

## Contrôles de qualité

- [ ] Seuls les blocs de `###` convenus **nouveaux** sous `{#latest}` ont été modifiés ; les archives et les mois plus anciens ont été préservés.
- [ ] Aucun nouvel identifiant de style Jira, URL de wiki interne, ou langage « voir le ticket ».
- [ ] Aucune **planification uniquement** clauses de non-responsabilité en italique (disponibilité générale, version limitée, déploiement au sommet, etc.) conservez les sous-sections de `{#latest}` affinées, celles-ci ont été supprimées conformément à la section [Supprimer pendant l’affinage (planification des versions)](#remove-during-polish-release-scheduling) ; les blocs de badge Beta conviennent le cas échéant.
- [ ] Les paragraphes sont **2 à 3 phrases** chacun (maximum trois phrases par paragraphe).
- [ ] Copy reste **factuelle** et alignée sur la fonctionnalité décrite.

## Ressources supplémentaires

- [exemples.md](examples.md) — modèles avant/après.
- [generate-release-notes](../generate-release-notes/SKILL.md) : rédaction, archivage, badges Beta, liaison.
