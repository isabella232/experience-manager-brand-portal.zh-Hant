---
title: 使用自訂搜尋 Facet
seo-title: Use custom search facets
description: 管理員可以將搜索謂語添加到「篩選器」面板，以自定義搜索並使搜索功能變得通用。
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 10%

---

# 使用自訂搜尋 Facet {#use-custom-search-facets}

管理員可以將搜索謂詞添加到 [!UICONTROL 篩選器] 用於自定義搜索並使搜索功能變得通用的面板。

Brand Portal支援 [多面搜索](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) 對批准品牌資產進行細粒度搜索，這可能是由於 [**篩選器** 面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)。 搜索小平面可在「濾鏡」面板上通過 **[!UICONTROL 搜索表單]** 的下界。 在管理工具的「搜索Forms」頁中，存在名為「資產管理搜索欄」的預設搜索表單。 但是，管理員可以通過添加、修改或刪除搜索謂語來編輯預設搜索表單（資產管理搜索導軌）來自定義預設的「篩選器」面板，從而使搜索功能變得通用。

可以使用各種搜索謂語自定義 **[!UICONTROL 篩選器]** 的子菜單。 例如，添加屬性謂詞以搜索與在此謂詞中指定的單個屬性相匹配的資產。 添加選項謂詞以搜索與您為特定屬性指定的一個或多個值相匹配的資產。 添加日期範圍謂詞以搜索在指定日期範圍內建立的資產。

>[!NOTE]
>
>Experience Manager Assets允許組織 [從AEM Author發佈自定義搜索表單](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) 去Brand Portal，而不是在Brand Portal重新創造同樣的形式。

## 添加搜索謂詞 {#add-a-search-predicate}

將搜索謂詞添加到 **[!UICONTROL 篩選器]** 面板：

1. 要訪問管理工具，請按一下頂部工具欄上的Experience Manager徽標。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 搜索Forms]**。

   ![](assets/navigation-panel-1.png)

1. 在 **[!UICONTROL 搜索Forms]** ，選擇 **[!UICONTROL 資產管理搜索欄]**。

   ![](assets/search-forms-page.png)

1. 在頂部顯示的工具欄上，按一下 **[!UICONTROL 編輯]** 的子菜單。

   ![](assets/edit-search-form-1.png)

1. 在 [!UICONTROL 編輯搜索表單] 頁，從 [!UICONTROL 選擇謂詞] 的子菜單。 例如，拖動 **[!UICONTROL 屬性謂詞]**。

   的 **[!UICONTROL 屬性]** 欄位。 **[!UICONTROL 設定]** 頁籤中顯示屬性謂語。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >中的標題標籤 **[!UICONTROL 設定]** 頁籤標識您選擇的謂詞類型。

1. 在 **[!UICONTROL 設定]** 頁籤，輸入屬性謂詞的標籤、佔位符文本和說明。

   * 選擇 **[!UICONTROL 部分搜索]**，如果要允許基於指定屬性值對資產進行部分短語搜索（和通配符搜索）。 預設情況下，謂詞支援全文搜索。
   * 選擇 **[!UICONTROL 忽略大小寫]**，如果希望基於屬性值的資產搜索不區分大小寫。 預設情況下，在搜索篩選器中搜索屬性值時區分大小寫。

   >[!NOTE]
   >
   >選擇 **[!UICONTROL 部分搜索]** 複選框， **[!UICONTROL 忽略大小寫]** 的下界。

1. 在 **[!UICONTROL 屬性名稱]** 欄位，開啟屬性選取器，並選擇執行搜索時所依據的屬性。 或者，輸入屬性的名稱。 例如，輸入 `  jcr :content/metadata/dc:title` 或 `./jcr:content/metadata/dc:title`。

   >[!NOTE]
   >
   >在Brand Portal，除了那些 `xmp`) `jcrcontent/metadata` 共 `dam:asset` 預設情況下為索引。
   >
   >建立屬性謂詞時，可以使用索引的任何屬性。 如果配置了任何非索引屬性，則未索引屬性上的搜索查詢可能不會提供任何搜索結果。

   ![](assets/title-prop.png)

1. 按一下 **[!UICONTROL 完成]** 按鈕。
1. 從 [!UICONTROL 資產] 用戶介面，按一下覆蓋表徵圖並選擇 **[!UICONTROL 篩選]** 導航至 **[!UICONTROL 篩選器]** 的子菜單。 The **[!UICONTROL Property]** predicate is added to the panel.

   ![](assets/property-filter-panel.png)

1. 在中輸入要搜索的資產的標題 **[!UICONTROL 屬性]** 的子菜單。 例如，&quot;Adobe&quot;。 執行搜索時，標題與「Adobe」匹配的資產將顯示在搜索結果中。

## 搜索謂詞清單 {#list-of-search-predicates}

與添加 **[!UICONTROL 屬性]** 謂語，您可以將以下謂語添加到 **[!UICONTROL 篩選器]** 面板：

