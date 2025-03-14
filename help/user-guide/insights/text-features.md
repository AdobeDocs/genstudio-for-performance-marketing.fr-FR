---
title: Fonctionnalités de texte
description: Découvrez la fonction de texte des catégories d’attributs utilisées dans GenStudio for Performance Marketing.
feature: Insights, Attributes, Generative AI
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
source-git-commit: 808ffdb7f55f7ff938e9346b8513fab46f86df7c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 1%

---

# Fonctionnalités de texte

Les fonctions de texte incluent des nombres pour certains éléments de texte, tels que des mots, des phrases, des émoticônes, ainsi que des classifications pour la sémantique, l’émotion et le ton utilisés pour l’analyse avec [!DNL Insights]. Le texte peut également recevoir un score de lisibilité.

GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités de machine learning pour étudier le texte et appliquer des [!UICONTROL attributs de média] en fonction des tons de texte et du récit marketing associés. Le processus valide le texte d’entrée pour s’assurer qu’il contient des caractères alphanumériques, en supprimant les espaces blancs supplémentaires et les caractères non imprimables, et en tronquant le texte au maximum autorisé de 1 500 mots. Avant d’appliquer les balises d’attribut détectées, l’IA prédit la tonalité dominante.

## Ton de la voix

Le ton représente un caractère général, une attitude ou une atmosphère manifestée par le langage. Un simple choix de mots et de ponctuation, de structure de phrase et de style peut modifier le ton de votre message. Par exemple, considérez les messages urgents suivants en utilisant les trois niveaux de tonalité de base :

- `Formal`

  ```
  Take advantage of this distinctive and exceptional opportunity!
  ```

- `Conversational`

  ```
  Don't miss out on this great opportunity!
  ```

- `Direct`

  ```
  Don't miss the chance!
  ```

L’IA détecte en outre un ton plus nuancé. En reprenant la même instruction urgente de l’exemple précédent, la version suivante utilise un ton `poetic` fantaisiste :

- `Poetic`

  ```
  Embrace the moment, without delay, for this occasion won't always stay.
  ```

Les autres valeurs secondaires de tonalité sont les suivantes : `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal`

## Narratif

Les attributs narratifs vous aident à identifier les médias qui communiquent les valeurs, l’objectif ou l’identité qui résonnent avec votre audience cible.

| Narratif | Description | Exemple |
| ----------------- | ----------- | ------- |
| `Authenticity` |             |         |
| `Celebration` |             |         |
| `Community` |             |         |
| `Convenience` |             |         |
| `Empowerment` |             |         |
| `Exploration` |             |         |
| `Futuristic` |             |         |
| `Hype` |             |         |
| `Indulgence` |             |         |
| `Peace of mind` |             |         |
| `Personalization` |             |         |
| `Prestige` |             |         |
| `Timelessness` |             |         |
| `Versatility` |             |         |
| `Well-being` |             |         |

## Score de lisibilité

Le score de lisibilité évalue la facilité de lecture et de compréhension d’un texte. Cela permet de s’assurer que votre contenu est adapté à votre audience cible. Les scores sont basés sur divers facteurs, notamment la longueur de la phrase et la complexité des mots.

| Score | Niveau scolaire | Notes |
| ----------- | ------------------ | ------------------------------------------------------------------------- |
| 100-90 | 5e année | Très facile à lire. Facilement compris par un étudiant moyen de 11 ans. |
| 90.0-80.0 | 6e année | Facile à lire. Conversation en anglais pour les consommateurs. |
| 80,0-70,0 | 7e année | Assez facile à lire. |
| 70,0-60,0 | 8ème et 9ème année | Anglais ordinaire. Facilement compris par les élèves de 13 à 15 ans. |
| 60.0-50.0 | de la 10e à la 12e année | Plutôt difficile à lire. |
| 50,0-30,0 | Collège | Difficile à lire. |
| 30,0-0,0 | Diplômé de l&#39;université | Très difficile à lire. Mieux compris par les diplômés universitaires. |

## Nombre de mots

À déterminer

Le tableau suivant répertorie les catégories de fonctionnalités d’image reconnues par l’IA dédiée à GenStudio for Performance Marketing.

| Catégorie | Description | Exemple |
| -------------------- | ------------- | --------------------- |
| Nombre d’émotions |             |        |
| Nombre de balises de hachage |             |        |
| Mots-clés |             |        |
| Émotions marketing | Les émotions sont ciblées dans les messages marketing pour évoquer des sentiments et des réponses spécifiques du public, ce qui peut améliorer l&#39;engagement et la connexion avec la marque. | `Aspiration`, `Challenge`, `Curiosity`, `Exclusivity`, `Fascination`, `Gratification`, `Recognition`, `Trust`, `Urgency` |
| Stratégies de persuasion | Techniques utilisées pour influencer le comportement des consommateurs et inciter à des actions souhaitées. Ces stratégies ciblent des déclencheurs psychologiques et des segments de clientèle spécifiques pour améliorer l’efficacité des messages marketing. | `Social identity`, `Social proof`, `Endorsement`, `Concreteness`, `Foot in the door`, `Overcoming reactance`, `Reciprocity`, `Comparison`, `Social impact`, `Scarcity`, `Anthropomorphism` |
| Ton de la voix | Caractère général, attitude ou atmosphère véhiculée dans un message marketing par le choix des mots, la ponctuation, la structure de la phrase et le style. | `Enthusiastic`, `Assertive`, `Humorous/Witty`, `Inspirational`, `Empathetic`, `Sensory`, `Storytelling`, `Poetic`, `Quantitative`, `Personal` |
