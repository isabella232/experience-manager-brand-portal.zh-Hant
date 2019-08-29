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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 將預設集、架構和Facet發佈至品牌入口網站 {#publish-presets-schema-and-facets-to-brand-portal}

文章會探討 [!DNL AEM] 從「作者」實例將影像預設集、中繼資料結構和自訂搜尋Facet發佈 [!DNL Brand Portal]到。發佈功能可讓組織重復使用影像預設集、中繼資料結構，以及 [!DNL AEM] 在作者實例中建立/修改的搜尋Facet，進而減少重復作業。

>[!NOTE]
>
>發佈影像預設集、中繼資料結構以及從 [!DNL AEM] 「作者」實例搜尋Facet的 [!DNL Brand Portal] 功能可供使用 [!DNL AEM 6.2 SP1-CFP7][!DNL AEM 6.3 SP 1-CFP 1 (6.3.1.1)] 。

## 將影像預設集發佈至品牌入口網站 {#publish-image-presets-to-brand-portal}

影像預設集是影像傳送時套用至影像的大小和格式指令集。您可以在下列位置建立和修改影像預設集 [!DNL Brand Portal]。或者 [!DNL AEM] ，如果作者實例以動態媒體模式執行，則使用者可以在 [!DNL AEM] 「作者」中建立預設集並將其發佈， [!DNL AEM Assets Brand Portal]並避免重新建立相同的預設集 [!DNL Brand Portal]。\
建立預設集後，就會在資產詳細資料轉譯邊欄和下載對話方塊上列為動態轉譯。

>[!NOTE]
>
>[!DNL AEM] 如果作者實例未在 [!DNL Dynamic Media] 模式中執行(客戶尚未購買) [!DNL Dynamic Media]，則不會在上傳時建立資產 [!UICONTROL 的Bundrary TIFF] 轉譯。影像預設集或動態轉譯可在資產 [!UICONTROL 的MerdMid TIFF] 上運作，因此如果 [!UICONTROL 「Authrid TIFF」(縱向TIFF)] 無法在 [!DNL AEM] Author實例上使用，也無法使用 [!DNL Brand Portal] 。因此，資產詳細資料頁面的轉譯邊欄並不會出現動態轉譯，並且會下載對話方塊。

若要將影像預設集發佈 [!DNL Brand Portal]至：

1. [!DNL AEM] 在「作者」實例中，點選/按一下 [!DNL AEM] 標誌以存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產]** &gt; **[!UICONTROL 影像預設集]**」。
2. 從影像預設集清單中選取影像預設集或多個影像預設集，然後按一下/點選 **[!UICONTROL 「發佈至品牌入口網站]**」。

![](assets/publishpreset.png)

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL 「發佈至品牌入口網站]** 」時，影像預設集會佇列等候發佈。建議使用者監控複製代理程式的記錄，確認發佈是否成功。

若要取消發佈影像預設集 [!DNL Brand Portal]，請從：

1. [!DNL AEM] 在「作者」實例中，點選/按一下 [!DNL AEM] 標誌以存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產]** &gt; **[!UICONTROL 影像預設集]**」。
2. 選取影像預設集，然後從頂端可用的選項中選取 **[!UICONTROL 「從品牌入口網站]** 移除」。

## 將中繼資料結構發佈至品牌入口網站 {#publish-metadata-schema-to-brand-portal}

中繼資料結構描述資產/系列屬性頁面上顯示的版面和屬性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果使用者已編輯「作者」實例上 [!DNL AEM] 的預設結構，而且想要使用與上一個預設結構相同的架構 [!DNL Brand Portal]，則只能將中繼資料結構表單發佈 [!DNL Brand Portal]至。在這種情況下，預設結構會 [!DNL Brand Portal] 以 [!DNL AEM] 從「作者」例項發佈的預設結構碼過度覆寫。

如果使用者已在 [!DNL AEM] 「作者」實例上建立自訂結構，則可以將自訂結構發佈至該自 [!DNL Brand Portal] 訂結構，而不需重新建立相同的自訂結構。然後，使用者可以將此自訂結構套用至任何資料夾/系列 [!DNL Brand Portal]。

>[!NOTE]
>
>無法將預設結構配置發佈 [!DNL Brand Portal] 至鎖定於 [!DNL AEM] 例項(即未編輯)的預設結構。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果資料夾有套用在 [!DNL AEM] 作者實例上的結構，也必須存在相同 [!DNL Brand Portal] 的結構，以維持 [!DNL AEM] 「作者」上資產屬性頁面的一致性 [!DNL Brand portal]。

