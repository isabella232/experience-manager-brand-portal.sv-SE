---
title: Överför resurser och publicera Contribute-mappen från Brand Portal till Experience Manager Assets
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: Få insikt i hur du överför nya resurser och publicerar bidragsmappen från Brand Portal till Experience Manager Assets.
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: e95dbff93ec4d207fe32a1752f9ccf59ee7c4e90
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Publicera en mapp för bidrag till Experience Manager Assets {#using-asset-souring-in-bp}

Brand Portal-användare med lämplig behörighet kan överföra flera resurser, eller mappar som innehåller flera resurser, till bidragsmappen. Brand Portal-användare kan dock bara överföra resurser till mappen **NEW**. Mappen **SHARED** är avsedd för distribution av baslinjeresurser (referensinnehåll) som kan användas av Brand Portal-användare när nya resurser skapas för bidrag.

Brand Portal-användare som har behörighet att komma åt mappen för bidrag kan utföra följande åtgärder:

* [Hämta resurskrav](#download-asset-requirements)
* [Överför nya resurser till mappen för bidrag](#uplad-new-assets-to-contribution-folder)
* [Publicera en mapp för bidrag till Experience Manager Assets](#publish-contribution-folder-to-aem)

## Hämta resurskrav {#download-asset-requirements}

Brand Portal-användare får automatiskt e-post-/pulsmeddelanden varje gång en avgiftsbelagda mapp delas av Experience Manager Assets-användaren, så att de kan hämta det korta (resurskrav) dokumentet samt hämta basresurserna (referensinnehåll) från **DELADE**-mappen för att vara säkra på att de förstår tillgångskraven.

Brand Portal-användare utför följande åtgärder för att ladda ned mediefiler:

* **Ladda ned i korthet**: Ladda ned översikten (tillgångskravsdokument) som är bifogad till mappen för bidrag och som innehåller resursrelaterad information som typ av resurser, syfte, format som stöds, maximal storlek på mediefilen osv.
* **Hämta baslinjeresurser**: Hämta baslinjeresurser som kan användas för att förstå vilka typer av resurser som krävs. Brand Portal-användare kan använda dessa resurser som referens för att skapa nya resurser som kan bidra.

Brand Portal Dashboard visar alla befintliga mappar som är tillåtna för Brand Portal-användaren tillsammans med den nyligen delade bidragsmappen. I det här exemplet har Brand Portal-användaren bara åtkomst till den nyligen skapade mappen för bidrag, ingen annan befintlig mapp delas med användaren.

**Så här hämtar du resurskrav:**

1. Logga in på din Brand Portal-instans.
1. Välj mapp för bidrag från Brand Portal Dashboard.
1. Klicka på **[!UICONTROL Properties]**. Fönstret Egenskap som innehåller informationen om bidragsmappen öppnas.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. Klicka på alternativet **[!UICONTROL Download Brief]** om du vill hämta tillgångskravsdokumentet på den lokala datorn.

   ![](assets/download.png)

1. Gå tillbaka till Brand Portal Dashboard.
1. Klicka för att öppna mappen för bidrag, du kan se två undermappar -**[!UICONTROL SHARED]** och **[!UICONTROL NEW]** i mappen för bidrag. Mappen SHARED innehåller alla baslinjeresurser (referensinnehåll) som delas av administratörerna.
1. Du kan hämta mappen **[!UICONTROL SHARED]** som innehåller alla baslinjeresurser på den lokala datorn.
Du kan också öppna mappen **[!UICONTROL SHARED]** och klicka på ikonen **Hämta** för att hämta enskilda filer/mappar.

   ![](assets/download.png)

   ![](assets/download-asset-requirement4.png)

Gå igenom översikten (tillgångskravsdokument) och hänvisa till bastillgångarna för att förstå tillgångskraven. Nu kan du skapa nya resurser för bidrag och överföra dem till mappen för bidrag.


## Överför resurser till mappen för bidrag {#uplad-new-assets-to-contribution-folder}

Efter att ha gått igenom resurskraven kan Brand Portal-användare skapa nya resurser för bidrag och överföra dem till mappen NEW i mappen för bidrag.

>[!NOTE]
>
>Brand Portal-användare kan bara överföra resurser till mappen NEW.
>
>Den maximala överföringsgränsen för alla Brand Portal-klientorganisationer är **10** GB, som tillämpas kumulativt på alla bidragsmappar.

>[!NOTE]
>
>Vi rekommenderar att du frigör överföringsutrymmet efter att du har publicerat bidragsmappen till Experience Manager Assets så att den är tillgänglig för övriga Brand Portal-användare för bidrag.
>
>Om du behöver utöka din Brand Portal-klientorganisations överföringsgräns utöver **10** GB kontaktar du kundsupport och anger kraven.


**Så här överför du nya resurser:**

1. Logga in på din Brand Portal-instans.
På Brand Portal-kontrollpanelen visas alla befintliga mappar som är tillåtna för Brand Portal-användaren tillsammans med den nyligen delade bidragsmappen.

1. Markera mappen för bidrag och klicka för att öppna den. Mappen för bidrag innehåller två undermappar - **[!UICONTROL SHARED]** och **[!UICONTROL NEW]**.

1. Klicka på mappen **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets4.png)

1. Klicka på **[!UICONTROL Create]** > **[!UICONTROL Files]** om du vill överföra enskilda filer eller mappar (.zip) som innehåller flera resurser.

   ![](assets/upload-new-assets5.png)

1. Bläddra och överför resurser (filer eller mappar) till mappen **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets6.png)

När du har överfört alla resurser eller mappar till mappen NYTT publicerar du mappen för bidrag till Experience Manager Assets.


## Publicera en mapp för bidrag till Experience Manager Assets {#publish-contribution-folder-to-aem}

Brand Portal-användare kan publicera bidragsmappen på Experience Manager Assets utan att ha tillgång till författarinstansen i Experience Manager.

Se till att du har gått igenom resurskraven och överför de nyskapade resurserna i mappen **NEW** i mappen för bidrag.

**Så här publicerar du bidragsmappen:**

1. Logga in på din Brand Portal-instans.

1. Välj mapp för bidrag från Brand Portal Dashboard.
1. Klicka på **[!UICONTROL Publish to AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

Ett e-post-/pulsmeddelande skickas till Brand Portal-användare och -administratörer i olika stadier av publiceringsarbetsflödet:

1. **Köad**  - Ett meddelande skickas till Brand Portal-användare och Brand Portal-administratörer när ett publiceringsarbetsflöde utlöses i Brand Portal.

1. **Fullständigt**  - Ett meddelande skickas till Brand Portal-användare och Brand Portal-administratörer när mappen för bidrag har publicerats i Experience Manager Assets.

När de nyskapade resurserna har publicerats i Experience Manager Assets kan Brand Portal-användarna ta bort dem från mappen NEW. Brand Portal-administratören kan ta bort resurserna från både NYTT och Delat.

När målet att skapa bidragsmappen är uppfyllt kan Brand Portal-administratören ta bort bidragsmappen och frigöra överföringsutrymmet för andra användare.

## Status för publiceringsjobb {#publishing-job-status}

Det finns två rapporter som administratörer kan använda för att visa statusen för resursavgiftsmapparna som publicerats från Brand Portal till Experience Manager Assets.

* I Brand Portal går du till **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]**. Den här rapporten visar statusen för alla publiceringsjobb i olika faser av publiceringsarbetsflödet.

   ![](assets/contribution-folder-status.png)

* Gå till **[!UICONTROL Assets]** > **[!UICONTROL Jobs]** i Experience Manager Assets (lokal eller hanterad tjänst). Den här rapporten visar det slutliga tillståndet (Slutfört eller Fel) för alla publiceringsjobb.

   ![](assets/publishing-status.png)

* Navigera till **[!UICONTROL Assets]** > **[!UICONTROL Jobs]** i Experience Manager Assets som Cloud Service.

   Du kan också navigera direkt till **[!UICONTROL Jobs]** från den globala navigeringen.

   Den här rapporten visar det slutliga läget (Slutfört eller Fel) för alla publiceringsjobb, inklusive import av resurser från Brand Portal till Experience Manager Assets som en Cloud Service.

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->
