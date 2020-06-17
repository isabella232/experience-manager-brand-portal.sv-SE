---
title: Skapa Contribute-mapp
seo-title: Skapa Contribute-mapp
description: 'Få insikt i hur du skapar en mapp för bidrag i AEM Assets. '
seo-description: Få insikt i hur du skapar en mapp för bidrag i AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ac5952c318baae8400928592d9a372ab966191cf
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# Skapa avgiftsmapp {#create-contribution-folder}

AEM-administratörer och icke-adminanvändare som har behörighet att skapa en ny mapp kan skapa en **Contribute** -mapp i AEM Assets.
Om du vill skapa en **Contribute** -mapp skapar du en ny mapp av typen **Asset Contribution**, som ser till att den nya mappen som skapas är öppen för att skickas in av Brand Portal-användare.  Detta utlöser automatiskt ett arbetsflöde som skapar ytterligare två undermappar, **delade** och **NYA**, i den nya **Contribute** -mappen.

**Så här skapar du en ny bidragsmapp:**
1. Logga in på din AEM-författarinstansStandard-URL: http:// localhost:4502/aem/start.html
1. Navigera till **[!UICONTROL Assets > Files]** Den visar alla befintliga mappar i AEM Assets-databasen.
1. Klicka **[!UICONTROL Create]** för att skapa en ny mapp. Popup-fönstret Skapa mapp öppnas.
1. Ange **[!UICONTROL Title]** och **[!UICONTROL Name]** markera kryssrutan **[!UICONTROL Asset Contribution]**.
Du bör använda små alfabet utan blanksteg för att namnge mappen.
1. Klicka på **[!UICONTROL Create]**.
   ![](assets/create-contribution-folder.png)
1. Du kan se den nyligen skapade mappen för bidrag i AEM Assets-databasen.
1. Klicka för att öppna mappen för bidrag, du kan se två undermappar **[!UICONTROL SHARED]** och **[!UICONTROL NEW]** skapas automatiskt i mappen för bidrag.\
   ![](assets/contribution-folder.png)

Du kan nu konfigurera Contribute-mappens egenskaper. Se [Konfigurera egenskaper](brand-portal-configure-contribution-folder-properties.md)för Contribute-mappen.

>[!NOTE]
>
>Se till att du ger Contribute-mappen ett lämpligt namn eftersom du inte kan ändra mappnamnet när du har skapat det.
>
>Kapsling av Contribute-mappen stöds inte. Skapa inte en Contribute-mapp i en annan Contribute-mapp.

