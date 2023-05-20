---
title: 將預設集、結構和 Facet 發佈至 Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: 瞭解如何發佈品牌入口網站的預設集、綱要和 facet。
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

文章 delves 至發佈影像預設集、中繼資料架構，以及從 AEM 作者執行個體到品牌入口網站的自訂搜尋方面。 發佈功能可讓組織重新使用「影像預設集」、「中繼資料架構」和「AEM 作者執行個體建立/修改的搜尋方面，從而減少重複工作。

>[!NOTE]
>
>發佈影像預設集、中繼資料綱要和搜尋方面的功能，AEM 6.2 SP1-CFP7 和作者 6.3 SP 1-CFP 1 （6.3.1.1）。

## Publish 影像預設集至品牌入口網站 {#publish-image-presets-to-brand-portal}

影像預設集是一組在影像傳遞時套用至影像的大小調整和格式命令。 影像預設集可在品牌入口網站建立和修改。 或者，如果 AEM 作者執行個體在動態媒體模式下執行，則使用者可以在 AEM 建立預設集，並將其作者發佈，避免在 AEM Assets 重新建立相同的預設集。\
建立預設集後，它會在資產詳細轉譯邊欄和下載對話方塊上以動態轉譯的形式列出。

>[!NOTE]
>
>如果 AEM 作者執行個體未在動態媒體模式 ]**中**[!UICONTROL  執行（客戶尚未購買動態媒體），則 **[!UICONTROL 轉譯時不會建立資產的棱錐 TIFF]** 上傳。影像預設集或動態轉譯會在資產的棱錐 TIFF ]**上**[!UICONTROL  運作，因此如果 **[!UICONTROL AEM 作者上無法使用金字塔 tiff]** ，則不能在執行個體上使用。因此，在轉譯邊欄的資產詳細資料頁面和下載對話中，不存在動態轉譯轉譯。

要發佈影像預設集至品牌入口網站：

1. 在 AEM 作者執行個體中，點擊/按一下 AEM 標誌以存取全域導覽主控台，然後點擊/按一下工具圖示並導覽至 **[!UICONTROL Assets > 影像預設集]** 。
1. 從影像預設清單中選擇影像預設或多個影像預設，然後按一下/點擊 **[!UICONTROL 發佈到Brand Portal]**。

![](assets/publishpreset.png)

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL Publish 以品牌入口網站]** 影像預設集已排入佇列以供發佈。 建議使用者監視複製代理程式的記錄，以確認發佈是否成功。

要從品牌入口網站取消發佈影像預設集：

1. 在 AEM 作者執行個體中，點擊/按一下 AEM 標誌以存取全域導覽主控台，然後點擊/按一下 **[!UICONTROL 工具]** 圖示並導覽至 **[!UICONTROL Assets > 影像預設集]** 。
1. 選取影像預設集，然後從頂部可用的選項中選取 **[!UICONTROL 品牌入口網站]** 移除。

## Publish 中繼資料綱要品牌入口網站  {#publish-metadata-schema-to-brand-portal}

中繼資料綱要說明資產/集合的屬性頁面上顯示的佈局和屬性。

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

如果使用者已編輯 AEM 執行個體作者上的預設綱要，且願意在綱要上使用與預設綱要相同的品牌入口網站，他們只需發佈中繼資料綱要表單品牌入口網站。 在這種情況下，品牌入口網站的預設綱要由從 AEM 作者執行個體發佈的預設架構 ridden。

如果使用者已在 AEM 作者執行個體建立自訂綱要，則可以發佈自訂綱要品牌入口網站，而不是在那裡重新建立相同的自訂綱要。 然後使用者便可將此自訂綱要套用至品牌入口網站中的任何資料夾/集合。

>[!NOTE]
>
>如果預設架構已在 AEM 執行個體（即未編輯），則無法發佈至品牌入口網站。

![](assets/default-schema-form.png)

>[!NOTE]
>
>如果資料夾在 AEM 作者執行個體上套用了綱要，則相同的綱要也必須存在於品牌入口網站上，才能在資產頁面和 AEM 中維持作者屬性品牌入口網站的一致性。

若要發佈中繼資料綱要從 AEM 作者執行個體到品牌入口網站：

