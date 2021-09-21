---
title: 使用 Brand Portal 設定 AEM Assets
seo-title: Configure AEM Assets with Brand Portal
description: 深入了解如何使用Brand Portal設定AEM Assets。
seo-description: Get an insight into configuring AEM Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: ea3242459776037499b21b33ba40357afc8bf234
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 21%

---

# 使用 Brand Portal 設定 AEM Assets {#configure-integration}

使用Brand Portal設定Adobe Experience Manager資產，可為Brand Portal使用者啟用資產發佈、資產分發和資產貢獻功能。 它可讓AEM Assets使用者發佈資產，並與Brand Portal使用者分發資產。 Brand Portal使用者可以上傳新資產至資產貢獻資料夾，並將其發佈回AEM Assets，以存取共用資產和貢獻內容。

支援使用Brand Portal設定AEM Assets:

* AEM Assets as a Cloud Service 
* AEM Assets（內部部署和托管服務）6.3和更新版本

AEM Assets as aCloud Service會透過從Cloud Manager啟動Brand Portal自動設定。 啟動工作流程會在後端建立必要的設定，並在與AEM Assets(作為Cloud Service例項)相同的IMS組織上啟動Brand Portal。

然而，AEM Assets（內部部署和托管服務）是使用Brand Portal Developer Console手動設定，其會擷取AdobeIdentity Management服務(IMS)代號，以授權Brand Portal租用戶。

>[!NOTE]
>
>***適用於AEM Assets 6.3及更新版本***
>
>之前，Brand Portal是透過舊版OAuth閘道在傳統介面中設定，該閘道使用JSON網頁代號(JWT)交換來取得IMS代號以進行授權。
>
>自2020年4月6日起，不再支援透過舊版OAuth進行設定，且已變更為透過Adobe開發人員控制台進行設定。


>[!TIP]
>
>***僅適用於現有客戶（內部部署和托管服務）***
>
>舊版OAuth閘道設定將可繼續供現有客戶使用。
>
>若您遇到舊版OAuth閘道設定的問題，請刪除現有設定，並透過Adobe開發人員控制台建立新設定。

使用Brand Portal設定AEM Assets的步驟會因您的AEM版本、您是首次設定或升級現有設定而有所不同：

| **AEM版本** | **新配置** | **升級配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [啟用Brand Portal](https://docs.adobe.com/content/help/zh-Hant/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/zh-Hant/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/zh-Hant/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/zh-Hant/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/zh-Hant/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8和更新版本）** | [建立設定](https://helpx.adobe.com/tw/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升級配置](https://helpx.adobe.com/tw/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 聯絡支援 | 聯絡支援 |
