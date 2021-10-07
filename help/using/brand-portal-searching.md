---
title: 在 Brand Portal 上搜尋資產
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Brand Portal搜尋功能可讓您使用omnisearch快速搜尋相關資產，而搜尋篩選器可協助您進一步縮小搜尋範圍。 將搜尋儲存為智慧型集合，以供日後使用。
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1124'
ht-degree: 5%

---

# 在 Brand Portal 上搜尋資產 {#search-assets-on-brand-portal}

Brand Portal搜尋功能可讓您使用omnisearch和facet搜尋來快速搜尋相關資產，這些搜尋使用篩選器來協助您進一步縮小搜尋範圍。 您也可以將搜尋儲存為未來的智慧型集合。

## 使用Omnisearch搜尋資產 {#search-assets-using-omnisearch}

若要在Brand Portal上搜尋資產：

1. 在工具列中，按一下&#x200B;**[!UICONTROL Search]**&#x200B;圖示，或按「**[!UICONTROL /]**」鍵以啟動Omnisearch。

   ![](assets/omnisearchicon-1.png)

1. 在搜尋方塊中，輸入您要搜尋資產的關鍵字。

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Omnisearch中至少需要3個字元，才能顯示搜尋建議。

1. 從下拉式清單中顯示的相關建議中選取，以快速存取相關資產。

   ![](assets/assets-search-result.png)

   *使用Omnisearch搜尋資產*

若要了解智慧標籤資產的搜尋行為，請參閱[了解搜尋結果和行為](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html)。

## 在「篩選器」面板中使用Facet進行搜尋 {#search-using-facets-in-filters-panel}

在「篩選器」面板中搜尋Facet可為您的搜尋體驗增加粒度，並讓搜尋功能更有效率。 搜尋Facet使用多個維度（述詞），可讓您執行複雜的搜尋。 您可以輕鬆深入到所需的詳細程度，以便進行更集中的搜尋。

例如，如果要查找影像，則可以選擇要點陣圖還是向量影像。 您可以在「檔案類型」搜尋刻面中指定影像的MIME類型，進一步縮小搜尋範圍。 同樣，在搜索文檔時，可以指定格式，例如PDF或MS Word格式。

![Brand Portal中的「篩選」面](assets/file-type-search.png "板Brand Portal中的「篩選」面板")

**[!UICONTROL 「篩選器」]**&#x200B;面板包含一些標準面，例如 — **[!UICONTROL 路徑瀏覽器]**、**[!UICONTROL 檔案類型]**、**[!UICONTROL 檔案大小]**、**[!UICONTROL 狀態]**&#x200B;和&#x200B;**[!UICONTROL 方向]**。 不過，您可以[新增自訂搜尋Facet](../using/brand-portal-search-facets.md)，或透過在基礎搜尋表單中新增或移除謂語，從&#x200B;**[!UICONTROL 篩選器]**&#x200B;面板中移除特定搜尋Facet。 請參閱Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates)上可用和可用的[搜尋述詞清單。

若要將篩選器套用至您的搜尋，請使用可用的[搜尋Facet](../using/brand-portal-search-facets.md):

1. 按一下覆蓋圖示並選取&#x200B;**[!UICONTROL Filter]**。

   ![](assets/selectorrail.png)

1. 從左側的&#x200B;**[!UICONTROL 篩選器]**面板中，選取適當的選項以套用相關篩選器。
例如，使用下列標準篩選器：

   * **[!UICONTROL 路徑]** 瀏覽器以搜尋特定目錄中的資產。路徑瀏覽器的謂語的預設搜索路徑為`/content/dam/mac/<tenant-id>/`，可通過編輯預設搜索表單來配置。
   >[!NOTE]
   >
   >對於非管理員用戶，[!UICONTROL Filter]面板中的[!UICONTROL 路徑瀏覽器]只顯示與其共用的資料夾（及其上階資料夾）的內容結構。\
   >若為管理員使用者，路徑瀏覽器可讓您導覽至Brand Portal中的任何資料夾。

   * **[!UICONTROL 檔]** 案類型，指定您要尋找的資產檔案的類型（影像、檔案、多媒體、封存）。此外，您還可以縮小搜索範圍，例如，指定MIME類型（Tiff、點陣圖、GIMP影像）以用於影像或格式(PDF或MS Word)。
   * **[!UICONTROL 檔]** 案大小：根據資產大小搜尋資產。您可以指定大小範圍的下限和上限以縮小搜尋範圍，並指定要搜尋的單位。
   * **** 狀態：根據資產狀態搜索資產，例如「批准」(Approved)、「請求更改」(Requested)、「拒絕」(Rejected)、「待定」(Pending)和「到期」(Expiration)。
   * **[!UICONTROL 平]** 均評分以根據資產評等來搜尋資產。
   * **** 方向：根據資產的方向（水準、垂直、平方）來搜尋資產。
   * **** 樣式：根據資產的樣式（彩色、單色）來搜尋資產。
   * **[!UICONTROL 視]** 頻格式，根據其格式(DVI、Flash、MPEG4、MPEG、OGG Theora、QuickTime、Windows Media、WebM)搜索視頻資產。

   您可以編輯基礎的「搜尋表單」，在「篩選器」面板中使用[自訂搜尋Facet](../using/brand-portal-search-facets.md)。

   * **[!UICONTROL 屬]** 性述詞（如果用於搜尋表單中）可讓您搜尋符合述詞所對應之中繼資料屬性的資產。\
      例如，如果「屬性述詞」對應至[!UICONTROL `jcr:content /metadata/dc:title`]，您可以根據資產的標題來搜尋資產。\
      [!UICONTROL 屬性述詞]支援下列項目的文字搜尋：

      **部分詞組**
