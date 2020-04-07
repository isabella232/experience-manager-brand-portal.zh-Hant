---
title: 使用品牌入口網站設定AEM資產
seo-title: 使用品牌入口網站設定AEM資產
description: 深入瞭解如何使用品牌入口網站設定AEM資產。
seo-description: 深入瞭解如何使用品牌入口網站設定AEM資產。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 75d69f85a4178b78eba15a13f865a602e73d3a88

---


# 使用品牌入口網站設定AEM資產 {#configure-integration}

Adobe Experience Manager(AEM)Assets是透過Adobe I/O以品牌入口網站設定，Adobe I/O會購買IMS Token以授權您的品牌入口網站租用戶。 AEM Assets雲端服務、AEM Assets 6.3及更新版本現在支援品牌入口網站。

設定AEM Assets可以與品牌入口網站一起服務，讓您可以與品牌入口網站使用者一起發佈和分發資產。 但是，在AEM 6.3（及更新版本）上設定品牌入口網站可讓品牌入口網站使用者使用資產發佈、資產分發和資產貢獻功能。

>[!NOTE]
>
>***針對AEM Assets 6.3和更新版本***
>
>之前，品牌入口網站是透過舊版OAuth閘道在傳統使用者介面中設定，該閘道使用JWT代號交換來取得IMS存取代號以進行授權。
>
>自2020年4月6日起，不再支援透過舊版OAuth進行的設定，並變更為透過Adobe I/O進行設定。


>[!TIP]
>
>***僅限現有客戶***
>
>建議您繼續使用現有的舊版OAuth閘道設定。 萬一您遇到舊版OAuth閘道設定的問題，請刪除現有的設定，並透過Adobe I/O建立新的設定。


設定具有品牌入口網站的AEM資產的步驟依您的AEM版本而異，以及您是首次設定或升級現有的設定：

| **AEM版本** | **新設定** | **升級配置** |
|---|---|---|
| **AEM Assets 雲端服務** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brandportal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5（6.5.4.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4（6.4.8.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3（6.3.3.8和更新版本）** | [建立設定](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升級配置](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 聯絡支援 | 聯絡支援 |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
