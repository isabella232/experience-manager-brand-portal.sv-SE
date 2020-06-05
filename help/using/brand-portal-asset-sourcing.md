---
title: Resurshantering i varumärkesportalen
seo-title: Resurshantering i varumärkesportalen
description: Få en inblick i funktionen för resurskälla som lanserats i Adobe Experience Manager Assets Brand Portal.
seo-description: Få en inblick i funktionen för resurskälla som lanserats i Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: resurser
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 465b80ada85284ab0379e4a5922def32fffbfeb2
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---


# Resurskälla - översikt {#overview-asset-sourcing-in-bp}

**Med Resurshantering** kan AEM-användare (administratörer/icke-admin-användare) skapa nya mappar med en extra **Asset Contribution** -egenskap, vilket säkerställer att den nya mappen som skapas är öppen för att skickas in av Brand Portal-användare. Detta utlöser automatiskt ett arbetsflöde som skapar ytterligare två undermappar, **delade** och **NYA**, i den nya **Contribute** -mappen. AEM Administrator definierar sedan behovet genom att ladda upp en översikt över de typer av resurser som ska läggas till i bidragsmappen samt en uppsättning baslinjeresurser till **SHARED** -mappen för att säkerställa att BP-användarna har den referensinformation de behöver. Administratören kan sedan ge aktiva Brand Portal-användare åtkomst till mappen för bidrag innan den nya **Contribute** -mappen publiceras på varumärkesportalen. När användaren är klar med att lägga till innehåll i mappen **NEW** kan han eller hon publicera mappen för bidrag i AEM-redigeringsmiljön. Observera att det kan ta några minuter att slutföra importen och återspegla det nya publicerade innehållet i AEM Assets.

Dessutom ändras inte alla befintliga funktioner. Användare av varumärkesportalen kan visa, söka efter och hämta resurser från bidragsmappen samt från andra tillåtna mappar. Administratörer kan dessutom dela mappen för bidrag ytterligare, ändra egenskaper och lägga till resurser i samlingar.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

>[!NOTE]
>
>Resurshantering i varumärkesportalen stöds i AEM 6.5.2.0 och senare.
>
>Funktionen stöds inte i tidigare versioner - AEM 6.3 och AEM 6.4.
>
>Kontakta Adobes support för att uppgradera din AEM-instans till den senaste AEM-versionen som stöds.


![Källa för varumärkesportalresurser](assets/asset-sourcing.png)


>[!NOTE]
>
>Det finns ett känt fel i AEM 6.5.4. Användare av varumärkesportalen kan inte publicera resurser i mappen för bidrag till AEM Resurser när de uppgraderar till Adobe Developer Console.
>
>Problemet åtgärdas i AEM 6.5.5. Du kan uppgradera din AEM Assets-instans till den senaste Service Pack AEM 6.5.5 och [uppgradera dina konfigurationer](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) på Adobe Developer Console.
>
>Om du vill åtgärda AEM 6.5.4 direkt rekommenderar vi att du [hämtar snabbkorrigeringen](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) och installerar den på din författarinstans.


## Förutsättningar {#prerequisites}

* AEM 6.5.0.2 eller senare.
* Kontrollera att din AEM Assets-instans har konfigurerats med varumärkesportalen. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Se även {#reference-articles}

**För administratörer**

* [Konfigurera resurskälla i AEM](brand-portal-configure-asset-sourcing.md)
* [Överför användarlista för varumärkesportalen](brand-portal-configure-asset-sourcing.md)
* [Konfigurera bidragsmapp](brand-portal-contribution-folder.md)
* [Överför baslinjeresurser till avgiftsmappen](brand-portal-upload-baseline-assets.md)
* [Publicera mapp för bidrag till varumärkesportalen](brand-portal-publish-contribution-folder-to-brand-portal.md)

**För varumärkesportalanvändare**

* [Hämta resurskrav](brand-portal-download-asset-requirements.md)
* [Överför nya resurser till mappen för bidrag](brand-portal-upload-assets-to-contribution-folder.md)
* [Publicera mapp för bidrag till AEM Resurser](brand-portal-publish-contribution-folder-to-aem-assets.md)
