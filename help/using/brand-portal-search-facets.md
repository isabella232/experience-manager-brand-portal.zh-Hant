---
title: 使用自訂搜尋Facet
seo-title: 使用自訂搜尋Facet
description: 管理員可以將搜尋預覽新增至「篩選器」面板，自訂搜尋並使搜尋功能更加多功能。
seo-description: 管理員可以將搜尋預覽新增至「篩選器」面板，自訂搜尋並使搜尋功能更加多功能。
uuid: 986fba5a-fac5-4128-ac75-d04 da5 b52 d45
content-type: 引用
topic-tags: 管理
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: 19fa028-246b-42c7-869f-97c95c a1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 使用自訂搜尋Facet {#use-custom-search-facets}

管理員可以將搜尋預覽新增至 [!UICONTROL 「篩選器] 」面板，自訂搜尋並使搜尋功能更加多功能。

品牌入口網站支援 [Facet搜尋](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) ，以精細搜尋已核准的品牌資產，因為 [**「篩選器** 」面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)是可能的。「篩選器」面板可透過管理工具中 **[!UICONTROL 的「搜尋表單]** 」提供。管理工具中的「搜尋表單」頁面存在名為「資產管理搜尋邊欄」的預設搜尋表單。不過，管理員可以借由新增、修改或移除搜尋預期詞，借由編輯預設搜尋表單(資產管理搜尋邊欄)來自訂預設「篩選」面板，使搜尋功能更加豐富。

您可以使用各種搜尋預期詞來自訂 **[!UICONTROL 「篩選」]** 面板。例如，新增屬性述詞，搜尋符合您在本預覽中指定之單一屬性的資產。新增選項預覽，以搜尋符合特定屬性所指定之一或多個值的資產。新增日期範圍述詞，搜尋在指定日期範圍內建立的資產。

>[!NOTE]
>
>AEM可讓組織 [將自訂搜尋表單從AEM作者發佈](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) 至品牌入口網站，而不是在品牌入口網站上重新建立相同表格。

## 新增搜尋預覽 {#add-a-search-predicate}

若要新增搜尋預覽至 **[!UICONTROL 「篩選」]** 面板：

1. 若要存取管理工具，請從頂端的工具列按一下AEM標誌。

   ![](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 搜尋表單]**。

   ![](assets/navigation-panel-1.png)

3. 在 **[!UICONTROL 搜尋表單]** 頁面中，選取 **[!UICONTROL 資產管理搜尋邊欄]**。

   ![](assets/search-forms-page.png)

4. 在出現在頂端的工具列上，按一下 **[!UICONTROL 「編輯]** 」以開啓編輯搜尋表單。

   ![](assets/edit-search-form-1.png)

5. 在 [!UICONTROL 「編輯搜尋表單] 」頁面中，將預覽從 [!UICONTROL 「選擇Predicate] 」標籤拖曳至主窗格。例如，拖曳 **[!UICONTROL 屬性Predicate]**。

   **[!UICONTROL 「屬性]** 」欄位會出現在主窗格中，而右側的「 **[!UICONTROL 設定」]** 標籤會顯示屬性預設值。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL 「設定」]** 標籤中的標題標籤可識別您選取的預覽字詞類型。

6. 在 **[!UICONTROL 「設定]** 」標籤中，輸入屬性述詞的標籤、預留位置文字和說明。

   * 如果您想要根據指定的屬性值允許部分詞組搜尋(和萬用字元搜尋)，請選取 **[!UICONTROL 部分搜尋]**。預設情況下，predicate支援全文搜尋。
   * 如果您想要根據屬性值不區分大小寫，請選取 **[!UICONTROL 忽略大小寫]**。依預設，搜尋篩選條件中的屬性值會區分大小寫。
   >[!NOTE]
   >
   >選取 **[!UICONTROL 部分搜尋]** 核取方塊時，預設會選取 [!UICONTROL 忽略大小寫] 。

7. 在 [!UICONTROL 「屬性名稱] 」欄位中，開啓屬性選擇器並選取執行搜尋所依據的屬性。或者，輸入屬性的名稱。例如，輸入 [!UICONTROL `  jcr :content/metadata/dc:title`] 或 [!UICONTROL `./jcr:content/metadata/dc:title`]。

   ![](assets/title-prop.png)

8. 按一下 **[!UICONTROL 「完成]** 」以儲存設定。
9. 從 [!UICONTROL 「資產] 」使用者介面中，按一下覆蓋圖示，然後選擇 **[!UICONTROL 「篩選」]** 以導覽至 **[!UICONTROL 「篩選」]** 面板。**[!UICONTROL Property]** Predicate is added to the panel.

   ![](assets/property-filter-panel.png)

10. 輸入要在 **[!UICONTROL 「屬性]** 」文字方塊中搜尋之資產的標題。例如，「Adobe」。當您執行搜尋時，搜尋結果中會顯示與「Adobe」相符的資產。

## 搜尋預期詞清單 {#list-of-search-predicates}

類似於新增 **[!UICONTROL 屬性]** 述詞，您可以將下列預覽新增至 **[!UICONTROL 「篩選」]** 面板：

