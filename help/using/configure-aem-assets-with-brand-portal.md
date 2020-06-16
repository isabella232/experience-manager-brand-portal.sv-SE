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
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 9%

---


# Konfigurera AEM Assets med varumärkesportalen {#configure-integration}

Adobe Experience Manager (AEM) Assets konfigureras med Brand Portal via Adobe Developer Console, som anskaffar en IMS-token för auktorisering av din varumärksportal. Brand Portal stöds nu i molntjänsten AEM Assets, AEM Assets 6.3 och senare.

Om du konfigurerar AEM Assets kan du använda Brand Portal för att publicera och distribuera resurser hos Brand Portal-användarna. Med Configuring Brand Portal on AEM 6.3 (och senare) kan man publicera resurser, distribuera resurser och bidra med resurser för dem som använder varumärkesportalen.

>[!NOTE]
>
>***För AEM Assets 6.3 och senare***
>
>Tidigare konfigurerades varumärkesportalen i Classic UI via äldre OAuth Gateway, som använder JWT-tokenutbyte för att erhålla en IMS Access-token för auktorisering.
>
>Konfiguration via äldre OAuth stöds inte längre från 6 april 2020 och har ändrats till att konfigureras via Adobe Developer Console.


>[!TIP]
>
>***Endast för befintliga kunder***
>
>Äldre OAuth Gateway-konfiguration fortsätter att fungera för befintliga kunder.
>
>Om du får problem med äldre OAuth Gateway-konfiguration tar du bort den befintliga konfigurationen och skapar en ny konfiguration via Adobe Developer Console.


Stegen för att konfigurera AEM Assets med varumärkesportalen skiljer sig åt beroende på din AEM-version, om du konfigurerar för första gången eller uppgraderar befintliga konfigurationer:

| **AEM-version** | **Ny konfiguration** | **Uppgraderingskonfiguration** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 och senare)** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 och senare)** | [Skapa en konfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Uppgraderingskonfiguration](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 och senare)** | [Skapa en konfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Uppgraderingskonfiguration](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Kontakta supporten | Kontakta supporten |


