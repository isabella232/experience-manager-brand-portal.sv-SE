---
title: Stöd för dynamisk video på varumärkesportalen
seo-title: Stöd för dynamisk video på varumärkesportalen
description: Stöd för dynamisk video på varumärkesportalen
seo-description: Stöd för dynamisk video på varumärkesportalen
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: b69025074080b83ac699da434fc525fea1cb100a
workflow-type: tm+mt
source-wordcount: '1136'
ht-degree: 0%

---


# Dynamiskt videostöd på varumärkesportalen {#dynamic-video-support-on-brand-portal}

Förgranska och spela upp videor på ett flexibelt sätt på varumärkesportalen med stöd för dynamiska media. Hämta även dynamiska återgivningar från portalen och delade länkar.
Användare av varumärkesportalen kan:

* Förhandsgranska videoklipp på sidan Resursinformation, i kortvyn och på sidan för förhandsgranskning av länkdelning.
* Spela upp videokodningar på sidan Resursinformation.
* Visa dynamiska återgivningar på fliken Återgivningar på sidan Resursinformation.
* Ladda ned videokoder och mappar med videoklipp.

>[!NOTE]
>
>Om du vill arbeta med videoklipp och publicera dem på varumärkesportalen kontrollerar du att AEM Author-instansen har konfigurerats antingen i läget Dynamic Media Hybrid eller i läget Dynamic Media **[!DNL Scene 7]**.

För att förhandsgranska, spela upp och ladda ned videor visar Brand Portal följande två konfigurationer för administratörer:

* [Dynamic Media Hybrid-](#configure-dm-hybrid-settings)
konfigurationOm AEM Author-instansen körs i läget för dynamisk mediefyllning.
* [Dynamisk  [!DNL Scene 7] ](#configure-dm-scene7-settings)
mediakonfigurationOm AEM Author-instansen körs i dynamiskt **[!DNL Scene 7]** medieläge.
Ange någon av dessa konfigurationer baserat på de konfigurationer du ställt in i din AEM Author-instans som Brand Portal-klienten replikeras med.

>[!NOTE]
>
>Dynamiska videor stöds inte på innehavare av varumärkesportaler som konfigurerats med AEM Author som körs i **[!UICONTROL Scene7Connect]**-körningsläge.

## Hur spelas dynamiska videor upp? {#how-are-dynamic-videos-played}

![Videokodningar hämtas från molnet](assets/VideoEncodes.png)

Om dynamiska mediekonfigurationer ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) eller [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) konfigurationer) har konfigurerats på varumärkesportalen hämtas de dynamiska återgivningarna från **[!DNL Scene 7]**-servern. Videokodningar förhandsvisas och spelas upp utan fördröjning och kvalitetsförvrängning.

Eftersom videokoderna inte lagras i databasen för varumärkesportaler och hämtas från **[!DNL Scene 7]**-servern måste du se till att de dynamiska mediekonfigurationerna på AEM Author Instance och Brand Portal är desamma.

>[!NOTE]
>
>Videovisningsprogram och visningsförinställningar stöds inte i varumärkesportalen. Videoklipp förhandsgranskas och spelas upp på standardvisningsprogrammen i varumärkesportalen.

## Förutsättningar {#prerequisites}

Om du vill arbeta med dynamiska videoklipp på varumärkesportalen ska du se till att:

