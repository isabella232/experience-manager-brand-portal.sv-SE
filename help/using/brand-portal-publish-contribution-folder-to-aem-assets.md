---
title: Publicera i Contribute-mapp till AEM Assets
seo-title: Publicera i Contribute-mapp till AEM Assets
description: Få insikt i hur du publicerar mappen för bidrag till AEM Assets i varumärkesportalen.
seo-description: Få insikt i hur du publicerar mappen för bidrag till AEM Assets i varumärkesportalen.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 413a6bd17d689d0af0cce20bbd7dedb6ae3cf9b5

---


# Publicera mapp för bidrag till AEM Resurser {#publish-contribution-folder-to-aem}

Användare av varumärkesportalen kan publicera mappen för bidrag till AEM Resurser utan att behöva ha tillgång till AEM-författarinstansen.

Se till att du har gått igenom [resurskraven](brand-portal-download-asset-requirements.md) och överfört de nyskapade resurserna i mappen **NEW** i mappen för bidrag. Se [Överför resurser till mappen](brand-portal-upload-assets-to-contribution-folder.md)för bidrag.

**Så här publicerar du bidragsmappen:**

1. Logga in på din Brand Portal-instans.
1. Välj mapp för bidrag från kontrollpanelen för varumärkesportalen.
1. Klicka på **[!UICONTROL Publish to AEM]** ![](assets/export.png).
   ![](assets/publish-contribution-folder-to-aem.png)

Ett e-post-/pulsmeddelande skickas till varumärkesportalen och AEM, administratör och användare i olika faser av publiceringsarbetsflödet:
1. **Köad** - När arbetsflödesutlösare publiceras i Brand Portal publiceras mappen för bidrag från Brand Portal till AEM.
1. **Pågående** - När AEM Resurser börjar importera mappen för bidrag.
1. **Slutförd** - När publiceringsåtgärden har slutförts importeras mappen för bidrag till AEM Resurser.