若要將中繼資料結構從 [!DNL AEM] 作者實例發佈 [!DNL Brand Portal]至：

1. [!DNL AEM] 在「作者」實例中，點選/按一下AEM logo即可存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產]** &gt; **[!UICONTROL 中繼資料結構」]**。
2. 選取中繼資料結構，然後從上方可用選項選擇 **[!UICONTROL 「發佈至品牌入口網站]** 」。

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL 「發佈至品牌入口網站]**」時，中繼資料結構將會佇列等候發佈。建議使用者監控複製代理程式的記錄，確認發佈是否成功。

若要取消發佈中繼資料結構， [!DNL Brand Portal]請從：

1. [!DNL AEM] 在「作者」實例中，點選/按一下 [!DNL AEM] 標誌以存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「資產]** &gt; **[!UICONTROL 中繼資料結構」]**。
2. 選取中繼資料結構，然後從上方可用選項中選取 **[!UICONTROL 「從品牌入口網站]** 移除」。

## 將搜尋Facet發佈至品牌入口網站 {#publish-search-facets-to-brand-portal}

搜尋表單可為使用者提供 [Facet搜尋](../using/brand-portal-search-facets.md) 的功能 [!DNL Brand Portal]。搜尋Facet會增加更精細的搜尋粒度 [!DNL Brand Portal]。在搜尋 [表單中新增](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) 的所有預測都可供使用者使用，作為搜尋篩選器中的搜尋Facet。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您願意使用自訂搜尋表單 **[!UICONTROL 「資產管理搜尋邊欄]** 」 [!DNL AEM] 從「作者」例項，而不是重新建立相同的表單， [!DNL Brand Portal] 可以將自訂的搜尋表單從 [!DNL AEM] 「作者」實例發佈 [!DNL Brand Portal]到。

>[!NOTE]
>
>無法發佈鎖定搜尋表單 **[!UICONTROL 資產管理搜尋邊欄]** 至AEM資產 [!DNL Brand Portal] 除非已編輯。編輯並發佈到 [!DNL Brand Portal]之後，此搜尋表單會覆寫搜尋表單 [!DNL Brand Portal]。

若要將編輯的搜尋Facet從 [!DNL AEM] 「作者」實例發佈 [!DNL Brand Portal]至：

1. 點選/按一下 [!DNL AEM] 標誌，然後前往 **[!UICONTROL 「工具]** &gt; **[!UICONTROL 一般]** &gt; **[!UICONTROL 搜尋表單]**」。
2. 選取編輯的搜尋表單，然後選取 **[!UICONTROL 「發佈至品牌入口網站]**」。

   >[!NOTE]
   >
   >當使用者按一下 **[!UICONTROL 「發佈至品牌入口網站]**」時，搜尋Facet會佇列等候發佈。建議使用者監控複製代理程式的記錄，確認發佈是否成功。

若要取消發佈搜尋表單 [!DNL Brand Portal]：

1. [!DNL AEM] 在「作者」實例中，點選/按 [!DNL AEM] 一下標誌以存取全域導覽控制台，並點選/按一下「工具」圖示並導覽至 **[!UICONTROL 「一般]** &gt; **[!UICONTROL 搜尋表單]**」。
2. 選取搜尋表單，然後從上方可用選項中選擇 **[!UICONTROL 「從品牌入口網站]** 移除」。

>[!NOTE]
>
>「從品牌入口網站 **[!UICONTROL 取消發佈」]** 動作會在品牌入口網站上保留預設搜尋表單，且不會還原至發佈前所使用的最後一個搜尋表單。

### 限制 {#limitations}

1. 很少搜尋預測詞不適用於搜尋篩選器 [!DNL Brand Portal]。當這些搜尋預測是從 [!DNL AEM] 「作者」例項發佈為搜尋表單的一部分時， [!DNL Brand Portal]會被過濾掉。因此，使用者在所發佈的表格中，看到的預覽詞數目較少 [!DNL Brand Portal]。請參閱 [適用於品牌入口網站篩選條件的搜尋預測](../using/brand-portal-search-facets.md#list-of-search-predicates)。

2. 對於 [!UICONTROL 「選項] 」預覽，如果使用者使用任何自訂路徑來讀取AEM作者實例的選項，則無法在品牌入口網站上運作。這些額外路徑和選項不會使用搜尋表單發佈至品牌入口網站。在這種情況下，使用者可以選取「選項Predicate」中「新增選項」中的「 **[!UICONTROL 手動]********[!UICONTROL 」選項]** ，以手動方式新增這些選項 [!DNL Brand Portal]。

![](assets/options-predicate-manual.png)
