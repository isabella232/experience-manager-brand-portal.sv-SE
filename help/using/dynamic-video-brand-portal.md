---
title: Dynamiskt videostöd i Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Dynamiskt videostöd i Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: beabaa4e5cca4c2554111861b15902cac54ccd4c
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Dynamiskt videostöd i Brand Portal {#dynamic-video-support-on-brand-portal}

Förgranska och spela upp videor på ett anpassat sätt på Brand Portal med Dynamic Media support. Hämta även dynamiska återgivningar från portalen och delade länkar.
Brand Portal-användare kan:

* Förhandsgranska videoklipp på sidan Resursinformation, i kortvyn och på sidan för förhandsgranskning av länkdelning.
* Spela upp videokodningar på sidan Resursinformation.
* Visa dynamiska återgivningar på fliken Återgivningar på sidan Resursinformation.
* Ladda ned videokoder och mappar med videoklipp.

>[!NOTE]
>
>Om du vill arbeta med videofilmer och publicera dem på Brand Portal måste du kontrollera att författarinstansen för Experience Manager är inställd på Dynamic Media Hybrid-läge eller Dynamic Media **[!DNL Scene7]** läge.

För att förhandsgranska, spela upp och ladda ned videor visar Brand Portal följande två konfigurationer för administratörer:

* [Dynamic Media Hybrid-konfiguration](#configure-dm-hybrid-settings)
Om Experience Manager Author-instansen körs i läget Dynamic Media Hybrid.
* [Dynamic Media [!DNL Scene7] konfiguration](#configure-dm-scene7-settings)
Om Experience Manager Author-instansen körs på dynamiska media-**[!DNL Scene7]** läge.
Ange någon av dessa konfigurationer baserat på de konfigurationer som du anger i din Experience Manager Author-instans som Brand Portal-klientorganisationen replikeras med.

>[!NOTE]
>
>Dynamiska videor stöds inte på Brand Portal-klientorganisationer som är konfigurerade med Experience Manager Author som körs på **[!UICONTROL Scene7Connect]** körningsläge.

## Hur spelas dynamiska videor upp? {#how-are-dynamic-videos-played}

![Videokodningar hämtas från molnet](assets/VideoEncodes.png)

Om Dynamic Media-konfigurationer ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) eller [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) konfigurationer) har konfigurerats på Brand Portal, de dynamiska återgivningarna hämtas från **[!DNL Scene7]** server. Videokodningar förhandsvisas och spelas upp utan fördröjning och kvalitetsförvrängning.

Eftersom videokodningar inte lagras i Brand Portal-databasen och hämtas från **[!DNL Scene7]** ska du se till att Dynamic Media-konfigurationerna på Adobe Experience Manager Author Instance och Brand Portal är desamma.

>[!NOTE]
>
>Videovisningsprogram och visningsförinställningar stöds inte i Brand Portal. Videor förhandsvisas och spelas upp på standardvisningsprogrammen i Brand Portal.

## Förutsättningar {#prerequisites}

Om du vill arbeta med dynamiska videoklipp på Brand Portal måste du se till att:

* **Starta Experience Manager Author i Dynamic Media-läge**
Starta Experience Manager Author-instansen (som Brand Portal är konfigurerat med) antingen i [Dynamic Media - [!DNL Scene7] läge](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) eller in [Dynamic Media - hybridläge](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) eller
* **Konfigurera Dynamic Media-Cloud Services på författaren till Experience Manager**
Baserat på Dynamic Media-läget (Scene7-läge eller hybridläge) kan du ställa in Experience Manager Author [Dynamic Media-Cloud Services ([!DNL Scene7] läge)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) eller [Dynamic Media-Cloud Services (hybridläge)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) på Experience Manager Author from **verktyg** | **Cloud Services** | **Dynamic Media**.
* **Konfigurera Dynamic Media i Brand Portal**
Baserat på Dynamic Media molnkonfigurationer på Experience Manager Author kan du konfigurera [Dynamic Media-inställningar](#configure-dm-hybrid-settings) eller [[!DNL Scene7] inställningar](#configure-dm-scene7-settings) från Brand Portal administrationsverktyg.
Se till att [separata Brand Portal-hyresgäster](#separate-tenants) används för Experience Manager Author-instanser som har konfigurerats i Dynamic Media - **[!UICONTROL Scene7]** och Dynamic Media - hybrid-läge. Speciellt om du använder funktioner i Dynamic Media **[!UICONTROL S7]** och Dynamic Media Hybrid.
* **Publicera mappar med videokodning för Brand Portal**
Använd [videokodning](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) och publicera den mapp som innehåller multimedieresurser från Experience Manager Author till Brand Portal.
* **Tillåtslista IP-adresser i SPS om säker förhandsvisning är aktiverat**
Om du använder Dynamic Media-**[!DNL Scene7]** (med [säker förhandsvisning aktiverad](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) för ett företag) bör **[!DNL Scene7]** företagsadministratör [tillåtslista IP-adresserna till utgångarna](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) för respektive region med hjälp av SPS (**[!UICONTROL Scene7]** Publishing System) flash-gränssnitt.
IP-adresserna för Egress är följande:

| **Län** | **IP-adress för ägg** |
|--- |--- |
| NA | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

Om du vill tillåta någon av de här utgående IP-adresserna går du till [förbereda ditt konto för säker testningstjänst](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Bästa praxis

Följ de här stegen för att se till att dina dynamiska videoresurser förhandsvisas, spelas upp och hämtas från Brand Portal (och delade länkar):

### Separata innehavare för lägena Dynamic Media - Scene7 och Dynamic Media - Hybrid {#separate-tenants}

Om du använder båda Dynamic Media - **[!DNL Scene7]** läge och Dynamic Media - Funktioner i hybrid-läge, använd olika Brand Portal-klientorganisationer för Experience Manager Author-instanser som konfigurerats med Dynamic Media - **[!DNL Scene7]** och Dynamic Media - hybridlägen.


![Författare och BP 1:1-mappning](assets/BPDynamicMedia.png)

### Samma konfigurationsinformation på Experience Manager Author-instansen och Brand Portal

Se till att konfigurationsinformationen är densamma i Brand Portal och **[!UICONTROL Experience Manager Cloud Configuration]**. Samma konfigurationsinformation omfattar följande:

* **[!UICONTROL Title]**
* **[!UICONTROL Registration ID]**
* **[!UICONTROL Video Service URL]** in **[!UICONTROL Dynamic Media - Hybrid mode]**
* **[!UICONTROL Title]**
* Autentiseringsuppgifter (**[!UICONTROL Email]** och lösenord)
* **[!UICONTROL Region]**
* **[!UICONTROL Company]** i Dynamic Media - **[!DNL Scene7]** läge

### Tillåtelselista publika IP-adresser för utgångar för Dynamic Media Scene7-läge

Om Dynamic Media **[!UICONTROL Scene7]**-som [säker förhandsvisning aktiverad](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-används för att skicka videomaterial till Brand Portal, och sedan **[!UICONTROL Scene7]** skapar en dedikerad bildserver för testmiljöer eller interna program. Alla förfrågningar till den här servern kontrollerar den ursprungliga IP-adressen. Om den inkommande begäran inte finns i den godkända listan över IP-adresser returneras ett felsvar.
The **[!UICONTROL Scene7]** Företagsadministratören konfigurerar därför en godkänd lista över IP-adresser för företagets **[!UICONTROL Secure Testing]** miljö, genom **[!UICONTROL SPS]** (Scene7 Publishing System) flash-gränssnitt. Se till att IP-adressen för utgångar för din respektive region (från följande) läggs till i den godkända listan.
Om du vill tillåta någon av de här utgående IP-adresserna går du till [förbereda ditt konto för säker testningstjänst](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
IP-adresserna för utgångar är följande:

| **Län** | **IP-adress för ägg** |
|--- |--- |
| NA | 130.248.160.68, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| APAC | 63.140.44.54 |

## Konfigurera inställningar för Dynamic Media (Hybrid) {#configure-dm-hybrid-settings}

Om Experience Manager Author-instansen körs i läget för dynamisk mediefyllning ska du använda **[!UICONTROL Video]** från panelen Administrativa verktyg för att konfigurera inställningarna för Dynamic Media gateway.

>[!NOTE]
>
>The [videokodningsprofiler](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) publiceras inte till Brand Portal, utan hämtas från **[!UICONTROL Scene7]** server. För att videokodningar ska kunna spelas upp i Brand Portal måste därför konfigurationsinformationen vara densamma som [Dynamic Media-Cloud Services ([!DNL Scene7] läge)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) i Experience Manager Author.

Så här konfigurerar du Dynamic Media-konfigurationer för Brand Portal-klienter:

1. Markera Experience Manager-logotypen så att du kan komma åt administrationsverktygen från verktygsfältet längst upp i Brand Portal.
1. På panelen Administrationsverktyg väljer du **[!UICONTROL Video]** platta.

   ![Dynamic Media Hybrid Config på Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** sidan öppnas.

   ![Dynamic Media Hybrid Configuration på Brand Portal](assets/edit-dynamic-media-config.png)

1. Ange **[!UICONTROL Registration ID]** och **[!UICONTROL Video Service URL]** (URL för DM-Gateway). Se till att informationen är densamma som informationen i **[!UICONTROL Tools > Cloud Services]** i Experience Manager Author.
1. Välj **Spara** för att spara konfigurationen.

## Konfigurera inställningar för Dynamic Media Scene7 {#configure-dm-scene7-settings}

Om Experience Manager Author-instansen körs på Dynamic Media- **[!UICONTROL Scene7]** läge, använd sedan **[!UICONTROL Dynamic Media Configuration]** från panelen Administrationsverktyg för att konfigurera **[!UICONTROL Scene7]** serverinställningar.

Konfigurera Dynamic Media **[!UICONTROL Scene7]** konfigurationer på Brand Portal tenants:

1. Markera Experience Manager-logotypen så att du kan komma åt administrationsverktygen från verktygsfältet längst upp i Brand Portal.

2. På panelen Administrationsverktyg väljer du **[!UICONTROL Dynamic Media Configuration]** platta.

   ![DM [!UICONTROL Scene 7] konfiguration på Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** sidan öppnas.

   ![Scene 7 Configuration på Brand Portal](assets/S7Config.png)

3. Ange:

   * **[!UICONTROL Title]**
   * Autentiseringsuppgifter (**[!UICONTROL Email ID]** och **[!UICONTROL Password]**) för att få åtkomst till Scene7-servern
   * **[!UICONTROL Region]**

   Se till att dessa värden är desamma som de som finns i Experience Manager Author-instansen.

4. Välj **[!UICONTROL Connect to Dynamic Media]**.

5. Ange **[!UICONTROL Company name]** och **[!UICONTROL Save]** konfigurationen.
