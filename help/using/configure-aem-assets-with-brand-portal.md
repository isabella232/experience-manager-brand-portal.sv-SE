---
title: Konfigurera AEM Assets med varumärkesportalen
seo-title: Konfigurera AEM Assets med varumärkesportalen
description: Få insikt i hur du konfigurerar AEM Assets med varumärkesportalen.
seo-description: Få insikt i hur du konfigurerar AEM Assets med varumärkesportalen.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: bfb0c38bf8d5b542caf9d0d20d3168cdcac649b3
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 8%

---


# Konfigurera AEM Assets med varumärkesportalen {#configure-integration}

När du konfigurerar Adobe Experience Manager Assets med Brand Portal kan du publicera resurser, distribuera resurser och bidra med resurser för dem som använder Brand Portal. Med den kan AEM Assets-användare publicera och distribuera material med Brand Portal-användare. Brand Portal-användare kan komma åt de delade resurserna och bidra genom att överföra nya resurser till resursavgiftsmapparna och publicera dem tillbaka till AEM Assets.

Konfigurering av AEM Assets med varumärkesportalen stöds på:
* AEM Assets as a Cloud Service
* AEM Assets (lokal och Managed Services) 6.3 och senare

AEM Assets som Cloud Service konfigureras automatiskt med varumärkesportalen genom att aktivera varumärkesportalen från Cloud Manager. Aktiveringsarbetsflödet skapar de nödvändiga konfigurationerna i bakänden och aktiverar Brand Portal i samma IMS-organisation som i AEM Assets som en Cloud Service-instans.

AEM Assets (lokalt och Managed Services) konfigureras manuellt med Brand Portal via Adobe Developer Console, som köper en IMS-token (Adobe Identity Management Services) för godkännande av Brand Portal-klienten.

>[!NOTE]
>
>***För AEM Assets 6.3 och senare***
>
>Tidigare konfigurerades Brand Portal i det klassiska gränssnittet via äldre OAuth Gateway, som använder JSON Web token-utbyte för att erhålla en IMS-token för auktorisering.
>
>Konfiguration via äldre OAuth stöds inte längre från 6 april 2020 och har ändrats till att konfigureras via Adobe Developer Console.


>[!TIP]
>
>***Endast för befintliga kunder (lokalt och Managed Services)***
>
>Äldre OAuth Gateway-konfiguration fortsätter att fungera för befintliga kunder.
>
>Om du får problem med äldre OAuth Gateway-konfiguration tar du bort den befintliga konfigurationen och skapar en ny konfiguration via Adobe Developer Console.

Stegen för att konfigurera AEM Assets med varumärkesportalen skiljer sig åt beroende på vilken version du har AEM och om du konfigurerar för första gången eller uppgraderar de befintliga konfigurationerna:

| **AEM** | **Ny konfiguration** | **Uppgraderingskonfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Aktivera varumärkesportal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 och senare)** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 och senare)** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 och senare)** | [Skapa en konfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Uppgraderingskonfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Kontakta supporten | Kontakta supporten |
