---
title: Översikt över AEM Assets varumärkesportal
seo-title: Översikt över AEM Assets varumärkesportal
description: AEM Assets Brand Portal kan hjälpa er att enkelt skaffa, styra och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter.
seo-description: AEM Assets Brand Portal kan hjälpa er att enkelt skaffa, styra och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 59eeaedd7f66a0a5affa53f82f3ebbb2bcea535d
workflow-type: tm+mt
source-wordcount: '1467'
ht-degree: 2%

---


# Översikt över AEM Assets varumärkesportal {#overview-of-aem-assets-brand-portal}

Som marknadsförare behöver ni ibland samarbeta med kanalpartners och interna affärsanvändare för att snabbt skapa, hantera och leverera relevant digitalt innehåll till kunder. Snabb leverans av relevant innehåll under hela kundresan är avgörande för att öka efterfrågan, konvertering, engagemang och kundlojalitet.

Det är dock en utmaning att utveckla lösningar som stöder effektiv och säker delning av godkända varumärkeslogotyper, riktlinjer, kampanjresurser eller produktbilder med interna team, partners och återförsäljare.

**Adobe Experience Manager (AEM) Assets Brand** Portaler fokuserar på marknadsförarens behov av att effektivt samarbeta med globala Brand Portal-användare genom att tillhandahålla funktioner för tillgångsdistribution och materialbidrag.

Med mediedistribution kan ni enkelt skaffa, kontrollera och på ett säkert sätt distribuera godkända kreativa resurser till externa parter och interna företagsanvändare på olika enheter. Tillgångarna gör det möjligt för användarna på varumärkesportalen att överföra mediefiler till varumärkesportalen och publicera dem på AEM Assets, utan att man behöver ha tillgång till upphovsrättsmiljön. Avgiftsfunktionen kallas **Resurser i varumärkesportalen**. Tillsammans förbättrar det varumärkesportalens totala upplevelse av tillgångsdistribution och bidrag från användarna på varumärkesportalen (externa byråer/team), snabbar upp time-to-market för tillgångar och minskar risken för bristande efterlevnad och obehörig åtkomst.
Se [Resurshantering i varumärkesportalen](brand-portal-asset-sourcing.md).

I den webbläsarbaserade portalmiljön kan du enkelt överföra, bläddra bland, söka efter, förhandsgranska och exportera resurser i godkända format.

## Konfigurera AEM Assets med varumärkesportalen {#configure-brand-portal}

När du konfigurerar Adobe Experience Manager Assets med Brand Portal kan du publicera resurser, distribuera resurser och bidra med resurser för dem som använder Brand Portal.

>[!NOTE]
>
>Konfigurering av AEM Assets med varumärkesportalen stöds i AEM Assets som en Cloud Service, AEM Assets 6.3 och senare.

AEM Assets som Cloud Service konfigureras automatiskt med varumärkesportalen genom att aktivera varumärkesportalen från Cloud Manager. Aktiveringsarbetsflödet skapar de nödvändiga konfigurationerna i bakänden och aktiverar Brand Portal i samma IMS-organisation som i AEM Assets som en Cloud Service-instans.

AEM Assets (lokal och hanterad tjänst) konfigureras manuellt med Brand Portal med hjälp av Adobe Developer Console, som anskaffar en IMS-token (Adobe Identity Management Services) för godkännande av Brand Portal-klienten.

Mer information finns i [konfigurera AEM Assets med varumärkesportalen](../using/configure-aem-assets-with-brand-portal.md).

## Användarprofiler i varumärkesportalen {#Personas}

Varumärksportal har stöd för följande användarroller:

* Gästanvändare
* Visningsprogram
* Redigerare
* Administratör

I följande tabell visas de uppgifter som användare i dessa roller kan utföra:

