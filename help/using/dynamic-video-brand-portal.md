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
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 0%

---


# Stöd för dynamisk video på varumärkesportalen {#dynamic-video-support-on-brand-portal}

Förgranska och spela upp videor på ett flexibelt sätt på varumärkesportalen med stöd för Dynamic Media. Hämta även dynamiska återgivningar från portalen och delade länkar.
Användare av varumärkesportalen kan:

* Förhandsgranska videoklipp på sidan Resursinformation, i kortvyn och på sidan för förhandsgranskning av länkdelning.
* Spela upp videokodningar på sidan Resursinformation.
* Visa dynamiska återgivningar på fliken Återgivningar på sidan Resursinformation.
* Ladda ned videokoder och mappar med videoklipp.

>[!NOTE]
>
>Om du vill arbeta med videofilmer och publicera dem på varumärkesportalen kontrollerar du att din AEM Author-instans är inställd antingen i Dynamic Media hybridläge eller Dynamic Media- **[!DNL Scene 7]** läge.

För att förhandsgranska, spela upp och ladda ned videor visar Brand Portal följande två konfigurationer för administratörer:

* [Dynamic Media Hybrid-konfiguration](#configure-dm-hybrid-settings)om instansen AEM Author körs i läget för dynamisk mediefyllning.
* [Dynamic Media [!DNL Scene 7]-konfiguration](#configure-dm-scene7-settings)Om instansen AEM Author körs i läget för dynamiska media **[!DNL Scene 7]** .
Ange någon av dessa konfigurationer baserat på de konfigurationer som du anger i din AEM Author-instans med vilken Brand Portal-klientorganisationen replikeras.

>[!NOTE]
>
>Dynamiska videor stöds inte på innehavare av varumärkesportaler som konfigurerats med AEM Author som körs i **[!UICONTROL Scene7Connect]** runmode.

## Hur spelas dynamiska videor upp? {#how-are-dynamic-videos-played}

![Videokodningar hämtas från molnet](assets/VideoEncodes.png)

Om Dynamic Media-konfigurationer ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) - eller [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) -konfigurationer) har konfigurerats på Varumärksportal hämtas de dynamiska återgivningarna från **[!DNL Scene 7]** servern. Videokodningar förhandsvisas och spelas upp utan fördröjning och kvalitetsförvrängning.

Eftersom videokodningar inte lagras i databasen för varumärkesportaler och hämtas från **[!DNL Scene 7]** servern måste du se till att Dynamic Media på AEM Author Instance och Brand Portal är desamma.

>[!NOTE]
>
>Videovisningsprogram och visningsförinställningar stöds inte i varumärkesportalen. Videoklipp förhandsgranskas och spelas upp på standardvisningsprogrammen i varumärkesportalen.

## Förutsättningar {#prerequisites}

Om du vill arbeta med dynamiska videoklipp på varumärkesportalen ska du se till att:

