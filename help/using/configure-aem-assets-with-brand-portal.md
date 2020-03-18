---
title: Konfigurera AEM-resurser med varumärkesportalen
seo-title: Konfigurera AEM-resurser med varumärkesportalen
description: Få insikt i hur du konfigurerar AEM Assets med varumärkesportalen.
seo-description: Få insikt i hur du konfigurerar AEM Assets med varumärkesportalen.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 58110f1635a9e74340d4a8901e86c0c6a99cf4e2

---


# Konfigurera AEM-resurser med varumärkesportalen {#configure-integration}

Adobe Experience Manager Assets (AEM) är konfigurerat med varumärkesportalen via Adobe I/O, som anskaffar en IMS-token för auktorisering av er varumärkesportal. Konfigurationen möjliggör publicering av resurser, distribution av resurser och funktioner för komponentportalanvändare.

>[!NOTE]
>
>Tidigare konfigurerades varumärkesportalen i Classic UI via äldre OAuth Gateway, som använder JWT-tokenutbyte för att erhålla en IMS Access-token för auktorisering.
>
>Konfiguration via äldre OAuth stöds inte längre från 6 april 2020 och har ändrats till att konfigureras via Adobe I/O.
>
>Om du är en befintlig Brand Portal-användare med konfiguration för äldre OAuth Gateway rekommenderar vi att du tar bort de befintliga konfigurationerna och skapar en ny konfiguration för Adobe I/O.
>
>Den befintliga konfigurationen fortsätter dock att fungera om du inte ändrar konfigurationerna.

Stegen för att konfigurera AEM Assets med Brand Portal är olika beroende på din AEM-version, om du konfigurerar för första gången eller uppgraderar befintliga konfigurationer:

| **AEM-version** | **Ny konfiguration** | **Uppgraderingskonfiguration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 och senare)** | [Skapa konfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 och senare)** | [Skapa konfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 och senare)** | [Skapa konfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Uppgraderingskonfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Kontakta supporten | Kontakta supporten |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