| **謂詞名稱** | **說明** | **屬性** |
|-------|-------|----------|
| **[!UICONTROL 路徑瀏覽器]** | 搜索謂詞以在特定位置搜索資產。 **注：** *對於已登錄的用戶，「篩選器」上的路徑瀏覽器僅顯示與該用戶共用的資料夾（及其祖先）的內容結構。* <br> 管理員用戶可以通過使用路徑瀏覽器導航到該資料夾來搜索任何資料夾中的資產。 <br> 但是，非管理員用戶可以通過導航到路徑瀏覽器中的資料夾來搜索資料夾中的資產（他們可訪問）。 | <ul><li>欄位標籤</li><li>路徑</li><li>說明</li></ul> |
| **[!UICONTROL 屬性]** | 基於特定元資料屬性搜索資產。 **注：** *在選擇「部分搜索」(Partial Search)時，預設情況下會選擇「忽略大小寫」(Ignore Case)*。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>部分搜尋</li><li>忽略大小寫</li><li> 說明</li></ul> |
| **[!UICONTROL 多值屬性]** | 與屬性謂語類似，但允許多個輸入值，用分隔符分隔（預設為COMMA）[。])匹配任何輸入值的資產將在結果中返回。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>分隔符號支援</li><li>忽略大小寫</li><li>說明</li></ul> |
| **[!UICONTROL 標記]** | 搜索謂詞以基於標籤搜索資產。 可以配置Path屬性以填充「標籤」清單中的各種標籤。 *注意：管理員可能需要更改路徑值，例如， [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]，如果搜索表單的發AEM布位置，則路徑不包括租戶資訊，例如， [!UICONTROL `/etc/tags/<custom_tag_namespace>`]。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>路徑</li><li>說明</li></ul> |
| **[!UICONTROL 路徑]** | 搜索謂詞以在特定位置搜索資產。 | <ul><li>欄位標籤</li><li>路徑</li><li>說明</li></ul> |  |
| **[!UICONTROL 相對日期]** | 搜索謂詞，根據資產建立的相對日期搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>相對日期</li></ul> |
| **[!UICONTROL 範圍]** | 搜索謂詞以搜索位於指定屬性值範圍內的資產。 在「篩選器」面板中，可以指定範圍的最小和最大屬性值。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 日期範圍]** | 搜索謂詞以搜索在指定範圍內為日期屬性建立的資產。 在「篩選器」面板中，可以指定「開始」和「結束日期」。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>範圍文本（自）</li><li>範圍文本（至）</li><li>說明</li></ul> |
| **[!UICONTROL 日期]** | 基於日期屬性搜索基於滑塊的資產的搜索謂語。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 檔案大小]** | 搜索謂詞以根據資產大小搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>路徑</li><li>說明</li></ul> |
| **[!UICONTROL 上次修改的資產]** | 搜索謂詞以根據上次修改的日期搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 審批狀態]** | 搜索謂詞以基於批准元資料屬性搜索資產。 預設屬性名為 **大壩：狀態**。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 簽出狀態]** | 搜索謂詞，根據資產從AEM Assets發佈時的簽出狀態搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 簽出者]** | 搜索謂詞，根據已簽出資產的用戶搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 到期狀態]** | 搜索謂詞以根據到期狀態搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 集合成員]** | 搜索謂詞，根據資產是否是集合的一部分來搜索資產。 | 說明 |
| **[!UICONTROL 隱藏]** | 此謂語對最終用戶不顯式可見，它用於通常用於將搜索結果類型限制為 **大壩：資產**。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |

>[!NOTE]
>
>不使用 **[!UICONTROL 選項謂詞]**。 **[!UICONTROL 發佈狀態謂詞]**, **[!UICONTROL 分級謂詞]** 因為這些謂語在Brand Portal不起作用。

## 刪除搜索謂詞 {#delete-a-search-predicate}

要刪除搜索謂語，請執行以下步驟：

1. 按一下Adobe徽標以訪問管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 搜索Forms]**。

   ![](assets/navigation-panel-2.png)

1. 在 **[!UICONTROL 搜索Forms]** ，選擇 **[!UICONTROL 資產管理搜索欄]**。

   ![](assets/search-forms-page.png)

1. 在頂部顯示的工具欄上，按一下 **[!UICONTROL 編輯]** 的子菜單。

   ![](assets/edit-search-form-2.png)

1. 在 [!UICONTROL 編輯搜索表單] 的子菜單。 例如，選擇 **[!UICONTROL 屬性謂詞]**。

   的 **[!UICONTROL 設定]** 頁籤中顯示屬性謂詞欄位。

1. 要刪除屬性謂詞，請按一下bin表徵圖。 在 **[!UICONTROL 刪除欄位]** 對話框，按一下 **[!UICONTROL 刪除]** 確認刪除操作。

   的 **[!UICONTROL 屬性謂詞]** 欄位， **[!UICONTROL 設定]** 頁籤變為空。

   ![](assets/search-form-delete-predicate.png)

1. 要保存更改，請按一下 **[!UICONTROL 完成]** 的子菜單。
1. 從 **[!UICONTROL 資產]** 用戶介面，按一下覆蓋表徵圖並選擇 **[!UICONTROL 篩選]** 導航至 **[!UICONTROL 篩選器]** 的子菜單。 的 **[!UICONTROL 屬性]** 謂詞將從面板中刪除。

   ![](assets/property-predicate-removed.png)
