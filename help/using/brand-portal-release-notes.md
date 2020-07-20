---
title: 發行說明
seo-title: 發行說明
description: 深入瞭解Adobe Experience Manager Assets Brand Portal 6.4.6.2版中的功能、增強功能、已修正的重大問題和已知問題。
seo-description: 深入瞭解Adobe Experience Manager Assets Brand Portal 6.4.6.2版中的增強功能、已修正的重大問題和已知問題。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: ec588b0e9e1af5f813e13670a0616694aa9d5abe
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 4%

---


# 發行說明 {#release-notes}

深入瞭解Adobe Experience Manager Assets Brand Portal 6.4.6.2版本中的新功能、增強功能、已修正的重大問題和已知問題。

## 發行資訊 {#release-information}

| 產品 | Adobe Experience Manager Assets品牌入口網站 |
|---|---|
| 版本 | 6.4.6.2 |
| 日期 | 2020年6月 |

## 概覽 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部廠商和跨裝置的內部商業使用者。 它有助於提高資產共用的效率，加快資產上市時間，並降低不合規和未授權存取的風險。 品牌入口網站可讓使用者隨時隨地以公司核准的格式瀏覽、搜尋、預覽、下載和匯出資產。

## What&#39;s New in 6.4.6.2 {#what-s-new-in-6462}

### 已修正的重大問題 {#critical-issues-fixed-6462}

此版本包含下列重大問題的修正：

* 從品牌入口網站移除已發佈的中繼資料結構會導致錯誤。

* 如果管理員透過Adobe Developer Console以品牌入口網站設定Experience Manager Assets 6.5.4，品牌入口網站使用者無法將貢獻資料夾的資產從品牌入口網站發佈至Experience Manager。

* 重複複製父資料夾會導致衝突。

* 使用者無法產生「連結共用」報表。

* 使用者可使用copyPage命令複製品牌入口網站端點的MAC機密。

* cqTags導致在VA5克隆上重新建立索引。


### 已知問題 {#known-issues-6462}

此發行包含下列已知問題：

* 檢視器使用者目前可看到系列的共用連結。

* 如果階層中的檔案夾從AEM Assets重新命名，而包含資產的巢狀檔案夾已發佈至品牌入口網站，則在重新發佈根檔案夾之前，不會在品牌入口網站中更新檔案夾的標題。


## What&#39;s New in 6.4.6 {#what-s-new-in-646}

### New Features {#new-feature}

此版本包含下列新功能：

* 訪客登入品牌入口網站的驗證碼。 See, [Brand Portal guest access](../using/guest-access.md) for more information.

* AEM Assets雲端服務現在支援品牌入口網站。 您可以設定AEM Assets可以與品牌入口網站一起服務，以便與品牌入口網站使用者共用及分發資產。
如需詳細資訊，請參 [閱「使用品牌入口網站設定AEM Assets雲端服務」](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html)。

### 增強功能 {#enhancements-646}

此版本的品牌入口網站包含下列增強功能：

* 在AEM 6.3和更新版本中，AEM Assets和品牌入口網站之間的授權管道已變更。 AEM Assets現在已透過Adobe Developer Console設定品牌入口網站，該網站會購買IMS Token以授權您的品牌入口網站租用戶。

>[!NOTE]
>
>自2020年4月6日起，不再支援透過舊版OAuth進行的設定，並變更為透過Adobe Developer Console進行設定。

>[!TIP]
>
>***僅限現有客戶***
>
>舊版OAuth閘道設定將可繼續適用於現有客戶。
>
>如果您在舊版OAuth閘道配置中遇到問題，請刪除現有的配置，並透過Adobe Developer Console建立新的配置。

For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

### 已修正的重大問題 {#critical-issues-fixed}

此版本包含下列重大問題的修正：

* 中繼資料結構下拉式值無法在資產屬性中顯示。

* 中繼資料子架構不會根據資產屬性中的mimetype來顯示標籤。

* 取消發佈中繼資料結構會填入錯誤訊息，雖然結構已在後端移除。

* 預覽影像不會針對已發佈的資產顯示。

* 使用者無法發佈或取消發佈名稱中包含單一報價的資產。

* 下載多個資產時不會顯示條款與條件。

* 已解決次要安全性弱點。

### 已知問題 {#known-issues}

此發行包含下列已知問題：

* 在AEM 6.5.4上升級至Adobe Developer Console時，品牌入口網站使用者無法將貢獻資料夾資產發佈至AEM Assets。

   此問題將在下一個Service Pack 6.5.5中修正。

   如需AEM 6.5.4的立即修正，建議您下載 [修補程式](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，並安裝在您的作者實例上。

* 下載資產時，「排除系統轉譯」選項無法正常運作。


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

要確定哪些平台已通過此版本的Brand Portal認證，請參閱「技術需求」的「受支援的瀏覽器製作使用者介面 **」一節中的「** Support for Touch-optimized UI **」（針對觸控最佳化的UI支援）** 欄 [](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)。

## 連結 {#links}

* [adobe.com上的Adobe Experience Manager產品頁面](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Assets品牌入口網站檔案](https://helpx.adobe.com/tw/experience-manager/brand-portal/user-guide.html)

## 產品存取與支援（受限制的網站） {#product-access-and-support-restricted-sites}

這些網站僅提供給客戶使用。 如果您是客戶且需要存取權，請連絡您的Adobe客戶經理。

* [https://daycare.day.com](https://daycare.day.com)

* [產品存取](https://login.marketing.adobe.com)

* [Adobe客戶服務](https://helpx.adobe.com/contact.html)