* **Starta AEM Author i DM-läge (Dynamic Media)** Starta AEM Author-instansen (som Brand Portal är konfigurerad med) antingen i [Dynamic Media hybridläge](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) eller i [Dynamic Media [!DNL Scene 7]-läge](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Konfigurera Dynamic Media molntjänster på AEM Author** Baserat på Dynamic Media-läget som AEM Author körs på anger du antingen [Dynamic Media molntjänster](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) eller [[!DNL Scene 7] molntjänster](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) på AEM Author från **Verktyg** | **Cloud Service** | **Dynamic Media**.
* **Konfigurera Dynamic Media på varumärkesportalen** Baserat på Dynamic Media molnkonfigurationer på AEM Author, konfigurera [Dynamic Media-inställningar](#configure-dm-hybrid-settings) eller [[!DNL Scene 7]-inställningar](#configure-dm-scene7-settings) från administrationsverktygen för varumärkesportalen.
Se till att [separata Brand Portal-klientorganisationer](#separate-tenants) används för AEM Author-instanser som konfigurerats med Dynamic Media Hybrid och Dynamic Media- **[!UICONTROL Scene7]** lägen, om du använder funktioner för Dynamic Media Hybrid och Dynamic Media **[!UICONTROL S7]**.
* **Publicera mappar med videokodningar tillämpade på Brand Portal** Använd [videokodningar](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) och publicera den mapp som innehåller multimedieresurser från AEM Author-instansen till Brand Portal.
* **Tillåtslista IP-adresser i SPS om säker förhandsgranskning är aktiverat** Om Dynamic Media-**[!DNL Scene 7]** (med [säker förhandsvisning aktiverat](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) för ett företag) används bör **[!DNL Scene 7]** företagsadministratören [tillåtslista IP-adresserna](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) för offentliga utgångar för respektive region med hjälp av SPS (**[!UICONTROL Scene 7]** Publishing System) flash-gränssnitt.
IP-adresserna för Egress är följande:

| **Län** | **IP-adress för ägg** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Om du vill tillåta någon av dessa utgående IP-adresser läser du [förbereda ditt konto för säker testningstjänst](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Bästa praxis

Följ de här stegen för att se till att dina dynamiska videomaterial förhandsvisas, spelas upp och hämtas från varumärkesportalen (och delade länkar):

### Separata innehavare för lägena Dynamic Media Hybrid och Dynamic Media Scene 7 {#separate-tenants}

Om du använder både Hybrid-funktionerna i Dynamic Media **[!DNL Scene 7]** och Dynamic Media bör du använda olika Brand Portal-klientorganisationer för AEM Author-instanser som konfigurerats med Dynamic Media Hybrid och Dynamic Media- **[!DNL Scene 7]** lägen.<br />

![Författare och BP 1:1-mappning](assets/BPDynamicMedia.png)

### Samma konfigurationsinformation på AEM Author-instansen och varumärkesportalen

Kontrollera att konfigurationsinformationen - som **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (in **[!UICONTROL Dynamic Media Hybrid]**) och **[!UICONTROL Title]**, autentiseringsuppgifter (**[!UICONTROL Email]** och lösenord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (i Dynamic Media **[!DNL Scene 7]**) - är densamma i varumärkesportalen och **[!UICONTROL AEM cloud configuration]**.

### Tillåtelselista publika IP-adresser för Dynamic Media Scene 7-läge

Om Dynamic Media **[!UICONTROL Scene 7]** med [säker förhandsgranskning aktiverad](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)används för att skicka videomaterial till varumärkesportalen, skapar du **[!UICONTROL Scene 7]** en dedikerad bildserver för testmiljöer eller interna program. Alla förfrågningar till den här servern kontrollerar den ursprungliga IP-adressen. Om den inkommande begäran inte finns i den godkända listan över IP-adresser returneras ett felsvar.
Företagsadministratören **[!UICONTROL Scene-7]** konfigurerar därför en godkänd lista över IP-adresser för företagets **[!UICONTROL Secure Testing]** miljö via **[!UICONTROL SPS]** Flash-gränssnittet (Scene-7 Publishing System). Se till att IP-adressen för utgångar för din respektive region (från följande) läggs till i den godkända listan.
Om du vill tillåta någon av dessa utgående IP-adresser läser du [förbereda ditt konto för säker testningstjänst](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
IP-adresserna för utgångar är följande:

| **Län** | **IP-adress för ägg** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Konfigurera inställningar för Dynamic Media (Hybrid) {#configure-dm-hybrid-settings}

Om AEM Author-instansen körs i läget för dynamisk mediefyllning använder du **[!UICONTROL Video]** panelen Administrationsverktyg för att konfigurera inställningarna för Dynamic Media gateway.

>[!NOTE]
>
>Videokodningsprofilerna [publiceras inte till](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) Varumärkeportalen, utan hämtas från **[!UICONTROL Scene 7]** servern. För att videokodningar ska kunna spelas upp i Brand Portal måste du därför se till att konfigurationsinformationen är densamma som [[!UICONTROL Scene7-molnkonfigurationen]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) i din AEM Author-instans.

Så här konfigurerar du Dynamic Media på innehavare av varumärkesportaler:

1. Välj AEM-logotypen för att få åtkomst till administrationsverktygen från verktygsfältet högst upp i varumärkesportalen.
1. Markera **[!UICONTROL Video]** rutan på panelen Administrationsverktyg.

   ![Dynamic Media Hybrid Config på varumärkesportalen](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** sidan öppnas.

   ![Hybridkonfiguration för Dynamic Media på varumärkesportalen](assets/edit-dynamic-media-config.png)

1. Ange **[!UICONTROL Registration ID]** och **[!UICONTROL Video Service URL]** (URL för DM-gateway). Se till att de här detaljerna är samma som de i **[!UICONTROL Tools > Cloud Services]** din AEM Author-instans.
1. Välj **Spara** för att spara konfigurationen.

## Konfigurera inställningar för Dynamic Media Scene7 {#configure-dm-scene7-settings}

Om instansen AEM Author körs i Dynamic Media- **[!UICONTROL Scene 7]** läge använder du **[!UICONTROL Dynamic Media Configuration]** rutan från administratörsverktygspanelen för att konfigurera **[!UICONTROL Scene 7]** serverinställningarna.

Så här konfigurerar du Dynamic Media- **[!UICONTROL Scene 7]** konfigurationer för innehavare av varumärkesportaler:

1. Välj AEM-logotypen för att få åtkomst till administrationsverktygen från verktygsfältet högst upp i varumärkesportalen.

2. Markera **[!UICONTROL Dynamic Media Configuration]** rutan på panelen Administrationsverktyg.<br />
   ![DM- [!UICONTROL Scene 7] konfiguration på varumärkesportalen](assets/DMS7-Tile.png)
   **[!UICONTROL Edit Dynamic Media Configuration]** sidan öppnas.<br />
   ![Scene 7 Configuration on Brand Portal](assets/S7Config.png)

3. Ange:
   * **[!UICONTROL Title]**
   * Autentiseringsuppgifter (**[!UICONTROL Email ID]** och **[!UICONTROL Password]**) för att komma åt Scene 7-servern
   * **[!UICONTROL Region]**
Se till att de här värdena är samma som de i din AEM Author-instans.

4. Välj **[!UICONTROL Connect to Dynamic Media]**.

5. Ange **[!UICONTROL Company name]** och **[!UICONTROL Save]** konfigurationen.
