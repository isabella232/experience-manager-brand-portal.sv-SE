---
title: Publicera i Contribute-mapp till AEM Assets
seo-title: Publicera i Contribute-mapp till AEM Assets
description: Få insikt i hur du publicerar bidragsmappen till AEM Assets i varumärkesportalen.
seo-description: Få insikt i hur du publicerar bidragsmappen till AEM Assets i varumärkesportalen.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 6eb01e2eec7de6b704976c990fb6ffacbc67471a
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Publicera bidragsmapp till AEM Assets {#publish-contribution-folder-to-aem}

Användare av varumärkesportalen kan publicera bidragsmappen till AEM Assets utan att behöva ha tillgång till AEM författarinstans.

Kontrollera att du har gått igenom [resurskraven](brand-portal-download-asset-requirements.md) och överför de nyskapade resurserna i **mappen NEW** i mappen för bidrag. Se [Överför resurser till mappen för bidrag](brand-portal-upload-assets-to-contribution-folder.md).

**Så här publicerar du bidragsmappen:**

1. Logga in på din Brand Portal-instans.

1. Välj mapp för bidrag från kontrollpanelen för varumärkesportalen.
1. Klicka på **[!UICONTROL Publish to AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

Ett e-post-/pulsmeddelande skickas till Brand Portal-användare och -administratörer i olika stadier av publiceringsarbetsflödet:
1. **Köad**  - Ett meddelande skickas till användaren och administratören för varumärkesportalen när ett publiceringsarbetsflöde utlöses i varumärkesportalen.

1. **Fullständigt**  - Ett meddelande skickas till Brand Portal-användaren och Brand Portal-administratörerna när mappen för bidrag har publicerats i AEM Assets.


**Status för publiceringsjobb**

Det finns två rapporter som administratörer kan använda för att visa statusen för resursavgiftsmapparna som publicerats från Brand Portal till AEM Assets.

* Gå till **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]** i varumärkesportalen. Den här rapporten visar statusen för alla publiceringsjobb i olika faser av publiceringsarbetsflödet.

   ![](assets/contribution-folder-status.png)

* I AEM Assets-författarinstansen går du till **[!UICONTROL Tools]** > **[!UICONTROL Jobs]**. Den här rapporten visar det slutliga tillståndet (Slutfört eller Fel) för alla publiceringsjobb.

   ![](assets/publishing-status.png)




