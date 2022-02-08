---
title: 在 Brand Portal 上搜尋資產
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Brand Portal搜索功能允許您使用搜索功能快速搜索相關資產，搜索篩選器可幫助您進一步縮小搜索範圍。 將搜索另存為智慧集合，以備將來使用。
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: dc425522f134781b4420eb8643ee6ee65d98b6cc
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 5%

---

# 在 Brand Portal 上搜尋資產 {#search-assets-on-brand-portal}

Brand Portal搜索功能允許您使用nisearch快速搜索相關資產，而facet搜索則使用篩選器幫助您進一步縮小搜索範圍。 您可以在檔案或資料夾級別搜索資產，並將搜索結果另存為智慧集合。 但是，不能使用nisearch或facet搜索搜索集合的資產。

## 使用Omnisearch搜索資產 {#search-assets-using-omnisearch}

在Brand Portal搜索資產：

1. 在工具欄中，按一下 **[!UICONTROL 搜索]** 表徵圖，或按「**[!UICONTROL /]**」鍵啟動Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜索框中，為要搜索的資產鍵入關鍵字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >搜索建議時至少需要3個字元。

1. 從下拉清單中顯示的相關建議中進行選擇，以快速訪問相關資產。

   ![](assets/assets-search-result.png)

   *使用內部搜索的資產搜索*

要瞭解有智慧標籤資產的搜索行為，請參閱 [瞭解搜索結果和行為](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html)。

## 在「濾鏡」面板中使用小平面進行搜索 {#search-using-facets-in-filters-panel}

「篩選器」面板中的搜索小平面將粒度添加到您的搜索體驗中，並使搜索功能高效。 搜索小平面使用多個尺寸（謂語），使您能夠執行複雜的搜索。 您可以輕鬆細化到所需的詳細級別，以便進行更集中的搜索。

例如，如果要查找影像，則可以選擇是要點陣圖還是向量影像。 通過在「檔案類型」搜索方面中為影像指定MIME類型，可以進一步縮小搜索範圍。 同樣，在搜索文檔時，可以指定格式，例如PDF或MS Word格式。

![過濾器面板在Brand Portal](assets/file-type-search.png "過濾器面板在Brand Portal")

的 **[!UICONTROL 篩選器]** 面板包括幾個標準小平面，如 —  **[!UICONTROL 路徑瀏覽器]**。 **[!UICONTROL 檔案類型]**。 **[!UICONTROL 檔案大小]**。 **[!UICONTROL 狀態]**, **[!UICONTROL 方向]**。 但是， [添加自定義搜索小面](../using/brand-portal-search-facets.md) 或從中移除特定搜索小平面 **[!UICONTROL 篩選器]** 通過在基礎搜索表單中添加或刪除謂語來顯示面板。 請參閱可用和可用的清單 [搜索謂詞Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates)。

使用可用的 [搜索小面](../using/brand-portal-search-facets.md):

1. 按一下覆蓋表徵圖並選擇 **[!UICONTROL 篩選]**。

   ![](assets/selectorrail.png)

1. 從 **[!UICONTROL 篩選器]** 面板中，選擇適當的選項以應用相關篩選器。
例如，使用以下標準篩選器：

   * **[!UICONTROL 路徑瀏覽器]** 搜索特定目錄中的資產。 路徑瀏覽器謂詞的預設搜索路徑為 `/content/dam/mac/<tenant-id>/`，可通過編輯預設搜索表單來配置。
   >[!NOTE]
   >
   >對非管理員用戶， [!UICONTROL 路徑瀏覽器] 在 [!UICONTROL 篩選] 面板僅顯示與其共用的資料夾（及其上級資料夾）的內容結構。\
   >對於管理員用戶，路徑瀏覽器允許導航到Brand Portal的任何資料夾。

   * **[!UICONTROL 檔案類型]** 指定要查找的資產檔案的類型（影像、文檔、多媒體、存檔）。 此外，您還可以縮小搜索範圍，例如，為文檔指定影像或格式(PDF或MS Word)的MIME類型（Tiff、Bitmap、GIMP影像）。
   * **[!UICONTROL 檔案大小]** 根據資產規模搜索資產。 您可以指定大小範圍的下限和上限以縮小搜索範圍並指定要搜索的度量單位。
   * **[!UICONTROL 狀態]** 要根據資產狀態搜索資產，如審批（批准）、請求更改、拒絕、待定)和到期。
   * **[!UICONTROL 平均評級]** 根據資產評級搜索資產。
   * **[!UICONTROL 方向]** 根據資產的方向（水準、垂直、方形）搜索資產。
   * **[!UICONTROL 樣式]** 根據資產的樣式（彩色、單色）搜索資產。
   * **[!UICONTROL 視頻格式]** 根據其格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索視頻資產。

   您可以使用 [自定義搜索方面](../using/brand-portal-search-facets.md) 在「篩選器」面板中，編輯基礎的搜索表單。

   * **[!UICONTROL 屬性謂詞]** 如果在搜索表單中使用，則允許您搜索與謂詞映射到的元資料屬性匹配的資產。\
      例如，如果屬性謂詞映射到 [!UICONTROL `jcr:content /metadata/dc:title`]，您可以根據其標題搜索資產。\
      的 [!UICONTROL 屬性謂詞] 支援文本搜索：

      **部分詞組**
