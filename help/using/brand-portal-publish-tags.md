---
title: 將標記發佈至品牌入口網站
seo-title: 將標記發佈至品牌入口網站
description: 瞭解如何將標籤從AEM Assets發佈至品牌入口網站。
seo-description: 瞭解如何將標籤從AEM Assets發佈至品牌入口網站。
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: 發佈
products: SG_ PERIENCENCENAGER/Brand_ Portal
content-type: 引用
discoiquuid: 3c8e9251-195d-4c56-a9 a9-27bc8 b2 a82 a4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

瞭解如何將標籤從AEM Assets發佈至品牌入口網站。

標籤在組織資產時很有用，並可增強關聯資產的可存取性。標籤可視為隨附於資產的關鍵字或標籤(中繼資料)，並可讓資產快速找到作為搜尋結果。若要瞭解如何將標記指派給AEM Assets中的資產，請參閱 [使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

當相關標記已發佈至品牌入口網站時，標籤(與AEM中的資產和系列關聯)會自動發佈至品牌入口網站，並將其發佈至品牌入口網站。發佈的標籤有助於搜尋找到相關聯的資產。

>[!NOTE]
>
>不過，建議您先將標記發佈至品牌入口網站，然後再發佈標記所關聯的資產(和系列)。如此可確保更快速地將資產(和系列)發佈至品牌入口網站。

## Manage tags {#manage-tags}

您可以使用現有標籤附加至資產，或從AEM標記主控台建立新標記(**[!UICONTROL 工具|標記|AEM標記]**)。在這兩種情況下，您必須先將標記發佈至品牌入口網站，然後將它們與適當的資產建立關聯。

若要在AEM上建立標記、在品牌入口網站上發佈標籤，並將標記與適當資產(或系列)建立關聯，請遵循下列步驟：

1. **建立標記**&#x200B;以管理權限登入AEM作者實例，並從全域導覽存取 **[!UICONTROL AEM
Tags]** 主控台：

   1. 選取 **[!UICONTROL 工具]**

   2. 選取 **[!UICONTROL 一般]**

   3. 選取 **[!UICONTROL 標記]**

2. 選取 **[!UICONTROL 「建立]** 」，然後選取 **[!UICONTROL 「建立標記」]** 選項。
3. 指定：

   * **[!UICONTROL 標題]**
      *(必要)* 標記的顯示標題。
   * **[!UICONTROL Name]**
      *(必要)* 標記的名稱。如果未指定，則會從「標題」建立有效的節點名稱。請參閱 [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **說明**
      *(選用)* 標記的說明。
   * **標籤的標籤路徑** JCR路徑。

4. 選擇 **[!UICONTROL 「提交]** 」以建立標記。

   在AEM實例上建立標籤後，標籤將可附加至資產(使用該資產的「屬性」區段或「管理標記」區段)。

5. **將標籤發佈至品牌入口網站**。

   前往 **[!UICONTROL AEM標籤]** 主控台([!UICONTROL 工具|標記|AEM標記]))，選取所需標記並發佈至品牌入口網站。

6. **附加標籤至資產(或系列)**。

   選取資產(或系列)，然後使用該資產的「屬性」區段或「管理標記」區段附加所需標記。若要深入瞭解如何將標記指派給AEM Assets中的資產，請參閱 [使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

7. **將資產(或系列)發佈至品牌入口網站**。\
   當您將資產(或系列)發佈至品牌入口網站時，品牌入口網站也可以使用附加標籤。

   若要查看品牌入口網站中個別資產(或系列)的附加標籤，登入品牌入口網站並選取資產，請在「屬性」區段下查看附加的標記。

## 搜尋提升 {#search-promote}

AEM Assets Brand Portal可讓您根據關鍵字標記，讓特定資產成為搜尋的首要結果。

若要為搜尋關鍵字提升資產，請遵循下列步驟：

1. 在AEM作者實例上開啓資產的 **[!UICONTROL 「屬性]** 」頁面。
2. 前往 **[!UICONTROL 「進階]** 」標籤。
3. 在 ******[!UICONTROL 「搜尋關鍵字]** 」區段中的「搜尋促銷」中，選取 **[!UICONTROL 「新增」]** 以新增搜尋關鍵字或標籤。

   ![](assets/search-promote.png)

4. 儲存變更。
5. 將資產發佈至 Brand Portal.
6. 登入品牌入口網站。資產 **[!UICONTROL 區段]** 中 **[!UICONTROL 的]** 「進階」標籤。
請注意 **[!UICONTROL ，該資產的屬性也會顯示Search Promote]** 關鍵字。
