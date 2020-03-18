---
title: Administrera allmänna klientkonfigurationer
seo-title: Administrera allmänna klientkonfigurationer
description: Konfigurera hämtningsacceleration, skapa offentlig smart [!UICONTROL-samling], skapa offentlig [!UICONTROL-samling] och göra det möjligt för administratörsanvändare att ta bort resurser på klientorganisationer.
seo-description: Konfigurera hämtningsacceleration, skapa offentlig smart [!UICONTROL-samling], skapa offentlig [!UICONTROL-samling] och göra det möjligt för administratörsanvändare att ta bort resurser på klientorganisationer.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
translation-type: tm+mt
source-git-commit: ff0c8c23b6c76dc9027b560b9db4af2f4b35313e

---


# Administrera allmänna klientkonfigurationer {#administer-general-tenant-configurations}

Med AEM Assets Brand Portal kan organisationer konfigurera följande funktioner för specifika innehavare:

* Borttagning av resurser av administratörer
* Skapande av offentlig samling av icke-adminanvändare
* Skapande av offentlig smart samling av icke-adminanvändare
* Ladda ned acceleration
* Överordnad hierarki för delade mappar som är synliga för användare som inte är administratörer

Dessa konfigurationer har tillhandahållits som **[!UICONTROL General Settings]** konfigurationer på panelen Administrationsverktyg.

![](assets/general-configs.png)

**En** konfiguration som gör att administratörer kan ta bort resurser från varumärkesportalen. (Standard är aktiverat)

**B** Configuration som tillåter att icke-adminanvändare skapar offentliga samlingar. (Standard är aktiverat)

**C** Configuration som tillåter att icke-admin-användare skapar publika smarta samlingar. (Standard är aktiverat)

**D** Configuration för att tillåta nedladdningsacceleration av resurser som hämtats från portalen och från delade länkar. (Standard är inaktiverat)

**E** Configuration för att visa mapphierarkin (från roten) för delade mappar till icke-adminanvändare (redigerare, visningsprogram, gästanvändare). (Standard är inaktiverat)

## Aktivera/inaktivera allmänna konfigurationer {#enable-disable-general-configurations}

Så här aktiverar/inaktiverar du dessa konfigurationer:

1. Logga in med administratörsbehörighet.
1. Välj AEM-logotypen för att få tillgång till administrationsverktygen i verktygsfältet högst upp.
1. Öppna **[!UICONTROL General]** sidan genom **[!UICONTROL General Settings]** att markera på panelen Administrationsverktyg.
1. Använd respektive växlingsknapp för att aktivera/inaktivera någon av de allmänna konfigurationerna.
1. **[!UICONTROL Save]** ändringarna.
1. Logga ut för att ändringarna ska börja gälla.

## Tillåt administratörsanvändare att ta bort resurser från varumärkesportalen {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Allow users to delete]** kan organisationer tillåta (eller begränsa) användare med administratörsbehörighet att ta bort resurser och mappar från varumärkesportalen.

## Tillåt att offentliga samlingar skapas av icke-administratörer {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL Tillåt skapande av offentliga samlingar]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) konfigurationskontrollerar om icke-administratörer kan skapa offentliga samlingar på varumärkesportalen. Konfigurationen är aktiverad som standard. Genom att inaktivera konfigurationsorganisationerna kan de förhindra att det finns många offentliga samlingar på portalen så att systemutrymmet kan sparas.

## Tillåt att icke-administratörer skapar publika smarta samlingar {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL Tillåt att offentliga smarta samlingar skapas]](../using/brand-portal-searching.md#main-pars-header-500620467) konfigurationskontrollerar om icke-administratörer kan spara sina sökningar som smarta samlingar och göra dem offentliga för den klienten. Konfigurationen är aktiverad som standard. Genom att inaktivera konfigurationsorganisationerna kan du förhindra att det finns ett stort antal publika smarta samlingar som skapats av icke-adminanvändare på organisationens varumärkesportal.

## Tillåt hämtning av acceleration {#allow-download-acceleration}

[Med konfigurationen [!UICONTROL Tillåt hämtningsacceleration]](../using/accelerated-download.md) kan organisationer tillåta accelererad hämtning av resurser från Brand Portal och delade länkar genom att integrera med IBM Aspera Connect som är ett program som installeras vid behov. Programmet använder tillverkarspecifik teknik för att ta bort TCP-omkostnader.

## Aktivera mapphierarki {#enable-folder-hierarchy}

[Med konfigurationen [!UICONTROL Aktivera mapphierarki]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) kan administratörer styra hur icke-administratörsanvändare (redigerare, visningsprogram och gästanvändare) ser de delade mapparna efter inloggning.
