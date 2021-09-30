---
title: 發行說明
seo-title: Release Notes
description: 深入了解Adobe Experience Manager Assets Brand Portal 2021.10.0版中的功能、增強功能、已修正的重大問題，以及已知問題。
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2021.10.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: d5e39edc43d6d405e96edc76cbd1357ade58ea89
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 6%

---

# 發行說明 {#release-notes}

深入了解Adobe Experience Manager Assets Brand Portal 2021.10.0版中的新功能、增強功能、已修正的重大問題，以及已知問題。

## 發行資訊 {#release-information}

| 產品 | Adobe Experience Manager Assets Brand Portal |
|---|---|
| 版本 | 2021.10.0 |
| 日期 | 2021年10月 |

## 概覽 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可協助您跨裝置輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部人士和內部業務使用者。 它有助於提高資產共用的效率，加快資產上市時間，並降低不合規和未經授權的訪問風險。 Brand Portal可讓使用者隨時隨地以公司核准的格式來瀏覽、搜尋、預覽、下載和匯出資產。

## 2021.10.0的新增功能{#whats-new-in-2021.10.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### 已修正的重大問題 {#critical-issues-fixed}

此發行包含下列重大問題的修正：

* 從Brand Portal發佈的資產無法顯示在特定貢獻資料夾的Experience Manager資產中。
* 取消發佈貢獻資料夾時，Brand Portal租用戶的&#x200B;**[!UICONTROL totalUploadSize]**&#x200B;不會縮小。
* 使用者無法從資料夾中移除套用的中繼資料結構描述設定檔。
* 使用者權限頁面上的群組計數不正確。
* 瀏覽清單時，集合頁面所花費的時間過長。

<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->


### 已知問題 {#known-issues}

此版本包含下列已知問題：

* 使用者在移轉現有組織期間無法登入Brand Portal。

   不過，登入Brand Portal的作用中使用者仍可繼續運作，直到目前的工作階段過期為止。

* 從Brand Portal導覽至Admin Console時，管理員可能會看到額外的畫面來選取組織。


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

## 認證平台 {#certified-platforms}

若要確認哪些平台經認證可透過此版本的Brand Portal執行，請參閱[技術需求](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html)的&#x200B;**製作使用者介面支援瀏覽器**&#x200B;區段中表格的&#x200B;**觸控最佳化UI支援**&#x200B;欄。

## 連結 {#links}

* [Adobe Experience Manager Product Page on adobe.com](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal檔案](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## 產品存取與支援（受限網站） {#product-access-and-support-restricted-sites}

這些網站僅供客戶使用。 如果您是Adobe，需要存取權，請聯絡您的客戶經理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support](https://helpx.adobe.com/contact.html)
-->
