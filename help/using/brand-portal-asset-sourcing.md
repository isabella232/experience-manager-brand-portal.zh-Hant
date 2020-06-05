---
title: Asset Sourcing in Brand Portal
seo-title: Asset Sourcing in Brand Portal
description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: 資產
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 465b80ada85284ab0379e4a5922def32fffbfeb2
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---


# Asset Sourcing overview {#overview-asset-sourcing-in-bp}

**Asset Sourcing** allows AEM users (administrators/non-admin users) to create new folders with an additional **Asset Contribution** property, ensuring the new folder created open to asset submission by Brand Portal users. This automatically triggers a workflow which creates two additional sub folders, called **SHARED** and **NEW**, within the newly created **Contribution** folder. The AEM Administrator then defines the requirement by uploading a brief about the types of assets that should be added to the contribution folder, as well as a set of baseline assets, to the **SHARED** folder to ensure BP users have the reference information they need. The administrator can then grant active Brand Portal users access to the contribution folder before publishing the newly created **Contribution** folder to Brand Portal. Once the user is finished adding content in the **NEW** folder, they can publish the contribution folder back to the AEM author environment. Please note that it may take a few minutes to complete the import and reflect the newly published content within AEM Assets.

此外，所有現有功能都保持不變。 品牌入口網站使用者可從貢獻資料夾以及其他許可的資料夾檢視、搜尋及下載資產。 此外，管理員還可以進一步共用貢獻資料夾、修改屬性並將資產新增至系列。

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

>[!NOTE]
>
>AEM 6.5.2.0和更新版本支援品牌入口網站中的資產採購。
>
>舊版不支援此功能- AEM 6.3和AEM 6.4。
>
>Contact Adobe support to upgrade your AEM instance to the latest supported AEM version.


![Brand Portal Asset Sourcing](assets/asset-sourcing.png)


>[!NOTE]
>
>AEM 6.5.4中有已知問題。 品牌入口網站使用者無法在升級至Adobe Developer Console時，將貢獻資料夾的資產發佈至AEM Assets。
>
>AEM 6.5.5中的問題已修正。 您可以在Adobe Developer Console上將AEM Assets實例升級至最新的Service Pack AEM 6.5.5, [並升級您的組態](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 。
>
>如需AEM 6.5.4的立即修正，建議您下載 [修補程式](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，並安裝在您的作者實例上。


## 必備條件 {#prerequisites}

* AEM 6.5.0.2或更新版本。
* 請確定您的AEM Assets例項已設定為品牌入口網站。 See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## 另請參閱 {#reference-articles}

**For administrators**

* [Configure Asset Sourcing in AEM](brand-portal-configure-asset-sourcing.md)
* [Upload Brand Portal users list](brand-portal-configure-asset-sourcing.md)
* [Configure contribution folder](brand-portal-contribution-folder.md)
* [Upload baseline assets to contribution folder](brand-portal-upload-baseline-assets.md)
* [Publish contribution folder to Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**For Brand Portal users**

* [下載資產需求](brand-portal-download-asset-requirements.md)
* [Upload new assets to contribution folder](brand-portal-upload-assets-to-contribution-folder.md)
* [Publish contribution folder to AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
