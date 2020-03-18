---
title: Sök efter resurser på varumärkesportalen
seo-title: Sökning efter resurser och sparad sökning på AEM-varumärkesportalen
description: Med funktionen för varumärkesportalsökning kan du snabbt söka efter relevanta resurser med hjälp av sökning, och med sökfilter kan du begränsa sökningen ytterligare. Spara dina sökningar som smarta samlingar för framtiden.
seo-description: Med funktionen för varumärkesportalsökning kan du snabbt söka efter relevanta resurser med hjälp av sökning, och med sökfilter kan du begränsa sökningen ytterligare. Spara dina sökningar som smarta samlingar för framtiden.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Sök efter resurser på varumärkesportalen {#search-assets-on-brand-portal}

Med funktionen för varumärkesportalsökning kan du snabbt söka efter relevanta resurser med hjälp av sökning och ansiktssökning som använder filter för att ytterligare begränsa sökningen. Du kan även spara dina sökningar som smarta samlingar för framtiden.

## Söka efter resurser med Omnissearch {#search-assets-using-omnisearch}

Så här söker du efter resurser på varumärkesportalen:

1. Klicka på **[!UICONTROL Search]** ikonen i verktygsfältet eller tryck på &quot;**[!UICONTROL /]**&quot;-tangenten för att starta Omnissearch.

   ![](assets/omnisearchicon-1.png)

1. Skriv ett nyckelord för de resurser du vill söka efter i sökrutan.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Minst tre tecken krävs i sökningen för att sökförslagen ska visas.

1. Välj bland de relaterade förslag som visas i listrutan för att snabbt komma åt relevanta resurser.

   ![](assets/assets-search-result.png)

   *Resurssökning med omnissearch*

Mer information om sökbeteenden med smarta taggade resurser finns i [Information om sökresultat och beteenden](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html).

## Söka med ansikten på panelen Filter {#search-using-facets-in-filters-panel}

Sökfaktorer på panelen Filter ger en mer detaljerad sökupplevelse och gör sökfunktionen effektiv. Sökfacets använder flera dimensioner (predikatfärger) som gör att du kan utföra komplexa sökningar. Du kan enkelt gå ned till önskad detaljnivå för en mer fokuserad sökning.

Om du till exempel söker efter en bild kan du välja om du vill ha en bitmapp eller en vektorbild. Du kan begränsa sökningen ytterligare genom att ange MIME-typen för bilden i sökaspekten Filtyp. På samma sätt kan du ange formatet, t.ex. PDF- eller MS Word-format, när du söker efter dokument.<br />

![Panelen Filter i](assets/file-type-search.png "panelen för varumärkesportalfilterFilter i varumärkesportalen")

Panelen innehåller **[!UICONTROL Filters]** några standardaspekter, t.ex.- **[!UICONTROL Path Browser]**, **[!UICONTROL File Type]****[!UICONTROL File Size]**, **[!UICONTROL Status]** och **[!UICONTROL Orientation]**. Du kan dock [lägga till anpassade sökfaktorer](../using/brand-portal-search-facets.md) eller ta bort specifika sökfaktorer från **[!UICONTROL Filters]** panelen genom att lägga till eller ta bort predikaten i det underliggande sökformuläret. Se listan med tillgängliga och användbara [sökpredikatorer på varumärkesportalen](../using/brand-portal-search-facets.md#list-of-search-predicates).

Om du vill använda filter på sökningen använder du de tillgängliga [sökfunktionerna](../using/brand-portal-search-facets.md):

1. Klicka på övertäckningsikonen och välj **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

1. Välj lämpliga alternativ på panelen till vänster **[!UICONTROL Filters]** för att använda de relevanta filtren.
Använd till exempel följande standardfilter:

   * **[!UICONTROL Path Browser]** om du vill söka efter resurser i en viss katalog. Standardsöksökvägen för predikatet för sökvägsläsaren är `/content/dam/mac/<tenant-id>/`, som kan konfigureras genom att du redigerar standardsökformuläret.
   >[!NOTE]
   >
   >För icke-adminanvändare visas bara innehållsstrukturen i de mappar (och deras överordnade mappar) som delas med andra på [!UICONTROL Path Browser] [!UICONTROL Filter] panelen.\
   >Om du vill administrera användare kan du navigera till valfri mapp i varumärkesportalen med hjälp av Sökvägsläsaren.

   * **[!UICONTROL File Type]** för att ange typ (bild, dokument, multimedia, arkiv) av resursfilen som du söker efter. Du kan dessutom begränsa omfattningen av sökningen, till exempel ange MIME-typen (TIFF, Bitmapp, GIMP-bilder) för bilden eller formatet (PDF eller MS Word) för dokumenten.
   * **[!UICONTROL File Size]** om du vill söka efter resurser baserat på deras storlek. Du kan ange de nedre och övre gränserna för storleksintervallet för att begränsa sökningen och ange vilken måttenhet som ska sökas igenom.
   * **[!UICONTROL Status]** om du vill söka efter resurser baserat på tillgångsstatus, t.ex. Godkännande (Godkänd, Ändringar Begärd, Avvisad, Väntande) och Förfallotid.
   * **[!UICONTROL Average Rating]** för att söka efter resurser baserat på tillgångarnas värdering.
   * **[!UICONTROL Orientation]** om du vill söka efter resurser baserat på orienteringen (vågrät, lodrät, kvadratisk) för resurserna.
   * **[!UICONTROL Style]** om du vill söka efter resurser baserat på resursernas stil (färgad, monokrom).
   * **[!UICONTROL Video Format]** om du vill söka efter videoresurser baserat på deras format (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   Du kan använda [anpassade sökfunktioner](../using/brand-portal-search-facets.md) på panelen Filter genom att redigera det underliggande sökformuläret.

   * **[!UICONTROL Property Predicate]** om det används i sökformuläret kan du söka efter resurser som matchar en metadataegenskap som predikatet är mappat till.\
      Om du t.ex. mappar egenskapspredikatet till [!UICONTROL `jcr:content /metadata/dc:title`]kan du söka efter resurser baserat på deras titel.\
      Det finns [!UICONTROL Property Predicate] stöd för textsökningar för:

      **Delvisa fraser** Om du vill tillåta resurssökning med partiella fraser i egenskapspredikatet markerar du kryssrutan i **[!UICONTROL Partial Search]** Sökformulär.\
      På så sätt kan du söka efter de önskade resurserna även om du inte anger de exakta ord/fraser som används i metadata för resursen.\
      Du kan:
      * Ange ett ord som förekommer i din sökfras i ansiktet på panelen Filter. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
      * Ange en del av ordet, som finns i sökfrasen, tillsammans med jokertecknet (*) för att fylla i luckorna.
Om du till exempel söker efter:
         * **klättb*** returnerar alla resurser som har ord som börjar med tecknen&quot;klättra&quot; i titelfrasen.
         * ***klättb** returnerar alla resurser med ord som slutar med tecknen &quot;klättra&quot; i titelfrasen.
         * ***klättb*** returnerar alla resurser med ord som innehåller tecknen&quot;klättra&quot; i titelfrasen.
      **Icke-skiftlägeskänslig text** Om du vill tillåta icke-skiftlägeskänslig sökning i egenskapspredikatet markerar du kryssrutan i **[!UICONTROL Ignore Case]** Sökformulär. Som standard är textsökningen på egenskapspredikatet skiftlägeskänslig.
   >[!NOTE]
   >
   >När du markerar **[!UICONTROL Partial Search]** kryssrutan **[!UICONTROL Ignore Case]** markeras den som standard.

   ![](assets/wildcard-prop-1.png)

   Sökresultaten visas enligt de filter som används, tillsammans med antalet sökresultat.

   ![](assets/omnisearch-with-filters.png)

   Resultat av resurssökning med antal sökresultat.

1. Du kan enkelt navigera till ett objekt från sökresultatet och gå tillbaka till samma sökresultat med bakåtknappen i webbläsaren utan att behöva köra sökfrågan igen.

## Spara dina sökningar som en smart samling {#save-your-searches-as-smart-collection}

Du kan spara sökinställningarna som en smart samling för att snabbt kunna upprepa samma sökning utan att behöva göra om samma inställningar senare.

Så här sparar du sökinställningarna som en smart samling:

1. Tryck/klicka **[!UICONTROL Save Smart Collection]** och ange ett namn för den smarta samlingen.

   Om du vill att den smarta samlingen ska vara tillgänglig för alla användare väljer du **[!UICONTROL Public]**. Ett meddelande bekräftar att den smarta samlingen skapades och lades till i listan över dina sparade sökningar.

   >[!NOTE]
   >
   >Användare som inte är administratörer kan begränsas från att göra smarta samlingar offentliga för att undvika att ha ett stort antal publika smarta samlingar som skapats av icke-administratörer på organisationens varumärkesportal. Organisationer kan inaktivera **[!UICONTROL Allow public smart collections creation]** konfigurationen från de **[!UICONTROL General]** inställningar som finns på panelen Administrationsverktyg.

   ![](assets/save_smartcollectionui.png)

1. Om du vill spara den smarta samlingen med ett annat namn och markera eller avmarkera **[!UICONTROL Public]** kryssrutan klickar du på **[!UICONTROL Edit Smart Collection]**.

   ![](assets/edit_smartcollection.png)

1. I **[!UICONTROL Edit Smart Collection]** dialogrutan markerar du **[!UICONTROL Save As]** och anger ett namn för den smarta samlingen. Klicka på **[!UICONTROL Save]**.

   ![](assets/saveas_smartsearch.png)