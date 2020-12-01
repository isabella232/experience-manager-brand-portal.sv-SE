---
title: Administrera användaråtkomst på varumärkesportalen
seo-title: Administrera användaråtkomst på varumärkesportalen
description: Konfigurera gäståtkomst och åtkomst för nya användare på varumärkesportalen.
seo-description: Konfigurera gäståtkomst och åtkomst för nya användare på varumärkesportalen.
uuid: 522b499d-33a0-455f-ac7e-719face48009
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 393025b4-722d-4e81-8a47-f83415d0b9b6
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---


# Administrera användaråtkomst på varumärkesportalen {#administer-user-access-on-brand-portal}

Från och med AEM Assets Brand Portal 6.4.2 ger administratörer behörighet att konfigurera gäståtkomst och göra det möjligt för användare att begära åtkomst på organisationens varumärkesportal. Dessa konfigurationer har angetts som **[!UICONTROL Access Settings]**-konfigurationer på administrationspanelen. Båda inställningarna är inaktiverade som standard.

![](assets/access-configs.png)

****   AConfiguration som tillåter gäståtkomst på varumärkesportalen med hjälp av  **[!UICONTROL Guest Access?]** länken på välkomstskärmen för varumärkesportalen. (Standard är inaktiverat)

**BConfiguration**   som tillåter användare att begära åtkomst till varumärkesportalen med hjälp av  **[!UICONTROL Need access?]** länken på välkomstskärmen för varumärkesportalen. (Standard är inaktiverat)

## Tillåt gäståtkomst {#allow-guest-access}

Genom att tillåta gäståtkomst kan användarna komma åt de offentliga resurserna utan att behöva logga in på varumärkesportalen.
Administratören måste utföra följande steg för att tillåta gäståtkomst:

1. Välj AEM logotyp för att öppna administrationsverktygen i verktygsfältet högst upp.
1. På panelen Administrationsverktyg väljer du **[!UICONTROL Access]** för att öppna sidan **[!UICONTROL Access Settings]**.
1. Aktivera **[!UICONTROL Allow Guest Access]**-konfigurationen.
1. **[!UICONTROL Save]** ändringarna.
1. Logga ut för att ändringarna ska börja gälla.

![](assets/bp-welcome-screen.png)

## Tillåt användare att begära åtkomst {#allow-users-to-request-access}

Administratörer kan tillåta att användarna i organisationen begär åtkomst till varumärkesportalen från välkomstskärmen. Administratörer måste dock aktivera konfigurationen **[!UICONTROL Allow Users to Request Access]** så att länken för åtkomstbegäran visas på välkomstskärmen.

För att organisationsanvändare ska kunna begära åtkomst på varumärkesportalen måste administratörerna:

1. Välj AEM logotyp för att öppna administrationsverktygen i verktygsfältet högst upp.
1. På panelen Administrationsverktyg väljer du **[!UICONTROL Access]** för att öppna sidan **[!UICONTROL Access Settings]**.
1. Aktivera **[!UICONTROL Allow Users to Request Access]**-konfigurationen.
1. **[!UICONTROL Save]** ändringarna.
1. Logga ut för att ändringarna ska börja gälla.
