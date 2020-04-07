---
title: Vanliga frågor
seo-title: null
description: Få insikt i de vanliga frågorna i Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 9169407bbbfabd94be31c89c028be64e55afc064

---


# Frequently Asked Questions {#frequently-asked-questions}

Frågor och svar om varumärkesportalen fokuserar på frågor och problem som slutanvändarna kan råka ut för när de arbetar med den senaste versionen av AEM Assets Brand Portal 6.4.5 eller tidigare versioner.


## Frågor och svar om varumärkesportalen 6.4.6 {#faqs-bp646}

**Frågor. Den befintliga gamla OAuth-slutpunkten (`https://legacy-oauth.cloud.adobe.io/login`) fungerar inte. Vad kan vara den möjliga orsaken?**

**Ans.** Äldre OAuth-konfiguration är föråldrad. Du måste uppgradera AEM Assets-författarinstanserna till den senaste Service Pack-versionen och konfigurera den med Adobe IO. Mer information finns i [Konfigurera AEM-resurser med varumärkesportalen](configure-aem-assets-with-brand-portal.md) . För att äldre OAuth-konfiguration ska fungera tills du uppgraderar måste du dock uppdatera den äldre OAuth-slutpunkten till `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Frågor. Jag kan inte publicera resurserna i mappen för bidrag från Brand Portal till AEM Assets efter uppgradering till Adobe I/O. Min författarinstans finns på AEM 6.5.4. Vad kan vara den möjliga orsaken?**

**Ans.** Ja, det finns ett känt fel när du publicerar material i distributionsmappen till AEM Assets på AEM 6.5.4 med Adobe I/O. Problemet kommer att åtgärdas i nästa Service Pack.

Om du vill åtgärda AEM 6.5.4 direkt rekommenderar vi att du [hämtar snabbkorrigeringen](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) och installerar den på din AEM-författarinstans.


## Frågor och svar om varumärkesportalen 6.4.5 {#faqs-bp645}

**Frågor. Vilken är den största förändringen i version 6.4.5 av varumärkesportalen?**

**Ans.** AEM Assets Brand Portal 6.4.5 är en funktionsrelease som gör det möjligt för Brand Portal-användare att ladda upp innehåll inifrån Brand Portal och publicera Contribute-mappen till AEM Assets utan administratörsbehörighet.
Mer information finns i [Resurser i Varumärkesportalen](brand-portal-asset-sourcing.md).



**Frågor. Kommer jag att förlora åtkomsten till befintliga resurser, funktioner eller konfigurationer som jag har skapat?**

**Ans.** Alla befintliga funktioner och konfigurationer förblir intakta. Slutanvändarna påverkas inte och innehållet förblir intakt.



**Frågor. När ska jag byta till den nya versionen av varumärkesportalen?**

**Ans.** Varumärkesportalen 6.4.5 släpptes till produktion i oktober 2019. Och nästa Brand Portal-version förväntas släppas tredje kvartalet 2020.
För uppdateringar och versionsändringar bör du spåra [versionsinformation](brand-portal-release-notes.md) och [nyheter i varumärkesportalen](whats-new.md).



**Frågor. Kommer mina användare att påverkas?**

**Ans.** Brand Portal 6.4.5 finns endast i Brand Portal, så slutanvändarna påverkas inte.



**Frågor. Måste jag agera som varumärksportal?**

**Ans.** Brand Portal 6.4.5 innehåller en ny funktion som heter Asset Source. AEM-administratören måste konfigurera funktionen Resurser i AEM Resurser för att aktivera funktionen för användare på varumärkesportalen. Mer information finns i [Aktivera resurskälla](brand-portal-configure-asset-sourcing.md).



**Frågor. Vem kan skapa en Contribute-mapp?**

**Ans.** Alla AEM-användare som har behörighet att skapa en ny mapp i AEM Resurser kan skapa en **Contribute** -mapp. Om du vill skapa en **Contribute** -mapp skapar du en ny mapp av typen **Asset Contribution**.
Den här mappen delas med de aktiva Brand Portal-användarna för bidrag.



**Frågor. Vad innehåller en Contribute-mapp?**

**Ans.** Mappen **Contribute** innehåller två undermappar **NEW** och **SHARED**. Till att börja med är mappen NEW tom och mappen SHARED innehåller referensinnehållet (återanvändbara resurser) för Brand Portal-användarna.
Brand Portal-användarna kommer åt **Contribute** -mappen och överför innehåll i mappen **NEW** .



**Frågor.  Kan jag ändra namnet på en befintlig Contribute-mapp?**

**Ans.** **Nej**, du kan inte ändra namnet på en befintlig **Contribute** -mapp.



**Frågor. Vad är tillgångskrav utan bidrag?**

**Ans.** Det **korta** dokumentet som är bifogat till **Contribute** -mappen och referensinnehållet (återanvändbara resurser) som överförts i **SHARED** -mappen hjälper användaren på varumärkesportalen att förstå behovet av bidrag och förväntningar som medverkande och kallas tillsammans för tillgångskrav.



**Frågor. Kan jag överföra resurser till en tillåten mapp?**

**Ans.** Inte alla tillåtna mappar. En varumärkesportalanvändare kan bara överföra innehåll till **Contribute** -mappen som delas av AEM- eller varumärkesportaladministratören.



**Frågor. Hur får jag åtkomst till en Contribute-mapp?**

**Ans.** Du kan bara komma åt en **Contribute** -mapp om den har delats med dig. Du får ett meddelande via e-post/puls när en Contribute-mapp delas med dig. Du kan antingen komma åt Contribute-mappen via länken som delas i e-postmeddelandet, eller logga in på din Brand Portal-instans och navigera till klockikonen för att få meddelanden och få tillgång till Contribute-mappen.

>[!NOTE]
>
>Om du inte är en befintlig Brand Portal-användare ber du AEM-administratören att skapa din användare i AEM Admin Console och lägga till din profil i användarkonfigurationsfilen i användarlistan för Brand Portal-användare. Se Användare av [varumärkesportalen](brand-portal-configure-asset-sourcing.md).



**Frågor. Vilket format har CSV-filen för användarimport?**

**Ans.** Formatet är detsamma som det som stöds av Admin Console för import av större mängder användare. E-post, förnamn och efternamn är obligatoriska.



**Frågor. Vad fyller i listan med användare (medverkande på varumärkesportalen) i listrutan Tillgångsmedverkande användare?**

**Ans.** Användarna i listrutan fylls i från användarkonfigurationsfilen Brand Portal (.csv) som har överförts i AEM.



**Frågor. Var kan jag se status för import- och publiceringsjobb?**

**Ans.** I AEM kan du se status för en import på sidan för **asynkrona** jobb. I varumärkesportalen kan du se status för ett publiceringsjobb i **[!UICONTROL Verktyg > Resursbidragsstatus]**.



**Frågor. Hur ofta körs ett importjobb med regelbundna intervall i AEM?**

**Ans.** I AEM avsöks var femte minut.



**Frågor. Finns det någon begränsning för hur många gånger en mapp kan publiceras från varumärkesportalen till AEM Assets?**

**Ans.** Nej, alla resurser i mappen **NEW** publiceras till AEM Assets, oavsett om de publicerades tidigare. Varje gång en **Contribute** -mapp publiceras från varumärkesportalen till AEM Assets åsidosätter den innehållet i den **NYA** mappen.



**Frågor. Hur överför jag nya resurser i en Contribute-mapp?**

**Ans.** Mer information finns i den detaljerade dokumentationen om hur du [överför resurser till Contribute-mappen](brand-portal-upload-assets-to-contribution-folder.md).



**Frågor. Kan jag inte se miniatyrbilder/förhandsvisningar av resurserna som en användare på varumärkesportalen har överfört till den NYA mappen?**

**Ans.** Det är utformat, eftersom det inte finns något arbetsflöde att köra i varumärkesportaländen.



**Frågor. Vad händer om en mapp publiceras från AEM Assets till Brand Portal som är i full gång?**

**Ans.** I AEM bevaras loggar för varje gång en mapp publiceras på varumärkesportalen. Vid publiceringen placeras alla resurser som inte publiceras på varumärkesportalen i en replikeringskö. Alla resurser som läggs till i mappen efter att publiceringsjobbet har utlösts publiceras inte på varumärkesportalen. När AEM-användaren publicerar mappen igen publiceras endast resurser som inte publicerades tidigare (som finns i replikeringskön) på varumärkesportalen.
Detta gäller för alla mappar som publiceras från AEM Assets till Brand Portal, och delade mappar i en Contribute-mapp.



**Frågor. Vem kontaktar jag med frågor?**

**Ans.** Kontakta er kontoansvarige på Adobe eller kundsupport.


>[!NOTE]
>
>Releasedatan är preliminärt och kan komma att ändras. Kontakta er kontoansvarige på Adobe eller kundsupport för att få det uppdaterade releaseschemat.




## Produktåtkomst och support (begränsade platser) {#product-access-and-support-restricted-sites}

Dessa webbplatser är bara tillgängliga för kunder. Om du är kund och behöver åtkomst kontaktar du din kontoansvarige på Adobe.

* [](https://daycare.day.com) [Produktåtkomst](https://login.marketing.adobe.com)

* [Adobes kundtjänst](https://helpx.adobe.com/contact.html)
