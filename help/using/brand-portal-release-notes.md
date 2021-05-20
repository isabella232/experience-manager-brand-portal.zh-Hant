---
title: 發行說明
seo-title: 發行說明
description: 深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版中的功能、增強功能、已修正的重大問題，以及已知問題。
seo-description: 深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版中的增強功能、已修正的重大問題，以及已知問題。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 5%

---

# 發行說明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2021.02.0版中的新功能、增強功能、已修正的重大問題，以及已知問題。

## 發行資訊 {#release-information}

| 產品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 2021.02.0 |
| 日期 | 2021年2月 |

## 概覽 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可協助您跨裝置輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部人士和內部業務使用者。 它有助於提高資產共用的效率，加快資產上市時間，並降低不合規和未經授權的訪問風險。 Brand Portal可讓使用者隨時隨地以公司核准的格式來瀏覽、搜尋、預覽、下載和匯出資產。

## 2021.02.0的新增功能{#whats-new-in-2021.02.0}

### 新功能{#new-features}

此版本包含下列新功能：

* AEM Assets as aCloud Service現在有權使用預先設定的Brand Portal執行個體。 Cloud Manager使用者可在AEM Assets上以Cloud Service例項的形式啟用Brand Portal。

* AEM Assets現在以Cloud Service形式提供「資產來源補充」功能。 它可讓Brand Portal使用者將資產上傳至允許的貢獻資料夾，並將貢獻資料夾從Brand Portal發佈至AEM Assets，作為Cloud Service例項。

* 已在&#x200B;**[!UICONTROL 下載設定]**&#x200B;下引入其他&#x200B;**[!UICONTROL 資產下載]**&#x200B;設定。 它會在下載資料夾、集合或大量下載資產時，為每個資產建立個別的資料夾。

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### 增強功能 {#enhancements}

此版本包含下列增強功能：

* 若是資料夾下載，系統會使用共用連結為每個資產建立獨立的資料夾，而不考慮&#x200B;**[!UICONTROL 下載設定]**。
* 已修改Brand Portal **[!UICONTROL 使用狀況報表]**，僅反映作用中的Brand Portal使用者。

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### 修正的嚴重問題{#critical-issues-fixed}

此發行包含下列重大問題的修正：

* 如果只下載原始資產，資產會反映其自己的擴充功能，而且在手動將擴充功能變更為zip之前不會開啟。
* 按一下導覽箭頭時，集合資料夾的使用者介面沒有回應。
* **** 即使資料夾為空， **** 列視圖中也會顯示Createbutton。
* **[!UICONTROL 如果]** 在存取Brand Portal例項時略過Dispatcher,Omni searchfails會顯示414錯誤訊息(Request-URI Too Long)。
* 如果資產的檔案名稱中包含逗號(`,`)，則會下載空白的zip資料夾。
* 檢視器使用者可以取得選項，將使用者新增至其建立的集合。
* 使用共用連結下載資產（縮圖或Web轉譯）時，會出現不一致的行為。

請參閱[Brand Portal 2021.02.0的新功能](whats-new.md)。


### 已知問題 {#known-issues}

此版本包含下列已知問題：

* 使用者沒有收到Asset Sourcing發佈工作流程的電子郵件通知。

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## 語言 {#languages}

Brand Portal使用者介面提供下列語言版本：

* 英文
* 德文
* 法文
* 西班牙文
* 義大利文
* 巴西葡萄牙文
* 日文
* 簡體中文
* 韓文

## 認證平台{#certified-platforms}

若要確認哪些平台經認證可透過此版本的Brand Portal執行，請參閱[技術需求](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)的&#x200B;**製作使用者介面支援瀏覽器**&#x200B;區段中表格的&#x200B;**觸控最佳化UI支援**&#x200B;欄。

## 連結 {#links}

* [Adobe Experience Manager Product Page on adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets Brand Portal檔案](https://helpx.adobe.com/tw/experience-manager/brand-portal/user-guide.html)

## 產品存取與支援（限制網站）{#product-access-and-support-restricted-sites}

這些網站僅供客戶使用。 如果您是Adobe，需要存取權，請聯絡您的客戶經理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [產品存取](https://login.marketing.adobe.com)

* [Adobe客戶服務](https://helpx.adobe.com/contact.html)
