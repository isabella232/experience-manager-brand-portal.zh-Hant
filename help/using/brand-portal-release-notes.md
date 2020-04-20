---
title: 發行說明
seo-title: 發行說明
description: 深入瞭解Adobe Experience Manager Assets Brand Portal 6.4.6版中的功能、增強功能、已修正的重大問題和已知問題。
seo-description: 深入瞭解Adobe Experience Manager Assets Brand Portal 6.4.6版中的增強功能、已修正的重大問題和已知問題。
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 9bb1538165030f7f9e78af99bb89ea38897c3967

---


# 發行說明 {#release-notes}

深入瞭解Adobe Experience Manager Assets Brand Portal 6.4.6版本中的新功能、增強功能、已修正的重大問題和已知問題。

## 發行資訊 {#release-information}

| 產品 | Adobe Experience Manager Assets品牌入口網站 |
|---|---|
| 版本 | 6.4.6 |
| 日期 | 2020年3月 |

## 概覽 {#overview}

Adobe Experience Manager(AEM)Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部廠商和跨裝置的內部商業使用者。 它有助於提高資產共用的效率，加快資產上市時間，並降低不合規和未授權存取的風險。 品牌入口網站可讓使用者隨時隨地以公司核准的格式瀏覽、搜尋、預覽、下載和匯出資產。

## 6.4.6的新增功能 {#what-s-new-in-646}

### New Features {#new-feature}

此版本包含下列新功能：

* 訪客登入品牌入口網站的驗證碼。 如需詳細 [資訊，請參閱品牌入口網站](../using/guest-access.md) (Brand Portal)訪客存取。

* AEM Assets雲端服務現在支援品牌入口網站。 您可以設定AEM Assets可以與品牌入口網站一起服務，以便與品牌入口網站使用者共用及分發資產。
如需詳細資訊，請參 [閱「使用品牌入口網站設定AEM Assets雲端服務」](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html)。

### 增強功能 {#enhancements-646}

此版本的品牌入口網站包含下列增強功能：

* 在AEM 6.3和更新版本中，AEM Assets和品牌入口網站之間的授權管道已變更。 AEM Assets現在已透過Adobe I/O設定品牌入口網站，Adobe I/O會購買IMS Token以授權您的品牌入口網站租用戶。

   >[!NOTE]
   >
   >自2020年4月6日起，不再支援透過舊版OAuth進行的設定，並變更為透過Adobe I/O進行設定。


>[!TIP]
>
>***僅限現有客戶***
>
>建議您繼續使用現有的舊版OAuth閘道設定。 如果您在舊版OAuth閘道配置中遇到問題，請刪除現有配置並透過Adobe I/O建立新配置。


如需詳細資訊，請參 [閱「使用品牌入口網站設定AEM資產」](configure-aem-assets-with-brand-portal.md)

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

* 在AEM 6.5.4上升級至Adobe I/O時，品牌入口網站使用者無法將貢獻資料夾資產發佈至AEM資產。

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
