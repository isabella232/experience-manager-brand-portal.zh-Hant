---
title: 將標記發佈至 Brand Portal
seo-title: Publish tags to Brand Portal
description: 了解如何將標籤從Experience Manager資產發佈至Brand Portal。
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 4%

---

# 將標記發佈至 Brand Portal {#publish-tags-to-brand-portal}

了解如何將標籤從Experience Manager資產發佈至Brand Portal。

標籤可用來組織資產，並增強與資產相關聯的資產的可搜尋性。 標籤可視為與資產附加的關鍵字或標籤（中繼資料），並可讓您在搜尋後快速找到資產。 若要了解如何將標籤指派給Experience Manager資產中的資產，請參閱[使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

標籤(與AEM中的資產和集合相關聯)會在與相關聯標籤關聯的資產（和集合）發佈至Brand Portal時自動發佈至Brand Portal。 已發佈的標籤有助於讓搜尋找到相關的資產。

>[!NOTE]
>
>不過，建議您先只發佈標籤至Brand Portal，再發佈與標籤相關聯的資產（和集合）。 這可確保更快將資產（和集合）發佈至Brand Portal。

## 管理標籤 {#manage-tags}

您可以使用預先存在的標籤來附加至資產，或從AEM標籤控制台（**[!UICONTROL 工具）建立新標籤 |標籤 | AEM標籤]**)。 在這兩種情況下，您必須先將標籤發佈至Brand Portal，然後將標籤與適當的資產建立關聯。

若要在AEM上建立標籤、在Brand Portal上發佈標籤，以及將標籤與適當的資產（或集合）建立關聯，請遵循下列步驟：

1. **建立**
Tags以管理權限登入AEM Author例項，並從全域導覽存 **[!UICONTROL 取]** AEM Tagsconsole:

   1. 選擇&#x200B;**[!UICONTROL 工具]**

   1. 選擇&#x200B;**[!UICONTROL 常規]**

   1. 選擇&#x200B;**[!UICONTROL 標籤]**

1. 選擇&#x200B;**[!UICONTROL Create]**，然後選擇&#x200B;**[!UICONTROL Create Tag]**&#x200B;選項。
1. 指定下列設定：

   * **[!UICONTROL 標題]**

      *（必要）* 標籤的顯示標題。
   * **[!UICONTROL 名稱]**
      *（必要）* 標籤的名稱。如果未指定，則從標題中建立有效的節點名。 請參閱[TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **說明**

      *（選用）* 標籤的說明。
   * **標**
記的PathJCR路徑。

1. 選擇&#x200B;**[!UICONTROL Submit]**&#x200B;以建立標籤。

   在AEM例項上建立標籤後，該標籤便可附加至資產（使用該資產的「屬性」區段或「管理標籤」區段）。

1. **將標籤發佈至Brand Portal**。

   前往&#x200B;**[!UICONTROL AEM標籤]**&#x200B;控制台([!UICONTROL 工具 |標籤 | AEM標籤])，選取所需的標籤並發佈至Brand Portal。

1. **將標籤附加至資產（或集合）**。

   選取資產（或集合），然後使用該資產的「屬性」區段或「管理標籤」區段附加所需的標籤。 若要進一步了解如何在AEM Assets中將標籤指派給資產，請參閱[使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

1. **將資產（或集合）發佈至Brand Portal**。\
   將資產（或集合）發佈至Brand Portal時，附加的標籤也可在Brand Portal上使用。

   若要在Brand Portal中查看個別資產（或集合）的附加標籤，請登入Brand Portal並選取資產，「屬性」區段下方會顯示附加的標籤。

## 搜尋提升 {#search-promote}

AEM Assets Brand Portal可讓您根據關鍵字標籤，讓特定資產成為搜尋的最佳結果。

若要提升搜尋關鍵字的資產，請執行下列步驟：

1. 在AEM製作例項上，開啟資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁面。
1. 前往&#x200B;**[!UICONTROL 進階]**&#x200B;標籤。
1. 在&#x200B;**[!UICONTROL **[!UICONTROL  Elevate for search keywords ]**區段內的Search Promote]**&#x200B;中，選擇&#x200B;**[!UICONTROL Add]**&#x200B;以添加搜索關鍵字或標籤。

   ![](assets/search-promote.png)

1. 儲存變更。
1. 將資產發佈至 Brand Portal.
1. 登入Brand Portal。 在資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;區段中檢視&#x200B;**[!UICONTROL 進階]**標籤。
請注意，該資產的「屬性」中也會顯示**[!UICONTROL Search Promote]**&#x200B;關鍵字。
