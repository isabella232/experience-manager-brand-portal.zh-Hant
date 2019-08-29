---
title: 在品牌入口網站上搜尋資產
seo-title: AEM品牌入口網站上的資產搜尋和儲存搜尋
description: 品牌入口網站搜尋功能可讓您使用omnisearch快速搜尋相關資產，搜尋篩選器可協助您進一步縮小搜尋範圍。將搜尋儲存為未來智慧型系列。
seo-description: 品牌入口網站搜尋功能可讓您使用omnisearch快速搜尋相關資產，搜尋篩選器可協助您進一步縮小搜尋範圍。將搜尋儲存為未來智慧型系列。
uuid: c2955198-bdc0-4853-a13 a-661e6 a9 ec61 f
contentOwner: bdhar
content-type: 引用
products: SG_ PERIENCENCENAGER/Brand_ Portal
topic-tags: OpenAndPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12 a4 fe1 ba
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 在品牌入口網站上搜尋資產 {#search-assets-on-brand-portal}

[!DNL Brand Portal] 搜尋功能可讓您使用omnisearch和Facet搜尋快速搜尋相關資產，以協助您進一步縮小搜尋範圍。您也可以將搜尋儲存為未來智慧 [!UICONTROL 型系列] 。

## 使用Omnisearch搜尋資產 {#search-assets-using-omnisearch}

若要搜尋資產上 [!DNL Brand Portal]的資產：

1. 從工具列中按一下 **「搜尋** 」圖示，或按「**/**」鍵啓動Omnisearch。

   ![](assets/omnisearchicon-1.png)

2. 在搜尋方塊中，輸入您要搜尋之資產的關鍵字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >在omnisearch中需要至少個字元才能顯示搜尋建議。

3. 從顯示在下拉式清單中的相關建議中選取，以快速存取相關資產。

   ![](assets/assets-search-result.png)

   使用omnisearch進行資產搜尋

## 在篩選面板中使用Facet進行搜尋 {#search-using-facets-in-filters-panel}

在「篩選」面板中搜尋Facet，為您的搜尋體驗添加詳細程度，並提高搜尋功能。搜尋Facet使用多個維度(預測)，可讓您執行複雜搜尋。您可以輕鬆下鑽至所需的詳細程度，以進行更專注的搜尋。

例如，如果您要尋找影像，可以選擇要使用點陣圖或向量影像。您可以在「檔案類型搜尋」Facet中指定影像的MIME類型，進一步減少搜尋範圍。同樣地，在搜尋文件時，您可以指定格式，例如PDF或MS Word格式。

![[!DNL Brand Portal]](assets/file-type-search.png "Filters面板中的Filters面板[！DNL品牌入口網站]")

「篩選器」面板包含一些標準Facet，例如-路徑瀏覽器、檔案類型、檔案大小、狀態和方向。不過，您可以新增或移除基礎搜尋表單中的預覽， [新增自訂搜尋Facet或](../using/brand-portal-search-facets.md) 移除 **「篩選器** 」面板中的特定搜尋Facet。請參閱品牌入口網站上可用和可用 [搜尋預測的清單](../using/brand-portal-search-facets.md#list-of-search-predicates)。

若要套用篩選至您的搜尋，請使用可用 [的搜尋Facet](../using/brand-portal-search-facets.md)：

1. 按一下覆蓋圖示，然後選取 **「篩選**」。

   ![](assets/selectorrail.png)

2. 從左側的 **「篩選」** 面板中，選取適當的選項以套用相關篩選。
例如，使用下列標準篩選器：

   * **路徑瀏覽器** 可在特定目錄中搜尋資產。「路徑瀏覽器」的預設搜尋路徑為 */content/dam/mac/&lt; tenant-id&gt;/*，可透過編輯預設搜尋表單來設定。
   >[!NOTE]
   >
   >對於非管理員使用者，「篩選」面板中的「路徑瀏覽器」只會顯示與其共用的資料夾(及其相關資料夾)的內容結構。\
   >對於管理使用者，路徑瀏覽器允許導覽至任何資料夾 [!DNL Brand Portal]。

   * **檔案類型** 以指定您要尋找的資產檔案類型(影像、文件、多媒體、封存)。此外，您可以縮小搜尋範圍，例如指定文件的MIME類型(TIFF、Bitmap、GIMP影像)，以用於影像或格式(PDF或MS Word)。
   * **檔案大小** ，以根據其大小搜尋資產。您可以指定大小範圍的下限和上限，縮小搜尋範圍並指定搜尋單位。
   * **根據** 資產狀態搜尋資產的狀態，例如核准(已核准、已請求變更、已拒絕、待定)和過期。
   * **「平均評分** 」以根據資產評分搜尋資產。
   * **根據** 資產方向(水平、垂直、平方)搜尋資產。
   * **根據** 資產樣式(彩色、單色)搜尋資產的樣式。
   * **視訊格式** ，可根據其格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜尋視訊素材。
   您可以編輯「篩選」面板中的 [自訂搜尋Facet](../using/brand-portal-search-facets.md) ，方法是編輯基礎搜尋表單。

   * **Property Predicate** if used in the search form，allows you search for assets that相符a metadata property to which the predicate is patured is.\
      例如，如果「屬性Predicate」映射至 `jcr:content /metadata/dc:title`，則您可以根據其標題來搜尋資產。\
      Property Predicate支援文字搜尋：

      **部分詞組**
若要允許以屬性述詞中的部分詞組搜尋資產，請啓用「搜尋表單」中的**「部分搜尋」**&#x200B;核取方塊。\
      如此一來，便可讓您搜尋所需資產，即使您未指定資產中繼資料裡所使用的確切單字/詞組。\
      您可以：
*在「篩選」面板中，指定在Facet中所搜尋的片語中發生的單字。For example, if you search for the term **climb** (and Property Predicate is mapped to `dc:title` property), then all the assets with the word **climb** in their title phrase are returned.
*指定出現在搜尋片語中的單字部分，以及萬用字元(*)以填滿空隙。
例如，搜尋:
      **law*** 會傳回所有開頭為「爬升」字元的字詞，其標題為「爬升」。
      ***爬升** 會傳回所有具有字詞結尾為「爬升」字元的資產。
      ***爬升*** 會傳回所有包含字詞「爬升」字詞字詞的資產。\
      **不區分大小寫的文字**&#x200B;若要在屬性預覽中允許區分大小寫搜尋，請啓用搜尋表單中的 **「忽略大小寫** 」核取方塊。依預設，屬性預覽上的文字搜尋會區分大小寫。
   >[!NOTE]
   >
   >選取 **部分搜尋** 核取方塊時，預設會選取 **忽略大小寫** 。

   ![](assets/wildcard-prop-1.png)

   搜尋結果會根據套用的篩選器以及搜尋結果計數來顯示。

   ![](assets/omnisearch-with-filters.png)

   具有搜尋結果計數的資產搜尋結果

3. 您可以輕鬆從搜尋結果導覽至項目，然後使用瀏覽器中的上一頁按鈕返回相同的搜尋結果，而不需要重新執行搜尋查詢。

## 將搜尋儲存為智慧型集合 {#save-your-searches-as-smart-collection}

您可以將搜尋設定儲存為智慧型集合，以便快速重復相同的搜尋，而不必稍後重做相同的設定。

若要將搜尋設定儲存為智慧型集合：

1. 點選/按一下 **「儲存Smart Collection** 」，並提供智慧型系列的名稱。

   若要讓所有使用者存取智慧型系列，請選取 **「公用**」。會顯示一則訊息，確認智慧型系列已建立並新增至您儲存的搜尋清單中。

   >[!NOTE]
   >
   >非管理員使用者可能會受到限制，無法將智慧 [!UICONTROL 型集合] 設為公開，以避免非管理員使用者在組織中建立大量的公開智慧 [!UICONTROL 集合][!DNL Brand Portal]。組織可以停用「一般 **設定」中提供的「一般」設定中提供的公用智慧[!UICONTROL 型系列]建立****** 設定。

   ![](assets/save_smartcollectionui.png)

1. 若要儲存不同名稱的智慧型系列，並選取或清除 **「公用** 」核取方塊，請按一下 **「編輯智慧型集合**」。

   ![](assets/edit_smartcollection.png)

1. 在 **「編輯智慧型系列」** 對話方塊中，選取 **「另** 存新檔」並輸入智慧型集合的名稱。按一下&#x200B;**「儲存」**。

   ![](assets/saveas_smartsearch.png)
