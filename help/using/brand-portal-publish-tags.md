---
title: 將標記發佈至 Brand Portal
seo-title: 將標記發佈至 Brand Portal
description: 瞭解如何從AEM Assets發佈標籤至品牌入口網站。
seo-description: 瞭解如何從AEM Assets發佈標籤至品牌入口網站。
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---


# 將標記發佈至 Brand Portal {#publish-tags-to-brand-portal}

瞭解如何從AEM Assets發佈標籤至品牌入口網站。

標籤在組織資產時非常有用，並可增強與其關聯的資產的可搜尋性。 標籤可視為附加資產的關鍵字或標籤（中繼資料），並可讓搜尋結果快速找到資產。 若要瞭解如何在AEM Assets中指派標籤給資產，請參閱[使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

當具有相關標籤的資產（和系列）發佈至品牌入口網站時，標籤（與AEM中的資產和系列相關聯）會自動發佈至品牌入口網站。 發佈的標籤有助於讓搜尋找到相關的資產。

>[!NOTE]
>
>不過，建議您在發佈與標籤相關聯的資產（和系列）之前，先排他性地將標籤發佈至品牌入口網站。 這可確保資產（和系列）更快地發佈至品牌入口網站。

## 管理標籤{#manage-tags}

您可以使用預先存在的標籤來附加至資產，或從AEM標籤主控台（**[!UICONTROL 工具）建立新標籤 |標籤 | AEM Tags]**)。 在這兩種情況下，您必須先將標籤發佈至品牌入口網站，然後將其與適當的資產建立關聯。

若要在AEM上建立標籤、在品牌入口網站上發佈標籤，並將標籤與適當的資產（或系列）產生關聯，請依照下列步驟進行：

1. **建立**
標籤以管理權限登入AEM Author例項，並從全域導覽存 **[!UICONTROL 取]** AEM Tagsconsole:

   1. 選擇&#x200B;**[!UICONTROL 工具]**

   1. 選擇&#x200B;**[!UICONTROL 常規]**

   1. 選擇&#x200B;**[!UICONTROL 標籤]**

1. 選擇&#x200B;**[!UICONTROL 建立]** ，然後選擇&#x200B;**[!UICONTROL 建立標籤]**&#x200B;選項。
1. 指定下列設定：

   * **[!UICONTROL 標題]**

      *（必要）* 標籤的顯示標題。
   * **[!UICONTROL 名稱]**
      *（必要）* 標籤的名稱。如果未指定，則從「標題」建立有效的節點名稱。 請參閱[TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **說明**

      *（可選）* 標籤的說明。
   * **標籤**
標籤的PathJCR路徑。

1. 選擇&#x200B;**[!UICONTROL Submit]**&#x200B;以建立標籤。

   在AEM例項上建立標籤後，標籤便可附加至資產（使用該資產的「屬性」區段或「管理標籤」區段）。

1. **將標籤發佈至品牌入口網站**。

   前往&#x200B;**[!UICONTROL AEM Tags]**&#x200B;主控台([!UICONTROL 工具 |標籤 | AEM Tags])，選取所要的標籤並發佈至品牌入口網站。

1. **將標籤附加至資產（或系列）**。

   選取資產（或系列），然後使用該資產的「屬性」區段或「管理標籤」區段附加所要的標籤。 若要進一步瞭解如何在AEM Assets中指派標籤至資產，請參閱[使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

1. **將資產（或系列）發佈至品牌入口網站**。\
   當您將資產（或系列）發佈至品牌入口網站時，附加的標籤也可在品牌入口網站上使用。

   若要在品牌入口網站中查看個別資產（或系列）上的附加標籤，請登入品牌入口網站並選取資產，在「屬性」區段下，您會看到附加的標籤。

## 搜尋提升 {#search-promote}

AEM Assets品牌入口網站可讓您讓特定資產成為根據關鍵字標籤搜尋的最佳結果。

若要提升搜尋關鍵字的資產，請遵循下列步驟：

1. 在AEM作者例項上開啟資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁面。
1. 轉至「**[!UICONTROL 高級]**」頁籤。
1. 在&#x200B;**[!UICONTROL 「Elevate for search keywords]**」區段中的「Search Promote ]**」中，選擇「Add]**」以添加搜索關鍵字或標籤。**[!UICONTROL **[!UICONTROL 

   ![](assets/search-promote.png)

1. 儲存變更。
1. 將資產發佈至 Brand Portal.
1. 登入品牌入口網站。 在資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;區段中檢視&#x200B;**[!UICONTROL 進階]**標籤。
請注意，該資產的「屬性」中也會顯示**[!UICONTROL 搜尋促銷]**&#x200B;關鍵字。
