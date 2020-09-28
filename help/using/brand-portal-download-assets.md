---
title: Hämta resurser
seo-title: Hämta resurser
description: Alla användare kan samtidigt hämta flera resurser och mappar som är tillgängliga för dem. På så sätt kan godkända varumärkesresurser distribueras säkert för användning offline.
seo-description: Alla användare kan samtidigt hämta flera resurser och mappar som är tillgängliga för dem. På så sätt kan godkända varumärkesresurser distribueras säkert för användning offline.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: e497fb791030d74d9e5672b68387661ca7140d8a
workflow-type: tm+mt
source-wordcount: '1228'
ht-degree: 0%

---


# Hämta resurser {#download-assets}

<!-- Before update in Download experience - 26th Aug 2020 by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal förbättrar nedladdningen genom att användarna samtidigt kan hämta flera resurser och mappar som är tillgängliga för dem från Brand Portal. På så sätt kan godkända varumärkesresurser distribueras säkert för användning offline. Läs vidare för att lära dig hur du hämtar godkända resurser från Brand Portal och vad du kan förvänta dig av [hämtningsprestanda](../using/brand-portal-download-assets.md#expected-download-performance).

>[!NOTE]
>
>Installera IBM Aspera Connect 3.9.9 i webbläsartillägget innan du hämtar materialet från Brand Portal.


<!--
**Types of renditions in Brand Portal:**

* Original asset rendition

  It is the original binary of the asset uploaded in AEM Assets. 
  
  
* System renditions

  These are the thumbnail renditions which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 
  
* Custom renditions

  These are the additional renditions that an asset might have and its dynamic renditions. Any user can create additional custom renditions, whereas, only the AEM administrator can create dynamic renditions of an image in AEM Assets. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md).     
-->

## Konfigurera hämtning av resurser {#configure-download}

Med hämtningskonfigurationen kan administratören för varumärkesportalen definiera uppsättningen renderingar som är tillgängliga för användarna i varumärkesportalen för hämtning av resurserna. Administratören kan konfigurera resursinställningarna **[!UICONTROL Download]** från gränssnittet för varumärkesportalen.

De tillgängliga konfigurationerna är:

* **[!UICONTROL Fast Download]**

   Möjliggör snabb hämtning av resurserna. Mer information finns i [guiden för att snabba upp hämtningar från varumärkesportalen](../using/accelerated-download.md).

* **[!UICONTROL Custom Renditions]**

   Hämta anpassade och (eller) dynamiska återgivningar av resurserna.
Alla återgivningar av resurser utöver den ursprungliga resursen och systemgenererade återgivningar kallas för anpassade återgivningar. Den innehåller både statiska och dynamiska renderingar som är tillgängliga för resursen. Alla användare kan skapa en anpassad statisk återgivning i AEM Assets, medan bara AEM kan skapa anpassade dynamiska återgivningar. Mer information finns i [Använda bildförinställningar eller dynamiska återgivningar](../using/brand-portal-image-presets.md)

* **[!UICONTROL System Renditions]**

   Hämta systemgenererade återgivningar av resurserna. Det här är miniatyrbilder som skapas automatiskt i AEM Assets baserat på arbetsflödet&quot;DAM-uppdateringsresurs&quot;.

Logga in som administratör på din varumärkesportal och navigera till **[!UICONTROL Tools]** > **[!UICONTROL Download]**. Som standard är **[!UICONTROL Fast Download]** konfigurationen aktiverad i **[!UICONTROL Download Settings]**.

Administratörerna kan aktivera valfri kombination för att konfigurera hämtningsprocessen för resurser.

![](assets/download-configuration.png)


Beroende på konfigurationen förblir hämtningsarbetsflödet konstant för fristående resurser, flera resurser, mappar som innehåller resurser, licensierade eller olicensierade resurser och för att hämta resurser med hjälp av delningslänken.


* Om både **[!UICONTROL Custom Renditions]** och **[!UICONTROL System Renditions]** konfigurationer är inaktiverade hämtas de ursprungliga återgivningarna av resurserna utan att någon ytterligare dialogruta visas för användarna.

<!--
If all the three download configurations are turned-off, or only the **[!UICONTROL Fast Download]** configuration is enabled, the original assets are directly downloaded on your local system with no additional step required.
Test.. 
-->

