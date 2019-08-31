---
title: 將預設集、架構和Facet發佈至品牌入口網站
seo-title: 將預設集、架構和Facet發佈至品牌入口網站
description: 瞭解如何將預設集、架構和Facet發佈至品牌入口網站。
seo-description: 瞭解如何將預設集、架構和Facet發佈至品牌入口網站。
uuid: c836d9bb-074a-4113-9c91-b2 ff7658 b88 d
topic-tags: 發佈
products: SG_ PERIENCENCENAGER/Brand_ Portal
content-type: 引用
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 將預設集、架構和Facet發佈至品牌入口網站 {#publish-presets-schema-and-facets-to-brand-portal}

文章可讓您將AEM作者實例的影像預設集、中繼資料結構和自訂搜尋Facet發佈至品牌入口網站。發佈功能可讓組織重復使用影像預設集、中繼資料結構，以及在AEM作者實例中建立/修改的搜尋Facet，進而減少重復作業。

>[!NOTE]
>
>將影像預設集、中繼資料結構和搜尋Facet從AEM作者實例發佈到品牌入口網站的功能是AEM6.2SP1-CFP和AEM6.3 SP1-CFP(6.3.1.1) on wards。

## 將影像預設集發佈至品牌入口網站 {#publish-image-presets-to-brand-portal}

影像預設集是影像傳送時套用至影像的大小和格式指令集。您可以在Brand Portal建立和修改影像預設集。或者，如果AEM作者實例以動態媒體模式執行，則使用者可以在AEM Author中建立預設集並將其發佈至AEM Assets品牌入口網站，並避免在品牌入口網站上重新建立相同預設集。\
建立預設集後，就會在資產詳細資料轉譯邊欄和下載對話方塊上列為動態轉譯。

>[!NOTE]
>
>如果AEM作者實例未在 [!UICONTROL 動態媒體模式] 中執行(客戶尚未購買動態媒體)，則不會在上傳時建立資產 [!UICONTROL 的Bundrid TIFF] 轉譯。影像預設集或動態轉譯可在 [!UICONTROL 資產的Mercurid TIFF] 上運作，因此如果  AEM作者實例無法使用，則品牌入口網站也無法使用。因此，資產詳細資料頁面的轉譯邊欄並不會出現動態轉譯，並且會下載對話方塊。

若要將影像預設集發佈至品牌入口網站：

1. 在AEM作者實例中，點選/按一下AEM logo即可存取全域導覽主控台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產]** &gt; **[!UICONTROL 影像預設集]**」。
2. 從影像預設集清單中選取影像預設集或多個影像預設集，然後按一下/點選 **[!UICONTROL 「發佈至品牌入口網站]**」。

![](assets/publishpreset.png)

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL 「發佈至品牌入口網站]** 」時，影像預設集會佇列等候發佈。建議使用者監控複製代理程式的記錄，確認發佈是否成功。

若要從品牌入口網站取消發佈影像預設集：

1. 在AEM作者實例中，點選/按一下AEM logo即可存取全域導覽主控台，並點選/按一下 **[!UICONTROL 「工具]** 」圖示並導覽至 **[!UICONTROL 「資產&gt;影像預設集]**」。
2. 選取影像預設集，然後從頂端可用的選項中選取 **[!UICONTROL 「從品牌入口網站]** 移除」。

## 將中繼資料結構發佈至品牌入口網站 {#publish-metadata-schema-to-brand-portal}

中繼資料結構描述資產/系列屬性頁面上顯示的版面和屬性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果使用者已編輯AEM作者實例上的預設結構，而且想要使用與品牌入口網站上的預設結構相同的結構，則可以直接將中繼資料結構表單發佈至品牌入口網站。在這種情況下，品牌入口網站的預設結構會以從AEM作者實例發佈的預設結構碼覆寫。

如果使用者已在AEM作者實例上建立自訂結構，則可將自訂結構發佈至品牌入口網站，而無需在該處重新建立相同的自訂結構。然後，使用者可以將此自訂結構套用至品牌入口網站中的任何資料夾/系列。

