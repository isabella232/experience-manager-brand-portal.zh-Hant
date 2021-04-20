---
title: 使用 Brand Portal 設定 AEM Assets
seo-title: 使用 Brand Portal 設定 AEM Assets
description: 深入瞭解使用品牌入口網站設定AEM Assets。
seo-description: 深入瞭解使用品牌入口網站設定AEM Assets。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Administrator
translation-type: tm+mt
source-git-commit: 6b9433bd5a225a2bbaddc09980c9f7b866a75fe8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 22%

---


# 使用 Brand Portal 設定 AEM Assets {#configure-integration}

使用品牌入口網站設定Adobe Experience Manager資產可讓品牌入口網站使用者進行資產發佈、資產分發和資產貢獻功能。 它可讓AEM Assets使用者發佈資產，並與品牌入口網站使用者一起分發。 品牌入口網站使用者可以存取共用資產並借由上傳新資產至資產貢獻檔案夾並將其發佈回AEM Assets來貢獻。

在以下網站支援使用品牌入口網站設定AEM Assets:
* AEM Assets as a Cloud Service 
* AEM Assets（內部部署及管理服務）6.3及以上版本

AEM Assets作為Cloud Service，會從Cloud Manager啟動品牌入口網站，自動設定品牌入口網站。 啟動工作流程會在後端建立必要的設定，並在與AEM Assets相同的IMS組織上啟動品牌入口網站，做為Cloud Service例項。

然而，AEM Assets（內部部署及受管理服務）是使用Adobe開發人員主控台手動設定品牌入口網站，該主控台會購買AdobeIdentity Management服務(IMS)代號以授權品牌入口網站租戶。

>[!NOTE]
>
>***AEM Assets6.3及以上版本***
>
>之前，品牌入口網站是透過舊版OAuth閘道在傳統介面中設定，該閘道使用JSON Web Token(JWT)交換來取得IMS Token進行授權。
>
>自2020年4月6日起，不再支援透過舊版OAuth進行的設定，並變更為透過Adobe開發人員主控台進行設定。


>[!TIP]
>
>***僅適用於現有客戶（內部部署和受管理服務）***
>
>舊版OAuth閘道設定將可繼續適用於現有客戶。
>
>如果您在舊版OAuth閘道配置中遇到問題，請刪除現有配置，並透過Adobe開發人員主控台建立新的配置。

使用品牌入口網站設定AEM Assets的步驟因您的版AEM本、您是第一次設定或升級現有組態而異：

| **版AEM本** | **新設定** | **升級配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [啟動品牌入口網站](https://docs.adobe.com/content/help/zh-Hant/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0及以上版本）** | [建立設定](https://docs.adobe.com/content/help/zh-Hant/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/zh-Hant/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0及以上版本）** | [建立設定](https://docs.adobe.com/content/help/zh-Hant/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/zh-Hant/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM6.3（6.3.3.8及以上版本）** | [建立設定](https://helpx.adobe.com/tw/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升級配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 聯絡支援 | 聯絡支援 |
