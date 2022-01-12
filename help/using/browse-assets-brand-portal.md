---
title: 在Brand Portal上瀏覽資產
seo-title: Browse assets on Brand Portal
description: 在Brand Portal上使用不同的檢視選項和UI元素，瀏覽資產、周遊資產階層和搜尋資產。
seo-description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
exl-id: 405d7861-a140-44b1-ae1f-4f0839f05033
source-git-commit: 3abf39161febc536f431206c2f098e7d61a10846
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 2%

---

# 在Brand Portal上瀏覽資產 {#browsing-assets-on-brand-portal}

Experience Manager Assets Brand Portal提供多種功能和使用者介面元素，可方便您瀏覽資源、遍歷資產階層，以及在使用不同檢視選項時搜尋資產。

頂端工具列中的Experience Manager標誌可方便管理員使用者存取管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal左上角的邊欄選取器下拉式清單，顯示可導覽至資產階層、簡化搜尋及顯示資源的選項。

![](assets/siderail-1.png)

您可以使用Brand Portal右上角的檢視選取器中的任何可用檢視（卡片、欄和清單）來檢視、導覽及選取資產。

![](assets/viewselector.png)

## 檢視及選取資源 {#viewing-and-selecting-resources}

檢視、導覽和選取每個檢視在概念上在所有檢視中都相同，但處理方式有小的變化，視您使用的檢視而定。

您可以使用任何可用檢視來檢視、導覽及選取（以執行進一步動作）您的資源：

* 欄檢視
* 卡片檢視
* 清單檢視

### 卡片檢視

![](assets/card-view.png)

卡片視圖顯示當前級別上每個項目的資訊卡。 這些卡片提供下列詳細資料：

* 資產/資料夾的視覺表示法。
* 類型
* 標題
* 名稱
* 從AEM發佈資產至Brand Portal的日期和時間
* 大小
* 尺寸

您可以點選/按一下資訊卡（注意避免快速動作），向下導覽階層，或使用 [標題中的階層連結](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html).

![](assets/cardquickactions.png)

#### 非管理員使用者的卡片檢視

資料夾卡片在「卡片檢視」中，會向非管理員使用者（編輯者、檢視者和訪客使用者）顯示資料夾階層資訊。 此功能可讓使用者了解資料夾的位置，以及他們正在存取的父階層。
資料夾階層資訊對於區分名稱類似於從不同資料夾階層共用之其他資料夾的資料夾特別有用。 如果非管理員使用者不知道與他們共用之資產的資料夾結構，則名稱類似的資產/資料夾似乎會令人困惑。

* 個別卡片上顯示的路徑會遭截斷以符合卡片大小。 不過，使用者可將完整路徑視為將游標暫留在截斷路徑上的工具提示。

![](assets/folder-hierarchy1.png)

**檢視資產屬性的概觀選項**

非管理員使用者（編輯者、檢視者、訪客使用者）可使用概述選項來檢視所選資產/資料夾的資產屬性。 「概述」選項會顯示：

* 在頂端的工具列中選取資產/資料夾。
* 在下拉式清單中選取邊欄選取器。

選取 **[!UICONTROL 概述]** 選項，使用者可以查看資產建立的標題、路徑和時間。 然而，在資產詳細資料頁面上選取「概述」選項，可讓使用者查看資產的中繼資料。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 在卡片檢視中檢視設定

**[!UICONTROL 檢視設定]** 對話框開啟，選擇 **[!UICONTROL 檢視設定]** 從檢視選取器。 它可讓您調整「卡片」檢視中的資產縮圖大小。 這樣，您就可以個人化您的檢視，並控制顯示的縮圖數目。

![](assets/cardviewsettings.png)

### 清單檢視

![](assets/list-view.png)

清單視圖顯示當前級別上每個資源的資訊。 清單檢視提供下列詳細資訊：

* 資產的縮圖影像
* 名稱
* 標題
* 地區設定
* 類型
* Dimension
* 大小
* 評等
* 顯示資產階層的資料夾路徑
* 在Brand Portal上發佈資產的日期

路徑欄可讓您輕鬆識別資料夾階層中的資產位置。 您可以點選/按一下資源名稱，以向下導覽階層，並使用 [標題中的階層連結](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在清單檢視中檢視設定

清單檢視顯示資產 **[!UICONTROL 名稱]** 預設為第一欄。 其他資訊，例如資產 **[!UICONTROL 標題]**, **[!UICONTROL 地區]**, **[!UICONTROL 類型]**, **[!UICONTROL Dimension]**, **[!UICONTROL 大小]**, **[!UICONTROL 評等]**，也會顯示發佈狀態。 不過，您可以選取要顯示的欄，使用 **[!UICONTROL 檢視設定]**.

![](assets/list-view-setting.png)

### 欄檢視

![](assets/column-view.png)

使用列視圖可在一系列級聯列中導航內容樹。 此檢視可協助您視覺化及周遊資產階層。

在第一欄（最左邊）中選取資源時，右側第二欄會顯示子資源。 在第二欄中選取資源會在第三欄中的右側顯示子資源，以此類推。

您可以點選或按一下資源名稱或資源名稱右側的>形，以在樹狀結構中上下導覽。

* 點選或按一下時，資源名稱和>形箭號會強調顯示。
* 點選或按一下縮圖會選取資源。
* 選中後，複選標籤覆蓋在縮略圖上，並加亮資源名稱。
* 所選資源的詳細資訊會顯示在最終欄中。

在欄檢視中選取資產時，資產的視覺表示會顯示在最終欄中，並有下列詳細資料：

* 標題
* 名稱
* 尺寸
* 從AEM發佈資產至Brand Portal的日期和時間
* 大小
* 類型
* 「更多詳情」選項，前往資產的詳細資訊頁面

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

Deselecting All
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## 內容樹 {#content-tree}

除了這些檢視外，在您檢視並選取所需資產或資料夾時，使用樹狀檢視來下鑽資產階層。

若要開啟樹狀檢視，請點選/按一下左上方的邊欄選取器，然後選取 **[!UICONTROL 內容樹]** 的上界。

![](assets/contenttree.png)

從內容階層導覽至所需的資產。

![](assets/content-tree.png)

## 資產詳細內容 {#asset-details}

資產詳細資料頁面可讓您檢視資產、下載、共用資產的連結、將其移至集合，或檢視其屬性頁面。 它也可讓您連續導覽相同資料夾中其他資產的詳細資訊頁面。

![](assets/asset-detail.png)

若要檢視資產的中繼資料，或檢視其各種轉譯，請使用資產詳細資料頁面上的邊欄選取器。

![](assets/asset-overview.png)

您可以在資產詳細資訊頁面上檢視資產的所有可用轉譯，並從 **[!UICONTROL 轉譯]** 面板來預覽。

![](assets/renditions.png)

>[!CAUTION]
>
>(**Experience Manager Assetsas a Cloud Service** 僅限)下列已知問題將在即將發行的版本中修正：
>
>此 **[!UICONTROL 轉譯]** 面板不會列出2021年12月16日後發佈至Brand Portal之資產的所有靜態轉譯。
>
>此 **[!UICONTROL 轉譯]** 面板會列出資產的智慧型裁切轉譯，但使用者無法預覽或下載智慧型裁切轉譯。

若要開啟資產屬性頁面，請使用 **[!UICONTROL 屬性(p)]** 的上界。

![](assets/asset-properties.png)

您也可以在資產屬性頁面上檢視其所有相關資產(AEM上的來源或衍生資產)的清單，因為資產關係也會從AEM發佈至Brand Portal。
