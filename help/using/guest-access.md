---
title: Brand Portal 的訪客存取
seo-title: Guest Access to Brand Portal
description: 允許來賓訪問，並將工作量保存到無身份驗證的機載眾多用戶。
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 51dc6f9c3b3a59751d7910513279e52906d97b88
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# Brand Portal 的訪客存取 {#guest-access-to-brand-portal}

Experience Manager Assets·Brand Portal允許客人訪問門戶。 來賓用戶不需要憑據即可進入門戶，並且可以訪問門戶的公共資產（和集合）。 來賓會話中的用戶可以將資產添加到燈箱（私有集合）並下載該資產，直到其會話持續為止，除非來賓用戶選擇 [[!UICONTROL 結束會話]](#exit-guest-session)。

來賓訪問功能使組織能夠 [快速共用批准的資產](../using/brand-portal-sharing-folders.md#how-to-share-folders) 讓目標受眾在不必載他們的情況下實現。 Brand Portal6.4.2以後已裝備為多個併發來賓用戶服務，佔每個組織用戶配額總數的10%。 允許客戶訪問可節省時間，以管理和在Brand Portal的功能有限的用戶數量。\
組織可以使用組織的Brand Portal帳戶啟用（或禁用）來賓訪問 **[!UICONTROL 允許來賓訪問]** 選項 **[!UICONTROL 訪問]** 的子菜單。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 開始來賓會話 {#begin-guest-session}

要匿名輸入Brand Portal，請選擇 **[!UICONTROL 按一下這裡]** 對應 **[!UICONTROL 來賓訪問？]** 在Brand Portal的歡迎螢幕上。 輸入驗證碼安全檢查以授予使用Brand Portal的權限。

![](assets/bp-login-screen.png)

## 來賓會話持續時間 {#guest-session-duration}


來賓用戶會話保持活動狀態15分鐘。
這意味著 **[!UICONTROL 燈箱]** 會話開始時間後保留15分鐘，此後當前來賓會話將重新啟動，因此Lightbox狀態將丟失。

例如，來賓用戶在15時登錄到Brand Portal，並將資產添加到 **[!UICONTROL 燈箱]** 供15時05分下載。 如果用戶未下載 **[!UICONTROL 燈箱]** 在15:15小時（登錄後15分鐘內）之前收集（或其資產），用戶必須重新啟動會話。 的 **[!UICONTROL 燈箱]** 為空，這意味著如果會話丟失，上載的資產將不再可用。

## 允許併發來賓會話 {#concurrent-guest-sessions-allowed}

併發來賓會話的數量限制為每個組織用戶配額總數的10%。 這意味著，對於用戶配額為200的組織，最多可以同時使用20個來賓用戶。 第21個用戶被拒絕訪問，並且僅當20個活動來賓用戶中任何一個的會話結束時，才能作為來賓訪問。

>[!NOTE]
>
>如果許可用戶數超過合同值（配額）,Brand Portal不發送通知。 此外，它不限制許可用戶的任何活動。

## 來賓用戶與Brand Portal的交互 {#guest-user-interaction-with-brand-portal}

### 來賓UI導航

當以訪客身份進入Brand Portal時，用戶可以看到 [資產和資料夾共用](../using/brand-portal-sharing-folders.md#sharefolders) 公開或只與來賓用戶共用。 此視圖是僅內容視圖，它在卡、清單或列佈局中顯示資產。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理員已啟用，來賓用戶將在登錄到Brand Portal時看到資料夾樹（從根資料夾開始）和在各自父資料夾中排列的共用資料夾 [啟用資料夾層次結構](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 配置。

這些父資料夾是虛擬資料夾，不能對它們執行任何操作。 您可以使用鎖定表徵圖識別這些虛擬資料夾。

懸停或在中選擇操作任務時不可見 **[!UICONTROL 卡視圖]**，與共用資料夾不同。 **[!UICONTROL 概述]** 中選擇虛擬資料夾時顯示 **[!UICONTROL 列視圖]** 和 **[!UICONTROL 清單視圖]**。

>[!NOTE]
>
>虛擬資料夾的預設縮略圖是第一個共用資料夾的縮略圖。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 查看設定]** 選項允許來賓用戶在 **[!UICONTROL 卡視圖]** 或列顯示在 **[!UICONTROL 清單視圖]**。

![](assets/nav-guest-user.png)

的 **[!UICONTROL 內容樹]** 允許您在資產層次結構中移動。

![](assets/guest-login-ui.png)

Brand Portal **[!UICONTROL 概述]** 選項，供來賓用戶查看 **[!UICONTROL 資產屬性]** 資料夾。 的 **[!UICONTROL 概述]** 選項可見：

* 在頂部的工具欄中，選擇資產/資料夾。
* 在下拉清單中，選擇「Rail Selector（滑軌選擇器）」。

選擇 **[!UICONTROL 概述]** 選項，則用戶可以查看資產建立的標題、路徑和時間。 而在資產詳細資訊頁面上選擇 **[!UICONTROL 概述]** 選項，用戶可查看資產的元資料。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL 導航]** 選項允許在來賓會話中從檔案導航到集合，然後返回，以便用戶可以瀏覽檔案或集合中的資產。

**[!UICONTROL 篩選]** 選項允許來賓用戶使用管理員設定的搜索謂詞篩選資產檔案和資料夾。

### 來賓用戶權能

來賓用戶可以訪問Brand Portal的公共資產，也很少有進一步討論的限制。

**來賓用戶可以**:

* 訪問所有針對所有Brand Portal用戶的公用資料夾和集合。
* 瀏覽成員、詳細資訊頁面，並擁有所有公共資料夾和集合成員的完整資產視圖。
* 跨公共資料夾和集合搜索資產。
* 將資產添加到Lightbox集合。 對集合的這些更改在會話期間持續。
* 直接或通過Lightbox集合下載資產。

**來賓用戶不能**:

* 建立收藏和保存的搜索，或進一步共用它們。
* 訪問資料夾和集合設定。
* 將資產作為連結共用。

### 在來賓會話中下載資產

來賓用戶可以直接下載與來賓用戶在Brand Portal共用或專用共用的資產。 來賓用戶還可以將資產添加到 **[!UICONTROL 燈箱]** （公共集合），並下載 **[!UICONTROL 燈箱]** 在其會話過期之前收集。

要下載資產和收藏，請使用下載表徵圖：

* 快速操作縮略圖，顯示在資產或集合上方
* 頂部的工具欄，在選擇資產或收集時顯示

![](assets/download-on-guest.png)

選擇 **[!UICONTROL 啟用下載加速]** 上 [!UICONTROL 下載] 對話框 [提高下載效能](../using/accelerated-download.md)。

## 退出來賓會話 {#exit-guest-session}

要退出來賓會話，請使用 **[!UICONTROL 結束會話]** 的子菜單。 但是，如果用於來賓會話的瀏覽器頁籤處於非活動狀態，則會話在處於非活動狀態兩小時後自動過期。

![](assets/end-guest-session.png)

## 監視來賓用戶活動 {#monitoring-guest-user-activities}

管理員可以監視來賓用戶與Brand Portal的交互。 在Brand Portal生成的報告可提供客戶用戶活動的關鍵洞見。 比如說， **[!UICONTROL 下載]** 報告可用於跟蹤來賓用戶下載的資產計數。 **[!UICONTROL 用戶登錄]** 報告可以通知來賓用戶上次登錄門戶的時間以及指定持續時間內的登錄頻率。
