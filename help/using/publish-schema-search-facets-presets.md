---
title: 將預設集、結構和 Facet 發佈至 Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: 了解如何將預設集、結構和Facet發佈至Brand Portal。
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 2%

---

# 將預設集、結構和 Facet 發佈至 Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

文章會將影像預設集、中繼資料結構和自訂搜尋Facet，從AEM Author例項發佈至Brand Portal。 發佈功能可讓組織重複使用在AEM Author例項中建立/修改的影像預設集、中繼資料結構和搜尋Facet，減少重複的工作量。

>[!NOTE]
>
>將影像預設集、中繼資料結構和搜尋Facet從AEM Author例項發佈至Brand Portal的功能，可從AEM 6.2 SP1-CFP7和AEM 6.3 SP 1-CFP 1(6.3.1.1)開始使用。

## 將影像預設集發佈至Brand Portal {#publish-image-presets-to-brand-portal}

影像預設集是一組調整大小和格式化命令，在影像傳送時會套用至影像。 您可在Brand Portal中建立和修改影像預設集。 或者，如果AEM Author例項以動態媒體模式執行，則使用者可以在AEM Author中建立預設集，並將其發佈至AEM Assets Brand Portal，並避免在Brand Portal中重新建立相同的預設集。\
預設集建立後，資產詳細資料轉譯邊欄和下載對話方塊上會將其列為動態轉譯。

>[!NOTE]
>
>如果AEM Author例項未在&#x200B;**[!UICONTROL Dynamic Media模式]**&#x200B;中執行(客戶尚未購買Dynamic Media)，則上傳時不會建立資產的&#x200B;**[!UICONTROL 金字塔TIFF]**&#x200B;轉譯。 影像預設集或動態轉譯適用於資產的&#x200B;**[!UICONTROL 金字塔TIFF]**，因此，如果&#x200B;**[!UICONTROL 金字塔TIFF]**&#x200B;在AEM製作例項上不可用，則Brand Portal上也無法使用。 因此，資產詳細資料頁面和下載對話方塊的轉譯邊欄中不會顯示動態轉譯。

若要將影像預設集發佈至Brand Portal:

1. 在「AEM製作」例項中，點選/按一下AEM標誌以存取全域導覽主控台，並點選/按一下「工具」圖示，並導覽至&#x200B;**[!UICONTROL Assets > Image Presets]**。
1. 從影像預設集清單中選取影像預設集或多個影像預設集，然後按一下/點選&#x200B;**[!UICONTROL 發佈至Brand Portal]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>當使用者按一下「**[!UICONTROL 發佈至Brand Portal]**」時，影像預設集會排入佇列以進行發佈。 建議使用者監視復寫代理的記錄，以確認發佈是否成功。

若要從Brand Portal取消發佈影像預設集：

1. 在「AEM製作」例項中，點選/按一下AEM標誌以存取全域導覽主控台，並點選/按一下「工具」**[!UICONTROL 「工具」]**&#x200B;圖示，並導覽至「**[!UICONTROL 資產>影像預設集」]**。
1. 選取影像預設集，然後從上方可用的選項中選取「從Brand Portal移除」 **[!UICONTROL 。]**

## 將中繼資料結構發佈至Brand Portal  {#publish-metadata-schema-to-brand-portal}

中繼資料結構說明顯示在資產/集合屬性頁面上的配置和屬性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果使用者已編輯AEM Author例項上的預設結構，且願意使用與Brand Portal上的預設結構相同的結構，只要將中繼資料結構表單發佈至Brand Portal即可。 在這種情況下，Brand Portal的預設結構會因從AEM Author例項發佈的預設結構而過度使用。

如果使用者已在AEM Author例項上建立自訂結構，可將自訂結構發佈至Brand Portal，而非在該處重新建立相同的自訂結構。 然後，使用者可將此自訂結構套用至Brand Portal中的任何資料夾/集合。

>[!NOTE]
>
>如果預設結構鎖定在AEM例項（即未編輯），則無法將其發佈至Brand Portal。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果資料夾的AEM製作例項已套用結構，Brand Portal上也必須有相同的結構，才能維持AEM製作和Brand Portal上資產屬性頁面的一致性。

