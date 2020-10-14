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
source-git-commit: 2f6ec4ac56390b2243e1d1a2c2adb34eb9aad7b2
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 9%

---


# Konfigurera AEM Assets med varumärkesportalen {#configure-integration}

Om du konfigurerar Adobe Experience Manager Assets som en Cloud Service med Adobe Experience Manager Assets Brand Portal kan du publicera och distribuera resurser hos Brand Portal-användarna. Om du konfigurerar AEM 6.3 (och senare) med Brand Portal kan du publicera tillgångar, distribuera resurser och ge användarna möjlighet att bidra med resurser.

Adobe Experience Manager Assets har konfigurerats med Brand Portal via Adobe Developer Console, som köper en IMS-token (Adobe Identity Management Services) för auktorisering av din varumärksportal.

>[!NOTE]
>
>***För AEM Assets 6.3 och senare***
>
>Tidigare konfigurerades Brand Portal i det klassiska gränssnittet via äldre OAuth Gateway, som använder JSON Web token-utbyte för att erhålla en IMS-token för auktorisering.
>
>Konfiguration via äldre OAuth stöds inte längre från 6 april 2020 och har ändrats till att konfigureras via Adobe Developer Console.


>[!TIP]
>
>***Endast för befintliga kunder***
>
>Äldre OAuth Gateway-konfiguration fortsätter att fungera för befintliga kunder.
>
>Om du får problem med äldre OAuth Gateway-konfiguration tar du bort den befintliga konfigurationen och skapar en ny konfiguration via Adobe Developer Console.

Stegen för att konfigurera AEM Assets med varumärkesportalen skiljer sig åt beroende på vilken version du har AEM och om du konfigurerar för första gången eller uppgraderar de befintliga konfigurationerna:

| **AEM** | **Ny konfiguration** | **Uppgraderingskonfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 och senare)** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 och senare)** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 och senare)** | [Skapa en konfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Uppgraderingskonfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Kontakta supporten | Kontakta supporten |