* Om någon av **[!UICONTROL Custom Renditions]** - eller **[!UICONTROL System Renditions]** konfigurationerna är aktiverad visas ytterligare en **[!UICONTROL Download]** dialogruta där du kan välja om du vill hämta den ursprungliga resursen tillsammans med dess återgivningar eller bara hämta specifika återgivningar.

>[!NOTE]
>
>Endast administratörer kan hämta utgångna resurser. Mer information om utgångna resurser finns i [Hantera digitala rättigheter för resurser](../using/manage-digital-rights-of-assets.md).


## Steg för att hämta resurser {#steps-to-download-assets}

Så här hämtar du resurser eller mappar som innehåller resurser från varumärkesportalen:

1. I gränssnittet för varumärkesportalen gör du något av följande:

   * Markera de mappar eller resurser som du vill hämta. Klicka på **[!UICONTROL Download]** ikonen i verktygsfältet överst.

      ![](assets/downloadassets-1.png)

   * Om du vill hämta en viss resurs eller mapp för du pekaren över resursen eller mappen och klickar på **[!UICONTROL Download]** ikonen som finns i miniatyrbilderna för snabbåtgärden.

      ![](assets/downloadsingleasset-1.png)


      >[!NOTE]
      >
      >Om du hämtar materialet för första gången och inte har IBM Aspera Connect installerat i webbläsaren uppmanas du att installera Aspera Download Accelerator.

      >[!NOTE]
      >
      >Om de mediefiler du hämtar också innehåller licensierade mediefiler omdirigeras du till **[!UICONTROL Copyright Management]** sidan. På den här sidan markerar du resurserna, klickar **[!UICONTROL Agree]** och sedan på **[!UICONTROL Download]**. Om du inte håller med hämtas inte licensierade mediefiler.
      > 
      >Licensskyddade mediefiler har [licensavtal som är kopplade](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) till dem, vilket görs genom att objektets [metadataegenskap](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) ställs in i Experience Manager Assets.

      ![](assets/licensed-asset-download-1.png)

      <!--
     >>[!NOTE]
     >
     >Ensure to select all the required asset renditions while downloading them from the asset details page, and click **[!UICONTROL Download]**. The selected renditions are downloaded to your local machine.
     > 
     >Once you download, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the downloaded renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.
     >
     -->

      Om någon av **[!UICONTROL Custom Renditions]** eller **[!UICONTROL System Renditions]** konfiguration är aktiverad i **[!UICONTROL Download Settings]** visas **[!UICONTROL Download]** dialogrutan med **[!UICONTROL Asset(s)]** kryssrutan markerad som standard. Om **[!UICONTROL Fast Download]** konfigurationen är aktiverad är kryssrutan markerad som standard **[!UICONTROL Enable download acceleration]** .

      ![](assets/download-dialog.png)

      >[!NOTE]
      >
      >Om de hämtade resurserna är bildfiler, och du bara markerar kryssrutan **[!UICONTROL Asset(s)]** i **[!UICONTROL Download]** dialogrutan men inte har [behörighet av administratören att få åtkomst till de ursprungliga återgivningarna av bildfiler](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) , hämtas inga bildfiler och ett meddelande visas som anger att du har begränsats av administratören för åtkomst till de ursprungliga återgivningarna.

      ![](assets/restrictaccess-note.png)

