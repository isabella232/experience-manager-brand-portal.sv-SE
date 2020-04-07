---
title: Versionsinformation
seo-title: Versionsinformation
description: Få insikt i funktioner, förbättringar, åtgärdade kritiska problem och kända problem i Adobe Experience Manager Assets Brand Portal 6.4.6.
seo-description: Få insikt i förbättringarna, åtgärdade kritiska problem och kända problem i Adobe Experience Manager Assets Brand Portal 6.4.6.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: a357879f921ac88f89d1bc11bff379f1d0d3e681

---


# Versionsinformation {#release-notes}

Få en inblick i de nya funktionerna, förbättringarna, de allvarliga problemen och de kända problemen i Adobe Experience Manager Assets Brand Portal 6.4.6.

## Versionsinformation {#release-information}

| Produkt | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Version | 6.4.6 |
| Date | Mars 2020 |

## Översikt {#overview}

Adobe Experience Manager Assets Brand Portal (AEM) hjälper er att enkelt skaffa, kontrollera och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter. Det bidrar till att effektivisera resursdelning, snabbar upp time-to-market för tillgångar och minskar risken för bristande efterlevnad och obehörig åtkomst. Med Brand Portal kan man söka, förhandsgranska, ladda ned och exportera material i företagsgodkända format - när som helst, var som helst.

## Nyheter i 6.4.6 {#what-s-new-in-646}

### Nya funktioner {#new-feature}

Den här versionen innehåller följande nya funktioner:

* Captcha för gästinloggning på Brand Portal. Mer information finns i [Gäståtkomst](../using/guest-access.md) för varumärkesportalen.

* Brand Portal stöds nu med molntjänsten AEM Assets. Du kan konfigurera AEM Assets så att det kan användas tillsammans med varumärkesportalen för att dela och distribuera resurser med användare på varumärkesportalen.
Mer information finns i [Konfigurera molntjänsten AEM Assets med varumärkesportalen](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brandportal/configure-aem-assets-with-brand-portal.html).

### Förbättringar {#enhancements-646}

Den här versionen av varumärkesportalen innehåller följande förbättringar:

* I AEM 6.3 och senare ändras auktoriseringskanalen mellan AEM Assets och Brand Portal. AEM Assets har nu konfigurerats med Brand Portal via Adobe I/O, som anskaffar en IMS-token för auktorisering av din klient för varumärkesportalen.

   >[!NOTE]
   >
   >Konfiguration via äldre OAuth stöds inte längre från 6 april 2020 och har ändrats till att konfigureras via Adobe I/O.


>[!TIP]
>
>***Endast för befintliga kunder***
>
>Vi rekommenderar att du fortsätter använda den befintliga äldre OAuth Gateway-konfigurationen. Om du får problem med äldre OAuth Gateway-konfiguration tar du bort den befintliga konfigurationen och skapar en ny konfiguration via Adobe I/O.


Mer information finns i [Konfigurera AEM-resurser med varumärkesportalen](configure-aem-assets-with-brand-portal.md)

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

* Användare av varumärkesportalen kan inte publicera material i mappen för bidrag till AEM Assets när de uppgraderar till Adobe I/O på AEM 6.5.4.

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

* [](https://daycare.day.com) [Produktåtkomst](https://login.marketing.adobe.com)

* [Adobes kundtjänst](https://helpx.adobe.com/contact.html)