若要從AEM Author例項發佈中繼資料結構至Brand Portal:

1. 在「AEM製作」例項中，點選/按一下AEM標誌以存取全域導覽主控台，點選/按一下「工具」圖示，並導覽至&#x200B;**[!UICONTROL Assets >中繼資料結構]**。
1. 選取中繼資料結構，然後從頂端的可用選項中選取&#x200B;**[!UICONTROL 發佈至Brand Portal]**。

>[!NOTE]
>
>當使用者按一下「**[!UICONTROL 發佈至Brand Portal]**」時，中繼資料結構會排入佇列以進行發佈。 建議使用者監視復寫代理的記錄，以確認發佈是否成功。

若要從Brand Portal取消發佈中繼資料結構：

1. 在「AEM製作」例項中，點選/按一下AEM標誌以存取全域導覽主控台，點選/按一下「工具」圖示，並導覽至&#x200B;**[!UICONTROL Assets >中繼資料結構]**。
1. 選取中繼資料結構，然後從上方可用的選項中選取「從Brand Portal移除」。****

## 將搜尋Facet發佈至Brand Portal {#publish-search-facets-to-brand-portal}

搜尋表單為Brand Portal上的使用者提供[多面搜尋](../using/brand-portal-search-facets.md)的功能。 搜尋Facet可為Brand Portal上的搜尋賦予更精細的度。 搜尋表單中新增的所有[述詞](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html)都可供使用者在搜尋篩選器中作為搜尋Facet。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您願意從AEM製作例項使用自訂搜尋表單&#x200B;**[!UICONTROL Assets管理員搜尋邊欄]**，則您不必在Brand Portal上重新建立相同的表單，而是可以將自訂搜尋表單從AEM製作例項發佈至Brand Portal。

>[!NOTE]
>
>AEM Assets上鎖定的搜尋表單&#x200B;**[!UICONTROL Assets管理員搜尋邊欄]**&#x200B;無法發佈至Brand Portal，除非加以編輯。 編輯並發佈至Brand Portal後，此搜尋表單會覆寫Brand Portal上的搜尋表單。

若要將編輯過的搜尋面向從AEM Author例項發佈至Brand Portal:

1. 點選/按一下AEM標誌，然後前往「工具 **[!UICONTROL >一般 >搜 尋表格]**」。
1. 選擇已編輯的搜索表單，然後選擇&#x200B;**[!UICONTROL 發佈到Brand Portal]**。

   >[!NOTE]
   >
   >當使用者按一下「**[!UICONTROL 發佈至Brand Portal]**」時，搜尋Facet會排入佇列以進行發佈。 建議使用者監視復寫代理的記錄，以確認發佈是否成功。

若要從Brand Portal取消發佈搜尋表單：

1. 在「AEM製作」例項中，點選/按一下AEM標誌以存取全域導覽主控台，點選/按一下「工具」圖示，並導覽至&#x200B;**[!UICONTROL 一般>搜尋Forms]**。
1. 選擇搜索表單，然後從頂部可用的選項中選擇&#x200B;**[!UICONTROL 從Brand Portal中刪除]**。

>[!NOTE]
>
>**[!UICONTROL 從Brand Portal取消發佈]**&#x200B;動作會在Brand Portal上保留預設搜尋表單，且不會還原為發佈前使用的最後一個搜尋表單。

### 限制 {#limitations}

1. 少數搜尋述詞不適用於Brand Portal上的搜尋篩選器。 從AEM Author例項發佈到Brand Portal的搜尋表單內容時，會將這些搜尋述詞篩選掉。 因此，使用者在Brand Portal的已發佈表單中可看到較少的謂語。 請參閱[搜尋適用於Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates)上篩選器的述詞。

1. 若為[!UICONTROL 選項述詞]，如果使用者使用任何自訂路徑來讀取AEM Author例項中的選項，則無法在Brand Portal中運作。 這些額外的路徑和選項不會透過搜尋表單發佈至Brand Portal。 在此情況下，使用者可以在&#x200B;**[!UICONTROL **[!UICONTROL  Options Predicate ]**內選取**[!UICONTROL  Manual ]**中的Add Options]**&#x200B;選項，以在Brand Portal手動新增這些選項。

![](assets/options-predicate-manual.png)
