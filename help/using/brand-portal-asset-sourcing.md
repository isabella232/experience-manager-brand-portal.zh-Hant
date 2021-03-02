---
title: Brand Portal 中的 Asset Sourcing
seo-title: Brand Portal 中的 Asset Sourcing
description: 深入瞭解Adobe Experience Manager資產品牌入口網站中發佈的資產採購功能。
seo-description: 深入瞭解Adobe Experience Manager資產品牌入口網站中發佈的資產採購功能。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: 資產
feature: 品牌入口網站
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 5a61c42762e111b824163ce7d054d413a4da56bc
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 4%

---


# 資產來源補充概述{#overview-asset-sourcing-in-bp}

**Asset** SourcingAEM可讓使用者（管理員／非管理員使用者）使用額外的 **Asset** Contribution屬性建立新資料夾，以確保建立的新資料夾可供Brand Portal使用者提交資產。這會自動觸發在新建立的&#x200B;**Contribution**&#x200B;資料夾中建立另外兩個子資料夾的工作流程，名為&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**。 然AEM後，管理員將應添加到貢獻資料夾的資產類型以及一組基線資產的概述上載到&#x200B;**SHARED**&#x200B;資料夾，以確保BP用戶擁有他們需要的參考資訊，從而定義需求。 然後，管理員可以先授與作用中的品牌入口網站使用者對貢獻資料夾的存取權，再將新建立的&#x200B;**貢獻**&#x200B;資料夾發佈至品牌入口網站。 當使用者在&#x200B;**NEW**&#x200B;資料夾中新增內容後，就可以將貢獻資料夾發佈回作AEM者環境。 請注意，完成匯入並反映AEM Assets境內新發佈的內容可能需要幾分鐘的時間。

此外，所有現有功能都保持不變。 品牌入口網站使用者可從貢獻資料夾以及其他許可的資料夾檢視、搜尋及下載資產。 此外，管理員還可以進一步共用貢獻資料夾、修改屬性並將資產新增至系列。

## 必備條件 {#prerequisites}

* AEM Assets作為Cloud Service實例，AEM Assets6.5.2或更高版本。
* 請確定您的AEM Assets實例已配置品牌入口網站。 請參閱[使用品牌入口網站配置AEM Assets。](../using/configure-aem-assets-with-brand-portal.md)
* 請確定您的品牌入口網站租用戶已設定一個AEM Assets作者例項。

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![品牌入口網站資產來源補充](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM Assets6.5.4中存在已知問題。品牌入口網站使用者無法在升級至Adobe開發人員主控台時，將貢獻資料夾的資產發佈至AEM Assets。
>
>此問題已在AEM6.5.5中修正。您可以將AEM Assets實例升級至最新的Service Pack AEM 6.5.5和[，以升級Adobe開發人員控制台上的配置](https://docs.adobe.com/content/help/zh-Hant/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。
>
>如需6.AEM5.4的立即修正，建議您下載修補程式](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)並安裝在您的作者實例上。[

## 配置資產來源補充{#configure-asset-sourcing}

**Asset** Sourcing是在AEM Assets作者實例內配置的。管理員可以從&#x200B;**AEM Web Console Configuration**&#x200B;啟用「資產來源補充」功能標幟配置，並上傳&#x200B;**AEM Assets**&#x200B;中的有效品牌入口網站使用者清單。

>[!NOTE]
>
>預設情況下，資產來源補充在AEM Assets作為Cloud Service啟用。 管AEM理員可直接上傳有效品牌入口網站使用者，以允許他們存取「資產來源補充」功能。

>[!NOTE]
>
>在您從設定開始之前，請確定您的AEM Assets實例已設定品牌入口網站。 請參閱[使用品牌入口網站配置AEM Assets。](../using/configure-aem-assets-with-brand-portal.md)

以下視訊示範如何在您的AEM Assets作者例項上設定「資產來源補充」:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### 啟用資產來源補充{#enable-asset-sourcing}

管AEM理員可以從Web Console設定(AEM亦稱「設定管理員」)中啟用「資產採購」功能標幟。

>[!NOTE]
>
>此步驟不適用於AEM Assets作為Cloud Service。


**要啟用資產來源補充，請執行以下操作：**
1. 登入您的AEM Assets作者例項，並開啟「設定管理員」。
預設URL:http:// localhost:4502/system/console/configMgr.
1. 使用關鍵字&#x200B;**資產採購**&#x200B;進行搜尋，以找到&#x200B;**[!UICONTROL 資產採購功能標幟設定]**。
1. 按一下&#x200B;**[!UICONTROL 資產採購功能標籤配置]**&#x200B;以開啟配置窗口。
1. 選中&#x200B;**[!UICONTROL feature.flag.active.status]**&#x200B;複選框。
1. 按一下「**[!UICONTROL 儲存]**」。

![](assets/enable-asset-sourcing.png)

### 上傳品牌入口網站使用者清單{#upload-bp-user-list}

管AEM理員可以上傳包含AEM Assets活動品牌入口網站使用者清單的品牌入口網站使用者設定(.csv)檔案。 貢獻資料夾只能與使用者清單中定義的作用中品牌入口網站使用者共用。 管理員也可以在配置檔案中添加新用戶，並上傳修改的用戶清單。

>[!NOTE]
>
>CSV檔案的格式與大量使用者匯入的Admin Console支援的格式相同。 電子郵件、名字和姓氏是必填的。

管理員可以在Admin Console中添AEM加新用戶，如需詳細資訊，請參閱[管理用戶](brand-portal-adding-users.md)。 在Admin Console中新增使用者後，這些使用者可以新增至品牌入口網站使用者設定檔案，然後指派存取貢獻資料夾的權限。

**若要上傳品牌入口網站使用者清單：**
1. 登入您的AEM Assets實例。
1. 從&#x200B;**工具**&#x200B;面板，導覽至&#x200B;**[!UICONTROL 資產]** > **[!UICONTROL 品牌入口網站使用者]**。

1. 「品牌入口網站上傳參與者」視窗隨即開啟。
從本機電腦瀏覽並上傳包含作用中品牌入口網站使用者清單的**設定(.csv)檔案**。
1. 按一下「**[!UICONTROL 儲存]**」。

   ![](assets/upload-user-list2.png)


管理員可在設定貢獻資料夾時，從此使用者清單提供特定使用者的存取權。 只有指派給貢獻檔案夾的使用者才能存取貢獻檔案夾，並將資產從品牌入口網站發佈至AEM Assets。

## 另請參閱 {#reference-articles}

* [設定貢獻資料夾並發佈至品牌入口網站](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [將貢獻資料夾發佈至AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
