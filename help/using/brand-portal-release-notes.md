---
title: Versionsinformation
seo-title: Versionsinformation
description: Få en inblick i funktioner, förbättringar, åtgärdade kritiska problem och kända fel i Adobe Experience Manager Assets Brand Portal 2021.02.0.
seo-description: Få insikt i förbättringarna, åtgärdade kritiska problem och kända fel i Adobe Experience Manager Assets Brand Portal 2021.02.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 69cf1756a546355ed767ac13c51fb09932254dbc
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 5%

---


# Versionsinformation {#release-notes}

Få en inblick i de nya funktionerna, förbättringarna, de allvarliga problemen och de kända problemen i Adobe Experience Manager Assets Brand Portal 2021.02.0.

## Versionsinformation {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 2021.02.0 |
| Date | Februari 2021 |

## Översikt {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal hjälper er att enkelt skaffa, styra och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter. Det bidrar till att effektivisera resursdelning, snabbar upp time-to-market för tillgångar och minskar risken för bristande efterlevnad och obehörig åtkomst. Med Brand Portal kan man söka, förhandsgranska, ladda ned och exportera material i företagsgodkända format - när som helst, var som helst.

## Nyheter i 2021.02.0 {#whats-new-in-2021.02.0}

### Nya funktioner {#new-features}

Den här versionen innehåller följande nya funktioner:

* Ytterligare en **[!UICONTROL Asset Download]**-inställning har införts under **[!UICONTROL Download Settings]**. En separat mapp skapas för varje resurs när mappar, samlingar eller masshämtning av resurser hämtas. Se [hämtningsinställningar](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download).

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### Förbättringar {#enhancements}

Den här versionen innehåller följande förbättringar:

* För mapphämtning skapas en separat mapp för varje resurs med hjälp av en delningslänk oavsett **[!UICONTROL Download Settings]**.
* Varumärksportalen **[!UICONTROL Usage Report]** har ändrats så att den endast speglar de aktiva varumärkesportalsanvändarna.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Åtgärdade kritiska problem {#critical-issues-fixed}

Den här versionen innehåller korrigeringar av följande allvarliga problem:

* Om bara de ursprungliga resurserna hämtas, visar resursen ett eget filnamnstillägg och öppnas inte förrän filnamnstillägget ändras manuellt till zip.
* Användargränssnittet för samlingsmappen svarar inte när du klickar på navigeringspilen.
* **[!UICONTROL Create]** -knappen visas i  **[!UICONTROL Column]** vyn även när mapparna är tomma.
* **[!UICONTROL Omni search]** misslyckas med ett 414-felmeddelande (Request-URI Too Long) om dispatchern kringgås vid åtkomst till Brand Portal-instansen.
* En tom ZIP-mapp hämtas om resursen innehåller ett kommatecken (`,`) i filnamnet.
* Visningsprogramanvändarna kan lägga till användare i den samling de har skapat.
* Inkonsekvent beteende uppstår när en resurs (miniatyrbild eller webbåtergivning) laddas ned via delningslänk.

Se [vad som är nytt i Brand Portal 2021.02.0](whats-new.md).

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


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

Information om vilka plattformar som är certifierade att köras med den här versionen av varumärkesportalen finns i **Stöd för Touchoptimerat användargränssnitt** i tabellen i **Webbläsare som stöds för redigeringsanvändargränssnittet** i [Tekniska krav](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

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