|  | **Bläddra** | **Sökning** | **Hämta** | **Dela mappar** | **Dela en samling** | **Dela resurser som en länk** | **Åtkomst till administratörsverktyg** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Gästanvändare** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visningsprogram** | ✓ | ✓ | ✓ | x | x | x | x |
| **Redigerare** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administratör** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Gästanvändare kan bara bläddra bland, komma åt och söka resurser i gemensamma mappar och samlingar.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Gästanvändare {#guest-user}

Alla användare som har begränsad åtkomst till resurser på varumärkesportalen utan att behöva utföra autentisering är gästanvändare. Gästsessionen ger användarna åtkomst till gemensamma mappar och samlingar. Som gästanvändare kan du bläddra bland tillgångsinformation och ha en fullständig resursvy över medlemmar i gemensamma mappar och samlingar. Du kan söka efter, hämta och lägga till offentliga resurser i [!UICONTROL Lightbox]-samlingen.

Gästsessionen hindrar dig dock från att skapa samlingar och sparade sökningar och dela dem ytterligare. Användare i en gästsession har inte åtkomst till inställningar för mappar och samlingar och kan inte dela resurser som länkar. Här är en lista över uppgifter som en gästanvändare kan utföra:

[Bläddra bland och få tillgång till offentliga resurser](browse-assets-brand-portal.md)

[Sök efter offentliga resurser](brand-portal-searching.md)

[Hämta offentliga resurser](brand-portal-download-assets.md)

[Lägg till resurser i  [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visningsprogram {#viewer}

En standardanvändare i varumärkesportalen är vanligtvis en användare med rollen Viewer. En användare med den här rollen har åtkomst till tillåtna mappar, samlingar och resurser. Användaren kan också bläddra bland, förhandsgranska, hämta och exportera resurser (ursprungliga eller specifika återgivningar), konfigurera kontoinställningar och söka efter resurser. Här är en lista över uppgifter som en visningsprogram kan utföra:

[Bläddra bland resurser](browse-assets-brand-portal.md)

[Sök efter resurser](brand-portal-searching.md)

[Hämta resurser](brand-portal-download-assets.md)

### Redigeraren {#editor}

En användare med rollen Redigerare kan utföra alla uppgifter som en visningsprogram kan utföra. Dessutom kan redigeraren visa de filer och mappar som en administratör delar. Användaren som har rollen som redigerare kan även dela innehåll (filer, mappar, samlingar) med andra.

Förutom de uppgifter som en visningsprogram kan utföra kan en redigerare utföra följande ytterligare uppgifter:

[Dela mappar](brand-portal-sharing-folders.md)

[Dela en samling](brand-portal-share-collection.md)

[Dela resurser som en länk](brand-portal-link-share.md)

### Administratör {#administrator}

En administratör inkluderar en användare som är markerad som systemadministratör eller produktadministratör för varumärkesportalen i [!UICONTROL Admin Console]. En administratör kan lägga till och ta bort systemadministratörer och användare, definiera förinställningar, skicka e-post till användare och visa portalanvändning och lagringsrapporter.

En administratör kan utföra alla uppgifter som en redigerare kan utföra:

[Hantera användare, grupper och användarroller](brand-portal-adding-users.md)

[Anpassa skrivbordsunderlägg, sidhuvuden och e-postmeddelanden](brand-portal-branding.md)

[Använd anpassade sökfaktorer](brand-portal-search-facets.md)

[Använd metadatamatchformuläret](brand-portal-metadata-schemas.md)

[Använda bildförinställningar eller dynamiska återgivningar](brand-portal-image-presets.md)

[Arbeta med rapporter](brand-portal-reports.md)

Förutom ovanstående uppgifter kan en författare i AEM Assets utföra följande uppgifter:

[Konfigurera AEM Assets med varumärkesportalen](../using/configure-aem-assets-with-brand-portal.md)

[Publicera mappar på varumärkesportalen](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publicera samlingar på varumärkesportalen](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alternativt alias för varumärksportal-URL {#tenant-alias-for-portal-url}

Från och med varumärkesportalen 6.4.3 kan organisationer ha en alternativ (alias) URL för sin varumärksportal-klient. Du kan skapa alias-URL:en genom att ha ett alternativt prefix i URL:en.\
Observera att bara prefixet för varumärksportal-URL:en kan anpassas och inte hela URL:en. En organisation med den befintliga domänen **[!UICONTROL geomettrix.brand-portal.adobe.com]** kan till exempel få **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** skapad på begäran.

AEM Author-instansen kan bara vara [konfigurerad](../using/configure-aem-assets-with-brand-portal.md) med URL:en för klient-ID och inte med URL:en för klientalias (alternativ).

>[!NOTE]
>
>För att få ett alias för innehavarens namn i en befintlig portal-URL måste man kontakta supporten för Adobe i en ny begäran om att skapa klientalias. Denna begäran behandlas genom att först kontrollera om aliaset är tillgängligt och sedan skapa aliaset.
>
>Om du vill ersätta det gamla aliaset eller ta bort det gamla måste samma process följas.

## Begär åtkomst till varumärkesportalen {#request-access-to-brand-portal}

Användare kan begära åtkomst till varumärkesportalen från inloggningsskärmen. Dessa förfrågningar skickas till administratörer för varumärkesportalen, som ger användare åtkomst via Adobe [!UICONTROL Admin Console]. När åtkomst har beviljats får användarna ett e-postmeddelande.

Så här begär du åtkomst:

1. På inloggningssidan för varumärkesportalen väljer du **[!UICONTROL Click here]** som motsvarar **[!UICONTROL Need Access?]**. Om du vill ange gästsessionen väljer du **[!UICONTROL Click here]** som motsvarar **[!UICONTROL Guest Access?]**.

   ![Inloggningsskärm för varumärkesportal](assets/bp-login-requestaccess.png)

   Sidan [!UICONTROL Request Access] öppnas.

1. Om du vill begära åtkomst till en organisations varumärkesportal måste du ha en giltig [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] eller [!UICONTROL Federated ID].

   På sidan [!UICONTROL Request Access] loggar du in med ditt ID (scenario 1) eller skapar ett [!UICONTROL Adobe ID] (scenario 2):<br />
   ![[!UICONTROL Request access]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. Om du har en [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] eller [!UICONTROL Federated ID] klickar du på **[!UICONTROL Sign In]**.
Sidan [!UICONTROL Sign in] öppnas.
   1. Ange dina [!UICONTROL Adobe ID]-autentiseringsuppgifter och klicka på **[!UICONTROL Sign in]**.<br />

   ![Adobe loggar in](assets/bplogin_request_access_3.png)

   Du omdirigeras till sidan [!UICONTROL Request Access].<br />
   **Scenario 2**
   1. Om du inte har ett [!UICONTROL Adobe ID]-konto klickar du på **[!UICONTROL Get an Adobe ID]** på sidan [!UICONTROL Request Access] för att skapa ett.
Sidan [!UICONTROL Sign in] öppnas.
   1. Klicka på **[!UICONTROL Get an Adobe ID]**.
Sidan [!UICONTROL Sign up] öppnas.
   1. Ange för- och efternamn, e-post-ID och lösenord.
   1. Välj **[!UICONTROL Sign up]**.<br />

   ![](assets/bplogin_request_access_5.png)

   Du omdirigeras till sidan [!UICONTROL Request Access].

1. På nästa sida visas ditt namn och e-post-ID som används för att begära åtkomst. Lämna en kommentar till administratören och klicka på **[!UICONTROL Submit]**.<br />

   ![](assets/bplogin-request-access.png)

## Produktadministratörer ger åtkomst {#grant-access-to-brand-portal}

Produktadministratörer för varumärkesportalen får åtkomstbegäranden i sitt meddelandeområde på varumärkesportalen och via e-post i sin inkorg.

![Begärd avisering om åtkomst](assets/bplogin_request_access_7.png)

För att bevilja åtkomst måste produktadministratörer klicka på motsvarande meddelande i meddelandefältet i varumärkesportalen och sedan klicka på **[!UICONTROL Grant Access]**.
Alternativt kan produktadministratörer följa länken i e-postmeddelandet om åtkomstbegäran för att besöka Adobe [!UICONTROL Admin Console] och lägga till användaren i den relevanta produktkonfigurationen.

Du omdirigeras till startsidan för [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview). Använd Adobe [!UICONTROL Admin Console] för att skapa användare och tilldela dem till produktprofiler (som tidigare kallades produktkonfigurationer) som visas som grupper i varumärkesportalen. Mer information om hur du lägger till användare i [!UICONTROL Admin Console] finns i [Lägg till en användare](brand-portal-adding-users.md#add-a-user) (följ steg 4-7 i proceduren för att lägga till en användare).

## Språk i varumärkesportalen {#brand-portal-language}

Du kan ändra språk på varumärkesportalen från Adobe [!UICONTROL Experience Cloud Settings].

![Begärd avisering om åtkomst](assets/BPLang.png)

Så här ändrar du språk:

1. Välj [!UICONTROL User] > [!UICONTROL Edit Profile] på den översta menyn.<br />

   ![Redigera profil](assets/EditBPProfile.png)

1. Välj ett språk i listrutan [!UICONTROL Language] på sidan [!UICONTROL Experience Cloud Settings].

## Underhållsmeddelande för varumärkesportal {#brand-portal-maintenance-notification}

Innan Brand Portal är schemalagd för underhåll visas ett meddelande som en banderoll när du har loggat in på Brand Portal. Ett exempelmeddelande:

![](assets/bp_maintenance_notification.png)

Du kan stänga meddelandet och fortsätta använda varumärkesportalen. Det här meddelandet visas i varje ny session.

## Versions- och systeminformation {#release-and-system-information}

* [Nyheter](whats-new.md)
* [Versionsinformation](brand-portal-release-notes.md)
* [Filformat som stöds](brand-portal-supported-formats.md)

## Relaterade resurser {#related-resources}

* [Adobe kundtjänst](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)