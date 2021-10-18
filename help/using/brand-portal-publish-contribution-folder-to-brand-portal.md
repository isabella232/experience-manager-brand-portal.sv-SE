---
title: 'Konfigurera och publicera avgiftsbelagda mappar från Experience Manager Assets till Brand Portal '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Få insikt i hur man konfigurerar och publicerar en mapp för bidrag från Experience Manager Assets till Brand Portal.
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: e7545344a0fc6dd5e0176705a16625c2976e0de6
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# Konfigurera bidragsmappen i Experience Manager Assets {#configure-contribution-folder}

För samverkansbaserad resurskälla kan Experience Manager Assets-användare (administratörer och icke-adminanvändare som har behörighet) skapa nya mappar av typen **Resursbidrag**, och se till att den nya mappen som skapas är öppen för att skickas in av Brand Portal-användare.  Detta utlöser automatiskt ett arbetsflöde som skapar ytterligare två undermappar, som kallas **DELAD** och **NYTT**, i den nyligen skapade **Contribute**-mappen.

Experience Manager Assets-användare definierar sedan tillgångskraven genom att ladda upp en översikt över vilka typer av resurser som ska läggas till i bidragsmappen, samt en uppsättning baslinjeresurser, till **SHARED**-mappen så att Brand Portal-användare har den information de behöver. Administratören kan sedan ge aktiva Brand Portal-användare åtkomst till bidragsmappen innan den nya Contribute-mappen publiceras på Brand Portal.

I följande video visas hur du konfigurerar en Contribute-mapp i Experience Manager Assets:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets-användare utför följande åtgärder när de konfigurerar en mapp för bidrag:

