---
title: Versionsinformation
seo-title: Versionsinformation
description: Få en inblick i funktioner, förbättringar, åtgärdade kritiska problem och kända fel i Adobe Experience Manager Assets Brand Portal 2020.10.0.
seo-description: Få insikt i förbättringarna, åtgärdade allvarliga problem och kända fel i Adobe Experience Manager Assets Brand Portal 2020.10.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 4774d8a78657c89081d229ce596a3bd404ae1bc8
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 4%

---


# Versionsinformation {#release-notes}

Få en inblick i de nya funktionerna, förbättringarna, de allvarliga problemen och de kända problemen i Adobe Experience Manager Assets Brand Portal 2020.10.0.

## Versionsinformation {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2020.10.0 |
| Date | Oktober 2020 |

## Översikt {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal hjälper er att enkelt skaffa, styra och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter. Det bidrar till att effektivisera resursdelning, snabbar upp time-to-market för tillgångar och minskar risken för bristande efterlevnad och obehörig åtkomst. Med Brand Portal kan man söka, förhandsgranska, ladda ned och exportera material i företagsgodkända format - när som helst, var som helst.

## Nyheter 2020.10.0 {#whats-new-in-2020.10.0}

### Nya funktioner {#new-features}

Den här versionen innehåller följande nya funktioner:

* Dialogrutan har gjorts om i en listvy med ytterligare alternativ för att exkludera de återgivningar som inte är obligatoriska, använda samma uppsättning regler för liknande resurstyper och hämta de valda återgivningarna. **[!UICONTROL Download]** Se [Steg för att hämta resurser från varumärkesportalen](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* Navigera till **[!UICONTROL Files]**, **[!UICONTROL Collections]** och **[!UICONTROL Shared Links]** är nu möjligt från alla sidor i varumärkesportalen med ett klick.

* På **[!UICONTROL Renditions]** panelen på sidan med tillgångsinformation kan du nu välja den ursprungliga resursen och (eller) specifika resursåtergivningar och hämta dem direkt från **[!UICONTROL Renditions]** panelen utan att behöva öppna **[!UICONTROL Download]** dialogrutan. Se [Hämta resurser från sidan](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page)med resursinformation.

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Förutom de befintliga **[!UICONTROL Download]** konfigurationerna kan administratören för varumärkesportalen även [konfigurera behörigheter för olika användargrupper](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) att visa och (eller) hämta den ursprungliga resursen och dess återgivningar från sidan med tillgångsinformation. Dessa konfigurationer definierar vem som kan komma åt och (eller) hämta resursrenderingarna.

### Förbättringar {#enhancements}

Den här versionen innehåller följande förbättringar:

* Tröskelvärdet för sessionstimeout för gästanvändare har reducerats från 2 timmar till 15 minuter.
* Det extra **[!UICONTROL View pages]** alternativet har tagits bort för flersidiga PDF-filer eftersom användaren nu kan visa PDF-sidorna i Adobe Document Cloud Viewer.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Kända fel {#known-issues}

Den här versionen innehåller följande kända fel:

* Sök i **[!UICONTROL Asset Reports]** visningsgränssnittet utan sökresultat.
* DM-videokoderna är inte synliga för användare som inte är administratörer på sidan med resursinformation.
* Justeringen av storleken på de enskilda materialåtergivningarna och den totala hämtningsstorleken förvrängs i dialogrutan Hämta.



<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Språk {#languages}

Användargränssnittet Brand Portal finns på följande språk:

* Engelska
* Tyska
* Franska
* Spanska
* Italienska
* Brasiliansk portugisiska
* Japanska
* Förenklad kinesiska
* Koreanska

## Certifierade plattformar {#certified-platforms}

Om du vill ta reda på vilka plattformar som är certifierade för att köras med den här versionen av varumärkesportalen läser du i kolumnen **Stöd för pekoptimerat användargränssnitt** i tabellen i **webbläsare som stöds för redigeringsanvändargränssnittet** i [Tekniska krav](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Länkar {#links}

* [Adobe Experience Manager produktsida på adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Dokumentation för Assets Brand Portal](https://helpx.adobe.com/se/experience-manager/brand-portal/user-guide.html)

## Produktåtkomst och support (begränsade platser) {#product-access-and-support-restricted-sites}

Dessa webbplatser är bara tillgängliga för kunder. Om du är kund och behöver åtkomst kontaktar du din kontoansvarige på Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Produktåtkomst](https://login.marketing.adobe.com)

* [Adobe kundtjänst](https://helpx.adobe.com/contact.html)
