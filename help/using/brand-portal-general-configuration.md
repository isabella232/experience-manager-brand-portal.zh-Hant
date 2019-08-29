---
title: 管理一般租用戶組態
seo-title: 管理一般租用戶組態
description: 設定下載加速，公開智慧[！UICOHTROL系列]建立，公開[！建立UICOHTROL系列，並讓管理員使用者刪除租用戶的資產。
seo-description: 設定下載加速，公開智慧[！UICOHTROL系列]建立，公開[！建立UICOHTROL系列，並讓管理員使用者刪除租用戶的資產。
uuid: 3c46cd7c-c38 b-4bc7-b566-93f977 bc8227
contentOwner: Mgulati
topic-tags: 管理
content-type: 引用
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: f4c237bc-f6 a4-4bc4-af56-3d9 c3027 df4
translation-type: tm+mt
source-git-commit: ea7fdd2df0696ed309227fa77e3f79d0141bcb58

---


# 管理一般租用戶組態 {#administer-general-tenant-configurations}

[!DNL AEM] 資產 [!DNL Brand Portal] 可讓組織為特定租用戶設定下列功能：

* 管理員刪除資產
* 非管理員使用者建立公開 [!UICONTROL 系列]
* 非管理員使用者建立的公開智慧 [!UICONTROL 集合]
* 下載加速
* 非管理員使用者可見共用資料夾的父階層

這些組態已在管理工具面板上提供為 **一般設定** 設定。

![](assets/general-configs.png)

**** A Configuration to allow administrators to delete assets from [!DNL Brand Portal].(預設已啓用)

**B** 設定可讓非管理員使用者建立公用 [!UICONTROL 系列]。(預設已啓用)

**C** Configuration可讓非管理員使用者建立公用智慧 [!UICONTROL 型集合]。(預設已啓用)

**D** Configuration可允許下載從入口網站和共用連結下載的資產。(預設已停用)

**E** Configuration，將共用資料夾的資料夾階層(從根目錄)顯示給非管理員使用者(編輯、檢視者、訪客使用者)。(預設已停用)

## 啓用/停用一般設定 {#enable-disable-general-configurations}

若要啓用/停用每個組態：

1. 以管理員權限登入。
2. 從頂端的工具列選取 [!DNL AEM] 用來存取管理工具的標誌。
3. 從管理工具面板中，選取 **一般** 以開啓 **一般設定** 頁面。
4. 使用個別切換開關啓用/停用任何一般設定。
5. **儲存** 變更。
6. 登出可讓變更生效。

## 允許管理員使用者刪除 [!DNL Brand Portal]{#allow-admin-users-to-delete-assets-from-brand-portal}

**允許使用者刪除** 設定可讓組織允許(或限制)具有管理員權限的使用者刪除資產和資料夾 [!DNL Brand Portal]。

## 允許非管理員建立公用系列 {#allow-public-collections-creation-by-non-admins}

[允許公用 [!UICONTROL 系列]建立](./使用/brand-treal-share-[!UICONTROL collection]. md# main-pars-text-1915052376)設定控制非管理員是否能建立公用 [!UICONTROL 系列][!DNL Brand Portal]。預設會啓用設定。停用組態組織可防止設定組織在其入口網站上有多個公用 [!UICONTROL 系列]，以便儲存系統空間。

## 允許非管理員建立公開智慧型系列 {#allow-public-smart-collections-creation-by-non-admins}

[允許公用智慧型集合建立](../using/brand-portal-searching.md#main-pars-header-500620467) 組態控制非管理員是否可以將其搜尋儲存為智慧 [!UICONTROL 型集合] ，並為該租用戶公開這些搜尋。預設會啓用設定。借由停用組態組織，可防止非管理員使用者建立大量的公開智慧 [!UICONTROL 集合][!DNL Brand Portal]。

## 允許下載加速 {#allow-download-acceleration}

[允許下載加速](../using/accelerated-download.md) 設定可讓組織透過整合為隨選應用程式的IBM AsPera Connect，加速從 [!DNL Brand Portal] 和共用連結下載資產。此應用程式使用專利技術來移除TCP覆蓋。

## 啟用資料夾階層 {#enable-folder-hierarchy}

[「啓用資料夾階層](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) 」設定可讓管理員控制非管理員使用者(編輯、檢視者和來賓使用者)在登入後檢視共用資料夾的方式。
