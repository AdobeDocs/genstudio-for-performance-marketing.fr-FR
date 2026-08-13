---
title: Fonctions de texte
description: Découvrez la fonction de texte des catégories d’attributs utilisées dans GenStudio for Performance Marketing.
feature: Reporting and Insights, Text Attributes, Generative AI
exl-id: 7b81b0ae-0c62-468f-965c-fd8070644fb3
TQID: https://experienceleague.adobe.com/Oec5q249StCtuG-2-n1dYmJoEDRPaqLF2QANpwClQ3A
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
feature_v2:
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
  - id: fc314d1d-7cb9-4a38-8dbd-8f9b6478f40d
source-git-commit: 621f137c2c71c8ab6188c438f877eb3b3e457beb
workflow-type: tm+mt
source-wordcount: 1300
ht-degree: 1%

---

# Fonctionnalités de texte

Les fonctions de texte incluent des nombres pour certains éléments de texte, tels que des mots, des phrases, des émoticônes, ainsi que des classifications pour la sémantique, l’émotion et le ton utilisés pour l’analyse avec [!DNL Insights]. Le texte peut également recevoir un score de lisibilité.

GenStudio for Performance Marketing utilise l’IA d’Adobe et les fonctionnalités de machine learning pour étudier le texte et appliquer des [!UICONTROL attributs de média] en fonction des tons de texte et du récit marketing associés. Le processus valide le texte d’entrée pour s’assurer qu’il contient des caractères alphanumériques, en supprimant les espaces blancs supplémentaires et les caractères non imprimables, et en tronquant le texte au maximum autorisé de 1 500 mots. Avant d’appliquer les balises d’attribut détectées, l’IA prédit la tonalité dominante.

## Ton de la voix

Le ton représente un caractère général, une attitude ou une atmosphère manifestée par le langage. Un simple choix de mots et de ponctuation, de structure de phrase et de style peut modifier le ton de votre message. Par exemple, considérez les messages urgents suivants en utilisant les trois niveaux de tonalité de base :

| Ton | Description | Exemple |
| -------------- | ----------------------------------- | --------------------------------------------------------- |
| Formel | Un langage poli et professionnel. | `Take advantage of this distinctive and exceptional opportunity!` |
| Conversationnel | Langage convivial et informel. | `Don't miss out on this great opportunity!` |
| Direct | C&#39;est simple et direct. | `Don't miss the chance!` |

D’autres valeurs secondaires pour le ton permettent de distinguer plus finement le caractère et l’attitude de votre message. Dans la lignée de l&#39;exemple précédent d&#39;un message urgent, le GenAI peut détecter un ton _poétique_ dans cet exemple fantaisiste : `Embrace the moment, without delay, for this occasion won't always stay.`

Le tableau suivant répertorie les valeurs de tons reconnues par l’IA dédiée à GenStudio for Performance Marketing.

| Ton | Description | Exemple |
| -------------- | ------------------------------------------------ | --------------------------------------------------------- |
| Assertif | Confiante et ferme dans l&#39;expression. | `You need to act now to secure this deal!` |
| Direct | C&#39;est simple et direct. | `Don't miss the chance!` |
| Empathique | Compréhension et sensibilité. | `We understand your needs, and this is perfect for you.` |
| Enthousiaste | Afficher un plaisir, un intérêt ou une approbation intenses et enthousiastes. | `This is an amazing opportunity you can't miss!` |
| Humoristique/Spirituel | Léger et intelligent. | `Why wait? Grab this deal before it's gone!` |
| Inspirant | Encourageant et stimulant. | `Believe in yourself and seize this opportunity!` |
| Poétique | Artistique et expressif. | `Embrace the dawn of a new opportunity.` |
| Quantitatif | Basé sur des données numériques. | `99% of users loved this offer, and you will too.` |
| Sensoriel | Mobiliser les sens. | `Feel the excitement with this incredible offer!` |
| Storytelling | Narration d&#39;une histoire pour transmettre un message. | `Once upon a time, there was an offer you couldn't refuse.` |

## Attrait émotionnel

Les professionnels du marketing exploitent la puissance des émotions humaines pour créer une connexion forte entre le public et la marque. En puisant dans les sens du bonheur, de la peur, de l’excitation ou de la nostalgie, les professionnels du marketing peuvent concevoir des messages qui résonnent à un niveau plus profond, qui stimulent l’engagement et influencent le comportement des consommateurs. L’attrait émotionnel permet de diffuser un contenu plus pertinent et mémorisable, ce qui favorise la fidélité à la marque et encourage les actions souhaitées.

Les tactiques de persuasion, les émotions marketing et les styles narratifs fonctionnent ensemble pour cibler les segments de clientèle.

- **Les styles narratifs** tels que l’authenticité, la célébration et la communauté, permettent de véhiculer les valeurs et l’identité qui trouvent un écho auprès du public cible, créant ainsi un message plus attrayant et plus facilement identifiable.
- Les **tactiques de persuasion** telles que la rareté, les preuves sociales et la réciprocité, sont conçues pour influencer le comportement des consommateurs en faisant appel à leurs émotions et à leurs préférences.
- **Les émotions marketing** visent à stimuler les sentiments qui améliorent l&#39;engagement et la connexion avec la marque.

