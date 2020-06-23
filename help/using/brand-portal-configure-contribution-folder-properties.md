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
source-git-commit: d0c5adad47fdc83adfad79bae4119cb6d38caf5e
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# Konfigurera egenskaper för bidragsmapp {#configure-contribution-folder-properties}

AEM-administratören utför följande åtgärder när egenskaperna för en avgiftsmapp konfigureras.

* **Lägg till beskrivning**: Ange en beskrivning av bidragsmappen på hög nivå.
* **Överför i korthet**:  Överför tillgångskravsdokument som innehåller resursrelaterad information.
* **Lägg till medverkande**: Lägg till Brand Portal-användare eller -grupper för att ge dem åtkomst till mappen för bidrag.

Resurskravet avser den information som administratörer tillhandahåller för att hjälpa medverkande (varumärkesportalanvändare) att förstå behovet och kraven av bidragsmappen. Administratören överför ett tillgångskravsdokument som innehåller en sammanfattning om vilken typ av resurser som ska läggas till i avgiftsmappen och resursrelaterad information, till exempel syfte, typ av bilder, maxstorlek osv.

Administratören kan sedan ge Brand Portal-användare/grupper åtkomst till mappen för bidrag innan den nya Contribute-mappen publiceras på varumärkesportalen.

**Så här konfigurerar du bidragsmappens egenskaper:**
1. Logga in på din AEM-författarinstansStandard-URL: http:// localhost:4502/aem/start.html
1. Navigera till **[!UICONTROL Assets > Files]** och hitta mappen för bidrag.
1. Välj mapp för bidrag och klicka på **[!UICONTROL Properties]**![](assets/properties.png). Fönstret Mappegenskaper öppnas.
   ![](assets/contribution-folder-property1.png)
1. Navigate to **[!UICONTROL Asset Contribution]** tab.
1. Ange en hög nivå **[!UICONTROL Description]** för mappen för bidrag.
1. Klicka **[!UICONTROL Upload Brief]** för ![](assets/upload.png) att bläddra från den lokala datorn och ladda upp ett **tillgångskravsdokument**.
1. I **[!UICONTROL Add User or Group]** söker du efter och **[!UICONTROL Add]** på varumärkesportalen som du vill dela mappen för bidrag med. Det går inte att tilldela grupper en distributionsmapp.
Dessa Brand Portal-användare har behörighet att komma åt mappen för bidrag och överföra innehåll från gränssnittet för varumärkesportalen utan att behöva komma åt AEM-författarinstansen.

1. Klicka på **[!UICONTROL Save]**.
   ![](assets/contribution-folder-property2.png)

>[!NOTE]
>
>Sökresultaten baseras på användarlistan för varumärkesportalen som konfigurerats i AEM Assets. Se till att du har den uppdaterade användarlistan för varumärkesportalen. Se Användarlista för [Överför varumärkesportal](brand-portal-configure-asset-sourcing.md).

