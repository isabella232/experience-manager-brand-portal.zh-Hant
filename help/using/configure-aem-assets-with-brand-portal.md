---
title: 使用品牌入口網站設定AEM資產
seo-title: 使用品牌入口網站設定AEM資產
description: 深入瞭解如何使用品牌入口網站設定AEM資產。
seo-description: 深入瞭解如何使用品牌入口網站設定AEM資產。
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: eba4ee138d4f594c4c446a3cc8941f04fd46902c

---


# 使用品牌入口網站設定AEM資產 {#configure-integration}

Adobe Experience Manager(AEM)Assets是透過Adobe I/O以品牌入口網站設定，Adobe I/O會購買IMS Token以授權您的品牌入口網站租用戶。 此設定可讓品牌入口網站使用者使用資產發佈、資產分發和資產貢獻功能。

>[!NOTE]
>
>之前，品牌入口網站是透過舊版OAuth閘道在傳統使用者介面中設定，該閘道使用JWT代號交換來取得IMS存取代號以進行授權。
>
>自2020年4月6日起，不再支援透過舊版OAuth進行的設定，並變更為透過Adobe I/O進行設定。
>
>如果您是舊版OAuth閘道上具備設定的現有品牌入口網站使用者，建議您刪除現有的設定並在Adobe I/O上建立新的設定。
>
>但是，如果不修改配置，現有配置將繼續工作。

設定具有品牌入口網站的AEM資產的步驟依您的AEM版本而異，以及您是首次設定或升級現有的設定：

| **AEM版本** | **新設定** | **升級配置** |
|---|---|---|
| **AEM 6.5（6.5.4.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#Upgradeconfiguration) |
| **AEM 6.4（6.4.8.0和更新版本）** | [建立設定](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [升級配置](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#Upgradeconfiguration) |
| **AEM 6.3（6.3.3.8和更新版本）** | [建立設定](https://helpx.adobe.com/in/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [升級配置](https://helpx.adobe.com/in/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | 聯絡支援 | 聯絡支援 |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