若要允許以屬性述詞中的部分詞組搜尋資產，請啓用「搜尋表單」中的**[!UICONTROL 「部分搜尋」]**&#x200B;核取方塊。\
      如此一來，便可讓您搜尋所需資產，即使您未指定資產中繼資料裡所使用的確切單字/詞組。\
      您可以：
      * 在「篩選器」面板的Facet中，指定搜尋片語中出現的字詞。 例如，如果您搜尋詞&#x200B;**climb**（且「屬性述詞」對應至[!UICONTROL `dc:title`]屬性），則會傳回其標題片語中包含字詞&#x200B;**climb**&#x200B;的所有資產。
      * 指定搜尋片語中單字的一部分，連同萬用字元(*)填滿空隙。
例如，搜尋：
         * **climb*** 會傳回所有字詞開頭為標題片語中「climb」字元的資產。
         * ***** camber會傳回標題片語中字元結尾為「climb」的所有資產。
         * ***climb*** 會傳回標題片語中包含「climb」字元的所有資產。

若要允許屬性述詞中不區分大小寫的搜尋，請啟用       **非區分大小寫文**
字若要允許屬性述詞中非區分大小寫的搜尋，請啟用「搜尋 **[!UICONTROL 表單]** 」中的「忽略Casecheckbox」。依預設，屬性述詞的文字搜尋會區分大小寫。
   >[!NOTE]
   >
   >選中&#x200B;**[!UICONTROL 部分搜索]**&#x200B;複選框時，預設選中&#x200B;**[!UICONTROL 忽略大小寫]**。

   ![](assets/wildcard-prop-1.png)

   搜尋結果會根據套用的篩選條件以及搜尋結果計數顯示。

   ![](assets/omnisearch-with-filters.png)

   具有搜尋結果計數的資產搜尋結果。

1. 您可以輕鬆地從搜索結果導航到項目，並使用瀏覽器中的返回按鈕返回到相同的搜索結果，而無需重新運行搜索查詢。

## 將搜尋儲存為智慧型系列 {#save-your-searches-as-smart-collection}

您可以將搜尋設定儲存為智慧型系列，以便快速重複相同的搜尋，而不需稍後重做相同的設定。

要將搜索設定另存為智慧系列，請執行以下操作：

1. 點選/按一下&#x200B;**[!UICONTROL 儲存智慧型集合]**&#x200B;並提供智慧型集合的名稱。

   若要讓所有使用者都能存取智慧型集合，請選取&#x200B;**[!UICONTROL Public]**。 訊息會確認智慧型系列已建立，並新增至已儲存搜尋的清單中。

   >[!NOTE]
   >
   >可限制非管理員使用者將智慧型集合設為公用，以避免組織之Brand Portal上非管理員使用者建立大量公用智慧型集合。 組織可以從「管理工具」面板中可用的&#x200B;**[!UICONTROL 「一般」]**&#x200B;設定停用「允許建立公用智慧型集合」]**設定」。**[!UICONTROL 

   ![](assets/save_smartcollectionui.png)

1. 若要以不同名稱儲存智慧型集合，並選取或清除&#x200B;**[!UICONTROL Public]**&#x200B;核取方塊，請按一下&#x200B;**[!UICONTROL Edit Smart Collection]**。

   ![](assets/edit_smartcollection.png)

1. 在&#x200B;**[!UICONTROL 編輯智慧集合]**&#x200B;對話框中，選擇&#x200B;**[!UICONTROL 另存為]**&#x200B;並輸入智慧集合的名稱。 按一下「**[!UICONTROL 儲存]**」。

   ![](assets/saveas_smartsearch.png)
