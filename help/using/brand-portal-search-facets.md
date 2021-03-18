---
title: 使用自訂搜尋 Facet
seo-title: 使用自訂搜尋 Facet
description: 管理員可將搜尋謂語新增至「篩選」面板，以自訂搜尋並讓搜尋功能變得多功能。
seo-description: 管理員可將搜尋謂語新增至「篩選」面板，以自訂搜尋並讓搜尋功能變得多功能。
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: 管理員
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 使用自訂搜尋 Facet {#use-custom-search-facets}

管理員可將搜尋謂語新增至[!UICONTROL 篩選器]面板，以自訂搜尋並讓搜尋功能變得多功能。

品牌入口網站支援[多面搜尋](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)，以精細搜尋已核准的品牌資產，這可能是由於&#x200B;[**Filters**&#x200B;面板](../using/brand-portal-searching.md#search-using-facets-in-filters-panel)所致。 透過管理工具中的&#x200B;**[!UICONTROL 搜尋表單]**，在「篩選器」面板上提供搜尋Facet。 管理工具的「搜尋Forms」頁面中存在名為「資產管理搜尋邊欄」的預設搜尋表單。 不過，管理員可以透過新增、修改或移除搜尋謂語來編輯預設搜尋表單（資產管理搜尋邊欄），自訂預設的「篩選」面板，讓搜尋功能變得多功能。

您可以使用各種搜尋謂語來自訂&#x200B;**[!UICONTROL Filters]**&#x200B;面板。 例如，新增屬性述詞以搜尋符合您在此述詞中指定之單一屬性的資產。 新增選項述詞，以搜尋符合您為特定屬性所指定之一或多個值的資產。 新增日期範圍述詞，以搜尋在指定日期範圍內建立的資產。

>[!NOTE]
>
>AEM可讓組織[將自訂的搜尋表單從AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal)發佈至品牌入口網站，而不是在品牌入口網站上重新建立相同的表單。

## 添加搜索謂詞{#add-a-search-predicate}

要向&#x200B;**[!UICONTROL Filters]**&#x200B;面板添加搜索謂語：

1. 若要存取管理工具，請按一AEM下頂端工具列中的標誌。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下「搜尋Forms ]**」。**[!UICONTROL 

   ![](assets/navigation-panel-1.png)

1. 在&#x200B;**[!UICONTROL 搜尋Forms]**&#x200B;頁面中，選取&#x200B;**[!UICONTROL 資產管理搜尋邊欄]**。

   ![](assets/search-forms-page.png)

1. 在顯示在頂端的工具列上，按一下「編輯&#x200B;****」以開啟編輯搜尋表單。

   ![](assets/edit-search-form-1.png)

1. 在[!UICONTROL 編輯搜索表單]頁中，將[!UICONTROL 選擇謂詞]頁籤中的謂詞拖動到主窗格。 例如，拖曳&#x200B;**[!UICONTROL Property Predicate]**。

   **[!UICONTROL 屬性]**&#x200B;欄位會出現在主窗格中，而右側的&#x200B;**[!UICONTROL 設定]**&#x200B;標籤會顯示屬性謂語。

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >**[!UICONTROL Settings]**&#x200B;標籤中的標題標籤標識您選擇的謂詞類型。

1. 在&#x200B;**[!UICONTROL Settings]**&#x200B;標籤中，輸入屬性謂語的標籤、預留位置文字和說明。

   * 如果您想要根據指定的屬性值允許資產的部分片語搜尋（和萬用字元搜尋），請選取&#x200B;**[!UICONTROL 部分搜尋]**。 預設情況下，謂詞支援全文搜索。
   * 如果您希望基於屬性值的資產搜索不區分大小寫，請選擇「忽略大小寫」。 ****&#x200B;依預設，搜尋篩選器中的屬性值會區分大小寫。

   >[!NOTE]
   >
   >在選中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;複選框時，預設選擇&#x200B;**[!UICONTROL 忽略大小寫]**。

1. 在&#x200B;**[!UICONTROL 屬性名稱]**&#x200B;欄位中，開啟屬性選擇器並選取執行搜尋的屬性。 或者，輸入屬性的名稱。 例如，輸入 `  jcr :content/metadata/dc:title` 或 `./jcr:content/metadata/dc:title`。

   >[!NOTE]
   >
   >在品牌入口網站中，預設會為`dam:asset`的`jcrcontent/metadata`中所有屬性（以`xmp`開頭的屬性除外）建立索引。
   >
   >建立屬性謂語時，可以使用任何已編製索引的屬性。 如果配置了任何非索引屬性，則未索引屬性上的搜索查詢不能提供任何搜索結果。

   ![](assets/title-prop.png)

1. 按一下&#x200B;**[!UICONTROL Done]**&#x200B;保存設定。
1. 從[!UICONTROL Assets]使用者介面，按一下覆蓋圖示並選擇&#x200B;**[!UICONTROL Filter]**&#x200B;以導覽至&#x200B;**[!UICONTROL Filters]**&#x200B;面板。 The **[!UICONTROL Property]** predicate is added to the panel.

   ![](assets/property-filter-panel.png)

1. 在&#x200B;**[!UICONTROL Property]**&#x200B;文字方塊中輸入要搜尋的資產標題。 例如，「Adobe」。 當您執行搜尋時，標題符合「Adobe」的資產會顯示在搜尋結果中。

## 搜索謂語清單{#list-of-search-predicates}

與添加&#x200B;**[!UICONTROL Property]**&#x200B;謂語的方式類似，您可以將以下謂語添加到&#x200B;**[!UICONTROL Filters]**&#x200B;面板：

| **謂詞名稱** | **說明** | **屬性** |
|-------|-------|----------|
| **[!UICONTROL 路徑瀏覽器]** | 搜尋謂詞以搜尋特定位置的資產。 **注意：對** *於登入的使用者，「篩選」上的路徑瀏覽器只會顯示與使用者共用的資料夾（及其祖先）的內容結構。* <br> 管理員使用者可使用路徑瀏覽器導覽至任何資料夾，以搜尋該資產。<br> 但是，非管理員使用者可在路徑瀏覽器中導覽至該資料夾，以搜尋資料夾中的資產（可供他們存取）。 | <ul><li>欄位標籤</li><li>路徑</li><li>說明</li></ul> |
| **[!UICONTROL 屬性]** | 根據特定中繼資料屬性搜尋資產。 **注意：在選** *取「部分搜尋」時，預設會選取「忽略大小寫」*。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>部分搜尋</li><li>忽略大小寫</li><li> 說明</li></ul> |
| **[!UICONTROL 多值屬性]** | 與屬性謂語類似，但允許以分隔字元分隔的多個輸入值（預設值為COMMA[,]），以結果傳回符合任何輸入值的資產。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>分隔符號支援</li><li>忽略大小寫</li><li>說明</li></ul> |
| **[!UICONTROL 標記]** | 搜尋謂詞以根據標籤搜尋資產。 您可以設定Path屬性，以填入「標籤」清單中的各種標籤。 *注意：如果管理員發佈搜尋表單時，路徑不包含租用戶資訊，例如[!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]，則可能AEM需要變更路徑值。[!UICONTROL `/etc/tags/<custom_tag_namespace>`] | <ul><li>欄位標籤</li><li>屬性名稱</li><li>路徑</li><li>說明</li></ul> |
| **[!UICONTROL 路徑]** | 搜尋謂詞以搜尋特定位置的資產。 | <ul><li>欄位標籤</li><li>路徑</li><li>說明</li></ul> |  |
| **[!UICONTROL 相對日期]** | 搜尋謂詞以根據資產建立的相對日期來搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>相對日期</li></ul> |
| **[!UICONTROL 範圍]** | 搜尋謂詞，以搜尋位於指定屬性值範圍內的資產。 在「篩選器」面板中，您可以指定範圍的最小和最大屬性值。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 日期範圍]** | 搜尋謂詞，以搜尋在指定範圍內建立的日期屬性資產。 在「篩選」面板中，您可以指定開始和結束日期。 | <ul><li>欄位標籤</li><li>預留位置</li><li>屬性名稱</li><li>範圍文字（自）</li><li>範圍文字（至）</li><li>說明</li></ul> |
| **[!UICONTROL 日期]** | 根據日期屬性搜尋資產的滑桿式搜尋謂詞。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 檔案大小]** | 搜尋謂詞以根據資產大小搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>路徑</li><li>說明</li></ul> |
| **[!UICONTROL 上次修改的資產]** | 搜尋謂詞以根據上次修改的日期搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 核准狀態]** | 搜尋謂詞以根據核准中繼資料屬性搜尋資產。 預設屬性名稱為&#x200B;**dam:status**。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 簽出狀態]** | 從AEM Assets發佈資產時，搜尋謂詞以根據資產的檢出狀態來搜尋資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 簽出者]** | 搜尋謂詞，以根據已簽出資產的用戶搜索資產。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 到期狀態]** | 根據到期狀態搜尋資產的搜尋謂詞。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |
| **[!UICONTROL 系列成員]** | 搜尋謂詞，以根據資產是否屬於系列的一部分來搜尋資產。 | 說明 |
| **[!UICONTROL 隱藏]** | 此謂語不明確顯示給最終用戶，用於任何通常用於將搜索結果類型限制為&#x200B;**dam:Asset**&#x200B;的隱藏約束。 | <ul><li>欄位標籤</li><li>屬性名稱</li><li>說明</li></ul> |

