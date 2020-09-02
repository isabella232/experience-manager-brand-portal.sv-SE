---
title: Resurshantering i varumärkesportalen
seo-title: Resurshantering i varumärkesportalen
description: Få en inblick i den nya funktionen för resurskälla som lanserats i Adobe Experience Manager Assets Brand Portal.
seo-description: Få en inblick i den nya funktionen för resurskälla som lanserats i Adobe Experience Manager Assets Brand Portal.
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
source-git-commit: a32eed22ebfbc683fca96950fc2e08bf5cfaccb3
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# Resurskälla - översikt {#overview-asset-sourcing-in-bp}

**Med Resurshantering** kan AEM användare (administratörer/icke-admin-användare) skapa nya mappar med en extra **Asset Contribution** -egenskap, vilket säkerställer att den nya mappen som skapas är öppen för resursplacering av Brand Portal-användare. Detta utlöser automatiskt ett arbetsflöde som skapar ytterligare två undermappar, **delade** och **NYA**, i den nya **Contribute** -mappen. Den AEM administratören definierar sedan behovet genom att ladda upp en översikt över de typer av resurser som ska läggas till i bidragsmappen, samt en uppsättning baslinjeresurser, till **SHARED** -mappen för att säkerställa att BP-användarna har den referensinformation de behöver. Administratören kan sedan ge aktiva Brand Portal-användare åtkomst till mappen för bidrag innan den nya **Contribute** -mappen publiceras på varumärkesportalen. När användaren är klar med att lägga till innehåll i mappen **NEW** kan han eller hon publicera mappen för bidrag i den AEM författarmiljön. Observera att det kan ta några minuter att slutföra importen och återspegla det nya publicerade innehållet i AEM Assets.

Dessutom ändras inte alla befintliga funktioner. Användare av varumärkesportalen kan visa, söka efter och hämta resurser från bidragsmappen samt från andra tillåtna mappar. Administratörer kan dessutom dela mappen för bidrag ytterligare, ändra egenskaper och lägga till resurser i samlingar.

## Förutsättningar {#prerequisites}

* AEM 6.5.2 eller senare.
* Kontrollera att din AEM Assets-instans är konfigurerad med varumärkesportalen. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Se till att din varumärksportal är konfigurerad med en instans av AEM Assets-författare.

>[!NOTE]
>
>Resurshantering stöds inte som Cloud Service i AEM Assets.


>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Källa för varumärkesportalresurser](assets/asset-sourcing.png)


>[!NOTE]
>
>Det finns ett känt fel i AEM 6.5.4. Användare av varumärkesportalen kan inte publicera resurser i mappen för bidrag till AEM Assets när de uppgraderar till Adobe Developer Console.
>
>Problemet är åtgärdat i AEM 6.5.5. Du kan uppgradera din AEM Assets-instans till den senaste Service Pack-versionen AEM 6.5.5 och [uppgradera dina konfigurationer](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) på Adobe Developer Console.
>
>För att åtgärda AEM 6.5.4 rekommenderar vi att du [hämtar snabbkorrigeringen](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) och installerar den på din författarinstans.


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
* [Publicera bidragsmapp till AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
