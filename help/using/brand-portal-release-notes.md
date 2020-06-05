---
title: Versionsinformation
seo-title: Versionsinformation
description: Få insikt i funktioner, förbättringar, åtgärdade kritiska problem och kända problem i Adobe Experience Manager Assets Brand Portal 6.4.6.2.
seo-description: Få insikt i förbättringarna, åtgärdade kritiska problem och kända problem i Adobe Experience Manager Assets Brand Portal 6.4.6.2.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 9413aa609b5c0d66c9d23ddf9dcd9d28ec4da798
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 3%

---


# Versionsinformation {#release-notes}

Få en inblick i de nya funktionerna, förbättringarna, de allvarliga problemen och de kända problemen i Adobe Experience Manager Assets Brand Portal 6.4.6.2.

## Versionsinformation {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.6.2 |
| Date | Juni 2020 |

## Översikt {#overview}

Adobe Experience Manager Assets Brand Portal (AEM) hjälper er att enkelt skaffa, kontrollera och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter. Det bidrar till att effektivisera resursdelning, snabbar upp time-to-market för tillgångar och minskar risken för bristande efterlevnad och obehörig åtkomst. Med Brand Portal kan man söka, förhandsgranska, ladda ned och exportera material i företagsgodkända format - när som helst, var som helst.

## Nyheter i 6.4.6.2 {#what-s-new-in-6462}

### Allvarliga problem har åtgärdats {#critical-issues-fixed-6462}

Den här versionen innehåller korrigeringar av följande allvarliga problem:

* Om du tar bort ett publicerat metadataschema från varumärkesportalen uppstår ett fel.

* Om administratören konfigurerar Experience Manager Assets 6.5.4 med varumärkesportalen via Adobe Developer Console kan inte användaren på varumärkesportalen publicera resurser från varumärkesportalen till Experience Manager.

* Duplicerad replikering av de överordnade mapparna som orsakar konflikter.

* Användaren kan inte generera länkresursrapporten.

* Användare kan kopiera MAC-hemligheter för en varumärkesportalslutpunkt med hjälp av kommandot copyPage.

* cqTags som orsakar omindexering på VA5-klon.


### Kända fel {#known-issues-6462}

Den här versionen innehåller följande kända fel:

* Om en mapp i hierarkin byter namn från AEM Resurser och den kapslade mappen som innehåller en resurs publiceras på varumärkesportalen, uppdateras inte mappens namn i varumärkesportalen förrän rotmappen publiceras igen.


## Nyheter i 6.4.6 {#what-s-new-in-646}

### Nya funktioner {#new-feature}

Den här versionen innehåller följande nya funktioner:

* Captcha för gästinloggning på Brand Portal. See, [Brand Portal guest access](../using/guest-access.md) for more information.

* Brand Portal stöds nu med molntjänsten AEM Assets. Du kan konfigurera AEM Assets så att det kan användas tillsammans med varumärkesportalen för att dela och distribuera resurser med användare på varumärkesportalen.
Mer information finns i [Konfigurera molntjänsten AEM Assets med varumärkesportalen](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html).

### Förbättringar {#enhancements-646}

Den här versionen av varumärkesportalen innehåller följande förbättringar:

* I AEM 6.3 och senare ändras auktoriseringskanalen mellan AEM Assets och Brand Portal. AEM Assets har nu konfigurerats med Brand Portal via Adobe Developer Console, som köper en IMS-token för auktorisering av din varumärksportal.

>[!NOTE]
>
>Konfiguration via äldre OAuth stöds inte längre från 6 april 2020 och har ändrats till att konfigureras via Adobe Developer Console.



>[!TIP]
>
>***Endast för befintliga kunder***
>
>Äldre OAuth Gateway-konfiguration fortsätter att fungera för befintliga kunder.
>
>Om du får problem med äldre OAuth Gateway-konfiguration tar du bort den befintliga konfigurationen och skapar en ny konfiguration via Adobe Developer Console.


For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

### Allvarliga problem har åtgärdats {#critical-issues-fixed}

Den här versionen innehåller korrigeringar av följande allvarliga problem:

* Värden för rullgardinsmenyn för metadataschema visas inte i resursegenskaper.

* Delschemat Metadata visar inte flikar baserade på mimeType i resursegenskaper.

* Ett felmeddelande fylls i när metadatamatchemat avpubliceras, även om schemat tas bort vid backend.

* Förhandsvisningsbilden visas inte för en publicerad resurs.

* Användaren kan inte publicera eller avpublicera resurser som innehåller en enda offert i namnet.

* Villkoren visas inte när du hämtar flera resurser.

* Mindre säkerhetsluckor har åtgärdats.

### Kända fel {#known-issues}

Den här versionen innehåller följande kända fel:

* Användare av varumärkesportalen kan inte publicera resurser i mappen för bidrag till AEM Resurser när de uppgraderar till Adobe Developer Console på AEM 6.5.4.

   Problemet åtgärdas i nästa Service Pack 6.5.5.

   Om du vill åtgärda AEM 6.5.4 direkt rekommenderar vi att du [hämtar snabbkorrigeringen](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) och installerar den på din författarinstans.

* Alternativet Exkludera systemåtergivningar fungerar inte korrekt när du hämtar en resurs.


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

* [Adobe Experience Manager Product Page på adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Dokumentation för Assets Brand Portal](https://helpx.adobe.com/se/experience-manager/brand-portal/user-guide.html)

## Produktåtkomst och support (begränsade platser) {#product-access-and-support-restricted-sites}

Dessa webbplatser är bara tillgängliga för kunder. Om du är kund och behöver åtkomst kontaktar du din kontoansvarige på Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Produktåtkomst](https://login.marketing.adobe.com)

* [Adobes kundtjänst](https://helpx.adobe.com/contact.html)