若要允許以屬性述詞中的部分詞組搜尋資產，請啓用「搜尋表單」中的**[!UICONTROL 「部分搜尋」]**&#x200B;核取方塊。\
      如此一來，便可讓您搜尋所需資產，即使您未指定資產中繼資料裡所使用的確切單字/詞組。\
      您可以：
      * 在「過濾器」面板的方面中指定搜索短語中出現的單詞。 例如，如果搜索術語 **爬** (並且屬性謂詞映射到 [!UICONTROL `dc:title`] 屬性)，然後所有的資產 **爬** 將返回其標題短語。
      * 指定搜索短語中出現的單詞的一部分，以及通配符(*)以填補空白。
例如，搜尋：
         * **爬** 返回所有具有以其標題短語中的字元「climp」開頭的字詞的資產。
         * ***爬** 返回其標題短語中包含以字元「climp」結尾的所有資產。
         * ***爬*** 返回所有在其標題短語中包含「climp」字元的資產。

要允許屬性謂語中的非區分大小寫搜索，請啟用       **非區分大小寫的文本**
要允許屬性謂語中的非區分大小寫搜索，請啟用 **[!UICONTROL 忽略大小寫]** 複選框。 預設情況下，屬性謂語上的文本搜索區分大小寫。
   >[!NOTE]
   >
   >選擇 **[!UICONTROL 部分搜索]** 複選框， **[!UICONTROL 忽略大小寫]** 的下界。

   ![](assets/wildcard-prop-1.png)

   根據所應用的過濾器以及搜索結果計數顯示搜索結果。

   ![](assets/omnisearch-with-filters.png)

   具有搜索結果計數的資產搜索結果。

1. 您可以輕鬆地從搜索結果導航到項目，並使用瀏覽器中的後退按鈕返回到相同的搜索結果，而無需重新運行搜索查詢。

## 將搜索另存為智慧集合 {#save-your-searches-as-smart-collection}

您可以將搜索設定另存為智慧集合，以便能夠快速重複相同的搜索，而無需稍後重做相同的設定。 但是，不能在集合中應用搜索篩選器。

將搜索設定另存為智慧集合：

1. 點擊/按一下 **[!UICONTROL 保存智慧集合]** 並提供智慧收藏的名稱。

   要使智慧集合可供所有用戶訪問，請選擇 **[!UICONTROL 公共]**。 一條消息確認已建立智慧集合併將其添加到已保存的搜索清單中。

   >[!NOTE]
   >
   >非管理員用戶可以限制其公開智慧集合，以避免在組織的Brand Portal上擁有大量由非管理員用戶建立的公共智慧集合。 組織可以禁用 **[!UICONTROL 允許建立公共智慧集合]** 配置 **[!UICONTROL 常規]** 「管理工具」面板中提供的設定。

   ![](assets/save_smartcollectionui.png)

1. 要以其他名稱保存智慧集合，請選擇或清除 **[!UICONTROL 公共]** 複選框，按一下 **[!UICONTROL 編輯智慧集合]**。

   ![](assets/edit_smartcollection.png)

1. 在 **[!UICONTROL 編輯智慧集合]** 對話框，選擇 **[!UICONTROL 另存為]** 並輸入智慧集合的名稱。 按一下「**[!UICONTROL 儲存]**」。

   ![](assets/saveas_smartsearch.png)