>[!NOTE]
>
>請勿使用&#x200B;**[!UICONTROL Options Predicate]**、**[!UICONTROL Publish Status Predicate]**&#x200B;和&#x200B;**[!UICONTROL Rating Predicate]**，因為這些謂語在Brand Portal中無法運作。

## 刪除搜索謂語{#delete-a-search-predicate}

要刪除搜索謂語，請遵循以下步驟：

1. 按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下「搜尋Forms ]**」。**[!UICONTROL 

   ![](assets/navigation-panel-2.png)

1. 在&#x200B;**[!UICONTROL 搜尋Forms]**&#x200B;頁面中，選取&#x200B;**[!UICONTROL 資產管理搜尋邊欄]**。

   ![](assets/search-forms-page.png)

1. 在顯示在頂端的工具列上，按一下「編輯&#x200B;****」以開啟編輯搜尋表單。

   ![](assets/edit-search-form-2.png)

1. 在[!UICONTROL 編輯搜索表單]頁中，從主窗格中選擇要刪除的謂語。 例如，選擇&#x200B;**[!UICONTROL Property Predicate]**。

   右側的&#x200B;**[!UICONTROL Settings]**&#x200B;標籤會顯示屬性謂詞欄位。

1. 若要刪除屬性謂語，請按一下bin圖示。 在&#x200B;**[!UICONTROL 刪除欄位]**&#x200B;對話框中，按一下&#x200B;**[!UICONTROL 刪除]**&#x200B;以確認刪除操作。

   **[!UICONTROL 屬性謂語]**&#x200B;欄位會從主窗格中移除，而&#x200B;**[!UICONTROL 設定]**&#x200B;標籤會變成空白。

   ![](assets/search-form-delete-predicate.png)

1. 要保存更改，請按一下工具欄中的&#x200B;**[!UICONTROL Done]**。
1. 從&#x200B;**[!UICONTROL Assets]**&#x200B;使用者介面，按一下覆蓋圖示並選擇&#x200B;**[!UICONTROL Filter]**&#x200B;以導覽至&#x200B;**[!UICONTROL Filters]**&#x200B;面板。 **[!UICONTROL Property]** predicate已從面板中移除。

   ![](assets/property-predicate-removed.png)
