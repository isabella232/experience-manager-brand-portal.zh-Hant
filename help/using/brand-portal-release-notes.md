---
title: 發行說明
seo-title: 發行說明
description: 深入瞭解Adobe Experience Manager Assets Brand Portal 2020.10.0版中的功能、增強功能、已修正的重大問題和已知問題。
seo-description: 深入瞭解Adobe Experience Manager Assets Brand Portal 2020.10.0版本中的增強功能、已修正的重大問題和已知問題。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 4774d8a78657c89081d229ce596a3bd404ae1bc8
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 5%

---


# 發行說明 {#release-notes}

深入瞭解Adobe Experience Manager Assets Brand Portal 2020.10.0版本中的新功能、增強功能、已修正的重大問題和已知問題。

## 發行資訊 {#release-information}

| 產品 | Adobe Experience Manager Assets品牌入口網站 |
|---|---|
| 版本 | 2020.10.0 |
| 日期 | 2020年10月 |

## 概覽 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部廠商和跨裝置的內部商業使用者。 它有助於提高資產共用的效率，加快資產上市時間，並降低不合規和未授權存取的風險。 品牌入口網站可讓使用者隨時隨地以公司核准的格式瀏覽、搜尋、預覽、下載和匯出資產。

## What&#39;s New in 2020.10.0 {#whats-new-in-2020.10.0}

### New Features {#new-features}

此版本包含下列新功能：

* 「下 **[!UICONTROL 載]** 」對話方塊會在清單檢視中改版，並提供其他選項來排除不需要的轉譯、針對類似資產類型套用相同的規則集，以及下載選取的資產轉譯。 請參 [閱從品牌入口網站下載資產的步驟](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets)。

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* 現在，只要按 **[!UICONTROL 一下滑鼠]********** ，即可從所有品牌入口網站頁面導覽至「檔案」、「系列」和「共用連結」。

* 資產詳 **[!UICONTROL 細資訊頁面中的]** 「轉譯」面板現在可讓品牌入口網站使用者選取原始資產和（或）特定資產轉譯，並直接從「轉譯」面板下載它們，而不需開啟「下載」對 **[!UICONTROL 話方塊]****** 。 請參 [閱「從資產詳細資訊頁面下載資產」](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page)。

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* 除了現有的 **[!UICONTROL 下載設定]**[](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) ，品牌入口網站管理員也可以設定不同使用者群組的權限，以檢視和（或）從資產詳細資訊頁面下載原始資產及其轉譯。 這些設定將定義哪些人可以存取和（或）下載資產轉譯。

### 增強功能 {#enhancements}

此發行包含下列增強功能：

* 來賓用戶的會話超時閾值已從2小時減少到15分鐘。
* 多頁 **[!UICONTROL PDF的其他「檢視頁面]** 」選項已移除，因為使用者現在可以從Adobe Document Cloud檢視器檢視PDF頁面。


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### 已知問題 {#known-issues}

此發行包含下列已知問題：

* 「資產報表」 **[!UICONTROL 上的搜尋]** ，會顯示產品介面上的處理，但沒有搜尋結果。
* 非管理員使用者無法在資產詳細資料頁面上看到視訊DM編碼。
* 在「下載」對話方塊中，個別資產轉譯的大小與總下載大小的對齊方式會扭曲。



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

品牌入口網站使用者介面提供下列語言：

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

要確定哪些平台已通過此版本的Brand Portal認證，請參閱「技術需求」的「受支援的瀏覽器製作使用者介面 **」一節中的「支援觸控最佳化UI** 」 **欄**[](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)。

## 連結 {#links}

* [adobe.com上的Adobe Experience Manager產品頁面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets品牌入口網站檔案](https://helpx.adobe.com/tw/experience-manager/brand-portal/user-guide.html)

## 產品存取與支援（受限制的網站） {#product-access-and-support-restricted-sites}

這些網站僅提供給客戶使用。 如果您是客戶且需要存取權，請連絡您的Adobe客戶經理。

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [產品存取](https://login.marketing.adobe.com)

* [Adobe客戶服務](https://helpx.adobe.com/contact.html)
