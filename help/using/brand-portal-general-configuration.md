---
title: 管理一般租用戶組態
seo-title: Administer general tenant configurations
description: 配置下載加速、公共智慧集合建立、公共集合建立，並使管理員用戶能夠刪除租戶上的資產。
seo-description: Configure download acceleration, public smart collection creation, public collection creation, and enable admin users to delete assets on tenants.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# 管理一般租用戶組態 {#administer-general-tenant-configurations}

Experience Manager AssetsBrand Portal允許組織為特定租戶配置以下功能：

* 管理員刪除資產
* 非管理員用戶建立公共集合
* 非管理員用戶建立公共智慧集合
* 對非管理員用戶可見的共用資料夾的父層次結構

這些配置已提供為 **[!UICONTROL 常規設定]** 「管理工具」面板上的配置。

![](assets/general-config.png)

**A**   允許管理員從Brand Portal刪除資產的配置。 （預設為啟用）

**B**   允許非管理員用戶建立公共集合的配置。 （預設為啟用）

**C**   允許非管理員用戶建立公共智慧集合的配置。 （預設為啟用）

**D**  將共用資料夾的資料夾層次結構（從根目錄）顯示給非管理員用戶（編輯器、查看器、來賓用戶）的配置。 （預設為禁用）

## 啟用/禁用常規配置 {#enable-disable-general-configurations}

要啟用/禁用這些配置中的每個：

1. 以管理員權限登錄。
1. 從頂部工具欄中選擇Experience Manager徽標以訪問管理工具。
1. 從管理工具面板中，選擇 **[!UICONTROL 常規]** 開啟 **[!UICONTROL 常規設定]** 的子菜單。
1. 使用相應的切換開關啟用/禁用任何常規配置。
1. **[!UICONTROL 儲存變更。]**
1. 註銷以使更改生效。

## 允許管理員用戶從Brand Portal刪除資產 {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL 允許用戶刪除]** 配置使組織能夠允許（或限制）具有管理員權限的用戶從Brand Portal刪除資產和資料夾。

## 允許非管理員建立公共集合 {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL 允許建立公共集合]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) 配置控制非管理員是否可以在Brand Portal上建立公共集合。 預設情況下啟用配置。 通過禁用配置組織，可以阻止其門戶上有大量公共集合，以便節省系統空間。

## 允許非管理員建立公共智慧集合 {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL 允許建立公共智慧集合]](../using/brand-portal-searching.md#main-pars-header-500620467) 配置控制非管理員是否可以將其搜索保存為智慧集合併將其公開給該租戶。 預設情況下啟用配置。 通過禁用配置，組織可以防止在組織的Brand Portal上擁有大量由非管理員用戶建立的公共智慧集合。

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## 啟用資料夾階層 {#enable-folder-hierarchy}

[[!UICONTROL 啟用資料夾層次結構]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 配置允許管理員控制非管理員用戶（編輯器、查看器和來賓用戶）登錄後如何查看共用資料夾。
