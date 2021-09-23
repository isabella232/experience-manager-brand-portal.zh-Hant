---
title: Brand Portal 的訪客存取
seo-title: Guest Access to Brand Portal
description: 允許來賓訪問，無需驗證即可將眾多用戶上線。
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: e7877973da87362c5fddd6c3aa8135719eff044a
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 1%

---

# Brand Portal 的訪客存取 {#guest-access-to-brand-portal}

Experience ManagerAssets Brand Portal允許訪客存取入口網站。 來賓使用者不需要憑證即可進入入口網站，且可存取入口網站的公開資產（和集合）。 來賓工作階段中的使用者可以將資產新增至燈箱（私人收集）並下載資產，直到其工作階段持續為止；除非來賓使用者選擇[[!UICONTROL 結束工作階段]](#exit-guest-session)，否則工作階段從工作階段開始算起2小時。

訪客存取功能可讓組織以大規模快速將已核准資產](../using/brand-portal-sharing-folders.md#how-to-share-folders)與目標對象共用，而不需將其上線。 [Brand Portal 6.4.2以上版本已配備多個同時使用的訪客使用者，即每個組織總使用者配額的10%。 允許訪客存取可節省時間，在Brand Portal上管理和上架的幾十名功能有限的使用者。\
組織可以使用管理工具面板中的&#x200B;**[!UICONTROL Access]**&#x200B;設定中的&#x200B;**[!UICONTROL 允許來賓訪問]**&#x200B;選項，對組織的Brand Portal帳戶啟用（或停用）來賓訪問。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 開始來賓會話 {#begin-guest-session}

要匿名輸入Brand Portal，請選擇&#x200B;**[!UICONTROL 按一下這裡]**&#x200B;與&#x200B;**[!UICONTROL 來賓訪問相對應？]** 在Brand Portal歡迎畫面上。輸入驗證碼安全性檢查，以授與使用Brand Portal的存取權。

![](assets/bp-login-screen.png)

## 來賓會話持續時間 {#guest-session-duration}


來賓用戶會話保持活動狀態15分鐘。
這表示從會話開始時間起，**[!UICONTROL Lightbox]**&#x200B;的狀態將保留15分鐘，並在此後，當前來賓會話重新啟動，因此Lightbox狀態將丟失。

例如，訪客使用者於15時登入Brand Portal，並將資產新增至&#x200B;**[!UICONTROL Lightbox]**，以便於15:05時下載。 若使用者在15:15小時（登入後15分鐘內）之前(未下載&#x200B;**[!UICONTROL Lightbox]**&#x200B;集合（或其資產），使用者必須重新啟動工作階段。 **[!UICONTROL Lightbox]**&#x200B;空白，這表示如果工作階段遺失，已上傳的資產將不再可用。

## 允許的同時來賓會話 {#concurrent-guest-sessions-allowed}

同時訪客會話的數量限制為每組織用戶配額總數的10%。 這表示，對於用戶配額為200的組織，最多可以同時工作20個來賓用戶。 第21個用戶被拒絕訪問，只有在20個活動來賓用戶的會話結束時，才能作為來賓訪問。

## 與Brand Portal的訪客使用者互動 {#guest-user-interaction-with-brand-portal}

### 來賓UI導航

以來賓身分進入Brand Portal時，使用者可以公開或僅看到與來賓使用者共用的所有[資產和資料夾](../using/brand-portal-sharing-folders.md#sharefolders)。 此檢視是僅限內容的檢視，會以卡片、清單或欄配置顯示資產。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理員已啟用[啟用資料夾階層](../using/brand-portal-general-configuration.md#main-pars-header-1621071021)組態，則訪客使用者在登入Brand Portal時會看到資料夾樹（從根資料夾開始）和排列在其各自父資料夾中的共用資料夾。

這些父資料夾是虛擬資料夾，不能對其執行任何操作。 您可以使用鎖表徵圖識別這些虛擬資料夾。

暫留或在&#x200B;**[!UICONTROL 卡片檢視]**&#x200B;中選取時，不會顯示任何動作任務，這點與共用資料夾不同。 **** 在「欄檢視」和「清單檢視」中選取虛擬資料 **[!UICONTROL 夾時]** 會顯示 **[!UICONTROL 「概觀」按鈕]**。

>[!NOTE]
>
>虛擬資料夾的預設縮圖是第一個共用資料夾的縮圖影像。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 「檢]** 視設定」選項可讓訪客使用者調整「卡片檢視」中的 **[!UICONTROL 卡]** 片大小，或欄以在「清單檢 **[!UICONTROL 視」中顯示]**。

![](assets/nav-guest-user.png)

**[!UICONTROL 內容樹狀結構]**&#x200B;可讓您在資產階層中移動。

![](assets/guest-login-ui.png)

Brand Portal提供&#x200B;**[!UICONTROL 概述]**&#x200B;選項給來賓使用者，供他們檢視所選資產/資料夾的&#x200B;**[!UICONTROL 資產屬性]**。 **[!UICONTROL 概述]**&#x200B;選項可見：

* 在頂端的工具列中選取資產/資料夾。
* 在下拉式清單中選取「邊欄選取器」。

在選取資產/資料夾時選取&#x200B;**[!UICONTROL 概述]**&#x200B;選項時，使用者可以看到資產建立的標題、路徑和時間。 而在資產詳細資料頁面上選取&#x200B;**[!UICONTROL 概述]**&#x200B;選項，可讓使用者查看資產的中繼資料。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**** 左側邊欄的導覽選項可讓使用者從檔案導覽至集合，以及在來賓工作階段中返回，讓使用者可以瀏覽檔案或集合中的資產。

**** 篩選功能可讓訪客使用者使用管理員設定的搜尋述詞來篩選資產檔案和資料夾。

### 來賓用戶功能

訪客使用者可存取Brand Portal上的公用資產，也沒有其他限制。

**來賓用戶可以**:

* 存取所有Brand Portal使用者專用的所有公用資料夾和集合。
* 瀏覽成員、詳細資訊頁，並擁有所有公用資料夾和集合成員的完整資產視圖。
* 在公用資料夾和集合間搜尋資產。
* 新增資產至燈箱集合。 對集合所做的這些變更會在工作階段期間持續存在。
* 直接下載資產或透過燈箱集合下載資產。

**來賓用戶不能**:

* 建立集合和已儲存的搜尋，或進一步共用。
* 訪問資料夾和集合設定。
* 以連結形式共用資產。

### 在來賓工作階段中下載資產

訪客使用者可直接下載公開或專供訪客使用者在Brand Portal上共用的資產。 來賓使用者也可以將資產新增至&#x200B;**[!UICONTROL Lightbox]**（公開集合），並在工作階段過期前下載&#x200B;**[!UICONTROL Lightbox]**&#x200B;集合。

若要下載資產和集合，請使用下載圖示：

* 快速動作縮圖，顯示在將游標暫留在資產或集合上
* 頂端的工具列，會顯示在選取資產或集合時

![](assets/download-on-guest.png)

在[!UICONTROL 下載]對話方塊中選擇&#x200B;**[!UICONTROL 啟用下載加速]** ，可讓您[提升下載效能](../using/accelerated-download.md)。

## 退出來賓會話 {#exit-guest-session}

要退出來賓會話，請從標頭中可用的選項中使用&#x200B;**[!UICONTROL 結束會話]**。 不過，如果用於訪客工作階段的瀏覽器索引標籤非作用中，則工作階段閒置兩小時後會自動過期。

![](assets/end-guest-session.png)

## 監視來賓用戶活動 {#monitoring-guest-user-activities}

管理員可監控訪客使用者與Brand Portal的互動。 在Brand Portal中產生的報表可提供訪客使用者活動的重要深入分析。 例如，**[!UICONTROL Download]**&#x200B;報表可用來追蹤訪客使用者下載的資產計數。 **[!UICONTROL 使]** 用者登入報表可通知訪客使用者上次登入入口網站的時間，以及指定期間的登入頻率。