| **Predicate Name** | **說明** | **屬性** |
|-------|-------|----------|
| [!UICONTROL 路徑瀏覽器] | 搜尋素材，以便在特定位置搜尋資產。**注意：***對於登入使用者，「篩選」上的路徑瀏覽器只會顯示與使用者共用的資料夾(及其擁有人)的內容結構。*<br> 管理員使用者可使用路徑瀏覽器瀏覽至該資料夾，以在任何資料夾中搜尋資產。<br> 而非管理員使用者可透過導覽至路徑瀏覽器中的資料夾，在資料夾中搜尋資產(可存取)。 | <ul><li>欄位標籤</li><li>路徑</li><li>說明</li></ul> |
| [!UICONTROL 屬性] | 根據特定中繼資料屬性搜尋資產。**注意：***選取部分搜尋時，預設會選取忽略大小寫*。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>部分搜尋</li><li>忽略大小寫</li><li> 說明</li></ul> |
| [!UICONTROL 多值屬性] | 類似屬性預測，但允許多個輸入值(由分隔字元分隔)分隔的多個輸入值(預設為COMA[，])會在結果中傳回任何輸入值。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>分隔符號支援</li><li>忽略大小寫</li><li>說明</li></ul> |
| [!UICONTROL 標記] | 搜尋預覽以根據標記搜尋資產。您可以設定「路徑」屬性，在「標記」清單中填入各種標記。*注意：管理員可能需要變更路徑值(例如 [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]，如果他們從AEM發佈搜尋表單)，例如，路徑不包含租用者資訊 [!UICONTROL `/etc/tags/<custom_tag_namespace>`]。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>路徑</li><li>說明</li></ul> |
| [!UICONTROL 路徑] | 搜尋素材，以便在特定位置搜尋資產。 | <ul><li>欄位標籤</li><li>路徑</li><li>說明</li></ul> |  |
| [!UICONTROL 相對日期] | 搜尋素材，以根據其建立的相對日期來搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>相對日期</li></ul> |
| [!UICONTROL 範圍] | 搜尋預覽來搜尋位於指定之屬性值範圍內的資產。在「篩選」面板中，您可以指定範圍的最小和最大屬性值。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 日期範圍] | 搜尋預覽，用以搜尋日期屬性指定範圍內所建立的資產。在「篩選」面板中，您可以指定「開始」和「結束」日期。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>範圍文字(從)</li><li>範圍文字(若要)</li><li>說明</li></ul> |
| [!UICONTROL 日期] | 根據日期屬性的資產之基於滑桿搜尋的搜尋預測。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 檔案大小] | 搜尋素材，以根據其大小搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>路徑</li><li>說明</li></ul> |
| [!UICONTROL 上次修改的資產] | 搜尋預覽，以根據上次修改日期搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 核准狀態] | 搜尋預覽以根據核准中繼資料屬性搜尋資產。預設屬性名稱 **為dam：狀態**。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 簽出狀態] | 搜尋預測，以根據資產從AEM Assets發佈時的結帳狀態來搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 簽出者] | 搜尋素材，根據已取出資產的使用者來搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 到期狀態] | 搜尋預覽，以根據過期狀態搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| [!UICONTROL 系列成員] | 搜尋素材，根據資產是否屬於系列的一部分來搜尋資產。 | 說明 |
| [!UICONTROL 隱藏] | 此predicate並非明確顯示給一般使用者，且用於一般限制搜尋結果類型至 **dam的隱藏限制：資產**。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |

>[!NOTE]
>
>請勿使用 **[!UICONTROL 「選項Predicate]**」、 **[!UICONTROL 「Publish Status Predicate]**」和 **[!UICONTROL 「Calculation Predicate]** 」，因為這些Predicates無法在品牌入口網站中運作。

## 刪除搜尋預覽 {#delete-a-search-predicate}

若要刪除搜尋預覽，請遵循下列步驟：

1. 按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 搜尋表單]**。

   ![](assets/navigation-panel-2.png)

3. 在 **[!UICONTROL 搜尋表單]** 頁面中，選取 **[!UICONTROL 資產管理搜尋邊欄]**。

   ![](assets/search-forms-page.png)

4. 在出現在頂端的工具列上，按一下 **[!UICONTROL 「編輯]** 」以開啓編輯搜尋表單。

   ![](assets/edit-search-form-2.png)

5. 在 [!UICONTROL 「編輯搜尋表單] 」頁面中，從主窗格中選取您要刪除的預覽。例如，選取 **[!UICONTROL 「屬性Predicate]**」。

   右側的「 **[!UICONTROL 設定]** 」標籤會顯示屬性預覽欄位。

6. 若要刪除屬性預覽，請按一下bin圖示。在 **[!UICONTROL 「刪除欄位」]** 對話方塊中，按一下 **[!UICONTROL 「刪除]** 」以確認刪除動作。

   **[!UICONTROL 「屬性Predicate]** 」欄位會從主窗格中移除，而「 **[!UICONTROL 設定]** 」標籤會變成空白。

   ![](assets/search-form-delete-predicate.png)

7. 若要儲存變更，請按一下工具列 **[!UICONTROL 中的「完成]** 」。
8. 從 **[!UICONTROL 「資產]** 」使用者介面中，按一下覆蓋圖示，然後選擇 **[!UICONTROL 「篩選」]** 以導覽至 **[!UICONTROL 「篩選」]** 面板。**[!UICONTROL 「屬性]** 」Predicate會從面板中移除。

   ![](assets/property-predicate-removed.png)
