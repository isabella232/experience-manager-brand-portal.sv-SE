---
title: Konfigurera egenskaper för Contribute-mapp
seo-title: Konfigurera egenskaper för Contribute-mapp
description: 'Få information om hur du konfigurerar egenskaperna för en bidragsmapp i AEM Assets. '
seo-description: 'Få information om hur du konfigurerar egenskaperna för en bidragsmapp i AEM Assets. '
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
version: 6.5
discoiquuid: null
translation-type: tm+mt
source-git-commit: 0a3f1a4379398730e92e9ac85b04134f92af9d23
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Konfigurera egenskaper för bidragsmapp {#configure-contribution-folder-properties}

AEM utför följande åtgärder när du konfigurerar egenskaperna för en avgiftsmapp.

* **Lägg till beskrivning**: Ange en beskrivning av bidragsmappen på hög nivå.
* **Överför i korthet**:  Överför tillgångskravsdokument som innehåller resursrelaterad information.
* **Lägg till medverkande**: Lägg till Brand Portal-användare för att ge dem åtkomst till mappen för bidrag.

Resurskravet avser den information som administratörer tillhandahåller för att hjälpa medverkande (varumärkesportalanvändare) att förstå behovet och kraven av bidragsmappen. Administratören överför ett tillgångskravsdokument som innehåller en sammanfattning om vilken typ av resurser som ska läggas till i avgiftsmappen och resursrelaterad information, till exempel syfte, typ av bilder, maxstorlek osv.

**Så här konfigurerar du bidragsmappens egenskaper:**

1. Logga in på AEM författarinstansStandard-URL: http:// localhost:4502/aem/start.html
1. Navigera till **[!UICONTROL Assets > Files]** och hitta mappen för bidrag.
1. Välj mapp för bidrag och klicka på **[!UICONTROL Properties]** för att öppna fönstret Mappegenskaper.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Navigate to **[!UICONTROL Asset Contribution]** tab.
1. Ange en hög nivå **[!UICONTROL Description]** för mappen för bidrag.
1. Klicka **[!UICONTROL Upload Brief]** för att bläddra från den lokala datorn och ladda upp ett **tillgångskravsdokument**.

   ![](assets/upload.png)

1. I **[!UICONTROL Add User or Group]** fältet lägger du till Brand Portal-användare som du vill dela mappen för bidrag med. Dessa användare kan komma åt och överföra innehåll till mappen för bidrag via gränssnittet för varumärkesportalen.
1. Klicka på **[!UICONTROL Save]**.

   ![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>För närvarande kan inte grupper tilldelas till en avgiftsmapp.
>
>Sökresultaten baseras på användarlistan i varumärkesportalen som konfigurerats i AEM Assets. Se till att du har den uppdaterade användarlistan för varumärkesportalen. Se Användarlista för [Överför varumärkesportal](brand-portal-configure-asset-sourcing.md).