* **Starta AEM Author i DM-**
läge (Dynamic Media)Starta AEM Author-instansen (med vilken Brand Portal är konfigurerad) antingen i  [Dynamic Media Hybrid-](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) läge eller i  [Dynamic  [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Konfigurera Dynamic Media cloud services på AEM**
AuthorBaserat på det dynamiska medieläget är AEM Author aktiverat, ange antingen  [Dynamic Media cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) services eller  [[!DNL Scene 7] molntjänster ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) på AEM Author från  **Tools** |  **Cloud Services** |  **** Dynamic Media¥.
* **Konfigurera Dynamic Media på**
varumärkesportalenKonfigurera  [Dynamic Media på AEM Author med hjälp av Dynamic Media-](#configure-dm-hybrid-settings) inställningarna eller  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  inställningarna från administrationsverktygen för varumärkesportalen.
Se till att [separata Brand Portal-klientorganisationer](#separate-tenants) används för AEM Author-instanser som konfigurerats med Dynamic Media Hybrid och Dynamic Media **[!UICONTROL Scene7]**-lägen, om du använder funktioner för Dynamic Media Hybrid och Dynamic Media **[!UICONTROL S7]**.
* **Publicera mappar med videokodning på Brand**
PortalAnvänd  [videokodning ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) och publicera mappen med multimediematerial från AEM Author-instansen på Brand Portal.
* **Tillåtslista IP-adresser för Edge i SPS om säker förhandsvisning**
är aktiveratOm Dynamic Media-**[!DNL Scene 7]** (med  [säker förhandsgranskning ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) aktiverad för ett företag) bör  **[!DNL Scene 7]** företagsadministratören  [tillåtslista IP-adressen för offentliga utgångar för respektive region med hjälp av SPS (](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)  **[!UICONTROL Scene 7]** Publishing System) flash-gränssnittet.
IP-adresserna för Egress är följande:

| **Län** | **IP-adress för ägg** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

Om du vill tillåta någon av dessa utgående IP:n läser du [Förbered ditt konto för säker testningstjänst](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Bästa praxis

Följ de här stegen för att se till att dina dynamiska videomaterial förhandsvisas, spelas upp och hämtas från varumärkesportalen (och delade länkar):

### Separata innehavare för lägena Dynamic Media Hybrid och Dynamic Media Scene 7 {#separate-tenants}

Om du använder både Dynamic Media **[!DNL Scene 7]**- och Dynamic Media Hybrid-funktioner rekommenderar vi att du använder olika Brand Portal-klientenheter för AEM Author-instanser som konfigurerats med Dynamic Media Hybrid och Dynamic Media **[!DNL Scene 7]**-lägen.<br />

![Författare och BP 1:1-mappning](assets/BPDynamicMedia.png)

### Samma konfigurationsinformation på AEM Author-instansen och varumärkesportalen

Kontrollera att konfigurationsinformationen - som **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (i **[!UICONTROL Dynamic Media Hybrid]**) och **[!UICONTROL Title]**, autentiseringsuppgifter (**[!UICONTROL Email]** och lösenord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (i Dynamic Media **[!DNL Scene 7]**) - är samma i varumärkesportalen och **[!UICONTROL AEM cloud configuration]**.

### Tillåtslista IP-adresser för offentlig utgång för läget Dynamic Media Scene 7

Om den säkra förhandsvisningen av Dynamic Media **[!UICONTROL Scene 7]**-HAVING [aktiverad](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-används för att skicka videomaterial till varumärkesportalen skapar **[!UICONTROL Scene 7]** en dedikerad bildserver för testmiljöer eller interna program. Alla förfrågningar till den här servern kontrollerar den ursprungliga IP-adressen. Om den inkommande begäran inte finns i den godkända listan över IP-adresser returneras ett felsvar.
Företagsadministratören **[!UICONTROL Scene-7]** konfigurerar därför en godkänd lista över IP-adresser för företagets **[!UICONTROL Secure Testing]**-miljö via Flash-gränssnittet **[!UICONTROL SPS]** (Scene-7 Publishing System). Se till att IP-adressen för utgångar för din respektive region (från följande) läggs till i den godkända listan.
Om du vill tillåta någon av dessa utgående IP:n läser du [Förbered ditt konto för säker testningstjänst](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
IP-adresserna för utgångar är följande:

| **Län** | **IP-adress för ägg** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63.140.44.54 |

## Konfigurera inställningar för Dynamic Media (Hybrid) {#configure-dm-hybrid-settings}

Om AEM Author-instansen körs i dynamiskt medihybridläge använder du **[!UICONTROL Video]**-panelen från panelen Administrationsverktyg för att konfigurera Dynamic Media gateway-inställningarna.

>[!NOTE]
>
>[videokodningsprofilerna](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) publiceras inte till Varumärkesportalen, utan hämtas från **[!UICONTROL Scene 7]**-servern. För att videokodningar ska kunna spelas upp i varumärkesportalen måste därför konfigurationsinformationen vara densamma som [[!UICONTROL Scene7 cloud configuration]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) i din AEM Author-instans.

Så här konfigurerar du dynamiska mediekonfigurationer för innehavare av varumärkesportaler:

1. Välj AEM logotyp för att komma åt administrationsverktygen i verktygsfältet högst upp i varumärkesportalen.
1. Välj plattan **[!UICONTROL Video]** på panelen Administrationsverktyg.

   ![Dynamic Media Hybrid Config på varumärkesportalen](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** sidan öppnas.

   ![Dynamic Media Hybrid Configuration on Brand Portal](assets/edit-dynamic-media-config.png)

1. Ange **[!UICONTROL Registration ID]** och **[!UICONTROL Video Service URL]** (URL för DM-gateway). Se till att dessa uppgifter är desamma som de i **[!UICONTROL Tools > Cloud Services]** i din AEM Author-instans.
1. Välj **Spara** för att spara konfigurationen.

## Konfigurera Dynamic Media Scene7-inställningar {#configure-dm-scene7-settings}

Om AEM Author-instansen körs i läget Dynamic Media- **[!UICONTROL Scene 7]** använder du **[!UICONTROL Dynamic Media Configuration]**-panelen från panelen Administrationsverktyg för att konfigurera serverinställningarna för **[!UICONTROL Scene 7]**.

Så här ställer du in konfigurationer för Dynamic Media **[!UICONTROL Scene 7]** för innehavare av varumärkesportaler:

1. Välj AEM logotyp för att komma åt administrationsverktygen i verktygsfältet högst upp i varumärkesportalen.

2. Välj **[!UICONTROL Dynamic Media Configuration]**-rutan på panelen Administrationsverktyg.<br />
   ![DM- [!UICONTROL Scene 7] konfiguration på varumärkesportalen](assets/DMS7-Tile.png)
   **[!UICONTROL Edit Dynamic Media Configuration]** sidan öppnas.<br />
   ![Scene 7 Configuration on Brand Portal](assets/S7Config.png)

3. Ange:
   * **[!UICONTROL Title]**
   * Autentiseringsuppgifter (**[!UICONTROL Email ID]** och **[!UICONTROL Password]**) för att komma åt Scene 7-servern
   * **[!UICONTROL Region]**
Se till att dessa värden är desamma som i din AEM Author-instans.

4. Välj **[!UICONTROL Connect to Dynamic Media]**.

5. Ange **[!UICONTROL Company name]** och **[!UICONTROL Save]** konfigurationen.