1. 在 AEM 作者執行個體中，點擊/按一下 AEM 標誌以存取全域導覽主控台，然後點擊/按一下工具圖示並導覽至 **[!UICONTROL Assets > 中繼資料架構]** 。
1. 選取中繼資料綱要，然後從頂部可用的選項中選取 **[!UICONTROL 品牌入口網站]** Publish。

>[!NOTE]
>
>當使用者按一下 **[!UICONTROL Publish 來品牌入口網站]** 時，中繼資料的架構會排隊等候發佈。 建議使用者監視複製代理程式的記錄，以確認發佈是否成功。

若要從品牌入口網站取消發佈中繼資料綱要。。

1. 在 AEM 作者執行個體中，點擊/按一下 AEM 標誌以存取全域導覽主控台，然後點擊/按一下工具圖示並導覽至 **[!UICONTROL Assets > 中繼資料架構]** 。
1. 選取中繼資料綱要，然後從頂部可用的選項中選取 **[!UICONTROL 品牌入口網站]** 移除。

## 將搜索小平面發佈到Brand Portal {#publish-search-facets-to-brand-portal}

搜索表單提供 [多面搜索](../using/brand-portal-search-facets.md) 給Brand Portal的用戶。 搜索小面片使Brand Portal上的搜索更具精細度。 所有 [謂詞已添加](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) 在「搜索」(Search)窗體中，用戶可以在「搜索」(Search)過濾器中作為搜索小平面使用。

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

如果您願意使用自訂搜尋表單 **[!UICONTROL Assets Admin Search]** 邊欄從 AEM 作者執行個體中，請改為在品牌入口網站上重新建立相同的表單，發佈從搜尋 AEM 作者到執行個體。

>[!NOTE]
>
>已鎖定搜尋表單 **[!UICONTROL Assets Admin AEM Assets Search]** 邊欄無法發佈至品牌入口網站，除非已編輯。 編輯併發布至品牌入口網站後，此搜尋表單會覆蓋品牌入口網站上的搜尋表單。

若要發佈從 AEM 作者執行個體到品牌入口網站的已編輯搜尋方面：

1. 點選/按一下AEM標誌，然後前往「工具 **[!UICONTROL >一般 >搜 尋表格]**」。
1. 選取「已編輯的搜尋表單，然後選取 **[!UICONTROL Publish 以品牌入口網站]** 。

   >[!NOTE]
   >
   >當使用者按一下 **[!UICONTROL Publish 品牌入口網站]** 時，搜尋方面會排隊等候發佈。 建議使用者監視複製代理程式的記錄，以確認發佈是否成功。

若要從品牌入口網站取消發佈搜尋表單。。

1. 在 AEM 作者執行個體中，點擊/按一下 AEM 標誌以存取全域導覽主控台，然後點擊/按一下「工具」圖示並導覽至 **[!UICONTROL 一般 > Search Forms]** 。
1. 選取「搜尋」表單，然後從頂部可用的選項中選取 **[!UICONTROL 移除從品牌入口網站]** 。

>[!NOTE]
>
>品牌入口網站 ]**動作的**[!UICONTROL  取消發佈會保留品牌入口網站上的預設搜尋表單，且不會還原為發佈前的最後一個搜尋表單。

### 限制 {#limitations}

1. 少數搜尋謂語不適用於品牌入口網站上的搜尋篩選器。 當這些搜尋謂語以搜尋形式從 AEM 作者執行個體發佈到品牌入口網站時，會被篩選掉。 因此，使用者會在品牌入口網站的已發佈表單中看到的謂語數減少。 請參閱 [ 品牌入口網站 ](../using/brand-portal-search-facets.md#list-of-search-predicates) 上篩選器適用的搜尋謂語。

1. 對於 [!UICONTROL 選項謂詞]，如果用戶在AEM Author實例中使用任何自定義路徑讀取選項，則該路徑在Brand Portal無法工作。 這些附加路徑和選項不會隨搜索表單發佈到Brand Portal。 在這種情況下，用戶可以選擇 **[!UICONTROL 手動]** 選項 **[!UICONTROL 添加選項]** 內 **[!UICONTROL 選項謂詞]** 在Brand Portal手動添加這些選項。

![](assets/options-predicate-manual.png)
