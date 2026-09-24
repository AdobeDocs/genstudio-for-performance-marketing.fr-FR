---
title: Générer et affiner le contenu avec la génération dynamique
description: Découvrez comment générer du contenu intégré à la marque et l’affiner tour à tour dans une conversation avec des empreintes vocales et des repères visuels dans [!DNL GenStudio for Performance Marketing].
feature: Create Prompt, Generative AI, Content Generation
role: User
level: Beginner
source-git-commit: 22db02c07a9f33cb1c70df9286ad6eb143dafd38
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%
---
# Générer et affiner le contenu avec la génération avec état

[!DNL GenStudio for Performance Marketing] utilise la génération avec état pour vous aider à créer du contenu sur la marque, puis à l’affiner tour à tour dans une conversation, au lieu de recommencer à chaque fois avec une nouvelle invite. Au fur et à mesure que vous affinez, la génération se souvient de vos instructions précédentes et des variantes que vous conservez, puis applique uniquement la modification que vous demandez.

La génération avec état ajoute trois types de contexte à vos générations : l’impression vocale conserve une copie dans la voix de votre marque, les repères visuels une copie au sol dans une image ou une vidéo, et une URL de page web ajoute un contexte de référence à partir d’une page que vous choisissez.

## Générer et affiner le contenu

1. Dans [!DNL GenStudio for Performance Marketing], démarrez une génération pour votre canal et votre format. Consultez la [[!DNL Create] présentation](/help/user-guide/create/overview.md) pour commencer une génération pour chaque canal.
1. _Facultatif_ : pour ancrer la copie dans votre propre contenu créatif, sélectionnez **[!UICONTROL Sélectionner dans le contenu]**, puis choisissez une image ou une vidéo à utiliser comme [repère visuel](#ground-content-in-an-image-or-video).
1. Sélectionnez **[!UICONTROL Générer]**. [!DNL GenStudio for Performance Marketing] crée un ensemble de variantes et applique automatiquement votre [voix de marque](#keep-copy-in-your-brand-voice) sur les canaux pris en charge.
1. Affinez les résultats dans le tiroir de l’invite. Saisissez la modification souhaitée, par exemple `shorten the headline`, `make variant 2 punchier` ou `change the headline`. La génération applique uniquement cette modification et conserve vos instructions précédentes.
1. Pour conserver une variante pendant que vous continuez à affiner, saisissez une instruction dans le tiroir d’invite, telle que `keep variant 2`.
1. Lorsque le contenu est prêt, exportez-le ou envoyez-le pour révision.

## Contenu au sol dans une image ou une vidéo

Les repères visuels permettent à la génération de lire une image ou une vidéo que vous joignez, puis d’écrire une copie reflétant cette création. Le bouton (bascule) **[!UICONTROL Options de]** contrôle les repères visuels et est activé par défaut.

Pour utiliser un indice visuel, sélectionnez **[!UICONTROL Sélectionner à partir du contenu]** et choisissez une image ou une vidéo avant de la générer. Pour générer sans repère visuel, désactivez **[!UICONTROL les options de]**.

>[!NOTE]
>Les repères visuels ne sont pas disponibles pour les publicités display à plusieurs images ou les publicités de carrousel.

## Conserver une copie dans la voix de votre marque

La technique d’impression vocale applique la voix apprise de votre marque à la copie générée, de sorte qu’elle sonne sur la marque sans invite supplémentaire. Elle est activée par défaut pour les canaux qui ont des [&#x200B; Insights](/help/user-guide/insights/overview.md) tels que LinkedIn et Meta.

## Utiliser une page web comme contexte

Vous pouvez pointer la génération vers une page web et utiliser son contenu comme contexte. Dans le tiroir d’invite, saisissez une instruction contenant l’URL, telle que `Use this URL to generate an ad for this channel: https://www.example.com`.

>[!NOTE]
>Saisissez l’URL dans votre invite. Ne l&#39;ajoutez pas via _Paramètres_.

## Fonctionnalités connexes

- [Gérer les variantes](/help/user-guide/create/manage-variants.md) : modifiez et affinez les variantes générées directement sur la zone de travail.
- [Rédiger des invites efficaces](/help/user-guide/effective-prompts.md) : crée des invites qui génèrent de meilleurs résultats.
