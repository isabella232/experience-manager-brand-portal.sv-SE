---
title: Använda bildförinställningar eller dynamiska återgivningar
seo-title: Apply image presets or dynamic renditions
description: Precis som ett makro är en bildförinställning en fördefinierad samling kommandon för storleksändring och formatering som sparats under ett namn. Med bildförinställningar kan Experience Manager Assets Brand Portal dynamiskt leverera bilder i olika storlekar, format och egenskaper.
seo-description: Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable Experience Manager Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties.
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Admin
exl-id: 212a1b3a-686f-4250-be06-b679b6039887
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 2%

---

# Använda bildförinställningar eller dynamiska återgivningar {#apply-image-presets-or-dynamic-renditions}

Precis som ett makro är en bildförinställning en fördefinierad samling kommandon för storleksändring och formatering som sparats under ett namn. Med bildförinställningar kan Experience Manager Assets Brand Portal dynamiskt leverera bilder i olika storlekar, format och egenskaper.

En bildförinställning används för att generera dynamiska återgivningar av bilder som kan förhandsvisas och hämtas. När du förhandsgranskar bilder och deras återgivningar kan du välja en förinställning för att formatera om bilder enligt de specifikationer som angetts av administratören.

(*Om Experience Manager Assets-författarinstans körs på&#x200B;**Dynamic Media hybridläge***) Om du vill visa dynamiska återgivningar av en resurs i Brand Portal kontrollerar du att dess Pyramid-återgivning finns på den Experience Manager Assets-författarinstans som du publicerar på Brand Portal. När du publicerar resursen publiceras även dess PTIFF-återgivning till Brand Portal.

>[!NOTE]
>
>När du hämtar bilder och återgivningar av dem finns det inget alternativ att välja bland de befintliga förinställningarna. Du kan i stället ange egenskaper för en anpassad bildförinställning. Mer information finns i [Använda bildförinställningar vid hämtning av bilder](../using/brand-portal-image-presets.md#main-pars-text-1403412644).


Mer information om de parametrar som krävs när du skapar bildförinställningar finns i [Hantera bildförinställningar](../using/brand-portal-image-presets.md).

## Skapa en bildförinställning {#create-an-image-preset}

Experience Manager Assets-administratörerna kan skapa bildförinställningar som visas som dynamiska återgivningar på resursinformationssidan. Du kan skapa en bildförinställning från grunden eller spara en befintlig med ett nytt namn. När du skapar en bildförinställning väljer du en storlek för bildleverans och formateringskommandona. När en bild levereras för visning optimeras dess utseende enligt de valda kommandona.

>[!NOTE]
>
>Dynamiska återgivningar av en bild skapas med TIFF i Pyramid. Om Pyramid TIFF inte är tillgänglig för någon resurs går det inte att hämta dynamiska återgivningar för den resursen i varumärkesportalen.
>
>Om Experience Manager Assets-författarinstans körs på **Dynamic Media hybridläge** och sedan skapas och sparas Pyramid TIFF-återgivningar av bildresurser i Experience Manager Assets-databasen.
>
>Om Experience Manager Assets författarinstans körs **Dynamic Media Scene 7** och sedan finns Pyramid TIFF-återgivningar av bildresurser på Scene 7-servern.
>
>När sådana resurser publiceras på varumärkesportalen används bildförinställningar och dynamiska återgivningar visas.


1. Klicka på Experience Manager-logotypen i verktygsfältet överst för att öppna administrationsverktygen.

1. På panelen Administrationsverktyg klickar du på **[!UICONTROL Image Presets]**.

   ![](assets/admin-tools-panel-4.png)

1. Klicka på **[!UICONTROL Create]**.

   ![](assets/image_preset_homepage.png)

1. I **[!UICONTROL Edit Image Preset]** sida anger du värden i **[!UICONTROL Basic]** och **[!UICONTROL Advanced]** tabbar, inklusive ett namn. Förinställningarna visas i den vänstra rutan och kan användas direkt tillsammans med andra resurser.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >Du kan också använda **[!UICONTROL Edit Image Preset]** sida för att redigera egenskaperna för en befintlig bildförinställning. Om du vill redigera en bildförinställning markerar du den på sidan med bildförinställningar och klickar på **[!UICONTROL Edit]**.

1. Klicka på **[!UICONTROL Save]**. Bildförinställningen skapas och visas på sidan med bildförinställningar.
1. Om du vill ta bort en bildförinställning markerar du den på sidan med bildförinställningar och klickar på **[!UICONTROL Delete]**. Klicka på **[!UICONTROL Delete]** för att bekräfta borttagningen. Bildförinställningen tas bort från sidan med bildförinställningar.

## Använda bildförinställningar vid förhandsvisning av bilder  {#apply-image-presets-when-previewing-images}

När du förhandsgranskar bilder och deras återgivningar kan du välja bland de befintliga förinställningarna för att formatera om bilderna enligt de specifikationer som angetts av administratören.

1. Öppna en bild genom att klicka på den i Brand Portal-gränssnittet.
1. Klicka på överläggsikonen till vänster och välj **[!UICONTROL Renditions]**.

   ![](assets/image-preset-previewrenditions.png)

1. Från **[!UICONTROL Renditions]** väljer du lämplig dynamisk återgivning, till exempel **[!UICONTROL Thumbnail]**. Förhandsvisningsbilden återges baserat på vad du väljer för återgivningen.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Använda bildförinställningar vid hämtning av bilder {#apply-image-presets-when-downloading-images}

När du hämtar bilder och deras återgivningar från Brand Portal kan du inte välja bland de befintliga bildförinställningarna. Du kan dock anpassa förinställda bildegenskaper baserat på vilka du vill formatera om bilder.

1. Gör något av följande i Brand Portal-gränssnittet:

   * Håll pekaren över bilden som du vill hämta. På miniatyrbilderna för snabbåtgärder klickar du på **[!UICONTROL Download]** ikon.

   ![](assets/downloadsingleasset.png)

   * Markera den bild som du vill hämta. Klicka på knappen **[!UICONTROL Download]** ikon.

   ![](assets/downloadassets.png)

1. Från **[!UICONTROL Download]** väljer du önskade alternativ beroende på om du vill hämta resursen med eller utan dess återgivningar.

   ![](assets/donload-assets-dialog.png)

1. Om du vill hämta dynamiska återgivningar av resursen väljer du **[!UICONTROL Dynamic Rendition(s)]** alternativ.
1. Anpassa egenskaper för bildförinställningar utifrån vilka du vill formatera om bilden och dess återgivningar dynamiskt under hämtningen. Ange storlek, format, färgrymd, upplösning och bildmodifiering.

   ![](assets/dynamicrenditions.png)

1. Klicka på **[!UICONTROL Download]**. De anpassade dynamiska återgivningarna hämtas i en ZIP-fil tillsammans med bilden och de återgivningar som du valde att hämta. Ingen zip-fil skapas emellertid om en enskild resurs hämtas, vilket gör att hämtningen går snabbt.
