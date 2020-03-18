---
title: Konfigurera resurskälla
seo-title: Konfigurera resurskälla
description: Få insikt i hur ni konfigurerar funktionen för resurskälla i AEM Assets.
seo-description: Få insikt i hur ni konfigurerar funktionen för resurskälla i AEM Assets.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: aa6bd187124888cd62ca1f5c7192f9d65ac6ca8a

---


# Konfigurera resurskälla {#configure-asset-sourcing}

AEM-administratörer kan konfigurera **Resurser** inifrån AEM-författarinstansen. Administratören aktiverar konfigurationen av resurskällans funktionsflagga från **AEM Web Console Configuration** och överför listan över aktiva Brand Portal-användare i **AEM Resurser**.

>[!NOTE]
>
>Innan du börjar med konfigurationen bör du kontrollera att din AEM Resurser-instans har konfigurerats med Varumärkeportal. Se [Konfigurera AEM Assets med varumärkesportalen](../using/configure-aem-assets-with-brand-portal.md).


I följande video visas hur du konfigurerar resurskälla för din AEM-författarinstans:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

## Aktivera resurskälla {#enable-asset-sourcing}

AEM-administratörer kan aktivera Resurser inifrån AEM Web Console Configuration (alias Configuration Manager).

**Så här aktiverar du resurskälla:**
1. Logga in på din AEM-författarinstans och öppna Configuration ManagerDefault URL: http:// localhost:4502/system/console/configMgr
1. Sök med nyckelordet **Resurser** för att hitta **[!UICONTROL Asset Sourcing Feature Flag Config]**
1. Klicka **[!UICONTROL Asset Sourcing Feature Flag Config]** för att öppna konfigurationsfönstret
1. Kryssrutan Aktivera **[!UICONTROL feature.flag.active.status]**
1. Klicka på **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)

## Överför användarlista för varumärkesportalen {#upload-bp-user-list}

AEM-administratörer kan överföra användarkonfigurationsfilen för varumärkesportalen (.csv) som innehåller den aktiva användarlistan för varumärkesportalen i AEM Resurser. En mapp för bidrag kan bara delas med de aktiva Brand Portal-användare som definieras i användarlistan. Administratören kan även lägga till nya användare i konfigurationsfilen och överföra den ändrade användarlistan.

>[!NOTE]
>
>CSV-filens format är detsamma som det som stöds av Admin Console för bulkanvändarimport. E-post, förnamn och efternamn är obligatoriska.

Administratören kan lägga till nya användare i AEM Admin Console. Mer information finns i [Hantera användare](brand-portal-adding-users.md) . När du har lagt till användare i Admin Console kan dessa användare läggas till i användarkonfigurationsfilen för varumärkesportalen och sedan tilldelas behörighet att komma åt mappen för bidrag.

**Så här överför du användarlistan för varumärkesportalen:**
1. Logga in på din AEM-författarinstansStandard-URL: http:// localhost:4502/aem/start.html
1. Navigera från **verktygspanelen** ![](assets/tools.png) till **[!UICONTROL Assets > Brand Portal Users]**
   ![](assets/upload-user-list1.png)
1. Fönstret för ladda upp medverkande på varumärkesportalen öppnas.
Bläddra från den lokala datorn och överför **konfigurationsfilen** (.csv) som innehåller listan över aktiva Brand Portal-användare.
1. Klicka på **[!UICONTROL Save]**.
   ![](assets/upload-user-list2.png)


Administratörer kan ge åtkomst till specifika användare/grupper från den här användarlistan när de konfigurerar mappen för bidrag.

Mer information finns i [Konfigurera mapp](brand-portal-contribution-folder.md)för bidrag.