L’IA de GenStudio for Performance Marketing détecte et distingue ces caractéristiques en analysant le texte à la recherche de signaux émotionnels, de ton et de style narratif. L’IA utilise le traitement du langage naturel (NLP) et des algorithmes de machine learning pour identifier des modèles et classer le texte en fonction d’attributs émotionnels et persuasifs prédéfinis.

### Style narratif

Les attributs narratifs, ou facteurs d’attrait, permettent d’identifier les médias qui communiquent les valeurs, l’objectif ou l’identité qui trouvent un écho auprès de votre audience cible. Le tableau suivant répertorie les styles narratifs reconnus par l’IA dédiée à GenStudio for Performance Marketing.

| Facteur d&#39;appel | Description | Exemple |
| ----------------- | --------------------------------------------------------------------- | ------------------------------------------ |
| Authenticité | Authentique et réel, mettant souvent en avant la transparence et l&#39;honnêteté. | `A behind-the-scenes look at how our products are made.` |
| Célébration | Marquer des occasions spéciales ou des réalisations avec joie et festivité. | `Join us in celebrating our 10th anniversary with special offers!` |
| Communauté | Favoriser un sentiment d&#39;appartenance et de solidarité au sein d&#39;un groupe. | `Our brand is built on the strength of our community.` |
| Convivialité | Mettant l’accent sur la facilité d’utilisation et les avantages de gagner du temps. | `Get what you need with just one click.` |
| Autonomisation | Encourager et permettre aux individus de prendre le contrôle et les décisions. | `Empower yourself with our latest tools and resources.` |
| Exploration | Inviter à la découverte et à l&#39;aventure, souvent associée à de nouvelles expériences. | `Discover new horizons with our travel packages.` |
| Futuriste | Souligner l&#39;innovation et les idées avant-gardistes. | `Experience the future of technology today.` |
| Battage | Générer de l’excitation et de l’anticipation concernant un produit ou un événement. | `Don't miss out on the most anticipated event of the year!` |
| Indulgence | Séduisant par les fantasmes, les désirs ou les plaisirs. | `Treat yourself to the finest gourmet chocolates.` |
| Tranquillité d&#39;esprit | Rassurer et donner un sentiment de sécurité. | `Rest easy knowing your data is safe with us.` |
| Personnalisation | Adaptation des expériences ou des produits aux préférences individuelles. | `Get a custom-fit solution just for you.` |
| Prestige | Associer à un statut élevé et à l’exclusivité. | `Join the elite with our premium membership.` |
| Timelessness | Soulignant la qualité durable et l&#39;attrait classique. | `Our designs are timeless and never go out of style.` |
| Polyvalence | Mise en évidence de l’adaptabilité et des utilisations multiples. | `Our product fits seamlessly into any lifestyle.` |
| Bien-être | Favoriser la santé, le bonheur et le bien-être général. | `Enhance your well-being with our holistic approach.` |

### Tactique de persuasion

Les techniques de persuasion sont utilisées pour influencer le comportement des consommateurs et stimuler les actions souhaitées. Ces stratégies ciblent des déclencheurs psychologiques et des segments de clientèle spécifiques pour améliorer l’efficacité des messages marketing. Le tableau suivant répertorie les tactiques de persuasion reconnues par l’IA dédiée à GenStudio for Performance Marketing.

| Tactique | Description | Exemple |
| --------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Anthropomorphisme | Attribuer des caractéristiques humaines à des produits ou à des marques. | `Our friendly chatbot is here to help you.` |
| Comparaison | Mettre en évidence les différences entre les options pour influencer le choix. | `See how we compare to the competition.` |
| Concretesse | Fournir des détails spécifiques pour rendre le message plus tangible. | `Save 20% on your next purchase.` |
| Soutien | Avec l&#39;approbation de sources crédibles ou d&#39;influenceurs. | `Recommended by top industry experts.` |
| Pied dans la porte | En commençant par une petite demande pour augmenter la probabilité d’accord sur une demande plus grande. | `Try our free trial today.` |
| Surmonter la réactance | Réduire la résistance en reconnaissant et en traitant les objections. | `We understand your concerns, and here's how we address them.` |
| Réciprocité | Offrir quelque chose de valeur pour encourager une faveur de retour. | `Get a free gift with your purchase.` |
| Rareté | Créer un sentiment d’urgence en soulignant la disponibilité limitée. | `Only a few items left in stock!` |
| Identité sociale | Exploiter le sentiment d&#39;appartenance du consommateur à un groupe. | `Join our community of innovators.` |
| Impact social | Soulignant l&#39;impact positif sur la société ou l&#39;environnement. | `Your purchase helps plant a tree.` |
| Preuve sociale | Utiliser des témoignages ou du contenu généré par l’utilisateur pour établir la confiance. | `See why thousands of users love our product.` |

### Émotions marketing