>[!NOTE]
>
>如果已鎖定在AEM實例(未編輯)，則無法將預設結構發佈至品牌入口網站。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果資料夾已套用在AEM作者實例上，則品牌入口網站上也必須有相同的結構，才能維持AEM作者和品牌入口網站上資產屬性頁面的一致性。

若要將中繼資料結構從AEM作者實例發佈至品牌入口網站：

1. 在AEM作者實例中，點選/按一下AEM logo即可存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產&gt;中繼資料結構」]**。
2. 選取中繼資料結構，然後從上方可用選項選擇 **[!UICONTROL 「發佈至品牌入口網站]** 」。

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL 「發佈至品牌入口網站]**」時，中繼資料結構將會佇列等候發佈。建議使用者監控複製代理程式的記錄，確認發佈是否成功。

若要從品牌入口網站取消發佈中繼資料結構：

1. 在AEM作者實例中，點選/按一下AEM logo即可存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產&gt;中繼資料結構」]**。
2. 選取中繼資料結構，然後從上方可用選項中選取 **[!UICONTROL 「從品牌入口網站]** 移除」。

## 將搜尋Facet發佈至品牌入口網站 {#publish-search-facets-to-brand-portal}

搜尋表單可為品牌入口網站上的使用者提供 [Facet搜尋](../using/brand-portal-search-facets.md) 功能。搜尋Facet會更精細地呈現品牌入口網站上的搜尋。在搜尋 [表單中新增](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) 的所有預測都可供使用者使用，作為搜尋篩選器中的搜尋Facet。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您願意從AEM作者實例使用自訂搜尋表單 **[!UICONTROL 資產管理搜尋邊欄]** ，則無需在品牌入口網站上重新建立相同的表格，您可以將自訂的搜尋表單從AEM作者實例發佈至品牌入口網站。

>[!NOTE]
>
>鎖定搜尋表單 **[!UICONTROL 資產管理員搜尋邊欄]** 在AEM資產上無法發佈至品牌入口網站，除非已編輯。編輯並發佈至品牌入口網站後，此搜尋表單會覆寫品牌入口網站上的搜尋表格。

若要將編輯的搜尋Facet從AEM作者實例發佈至品牌入口網站：

1. 點選/按一下AEM標誌，然後前往 **[!UICONTROL 「工具]** &gt; **[!UICONTROL 一般]** &gt; **[!UICONTROL 搜尋表單]**」。
2. 選取編輯的搜尋表單，然後選取 **[!UICONTROL 「發佈至品牌入口網站]**」。

   >[!NOTE]
   >
   >當使用者按一下 **[!UICONTROL 「發佈至品牌入口網站]**」時，搜尋Facet會佇列等候發佈。建議使用者監控複製代理程式的記錄，確認發佈是否成功。

若要從品牌入口網站取消發佈搜尋表格：

1. 在AEM作者實例中，點選/按一下AEM logo即可存取全域導覽主控台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「一般&gt;搜尋表單]**」。
2. 選取搜尋表單，然後從上方可用選項中選擇 **[!UICONTROL 「從品牌入口網站]** 移除」。

>[!NOTE]
>
>「從品牌入口網站 **[!UICONTROL 取消發佈」]** 動作會在品牌入口網站上保留預設搜尋表單，且不會還原至發佈前所使用的最後一個搜尋表單。

### 限制 {#limitations}

1. 很少有搜尋預測詞適用於品牌入口網站上的搜尋篩選器。當這些搜尋Predicates是從AEM作者實例發佈至「品牌入口網站」時，將會被過濾掉。因此，使用者在「品牌入口網站」的發佈表格中，看到的預覽詞數目較少。請參閱 [適用於品牌入口網站篩選條件的搜尋預測](../using/brand-portal-search-facets.md#list-of-search-predicates)。

2. 對於 [!UICONTROL 「選項Predicate」]，如果使用者使用任何自訂路徑來讀取AEM作者實例的選項，則無法在品牌入口網站上運作。這些額外路徑和選項不會使用搜尋表單發佈至品牌入口網站。在這種情況下，使用者可以選取「選項Predicate」中「新增選項」中的「 **[!UICONTROL 手動]********[!UICONTROL 」選項，]** 以手動方式在品牌入口網站中新增這些選項。

![](assets/options-predicate-manual.png)
