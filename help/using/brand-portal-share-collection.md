---
title: Dela en samling
seo-title: Dela en samling
description: Administratörer för AEM Assets Brand Portal kan dela och ta bort delning av en samling eller en smart samling med behöriga användare. Redigerare kan bara visa och dela samlingar som de skapat, delat med dem och gemensamma samlingar.
seo-description: Administratörer för AEM Assets Brand Portal kan dela och ta bort delning av en samling eller en smart samling med behöriga användare. Redigerare kan bara visa och dela samlingar som de skapat, delat med dem och gemensamma samlingar.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Dela samlingar på varumärkesportalen {#share-collections-bp}

Administratörer för AEM Assets Brand Portal kan dela och ta bort delning av en samling eller en smart samling med behöriga användare. Redigerare kan bara visa och dela samlingar som de skapat, delat med dem och gemensamma samlingar. Redigerare kan dock inte ändra en offentlig samling till en icke-offentlig samling.

>[!NOTE]
>
>Redigerare kan inte ändra en offentlig samling till en icke-offentlig samling och har därför ingen **[!UICONTROL Public Collection]** kryssruta i **[!UICONTROL Collection Settings]** dialogrutan.

## Dela en samling {#share-collection}

Så här delar du en samling:

1. Klicka på övertäckningsikonen till vänster och välj **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. Klicka på i sidofältet till vänster **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

1. Gör något av följande i **[!UICONTROL Collections]** konsolen:

   * Håll pekaren över den samling du vill dela. Klicka på **[!UICONTROL Settings]** ikonen bland miniatyrbilderna för snabbåtgärder som är tillgängliga för samlingen.
   ![](assets/settings_thumbnail.png)

   * Markera den samling som du vill dela. Klicka på i verktygsfältet överst **[!UICONTROL Settings]**.
   ![](assets/collection-sharing.png)

1. I [!UICONTROL Collection Settings] dialogrutan väljer du de användare eller grupper som du vill dela samlingen med och väljer rollen för en användare eller grupp som ska matcha deras globala roll. Tilldela till exempel redigerarrollen till en global redigerare, visningsprogramrollen till ett globalt visningsprogram.

   Du kan även göra samlingen tillgänglig för alla användare oavsett deras gruppmedlemskap och roll genom att markera kryssrutan **[!UICONTROL Public Collection]** .

   >[!NOTE]
   >
   >Användare som inte är administratörer kan dock hindras från att skapa offentliga samlingar, så att du slipper ha flera offentliga samlingar så att systemutrymmet kan sparas. Organisationer kan inaktivera **[!UICONTROL Allow public collections creation]** konfigurationen från de [!UICONTROL General] inställningar som finns på panelen Administrationsverktyg.

   ![](assets/collection_sharingadduser.png)

   Redigerare kan inte ändra en offentlig samling till en icke-offentlig samling och har därför inte någon **[!UICONTROL Public Collection]** kryssruta tillgänglig i **[!UICONTROL Collection Settings]** dialogrutan.

   ![](assets/collection-setting-editor.png)

1. Markera **[!UICONTROL Add]** och sedan **[!UICONTROL Save]**. Samlingen delas med de valda användarna.

   >[!NOTE]
   >
   >En användares roll styr åtkomsten till resurser och mappar i en samling. Om en användare inte har åtkomst till resurser delas en tom samling med användaren. Dessutom styr en användares roll vilka åtgärder som är tillgängliga för samlingar.

## Ta bort delning av en samling {#unshare-a-collection}

Så här tar du bort delningen av en tidigare delad samling:

1. I **[!UICONTROL Collections]** konsolen väljer du den samling du vill ta bort delningen från.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. Klicka på symbolen bredvid användare eller grupper under **[!UICONTROL Collection Settings]** dialogrutan **[!UICONTROL Members]****[!UICONTROL x]** för att ta bort dem från listan med användare som du delade samlingen med.

   ![](assets/unshare_collection.png)

1. Klicka i varningsmeddelanderutan på **[!UICONTROL Confirm]** för att bekräfta att du inte vill dela.

   Klicka på **[!UICONTROL Save]**.

1. Logga in på varumärkesportalen med inloggningsuppgifterna för den användare du tog bort från den delade listan. Samlingen tas bort från **[!UICONTROL Collections]** konsolen.
