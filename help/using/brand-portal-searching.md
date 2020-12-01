---
title: 在 Brand Portal 上搜尋資產
seo-title: AEM品牌入口網站上的資產搜尋和儲存的搜尋
description: 品牌入口網站搜尋功能可讓您使用搜尋功能快速搜尋相關資產，而搜尋篩選器可協助您進一步縮小搜尋範圍。 將搜尋儲存為智慧型系列，以備日後使用。
seo-description: 品牌入口網站搜尋功能可讓您使用搜尋功能快速搜尋相關資產，而搜尋篩選器可協助您進一步縮小搜尋範圍。 將搜尋儲存為智慧型系列，以備日後使用。
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1163'
ht-degree: 5%

---


# 在 Brand Portal 上搜尋資產 {#search-assets-on-brand-portal}

品牌入口網站搜尋功能可讓您使用搜尋功能快速搜尋相關資產，而Facet搜尋則使用篩選器協助您進一步縮小搜尋範圍。 您也可以將搜尋儲存為智慧型系列，以供日後使用。

## 使用Omnisearch {#search-assets-using-omnisearch}搜尋資產

若要在品牌入口網站上搜尋資產：

1. 在工具列中，按一下&#x200B;**[!UICONTROL Search]**&#x200B;圖示，或按&quot;**[!UICONTROL /]**&quot;鍵以啟動Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜尋方塊中，輸入您要搜尋之資產的關鍵字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Omnisearch至少需要3個字元，才能顯示搜尋建議。

1. 從下拉式清單中顯示的相關建議中選取，以快速存取相關資產。

   ![](assets/assets-search-result.png)

   *使用Omnisearch進行資產搜尋*

若要瞭解智慧型標籤資產的搜尋行為，請參閱[瞭解搜尋結果和行為](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)。

## 在「篩選器」面板{#search-using-facets-in-filters-panel}中使用Facet進行搜尋

「篩選」面板中的搜尋Facet可為您的搜尋體驗增加精細度，並讓搜尋功能更有效率。 搜尋刻面使用多個維度（謂語），可讓您執行複雜的搜尋。 您可以輕鬆深入瞭解所需的詳細程度，以便進行更專注的搜尋。

例如，如果您要尋找影像，可以選擇要點陣圖還是向量影像。 您可以在「檔案類型」搜尋Facet中指定影像的MIME類型，進一步縮小搜尋範圍。 同樣地，在搜索文檔時，可以指定格式，例如PDF或MS Word格式。<br />

![品牌入口網站中的「篩](assets/file-type-search.png "選器」面板品牌入口網站中的「篩選器」面板")

**[!UICONTROL Filters]**&#x200B;面板包含一些標準刻面，例如- **[!UICONTROL 路徑瀏覽器]**、**[!UICONTROL 檔案類型]**、**[!UICONTROL 檔案大小]**、**[!UICONTROL Status]**&#x200B;和&#x200B;**[!UICONTROL Orientation&lt;a1/>。]**&#x200B;不過，您可以[新增自訂搜尋Facet](../using/brand-portal-search-facets.md)，或在基礎搜尋表單中新增或移除謂語，從&#x200B;**[!UICONTROL 篩選器]**&#x200B;面板移除特定搜尋Facet。 請參閱品牌入口網站](../using/brand-portal-search-facets.md#list-of-search-predicates)上可用和可用的[搜尋謂語清單。

若要將篩選器套用至您的搜尋，請使用可用的[搜尋Facets](../using/brand-portal-search-facets.md):

1. 按一下覆蓋圖示，然後選取&#x200B;**[!UICONTROL Filter]**。

   ![](assets/selectorrail.png)

