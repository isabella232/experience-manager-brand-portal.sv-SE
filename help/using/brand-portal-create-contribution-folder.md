---
title: Skapa Contribute-mapp
seo-title: Skapa Contribute-mapp
description: 'Få information om hur du skapar en mapp för bidrag i AEM Assets. '
seo-description: Få information om hur du skapar en mapp för bidrag i AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ca71b51ea51a92f23fc4c7d6682f73c4c204a5f2

---


# Skapa avgiftsmapp {#create-contribution-folder}

AEM-administratörer och icke-adminanvändare som har behörighet att skapa en ny mapp kan skapa en **Contribute** -mapp i AEM Resurser.
Om du vill skapa en **Contribute** -mapp skapar du en ny mapp av typen **Asset Contribution**, som ser till att den nya mappen som skapas är öppen för att skickas in av Brand Portal-användare.  Detta utlöser automatiskt ett arbetsflöde som skapar ytterligare två undermappar, **delade** och **NYA**, i den nya **Contribute** -mappen.

**Så här skapar du en ny bidragsmapp:**
1. Logga in på din AEM-författarinstansStandard-URL: http:// localhost:4502/aem/start.html
1. Navigera till **[!UICONTROL Resurser > Filer]** Den visar alla befintliga mappar i AEM Resurser-databasen.
1. Klicka på **[!UICONTROL Skapa]** för att skapa en ny mapp. Popup-fönstret Skapa mapp öppnas.
1. Ange **[!UICONTROL mappens namn]** och **[!UICONTROL namn]** och markera kryssrutan **[!UICONTROL Resursbidrag]**.
Du bör använda små alfabet utan blanksteg för att namnge mappen.
1. Klicka på **[!UICONTROL Skapa]**.
   ![](assets/create-contribution-folder.png)
1. Du kan se den nyligen skapade mappen för bidrag i AEM Resurser-databasen.
1. Klicka för att öppna mappen för bidrag så ser du att två undermappar -**[!UICONTROL DELADE]** och **[!UICONTROL NYA]** - automatiskt skapas i mappen för bidrag.\
   ![](assets/contribution-folder.png)

Du kan nu konfigurera Contribute-mappens egenskaper. Se [Konfigurera egenskaper](brand-portal-configure-contribution-folder-properties.md)för Contribute-mappen.

>[!NOTE]
>
>Se till att du ger Contribute-mappen ett lämpligt namn eftersom du inte kan ändra mappnamnet när du har skapat det.