---
title: Brand Portal 中的 Asset Sourcing
seo-title: Asset Sourcing in Brand Portal
description: 深入瞭解Adobe Experience Manager Assets Brand Portal發佈的資產來源補充功能。
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 1%

---

# 資產來源補充概覽 {#overview-asset-sourcing-in-bp}

**資產來源補充** 允許Experience Manager Assets用戶（管理員/非管理員用戶）使用其他 **資產貢獻** 屬性，確保新資料夾可由Brand Portal用戶提交資產。 這將自動觸發建立兩個附加子資料夾的工作流，該子資料夾稱為 **共用** 和 **新建**，位於新建立的 **貢獻** 的子菜單。 然後，管理員通過將應添加到貢獻資料夾的資產類型以及一組基準資產的簡介上載到 **共用** 資料夾，確保BP用戶具有所需的參考資訊。 然後，管理員可以在發佈新建立的稿件之前，授予活動的Brand Portal用戶對稿件資料夾的訪問權 **貢獻** 資料夾到Brand Portal。 用戶完成在 **新建** 資料夾，它們可以將貢獻資料夾發佈回Experience Manager作者環境。 請注意，完成導入並反映Experience Manager Assets內新發佈的內容可能需要幾分鐘時間。

此外，所有現有功能都保持不變。 Brand Portal用戶可以從貢獻資料夾以及其他允許的資料夾中查看、搜索和下載資產。 管理員可以進一步共用稿件資料夾、修改屬性和向集合添加資產。

![Brand Portal資產來源](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## 必備條件 {#prerequisites}

* Experience Manager Assetsas a Cloud Service案，Experience Manager Assets6.5.2或更高。
* 確保您的Experience Manager Assets實例已配置Brand Portal。 看， [將Experience Manager Assets配置為Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>預設情況下，Experience Manager Assetsas a Cloud Service、Experience Manager Assets和更高版本上啟用了「資產採購」功6.5.9。
>
>現有配置將繼續在早期版本上工作。

>[!NOTE]
>
>在Experience Manager Assets有個已知問6.5.4。Brand Portal用戶無法在升級到Adobe Developer控制台時向Experience Manager Assets發佈貢獻資料夾的資產。
>
>此問題已在Experience Manager Assets6.5.5解決。您可以將Experience Manager Assets實例升級到最新的Service Pack [升級配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) Adobe Developer控制台。

<!--

>For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.
-->

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### 上載Brand Portal用戶清單 {#upload-bp-user-list}

Experience Manager Assets管理員可以上傳包含Experience Manager Assets活動Brand Portal用戶清單的Brand Portal用戶配置(.csv)檔案，以允許他們訪問資產採購功能。

只能與用戶清單中定義的活動Brand Portal用戶共用貢獻資料夾。 管理員還可以在配置檔案中添加新用戶並上載修改的用戶清單。

>[!NOTE]
>
>確保您的Experience Manager Assets實例已配置Brand Portal。 看， [將Experience Manager Assets配置為Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。

>[!NOTE]
>
>CSV檔案的格式與批量用戶導入Admin Console中支援的格式相同。 電子郵件、名字和姓氏是必填項。

管理員可以在Admin Console中添加新用戶，請參見 [管理用戶](brand-portal-adding-users.md) 的上界。 在Admin Console中添加用戶後，這些用戶可以添加到Brand Portal用戶配置檔案，然後分配訪問貢獻資料夾的權限。

**要上載Brand Portal用戶清單：**

1. 登錄到您的Experience Manager Assets實例。
1. 從 **工具**  面板，導航至 **[!UICONTROL 資產]** > **[!UICONTROL Brand Portal用戶]**。

1. Brand Portal上載參與者窗口開啟。
從本地電腦瀏覽並上載 **配置(.csv)檔案** 包含活動的Brand Portal用戶清單。
1. 按一下「**[!UICONTROL 儲存]**」。

   ![](assets/upload-user-list2.png)


管理員可以在配置貢獻資料夾時從此用戶清單訪問特定用戶。 只有分配給貢獻資料夾的用戶才有權訪問貢獻資料夾並將資產從Brand Portal發佈到Experience Manager Assets。

## 另請參閱 {#reference-articles}

* [配置並發佈貢獻資料夾到Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [將稿資料夾發佈到Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