1. 從左側的&#x200B;**[!UICONTROL Filters]**面板中，選擇適當的選項以套用相關的濾鏡。
例如，請使用下列標準篩選：

   * **[!UICONTROL 路徑瀏]** 覽器，以搜尋特定目錄中的資產。路徑瀏覽器的謂詞的預設搜索路徑為`/content/dam/mac/<tenant-id>/`，可通過編輯預設搜索表單來配置該路徑。
   >[!NOTE]
   >
   >對於非管理員用戶，[!UICONTROL Filter]面板中的[!UICONTROL 路徑瀏覽器]僅顯示與其共用的資料夾（及其祖先資料夾）的內容結構。\
   >對於管理員使用者，路徑瀏覽器允許導覽至品牌入口網站中的任何資料夾。

   * **[!UICONTROL File]** Type，指定您要尋找的資產檔案的類型（影像、檔案、多媒體、封存）。此外，您還可以縮小搜尋範圍，例如，為檔案指定影像或格式（PDF或MS Word）的MIME類型(Tiff、Bitmap、GIMP Images)。
   * **[!UICONTROL File]** Size以根據資產大小來搜尋資產。您可以指定大小範圍的下限和上限，以縮小搜尋範圍並指定要搜尋的單位。
   * **[!UICONTROL 狀]** 態：依據資產狀態搜尋資產，例如核准（已核准、已請求變更、已拒絕、待定）和到期。
   * **[!UICONTROL 「平]** 均評分」，以根據資產的評分來搜尋資產。
   * **[!UICONTROL 方]** 向：根據資產的方向（水準、垂直、正方形）搜尋資產。
   * **[!UICONTROL Style]** 可根據資產的樣式（彩色、單色）來搜尋資產。
   * **[!UICONTROL 視訊]** 格式，以根據其格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)來搜尋視訊資產。

   您可以編輯基礎的搜尋表單，在「篩選」面板中使用[自訂搜尋Facet](../using/brand-portal-search-facets.md)。

   * **[!UICONTROL Property]** Predicateif（在搜尋表單中使用）可讓您搜尋符合中繼資料屬性的資產，此屬性是述詞所對應的。\
      例如，如果Property Predicate已映射至[!UICONTROL `jcr:content /metadata/dc:title`]，您可以根據資產的標題來搜尋資產。\
      [!UICONTROL Property Predicate]支援下列文字搜尋：

      **部分詞組**
若要允許以屬性述詞中的部分詞組搜尋資產，請啓用「搜尋表單」中的**[!UICONTROL 「部分搜尋」]**&#x200B;核取方塊。\
      如此一來，便可讓您搜尋所需資產，即使您未指定資產中繼資料裡所使用的確切單字/詞組。\
      您可以：
      * 在「篩選」面板的Facet中，指定在搜尋的片語中發生的字詞。 例如，如果您搜尋詞&#x200B;**climb**（而「屬性謂語」已映射至[!UICONTROL `dc:title`]屬性），則會傳回其標題片語中含有&#x200B;**climb**&#x200B;字詞的所有資產。
      * 指定字詞的一部分（發生在您搜尋的片語中），以及萬用字元(*)以填補空白。
例如，搜尋：
         * **climb*傳** 回所有具有字詞的資產，字詞開頭為標題字句中的字元「climb」。
         * ***** camben傳回所有資產的標題片語中，字詞結尾為「climb」。
         * ***climb*傳** 回所有包含字元「climb」的資產，其標題片語皆為字元。

若要允許屬性謂語中的非區分大小寫搜尋，請啟用       **非區分大小寫的**
文字若要允許屬性謂語中的非區分大小寫搜尋，請在搜尋表單中啟 **[!UICONTROL 用]** Ignore Casecheckbox。預設情況下，對屬性謂語的文本搜索區分大小寫。
   >[!NOTE]
   >
   >在選中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;複選框時，預設選擇&#x200B;**[!UICONTROL 忽略大小寫]**。

   ![](assets/wildcard-prop-1.png)

   搜尋結果會根據套用的篩選條件以及搜尋結果計數來顯示。

   ![](assets/omnisearch-with-filters.png)

   具有搜尋結果計數的資產搜尋結果。

1. 您可以輕鬆從搜尋結果導覽至項目，並使用瀏覽器中的上一頁按鈕返回相同的搜尋結果，而不需重新執行搜尋查詢。

## 將搜尋儲存為智慧型系列{#save-your-searches-as-smart-collection}

您可以將搜尋設定儲存為智慧型系列，以便快速重複相同的搜尋，而不需稍後重做相同的設定。

要將搜索設定保存為智慧系列，請執行以下操作：

1. 點選／按一下&#x200B;**[!UICONTROL 「儲存智慧型系列」]**，並提供智慧型系列的名稱。

   若要讓所有使用者都能存取智慧型系列，請選取&#x200B;**[!UICONTROL Public]**。 訊息會確認智慧型系列已建立並新增至儲存的搜尋清單。

   >[!NOTE]
   >
   >非管理員使用者可能無法公開智慧型系列，以避免組織品牌入口網站上有大量非管理員使用者建立的公開智慧型系列。 組織可以從「管理工具」面板中的「一般」設定停用「允許建立公用智慧型系列」的&#x200B;**[!UICONTROL 設定。]******

   ![](assets/save_smartcollectionui.png)

1. 要以不同的名稱保存智慧系列，並選中或清除&#x200B;**[!UICONTROL Public]**&#x200B;複選框，請按一下&#x200B;**[!UICONTROL 編輯智慧系列]**。

   ![](assets/edit_smartcollection.png)

1. 在&#x200B;**[!UICONTROL 編輯智慧型系列]**&#x200B;對話方塊中，選擇&#x200B;**[!UICONTROL 另存新檔]**&#x200B;並輸入智慧型系列的名稱。 按一下&#x200B;**[!UICONTROL 「儲存」]**。

   ![](assets/saveas_smartsearch.png)
