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
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

瞭解如何從 [!DNL AEM] 資產發佈標記至 [!DNL Brand Portal]。

標籤在組織資產時很有用，並可增強關聯資產的可存取性。標籤可視為隨附於資產的關鍵字或標籤(中繼資料)，並可讓資產快速找到作為搜尋結果。若要瞭解如何將標記指派至 [!DNL AEM] 資產中的資產，請參閱 [使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

標記(與資產和系列關聯) [!DNL AEM]會自動發佈至 [!DNL Brand Portal] 已發佈相關聯標記 [!DNL Brand Portal]的資產(和系列)。發佈的標籤有助於搜尋找到相關聯的資產。

>[!NOTE]
>
>不過，建議您先將標記發佈至 [!DNL Brand Portal] 發佈標記所關聯的資產(和系列)。如此可確保資產(和系列)的發佈速度更快 [!DNL Brand Portal]。

## Manage tags {#manage-tags}

您可以使用現有標籤附加至資產，或從 [!DNL AEM] 標籤控制台建立新標記(**工具|標記|[!DNL AEM]標記**)。在這兩種情況下，您必須先發佈 [!DNL Brand Portal] 標記並將其與適當資產關聯。

若要建立標記， [!DNL AEM]發佈標記， [!DNL Brand Portal]並將標記與適當資產(或系列)建立關聯，請遵循下列步驟：

1. **建立標記**[!DNL AEM] 以管理權限登入作者實例，並從全域導覽存取 **[!DNL AEM]「標記** 控制台」：

   1. 選取 **工具**

   2. 選取 **一般**

   3. 選取 **標記**

2. 選取 **「建立** 」，然後選取 **「建立標記」** 選項。
3. 指定：

   * **標題**
      *(必要)* 標記的顯示標題。
   * **名稱**
      *(必要)* 標記的名稱。如果未指定，則會從「標題」建立有效的節點名稱。請參閱 [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID)。
   * **說明**
      *(選用)* 標記的說明。
   * **標籤的標籤路徑** JCR路徑。

4. 選擇 **「提交** 」以建立標記。

   [!DNL AEM] 在例項建立標籤後，標籤將可附加至資產(使用該資產的「屬性」區段或「管理標記」區段)。

5. **將標籤發佈[!DNL Brand Portal]**&#x200B;至。

   前往 **[!DNL AEM]標籤** 控制台(工具|標記| [!DNL AEM] 標記))，選取所要的標記並發佈至 **[!DNL Brand Portal]**。

6. **附加標籤至資產(或系列)**。

   選取資產(或系列)，然後使用該資產的「屬性」區段或「管理標記」區段附加所需標記。若要深入瞭解如何將標記指派至 [!DNL AEM] 資產中的資產，請參閱 [使用標籤來組織資產](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)。

7. **將資產(或系列)發佈[!DNL Brand Portal]**&#x200B;至。\
   當您將資產(或系列)發佈至時， [!DNL Brand Portal]也會提供附加的標記 [!DNL Brand Portal]。

   若要查看個別資產(或系列)上的附加標記 [!DNL Brand Portal]，登入 [!DNL Brand Portal] 並選取資產，請在「屬性」區段下查看附加的標記。

## 搜尋提升 {#search-promote}

[!DNL AEM] 資產 [!DNL Brand Portal] 可讓您將特定資產作為根據關鍵字標記搜尋的首要結果。

若要為搜尋關鍵字提升資產，請遵循下列步驟：

1. 在作者實例上開啓資產的 **「屬性**[!DNL AEM] 」頁面。
2. 前往 **「進階** 」標籤。
3. 在 ******「搜尋關鍵字** 」區段中的「搜尋促銷」中，選取 **「新增」** 以新增搜尋關鍵字或標籤。

   ![](assets/search-promote.png)

4. 儲存變更。
5. Publish the asset to [!DNL Brand Portal].
6. [!DNL Brand Portal]登入。資產 **區段** 中 **的** 「進階」標籤。
請注意 **，該資產的屬性也會顯示Search Promote** 關鍵字。
