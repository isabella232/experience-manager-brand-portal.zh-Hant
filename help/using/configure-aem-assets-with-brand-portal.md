---
title: 透過 Brand Portal 設定 Experience Manager Assets
seo-title: Configure Experience Manager Assets with Brand Portal
description: 深入瞭解Experience Manager Assets與Brand Portal的配置。
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 454b05c05359a2068cc29124f826d5bd25a1bad1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 5%

---

# 透過 Brand Portal 設定 Experience Manager Assets {#configure-integration}

將Adobe Experience Manager資產配置為Brand Portal可為Brand Portal用戶啟用資產發佈、資產分配和資產貢獻功能。 它允許Experience Manager Assets用戶向Brand Portal用戶發佈和分發資產。 Brand Portal用戶可以訪問共用資產，並將新資產上載到資產貢獻資料夾並將其發佈回Experience Manager Assets。

支援將Experience Manager Assets配置為Brand Portal:

* Experience Manager Assetsas a Cloud Service
* Experience Manager Assets（現場及管理服務）6.5及以上

Experience Manager Assetsas a Cloud Service通過從雲管理器激活Brand Portal自動配置為Brand Portal。 激活工作流在後端建立所需的配置，並在與Experience Manager Assetsas a Cloud Service實例相同的IMS組織上激活Brand Portal。

然而，Experience Manager Assets（內部和托管服務）使用Adobe Developer控制台手動配置為Brand Portal，該控制台為Brand Portal租戶授權採購AdobeIdentity Management服務(IMS)令牌。

>[!NOTE]
>
>***用於Experience Manager Assets6.5及以上***
>
>此前，Brand Portal通過舊式OAuth網關在經典介面中配置，該網關使用JSON Web令牌(JWT)交換來獲取IMS令牌進行授權。
>
>從2020年4月6日起不再支援通過舊式OAuth進行配置，而是通過Adobe Developer控制台進行配置。


>[!TIP]
>
>***僅針對現有客戶（內部和托管服務）***
>
>舊式OAuth網關配置將繼續為現有客戶工作。
>
>如果舊式OAuth網關配置遇到問題，請刪除現有配置，並通過Adobe Developer控制台建立新配置。

將AEM Assets配置為Brand Portal的步驟AEM因您的版本以及您是首次配置還是升級現有配置而異：

| **版AEM本** | **新配置** | **升級配置** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [激活Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM6.5(6.5.4.0及以上)** | [建立設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
