---
title: 使用 Brand Portal 設定 AEM Assets
seo-title: 使用 Brand Portal 設定 AEM Assets
description: 深入瞭解如何使用品牌入口網站設定AEM資產。
seo-description: 深入瞭解如何使用品牌入口網站設定AEM資產。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 9%

---


# 使用 Brand Portal 設定 AEM Assets {#configure-integration}

使用Adobe Experience Manager Assets品牌入口網站將Adobe Experience Manager Assets設定為雲端服務，可讓您發佈資產並與品牌入口網站使用者分發。 但是，使用品牌入口網站設定AEM 6.3（及以上版本）可讓品牌入口網站使用者使用資產發佈、資產分發和資產貢獻功能。

Adobe Experience Manager Assets已透過Adobe Developer Console設定品牌入口網站，該網站會購買Adobe身分管理服務(IMS)Token，以授權您的品牌入口網站租用戶。

>[!NOTE]
>
>***針對AEM Assets 6.3和更新版本***
>
>之前，品牌入口網站是透過舊版OAuth閘道在傳統介面中設定，該閘道使用JSON Web Token(JWT)交換來取得IMS Token進行授權。
>
>自2020年4月6日起，不再支援透過舊版OAuth進行的設定，並變更為透過Adobe Developer Console進行設定。

>[!TIP]
>
>***僅限現有客戶***
>
>舊版OAuth閘道設定將可繼續適用於現有客戶。
>
>如果您在舊版OAuth閘道配置中遇到問題，請刪除現有的配置，並透過Adobe Developer Console建立新的配置。

設定具有品牌入口網站的AEM資產的步驟依您的AEM版本而異，以及您是第一次設定或升級現有的設定：

| **AEM版本** | **新設定** | **升級配置** |
|---|---|---|
| **AEM Assets 雲端服務** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8和更新版本）** | [建立設定](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升級配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 聯絡支援 | 聯絡支援 |
