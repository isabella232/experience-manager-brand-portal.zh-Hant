---
title: 將標記發佈至 Brand Portal
seo-title: Publish tags to Brand Portal
description: 瞭解如何將標籤從Experience Manager Assets發佈到Brand Portal。
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 4%

---

# 將標記發佈至 Brand Portal {#publish-tags-to-brand-portal}

瞭解如何將標籤從Experience Manager Assets發佈到Brand Portal。

標籤在組織資產和增強與其關聯的資產的搜索能力方面非常有用。 可以將標籤視為與資產附加的關鍵字或標籤（元資料），並允許在搜索結果中快速找到資產。 要瞭解如何為Experience Manager Assets的資產分配標籤，請參閱 [使用標籤來組織資產](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html)。

當將具有關聯標籤的資產(和集合AEM)發佈到Brand Portal時，標籤（與中的資產和集合相關聯）將自動發佈到Brand Portal。 發佈的標籤有助於使搜索能夠查找關聯的資產。

>[!NOTE]
>
>但是，建議在發佈與標籤關聯的資產（和集合）之前，只向Brand Portal發佈標籤。 這可確保更快地將資產（和收藏）發佈到Brand Portal。

## 管理標籤 {#manage-tags}

可以使用預先存在的標籤附加到資產或從「標籤」控制台創AEM建新標籤(**[!UICONTROL 工具 |標籤 |標AEM記]**)。 在這兩種情況下，您必須先將標籤發佈到Brand Portal，然後將它們與相應的資產關聯。

要在上建立標AEM簽，在Brand Portal上發佈標籤，並將標籤與相應的資產（或集合）關聯，請執行以下步驟：

1. **建立標籤**
使用管理權限和訪問權限登錄到AEM Author實例 **[!UICONTROL 標AEM記]** 從全局導航中獲得控制台：

   1. 選擇 **[!UICONTROL 工具]**

   1. 選擇 **[!UICONTROL 常規]**

   1. 選擇 **[!UICONTROL 標籤]**

1. 選擇 **[!UICONTROL 建立]** ，然後選擇 **[!UICONTROL 建立標籤]** 的雙曲餘切值。
1. 指定下列設定：

   * **[!UICONTROL 標題]**

      *（必需）* 標籤的顯示標題。
   * **[!UICONTROL 名稱]**
      *（必需）* 標籤的名稱。 如果未指定，則從標題建立有效的節點名稱。 請參閱 [標籤ID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html)。
   * **說明**

      *（可選）* 標籤的說明。
   * **標籤路徑**
標籤的JCR路徑。

1. 選擇 **[!UICONTROL 提交]** 的子菜單。

   在實例上建立標籤AEM後，該標籤將可以附加到該資產（使用該資產的「屬性」部分或「管理標籤」部分）。

1. **將標籤發佈到Brand Portal**。

   轉到 **[!UICONTROL 標AEM記]** 控制台([!UICONTROL 工具 |標籤 |標AEM記])，選擇所需的標籤並發佈到Brand Portal。

1. **將標籤附加到資產（或集合）**。

   選擇資產（或集合），然後使用該資產的「屬性」部分或「管理標籤」部分附加所需的標籤。 有關如何為AEM Assets的資產分配標籤的詳細資訊，請參閱 [使用標籤來組織資產](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html)。

1. **將資產（或收集）發佈到Brand Portal**。\
   當您將資產（或集合）發佈到Brand Portal時，附加的標籤也可在Brand Portal上使用。

   要查看Brand Portal各資產（或集合）上的附加標籤，請登錄Brand Portal並選擇該資產，在「屬性」部分下，您將看到附加標籤。

## 搜尋提升 {#search-promote}

AEM Assets Brand Portal允許您根據關鍵字標籤將特定資產作為搜索的最佳結果。

要提升搜索關鍵字的資產，請執行以下步驟：

1. 開啟 **[!UICONTROL 屬性]** 作者實例上的資AEM產頁面。
1. 轉到 **[!UICONTROL 高級]** 頁籤。
1. 在 **[!UICONTROL 搜索升級]** 內 **[!UICONTROL 提升搜索關鍵字]** 選擇 **[!UICONTROL 添加]** 的子菜單。

   ![](assets/search-promote.png)

1. 儲存變更。
1. 將資產發佈至 Brand Portal.
1. 登錄Brand Portal。 視圖 **[!UICONTROL 高級]** 頁籤 **[!UICONTROL 屬性]** 的下界。
請注意 **[!UICONTROL 搜索升級]** 關鍵字在該資產的「屬性」中也可見。
