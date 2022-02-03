---
title: 瀏覽Brand Portal上的資產
seo-title: Browse assets on Brand Portal
description: 使用Brand Portal上的不同視圖選項和UI元素瀏覽資產、遍歷資產層次結構和搜索資產。
seo-description: Browse through assets, traverse asset hierarchies, and search assets, using different view options and UI elements on Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
exl-id: 405d7861-a140-44b1-ae1f-4f0839f05033
source-git-commit: a219adc020d63897b10dca83d9ce31fd3ebf847c
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 3%

---

# 瀏覽Brand Portal上的資產 {#browsing-assets-on-brand-portal}

Experience Manager AssetsBrand Portal提供各種功能和用戶介面元素，方便瀏覽資源、遍歷資產層次結構以及使用不同視圖選項搜索資產。

頂部工具欄中的Experience Manager徽標方便管理員用戶訪問管理工具面板。

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)

Brand Portal左上角的鐵路選擇器向下下拉，以顯示導航到資產層次結構、簡化搜索和顯示資源的選項。

![](assets/siderail-1.png)

您可以使用Brand Portal右上角的視圖選擇器中的任何可用視圖（卡、列和清單）查看、瀏覽和選擇資產。

![](assets/viewselector.png)

## 查看和選擇資源 {#viewing-and-selecting-resources}

查看、導航和選擇每個視圖在概念上在所有視圖上都相同，但在處理方面有小的變化，具體取決於您使用的視圖。

您可以使用以下任何可用視圖查看、瀏覽和選擇資源（以執行進一步操作）:

* 欄檢視
* 卡片檢視
* 清單檢視

### 卡片檢視

![](assets/card-view.png)

「卡」視圖顯示當前層每個物料的資訊卡。 這些卡提供以下詳細資訊：

* 資產/資料夾的可視表示。
* 類型
* 標題
* 名稱
* 資產從Brand Portal發佈的日期和時AEM間
* 大小
* 尺寸

您可以點擊/按一下卡（注意避免快速操作），或使用 [標題中的麵包屑](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html)。

![](assets/cardquickactions.png)

#### 非管理員用戶的卡視圖

資料夾卡在「卡視圖」中向非管理員用戶（編輯器、查看器和來賓用戶）顯示資料夾層次結構資訊。 此功能使用戶能夠瞭解資料夾的位置，以及他們訪問的與父層次結構相關的資料夾。
資料夾層次結構資訊對於區分具有與從不同資料夾層次結構共用的其他資料夾相似名稱的資料夾特別有用。 如果非管理員用戶不知道與他們共用的資產的資料夾結構，則名稱相似的資產/資料夾似乎令人困惑。

* 截斷各個卡上顯示的路徑以適合卡大小。 但是，用戶可以將完整路徑視為懸停在截斷路徑上的工具尖。

![](assets/folder-hierarchy1.png)

**查看資產屬性的概覽選項**

非管理員用戶（編輯器、查看器、來賓用戶）可使用「概述」選項查看選定資產/資料夾的資產屬性。 「概述」(Overview)選項可見：

* 的上界。
* 中。

選擇 **[!UICONTROL 概述]** 選項，則用戶可以查看資產建立的標題、路徑和時間。 但是，在資產詳細資訊頁面上，選擇「概覽」選項允許用戶查看資產的元資料。

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### 查看卡視圖中的設定

**[!UICONTROL 查看設定]** 對話框開啟，選擇 **[!UICONTROL 查看設定]** 的下界。 它使您能夠在「卡」視圖中調整資產縮略圖的大小。 這樣，您可以個性化視圖並控制顯示的縮略圖數。

![](assets/cardviewsettings.png)

### 清單檢視

![](assets/list-view.png)

清單視圖顯示當前層中每個資源的資訊。 「清單」視圖提供以下詳細資訊：

* 資產縮略圖
* 名稱
* 標題
* 地區設定
* 類型
* Dimension
* 大小
* 評等
* 顯示資產層次結構的資料夾路徑
* 在Brand Portal發佈資產的日期

「路徑」(Path)列使您可以輕鬆地標識資料夾層次結構中的資產位置。 您可以按一下/按一下資源名稱向下瀏覽層次結構，然後使用 [標題中的麵包屑](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/essentials/basic-handling.html)。

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### 在清單視圖中查看設定

清單視圖顯示資產 **[!UICONTROL 名稱]** 作為第一列。 其他資訊，如資產 **[!UICONTROL 標題]**。 **[!UICONTROL 區域設定]**。 **[!UICONTROL 類型]**。 **[!UICONTROL Dimension]**。 **[!UICONTROL 大小]**。 **[!UICONTROL 評級]**，也顯示發佈狀態。 但是，您可以使用 **[!UICONTROL 查看設定]**。

![](assets/list-view-setting.png)

### 欄檢視

![](assets/column-view.png)

使用列視圖可在一系列級聯列中導航內容樹。 此視圖可幫助您可視化和遍歷資產層次結構。

在第一列（最左側）中選擇資源時，在右側的第二列中顯示子資源。 在第二列中選擇資源時，會在右側的第三列中顯示子資源，依此類推。

通過點擊或按一下資源名稱或資源名稱右側的字形，可以在樹中上下導航。

* 點擊或按一下時，資源名稱和字元會加亮顯示。
* 點擊或按一下縮覽圖可選擇資源。
* 選中後，複選標籤將疊加在縮略圖上，並加亮資源名稱。
* 選定資源的詳細資訊顯示在最終列中。

在列視圖中選擇資產時，資產的可視表示將與以下詳細資訊一起顯示在最終列中：

* 標題
* 名稱
* 尺寸
* 資產從Brand Portal發佈的日期和時AEM間
* 大小
* 類型
* 「更多詳細資訊」選項，轉到資產的詳細資訊頁面

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

除了這些視圖外，在查看和選擇所需資產或資料夾時，使用樹視圖可細化資產層次結構。

要開啟樹視圖，請點擊/按一下左上方的滑軌選擇器，然後選擇 **[!UICONTROL 內容樹]** 的子菜單。

![](assets/contenttree.png)

從內容層次結構中，導航到所需的資產。

![](assets/content-tree.png)

## 資產詳細內容 {#asset-details}

資產詳細資訊頁面允許您查看資產、下載、共用資產連結、將其移動到集合或查看其屬性頁面。 它還允許您連續瀏覽同一資料夾的其他資產的詳細資訊頁面。

![](assets/asset-detail.png)

要查看資產的元資料或查看其各種格式副本，請使用資產詳細資訊頁面上的導軌選擇器。

![](assets/asset-overview.png)

您可以在資產詳細資訊頁面上查看資產的所有可用格式副本，然後從 **[!UICONTROL 格式副本]** 按鈕。

![](assets/renditions.png)

<!-- removed as it is fixed in 2022.02.0 release
>[!CAUTION]
>
>(**Experience Manager Assets as a Cloud Service** only) The following known issues will be fixed in the upcoming release:
>
>The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal after December 16, 2021.
>
>The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
-->

要開啟資產屬性頁，請使用 **[!UICONTROL 屬性(p)]** 的上界。

![](assets/asset-properties.png)

您還可以在資產的屬性頁面上查看其所有相關資產(源AEM或派生資產)的清單，因為資產關係也會從發佈到AEMBrand Portal。
