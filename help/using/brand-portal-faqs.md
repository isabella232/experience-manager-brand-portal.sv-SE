---
title: Vanliga frågor
seo-title: null
description: Få information om vanliga frågor och svar i Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 4983e2e160b5cfb213e249f731e1858fab2cf972
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---


# Vanliga frågor och svar {#frequently-asked-questions}

Vanliga frågor och svar om varumärkesportalen fokuserar på frågor och problem som slutanvändarna kan råka ut för när de arbetar med den senaste utgåvan av AEM Assets Brand Portal 6.4.6 eller tidigare versioner.


## Frågor och svar om varumärkesportalen 6.4.6 {#faqs-bp646}

**Frågor. Den befintliga gamla OAuth-slutpunkten (`https://legacy-oauth.cloud.adobe.io/login`) fungerar inte. Vad kan vara den möjliga orsaken?**

**Ans.** Äldre OAuth-konfiguration är föråldrad. Du måste uppgradera AEM Assets-författarinstanser till det senaste Service Pack-paketet och konfigurera det via Adobe Developer Console. Mer information finns i [Konfigurera AEM Assets med varumärkesportalen](configure-aem-assets-with-brand-portal.md). För att äldre OAuth-konfiguration ska fungera tills du uppgraderar måste du dock uppdatera den äldre OAuth-slutpunkten till `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Frågor. Jag kan inte publicera resurserna i mappen för bidrag från Brand Portal till AEM Assets efter att ha uppgraderat till Adobe Developer Console. Min författarinstans är på AEM 6.5.4. Vad kan vara den möjliga orsaken?**

**Ans.** Ja, det finns ett känt fel när du publicerar resurser i mappen för bidrag till AEM Assets på AEM 6.5.4 via Adobe Developer Console.

Problemet är åtgärdat i AEM 6.5.5. Du kan uppgradera din AEM Assets-instans till den senaste Service Pack-versionen AEM 6.5.5 och [uppgradera dina konfigurationer](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) på Adobe Developer Console.

För omedelbar korrigering AEM 6.5.4 rekommenderar vi att du [hämtar snabbkorrigeringen](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) och installerar den på din AEM författarinstans.

**Frågor. Jag ser inte innehållet i mappen för bidrag som publicerats från Brand Portal i AEM Assets. Vad kan vara den möjliga orsaken?**

**Ans.** Kontakta din AEM Assets-administratör för att verifiera konfigurationerna och se till att din varumärkesportal-klient bara är konfigurerad med en AEM Assets-författarinstans.

Detta kan inträffa när du har konfigurerat en innehavare av en varumärkesportal på flera instanser av AEM Assets-författare. Administratören konfigurerar till exempel samma varumärkesportal-klient på AEM Assets författarinstans i staging- och produktionsmiljön. I det här fallet utlöses resurspubliceringen i Brand Portal, men AEM Assets-författarinstansen kunde inte importera resurskoden som replikeringsagenten inte får den begärda token.


**Frågor. Jag kan inte publicera material från AEM Assets till varumärkesportalen. Replikeringsloggen anger att anslutningen gjorde timeout. Finns det en snabbkorrigering?**

**Ans.** Publiceringen misslyckas vanligtvis med ett timeout-fel om det finns flera väntande begäranden i replikeringskön. Kontrollera att replikeringsagenterna är konfigurerade för att undvika timeout för att lösa problemet.

Utför följande steg för att konfigurera replikeringsagenten:
1. Logga in på din AEM Assets-författarinstans.
1. Gå till **[!UICONTROL Deployment]** > **[!UICONTROL Replication]** på panelen **Verktyg**.
1. Klicka på **[!UICONTROL Agents on author]** på sidan Replikering. Du kan se de fyra replikeringsagenterna för din Brand Portal-klient.
1. Klicka på replikeringsagentens URL för att öppna agentinformationen.
1. Klicka på **[!UICONTROL Edit]** om du vill ändra inställningarna för replikeringsagenten.
1. Klicka på fliken **[!UICONTROL Extended]** i Agentinställningar.
1. Markera kryssrutan **[!UICONTROL Close Connection]**.
1. Upprepa steg 4 till 7 för att konfigurera alla fyra replikeringsagenterna.
1. Starta om servern och bekräfta anslutningen.


## Frågor och svar om varumärkesportalen 6.4.5 {#faqs-bp645}

**Frågor. Vilken är den största förändringen i varumärkesportalen 6.4.5?**

**Ans.** AEM Assets Brand Portal 6.4.5 är en funktionsrelease som tillåter användare av Brand Portal att ladda upp innehåll inifrån Brand Portal och publicera Contribute-mappen till AEM Assets utan administratörsbehörighet.
Mer information finns i [Resurshantering i varumärkesportalen](brand-portal-asset-sourcing.md).



**Frågor. Kommer jag att förlora åtkomsten till befintliga resurser, funktioner eller konfigurationer som jag har skapat?**

**Ans.** Alla befintliga funktioner och konfigurationer förblir intakta. Slutanvändarna påverkas inte och innehållet förblir intakt.



**Frågor. När ska jag gå till den nya versionen av varumärkesportalen?**

**Ans.** Varumärkesportalen 6.4.5 släpptes till produktion i oktober 2019. Och nästa Brand Portal-version förväntas släppas tredje kvartalet 2020.
För uppdateringar och versionsändringar bör du spåra [versionsinformationen](brand-portal-release-notes.md) och [Nyheter i varumärkesportalen](whats-new.md).



**Frågor. Kommer mina användare att påverkas?**

**Ans.** Brand Portal 6.4.5 finns endast i Brand Portal, så slutanvändarna påverkas inte.



**Frågor. Behöver jag som varumärkesportalanvändare vidta någon åtgärd?**

**Ans.** Brand Portal 6.4.5 innehåller en ny funktion som heter Asset Source. AEM måste konfigurera funktionen Resurshantering i AEM Assets för att aktivera funktionen för användare på varumärkesportalen. Mer information finns i [Aktivera resurskälla](brand-portal-asset-sourcing.md).



**Frågor. Vem kan skapa en Contribute-mapp?**

**Ans.** Alla AEM som har behörighet att skapa en ny mapp i AEM Assets kan skapa en  **** Contribute-mapp. Om du vill skapa en **Contribute**-mapp skapar du en ny mapp av typen **Resursbidrag**.
Den här mappen delas med de aktiva Brand Portal-användarna för bidrag.



**Frågor. Vad innehåller en Contribute-mapp?**

**Ans.** **Mappen** Contribute innehåller två undermappar  **** NEW **och SHARED**. Till att börja med är mappen NEW tom och mappen SHARED innehåller referensinnehållet (återanvändbara resurser) för Brand Portal-användarna.
Brand Portal-användarna kommer åt mappen **Contribute** och överför innehåll i mappen **NEW**.



**Frågor.  Kan jag ändra namnet på en befintlig Contribute-mapp?**

**Ans.** **Nej**, du kan inte ändra namnet på en befintlig  **** Contribute-mapp.



**Frågor. Vad är tillgångskrav utan bidrag?**

**Ans.** Det  **** dokument som är bifogat till  **** Contributionsmappen och referensinnehållet (återanvändbara resurser) som överförts i  **** SHAREDappen hjälper användaren på varumärkesportalen att förstå behovet av bidrag och förväntningar som medverkande och kallas tillsammans för tillgångskrav.



**Frågor. Kan jag överföra resurser till en tillåten mapp?**

**Ans.** Inte alla tillåtna mappar. En varumärkesportalanvändare kan bara överföra innehåll till mappen **Contribute** som delas av AEM- eller varumärkesportaladministratören.



**Frågor. Hur får jag åtkomst till en Contribute-mapp?**

**Ans.** Du kan bara komma åt en  **** Contribute-mapp om den har delats med dig. Du får ett meddelande via e-post/puls när en Contribute-mapp delas med dig. Du kan antingen komma åt Contribute-mappen via länken som delas i e-postmeddelandet, eller logga in på din Brand Portal-instans och navigera till klockikonen för att få meddelanden och få tillgång till Contribute-mappen.

>[!NOTE]
>
>Om du inte är en befintlig Brand Portal-användare ber du AEM att skapa din användare i AEM Admin Console och lägga till din profil i användarkonfigurationsfilen i listan med Brand Portal-användare.

**Frågor. Vilket format har CSV-filen för användarimport?**

**Ans.** Formatet är samma som det som stöds av Admin Console för massanvändarimport. E-post, förnamn och efternamn är obligatoriska.



**Frågor. Vad fyller i listan med användare (Brand Portal-medverkande) i listrutan Tillgångsmedverkande användare?**

**Ans.** Användarna i listrutan fylls i från användarkonfigurationsfilen för Brand Portal (.csv) som har överförts i AEM.



**Frågor. Var kan jag se status för import- och publiceringsjobb?**

**Ans.** I AEM kan du se status för en import på  **** asynkrona jobbsidor. I varumärkesportalen kan du se status för ett publiceringsjobb i **[!UICONTROL Tools > Asset Contribution status]**.



**Frågor. Vilken frekvens har ett importjobb som körs regelbundet i AEM?**

**Ans.** I AEM avsöks var femte minut.



**Frågor. Finns det någon begränsning för hur många gånger en mapp kan publiceras från varumärkesportalen till AEM Assets?**

**Ans.** Nej, alla resurser i  **** mappen NEW publiceras till AEM Assets oavsett om de publicerades tidigare. Varje gång en **Contribute**-mapp publiceras från Brand Portal till AEM Assets åsidosätter den innehållet i mappen **NEW**.



**Frågor. Hur överför jag nya resurser i en Contribute-mapp?**

**Ans.** Mer information finns i den detaljerade dokumentationen om hur du  [överför resurser till Contribute-mappen](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Frågor. Kan jag inte se miniatyrbilder/förhandsgranskningar av resurserna som en användare på varumärkesportalen har överfört till den NYA mappen?**

**Ans.** Det är utformat, eftersom det inte finns något arbetsflöde att köra i varumärkesportaländen.



**Frågor. Vad händer om en mapp publiceras från AEM Assets till Brand Portal som är i full gång?**?

**Ans.** I AEM bevaras loggar för varje gång en mapp publiceras på varumärkesportalen. Vid publiceringen placeras alla resurser som inte publiceras på varumärkesportalen i en replikeringskö. Alla resurser som läggs till i mappen efter att publiceringsjobbet har utlösts publiceras inte på varumärkesportalen. När AEM publicerar mappen igen publiceras endast resurser som inte publicerades tidigare (som finns i replikeringskön) på varumärkesportalen.
Detta gäller för alla mappar som publiceras från AEM Assets till varumärkesportalen och för delade mappar i en Contribute-mapp.

**Frågor. Vem kontaktar jag med frågor?**

**Ans.** Kontakta kontohanteraren för Adobe eller kundsupporten.

>[!NOTE]
>
>Releasedatan är preliminärt och kan komma att ändras. Kontakta kontohanteraren eller kundsupporten för Adobe för att få det uppdaterade releaseschemat.


## Produktåtkomst och support (begränsade platser) {#product-access-and-support-restricted-sites}

Dessa webbplatser är bara tillgängliga för kunder. Om du är kund och behöver åtkomst kontaktar du din kontoansvarige på Adobe.

* [](https://daycare.day.com) [Produktåtkomst](https://login.marketing.adobe.com)

* [Adobe kundtjänst](https://helpx.adobe.com/contact.html)
