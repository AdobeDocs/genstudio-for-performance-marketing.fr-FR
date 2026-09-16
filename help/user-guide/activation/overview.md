---
title: Vue d’ensemble d’Activate
description: Découvrez comment activer du contenu avec Adobe CX Enterprise et des applications tierces.
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
source-git-commit: 17b2262615e10d82905ce7ebec65857e9a0b9f2a
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 5%
---
# Adobe GenStudio for Performance Marketing Activate

GenStudio for Performance Marketing [!DNL Activate] vous permet de préparer et d’envoyer des expériences publicitaires aux canaux de publicités payantes, tels que Meta ou LinkedIn. _Activation_ prend une expérience publicitaire approuvée et ses ressources, applique la configuration requise par un canal spécifique, puis la diffuse directement à ce canal dans un statut inactif, désactivé. À partir de là, vous pouvez effectuer une révision finale dans le propre gestionnaire d’annonces publicitaires du canal avant que votre annonce ne soit publiée.

[!DNL Activate] diffuse directement votre expérience sur le canal, de sorte que vous n’ayez pas besoin d’exporter des fichiers ou de les charger manuellement vers le propre gestionnaire de publicités du canal.

Un gestionnaire ou un éditeur de système GenStudio doit connecter le compte publicitaire de chaque canal publicitaire payant avant de pouvoir activer une expérience publicitaire sur ce canal.

## Fonctionnalités d’Activate

Utilisez [!DNL Activate] pour préparer des expériences publicitaires pour leurs canaux de publicités payantes cibles. [Activez des expériences en bloc](create-activation.md) sur plusieurs canaux d’annonces payantes dans un seul tableau d’activation. Ensuite, [gérez vos activations](manage-activations.md) pour afficher le statut et les détails de chaque expérience activée.

>[!VIDEO](https://video.tv.adobe.com/v/3503540?captions=fre_fr&learn=on)

### Activer les expériences approuvées à partir du contenu

Sélectionnez une ou plusieurs expériences approuvées et publiées dans [!DNL Content] ou commencez à partir de la page de destination [!DNL Activate]. Contrairement aux versions précédentes d’[!DNL Activate], un seul tableau d’activation peut inclure des expériences pour plusieurs canaux d’annonces payantes à la fois, organisés par format et canal d’annonce.

>[!NOTE]
>
>[!DNL Content] appelle une destination telle que Meta ou LinkedIn sur un **canal**. [!DNL Activate] appelle la même destination une **plateforme** (par exemple, dans la **[!UICONTROL configuration de Platform]**). Les deux termes renvoient à la même chose.

### Configuration des détails de configuration de la publicité et de la plateforme

Chaque ligne du tableau d’activation représente une annonce publicitaire. Les ressources de création, les titres et la copie du corps approuvés sont verrouillés, car ils ont déjà été examinés et approuvés. Vous pouvez modifier les champs restants, tels que le texte call-to-action, l’URL de destination et les détails de configuration de la plateforme, tels que le compte publicitaire, la campagne et la visionneuse d’annonces. Modifiez les champs d’une ligne à la fois ou sélectionnez plusieurs lignes pour modifier les champs partagés en bloc.

### Examinez et publiez vos expériences sur leurs canaux publicitaires

Vérifiez que chaque ligne indique [!UICONTROL Prêt pour l’activation]. [!DNL Activate] signale les champs manquants ou non valides, les appels à l’action incompatibles et duplique les identifiants de suivi selon les [!UICONTROL Attention requise]. Lorsque chaque ligne est prête, cliquez sur **[!UICONTROL Envoyer à Platform]** pour publier toutes les annonces du tableau. [!DNL Activate] signale le statut de chaque publicité en temps quasi réel. Les publicités publiées avec succès incluent un lien profond vers la publicité dans le gestionnaire de publicités natif de la plateforme de destination. Les publicités ayant échoué renvoient un message d’erreur et peuvent être réessayées.