Les émotions sont ciblées dans les messages marketing pour évoquer des sentiments et des réponses spécifiques du public, ce qui peut améliorer l&#39;engagement et la connexion avec la marque. Le tableau suivant répertorie les émotions reconnues par l’IA dédiée à GenStudio for Performance Marketing.

| Émotion | Description | Exemple |
| ------------- | --------------------------------------------------------------------------- | --------------------------------------------------------- |
| Aspiration | Inspirer un désir d&#39;accomplir ou d&#39;atteindre quelque chose de plus grand. | `Imagine the possibilities with our premium service.` |
| Difficulté | Encourager le public à surmonter un obstacle ou à entreprendre une nouvelle tâche. | `Are you ready to take the next step in your career?` |
| Curiosité | Susciter l&#39;intérêt et le désir d&#39;en apprendre davantage. | `Discover the secrets behind our success.` |
| Exclusivité | Créer le sentiment de faire partie d’un groupe restreint. | `Join our exclusive club for members-only benefits.` |
| Fascination | Captivez le public avec du contenu fascinant ou passionnant. | `Be amazed by our latest innovations.` |
| Satisfaction | Satisfaction et plaisir d&#39;utiliser le produit ou le service. | `Enjoy the ultimate comfort with our luxury bedding.` |
| Reconnaissance | Reconnaître et évaluer les réussites ou le statut de l’audience. | `Get the recognition you deserve with our award-winning service.` |
| Confiance | Renforcer la confiance et la fiabilité de la marque. | `Trust us to deliver quality and excellence every time.` |
| Urgence | Favoriser une action immédiate en mettant l&#39;accent sur les opportunités urgentes. | `Act now before this limited-time offer expires!` |

## Score de lisibilité

Le score de lisibilité évalue la facilité de lecture et de compréhension d’un texte. Cela permet de s’assurer que votre contenu est adapté à votre audience cible. Les scores sont basés sur divers facteurs, notamment la longueur de la phrase et la complexité des mots. Le tableau suivant répertorie les niveaux de lisibilité reconnus par l’IA dédiée à GenStudio for Performance Marketing.

| Niveau de lisibilité | Description | Exemple |
| ------------------- | ------------------------------------------------------------------ | --------------------------------------------------------- |
| 5e année | Langage très simple, adapté aux jeunes enfants. | `The cat sat on the mat.` |
| 6e année | Langage simple et clair, adapté à un public général. | `You can find great deals on our website.` |
| 7e année | Facile à comprendre, avec un vocabulaire et une structure simples. | `Our new product is simple to use and very effective.` |
| 8ème et 9ème année | Langage clair et concis, adapté aux adolescents. | `This guide will help you understand the basics of our service.` |
| de la 10e à la 12e année | Langage plus complexe, adapté aux adolescents plus âgés et aux adultes. | `The comprehensive manual provides detailed instructions for setup.` |
| Collège | Langage avancé, adapté à un public instruit. | `The study explores the multifaceted implications of the new policy.` |
| Diplômé de l&#39;université | Langage très avancé, adapté aux experts et aux spécialistes. | `The dissertation delves into the intricacies of quantum mechanics.` |

## Comptages

La compréhension et l’exploitation des attributs de comptage, tels que le nombre de hashtags, le nombre de mots, le nombre de phrases et les ratios d’arrêts de mots, peuvent améliorer considérablement votre stratégie de contenu. Ces mesures offrent des informations précieuses sur l’efficacité et la portée de vos efforts marketing. Le tableau suivant répertorie les catégories de comptage reconnues par l’IA dédiée à GenStudio for Performance Marketing.

| Catégorie | Description | Exemple |
| --------------------- | --------------------------------------------------------------------------- | --------------------- |
| Nombre d’émotions | Nombre d’émoticônes présentes dans le texte. Les émotions peuvent améliorer l’engagement et transmettre rapidement les émotions. | `😊`, `🚀`, `❤️` |
| Nombre de balises de hachage | Nombre de hashtags utilisés dans le texte. Les hashtags permettent de catégoriser le contenu et d&#39;augmenter la visibilité sur les médias sociaux. | `#Marketing`, `#Sale` |
| Nombre de mots par phrase | Nombre moyen de mots par phrase dans le texte. Les phrases plus courtes sont souvent plus faciles à lire et à comprendre. | `10` |
| Nombre de mots | Nombre total de mots dans le texte. Un nombre de mots plus élevé peut fournir des informations plus détaillées, mais peut également nécessiter davantage d’effort de lecture. | `1500 words` |
| Proportion de mots vides | Rapport entre les mots vides et les mots significatifs dans le texte. Les mots vides (tels que « a » « an » « the ») sont souvent ignorés dans les requêtes et les résultats de recherche. Un taux élevé de mots vides peut rendre le contenu moins attrayant et plus difficile à lire. | `0.375` |
| Nombre de phrases | Nombre total de phrases dans le texte. Plus de phrases peuvent indiquer un contenu plus détaillé, mais des textes trop longs peuvent perdre l&#39;intérêt du lecteur. | `75 sentences` |