1. Markera kryssrutan om du vill hämta återgivningarna förutom de ursprungliga resurserna **[!UICONTROL Rendition(s)]** . Om du vill hämta de systemgenererade återgivningarna tillsammans med de anpassade återgivningarna avmarkerar du **[!UICONTROL Exclude System Renditions]** kryssrutan.

   ![](assets/download-system-rendition.png)

   * Om du bara vill hämta renderingarna avmarkerar du **[!UICONTROL Asset(s)]** kryssrutan.

      >[!NOTE]
      >
      >Som standard hämtas bara resurserna. Originalåtergivningar av bildfiler hämtas dock inte om du inte har [behörighet av administratören att ha tillgång till de ursprungliga återgivningarna av bildfiler](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * Markera kryssrutan om du vill dela de markerade resurserna med andra användare via en länk **[!UICONTROL Email]** . Ett e-postmeddelande skickas till användarna med nedladdningslänken. Mer information om hur du hämtar resurser från delade länkar finns i [Hämta resurser från delade länkar](../using/brand-portal-link-share.md#main-pars-header-1703469193).

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >Hämtningslänken i e-postmeddelanden upphör efter 45 dagar.
      >
      >Administratören kan anpassa e-postmeddelanden, det vill säga logotyp, beskrivning och sidfot, med hjälp av [funktionen Varumärke](../using/brand-portal-branding.md) .

   * Du kan välja en fördefinierad bildförinställning eller skapa en anpassad dynamisk återgivning i **[!UICONTROL Download]** dialogrutan.

      Om du vill använda en [anpassad bildförinställning för resursen och dess återgivningar](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages)markerar du **[!UICONTROL Dynamic Rendition(s)]** kryssrutan. Ange de förinställda bildegenskaperna (till exempel storlek, format, färgrymd, upplösning och bildmodifiering) för att använda den anpassade bildförinställningen när resursen och dess återgivningar hämtas. Om du bara vill hämta de dynamiska återgivningarna avmarkerar du **[!UICONTROL Asset(s)]** kryssrutan.

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal har stöd för att konfigurera Dynamic Media i både Hybird- och Scene 7-läge.
      >
      >(*Om AEM författarinstans körs i **läget***Dynamic Media Hybrid)      >Om du vill förhandsgranska eller hämta dynamiska återgivningar av en resurs kontrollerar du att det dynamiska mediet är aktiverat och att resursens Pyramid-tiff-återgivning finns på den AEM Assets-författarinstans där resurserna har publicerats. När en resurs publiceras på varumärkesportalen publiceras även dess Pyramid-återgivning.

   * Markera kryssrutan om du vill bevara mapphierarkin för varumärkesportalen när du hämtar resurser **[!UICONTROL Create separate folder for each asset]** . Som standard ignoreras mapphierarkin för varumärkesportalen och alla resurser hämtas i en mapp i det lokala systemet.

1. Klicka på **[!UICONTROL Download]**.

   Resurserna (och återgivningarna om de är markerade) hämtas som en zip-fil till den lokala mappen. Ingen ZIP-fil skapas emellertid om en enskild resurs hämtas utan någon av återgivningarna.

   Om administratören inte har [gett dig åtkomst till de ursprungliga återgivningarna](../using/brand-portal-adding-users.md#main-pars-procedure-202029708)hämtas inte de ursprungliga återgivningarna för de valda resurserna.

   >[!NOTE]
   >
   >Resurser som hämtas individuellt visas i resurshämtningsrapporten. Om en mapp som innehåller resurser däremot hämtas visas inte mappen och resurserna i hämtningsrapporten för resurser.


## Hämtningsprestanda förväntades {#expected-download-performance}

Filhämtningen kan variera för användare på olika platser på klienten, beroende på faktorer som lokal Internetanslutning och serverfördröjning. Den förväntade hämtningsprestandan för 2-GB-filer som observeras på olika klientplatser är följande, med Brand Portal-servern på Oregon i USA:

| Klientplats | Latens mellan klient och server | Förväntad hämtningshastighet | Tidsåtgång för att hämta en 2 GB-fil |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| Västra USA (N) Kalifornien) | 18 millisekunder | 7,68 MB/s | 4 minuter |
| Västra USA (Oregon) | 42 millisekunder | 3,84 MB/s | 9 minuter |
| Östra USA (N) Virginia) | 85 millisekunder | 1,61 MB/s | 21 minuter |
| APAC (Tokyo) | 124 millisekunder | 1,13 MB/s | 30 minuter |
| Noida | 275 millisekunder | 0,5 MB/s | 68 minuter |
| Sydney | 175 millisekunder | 0,49 MB/s | 69 minuter |
| London | 179 millisekunder | 0,32 MB/s | 106 minuter |
| Singapore | 196 millisekunder | 0,5 MB/s | 68 minuter |

>[!NOTE]
>
>Citerade data observeras under testförhållanden, som kan variera för användare på olika platser där olika fördröjningar och bandbredd kan förekomma.