* [Skapa avgiftsmapp](#create-contribution-folder)
* [Överför tillgångskrav och tilldela medverkande](#configure-contribution-folder-properties)
* [Upload baseline assets](#uplad-new-assets-to-contribution-folder)
* [Publish contribution folder from Experience Manager Assets to Brand Portal](#publish-contribution-folder-to-brand-portal)

## Create contribution folder {#create-contribution-folder}


Experience Manager Assets-administratörer och icke-adminanvändare som har behörighet att skapa en ny mapp kan skapa en mapp för bidrag i Experience Manager Assets.
Om du vill skapa en mapp för bidrag skapar du en ny mapp av typen Resursbidrag, som ser till att den nya mappen som skapas är öppen för överföring av resurser från Brand Portal-användare.  This automatically triggers a workflow which creates two additional sub folders, called SHARED and NEW, within the contribution folder.


>[!NOTE]
>
>Administratörerna kan skapa flera resursavgiftsmappar i en mapp.
>
>En mapp för resursbidrag innehåller mapparna NEW och SHARED för resursdistribution och bidrag. Skapa inte en resurs-, mapp- eller bidragsmapp i en bidragsmapp.


Du kan konfigurera bidragsmappens egenskaper separat och samtidigt som du skapar bidragsmappen. I det här exemplet konfigurerar vi egenskaperna separat.

**Så här skapar du en bidragsmapp:**

1. Log in to your Experience Manager Assets instance.

1. Navigera till **[!UICONTROL Assets]** > **[!UICONTROL Files]**. Den visar alla befintliga mappar i Experience Manager Assets-databasen.

1. Klicka på **[!UICONTROL Create]** för att skapa en ny mapp. **[!UICONTROL Create Folder]** öppnas.

1. Ange **[!UICONTROL Title]** och **[!UICONTROL Name]** för mappen och markera kryssrutan **[!UICONTROL Asset Contribution]**.
Vi rekommenderar att du använder gemener utan blanksteg för att namnge mappen.

1. Klicka på **[!UICONTROL Create]**. Du kan se bidragsmappen i Experience Manager Assets-databasen.

   >[!NOTE]
   >
   >En icke-admin-användare kan skapa och dela en resursavgiftsmapp, men kan inte ändra eller ta bort den.


   ![](assets/create-contribution-folder.png)

1. Klicka för att öppna mappen för bidrag så ser du att två undermappar -**[!UICONTROL SHARED]** och **[!UICONTROL NEW]** skapas automatiskt i mappen för bidrag.

   ![](assets/contribution-folder.png)


## Konfigurera egenskaper för bidragsmapp {#configure-contribution-folder-properties}

Experience Manager Assets-administratören utför följande åtgärder när egenskaperna för en avgiftsmapp konfigureras.

* **Lägg till beskrivning**: Ange en beskrivning av bidragsmappen på hög nivå.
* **Överför i korthet**: Överför tillgångskravsdokument som innehåller resursrelaterad information.
* **Lägg till medverkande**: Lägg till Brand Portal-användare för att ge dem åtkomst till mappen för bidrag.

Resurskravet avser den information som administratörer tillhandahåller för att hjälpa medverkande (Brand Portal-användare) att förstå behovet och kraven av bidragsmappen. Administratören överför ett tillgångskravsdokument som innehåller en sammanfattning om vilken typ av resurser som ska läggas till i avgiftsmappen och resursrelaterad information, till exempel syfte, typ av bilder, maxstorlek osv.

**Så här konfigurerar du bidragsmappens egenskaper:**

1. Log in to your Experience Manager Assets instance.

1. Navigera till **[!UICONTROL Assets > Files]** och leta upp mappen för bidrag.
1. Välj mapp för bidrag och klicka på **[!UICONTROL Properties]** för att öppna fönstret Mappegenskaper.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Navigate to **[!UICONTROL Asset Contribution]** tab.
1. Enter high-level **[!UICONTROL Description]** of the contribution folder.
1. Click **[!UICONTROL Upload Brief]** to browse from your local machine and upload an **Asset Requirement Document**.

   ![](assets/upload.png)

1. I fältet **[!UICONTROL Add User]** lägger du till Brand Portal-användare som du vill dela mappen för bidrag med. Dessa användare kan komma åt och överföra innehåll till bidragsmappen via Brand Portal gränssnitt.
1. Klicka på **[!UICONTROL Save]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>Sökresultaten baseras på Brand Portal användarlista som konfigurerats i Experience Manager Assets. Se till att du har den uppdaterade användarlistan för Brand Portal.

## Överför resurser till mappen för bidrag {#uplad-new-assets-to-contribution-folder}

Brand Portal-användare kan ladda ned mediefiler för att förstå behovet av bidrag.
De kan sedan skapa nya resurser för bidrag och överföra dem till mappen NYTT i mappen för bidrag.

>[!NOTE]
>
>Brand Portal-användare kan bara överföra resurser till mappen NEW.
>
>Den maximala överföringsgränsen för alla Brand Portal-klientorganisationer är **10** GB, som tillämpas kumulativt på alla bidragsmappar.


After publishing the newly created assets to Experience Manager Assets, the Brand Portal users can delete them from the NEW folder. Brand Portal-administratören kan ta bort resurserna från både NYTT och Delat.

Once the objective of creating the contribution folder is achieved, the Brand Portal administrator can delete the contribution folder to release the upload space for other users.

>[!NOTE]
>
>Vi rekommenderar att du frigör överföringsutrymmet när du har publicerat avgiftsbelagda mappar till Experience Manager Assets så att de är tillgängliga för övriga Brand Portal-användare.
>
>Om du behöver utöka din Brand Portal-klientorganisations överföringsgräns utöver **10** GB kontaktar du kundsupport och anger kraven.


**Så här överför du nya resurser:**

1. Logga in på din Brand Portal-instans.
På Brand Portal-kontrollpanelen visas alla befintliga mappar som är tillåtna för Brand Portal-användaren tillsammans med den nyligen delade bidragsmappen.

1. Markera mappen för bidrag och klicka för att öppna den. Mappen för bidrag innehåller två undermappar - **[!UICONTROL SHARED]** och **[!UICONTROL NEW]**.

1. Klicka på mappen **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets1.png)

1. Klicka på **[!UICONTROL Create]** > **[!UICONTROL Files]** om du vill överföra enskilda filer eller mappar (.zip) som innehåller flera resurser.

   ![](assets/upload-new-assets2.png)

1. Bläddra och överför resurser (filer eller mappar) till mappen **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets3.png)

När du har överfört alla resurser eller mappar till mappen NEW publicerar du mappen för bidrag till Experience Manager Assets.


## Publicera bidragsmapp till Brand Portal {#publish-contribution-folder-to-brand-portal}

När bidragsmappen har konfigurerats kan Experience Manager Assets-användare (administratör/icke-admin-användare) publicera bidragsmappen från Experience Manager Assets till Brand Portal. Brand Portal-användare som har behörighet att komma åt bidragsmappen får ett meddelande via e-post/puls när publiceringsåtgärden har slutförts.


**Så här publicerar du bidragsmappen:**

1. Logga in på din Experience Manager Assets-instans.

1. Navigera till **[!UICONTROL Assets > Files]** och leta reda på den mapp där du vill publicera till Brand Portal.
1. Välj mapp för bidrag och klicka på **[!UICONTROL Quick Publish]** > **[!UICONTROL Publish to Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   Du får ett meddelande när bidragsmappen har publicerats till Brand Portal.

Ett e-post-/pulsmeddelande skickas till de Brand Portal-användare som är tilldelade bidragsmappen. The Brand Portal users can access the contribution folder and begin contribution. See, [Upload assets to the contribution folder and publish to Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
