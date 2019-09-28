---
title: 品牌入口網站的訪客存取
seo-title: Guest Access to Brand Portal
description: 允許來賓訪問，並節省大量無需驗證的用戶上線的工作。
seo-description: Allow guest access and save the effort to onboard numerous users who do not need to be authenticated.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: 引用
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Guest Access to Brand Portal {#guest-access-to-brand-portal}

AEM Brand portal allows guest access to the portal. A guest user doesn't need credentials to enter the portal and has access to the public assets (and collections) of the portal. Users in the guest session can add assets to their lightbox (private collection) and download the same until their session lasts, which is 2 hours from the beginning of the session unless the guest user chooses to [!UICONTROL End Session].[](#exit-guest-session)

訪客存取功能可讓組織 [快速地與目標對象共用已核准的資產](../using/brand-portal-sharing-folders.md#how-to-share-folders) ，而不需將其上線。 Brand Portal 6.4.2版之後，已配備為多個並行來賓用戶提供服務，這是每個組織的用戶配額總量的10%。 允許訪客存取可節省管理和載入大量需要在品牌入口網站上使用有限功能的使用者的時間。\
Organizations can enable (or disable) guest access on Brand Portal account of the organization using Allow Guest Access option from Access settings in the administrative tools panel.********

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Begin guest session {#begin-guest-session}

To enter Brand Portal anonymously, select Click here corresponding to Guest Access?******** 在品牌入口網站歡迎畫面上。 使用者不需要尋找存取權，並等待管理員驗證他們，以授與使用品牌入口網站的存取權。

![](assets/bp-login-screen.png)

## 來賓會話持續時間 {#guest-session-duration}

來賓用戶會話保持活動狀態2小時。 這表示燈箱的狀態會保留到 [!UICONTROL Lightbox] 1小時後開始，而在2小時後，目前的來賓作業會重新啟動，因此燈箱狀態會遺失。\
例如，訪客使用者於15時登入品牌入口網站，並將資產新增至Lightbox，於16時50分下載。 如果使用者未在17:00之前下載 [!UICONTROL Lightbox] 集合（或其資產）, [!UICONTROL Lightbox] 將會變成空白，因為使用者必須在1小時結束時（即1700小時）重新啟動工作階段。

## 允許併發來賓會話 {#concurrent-guest-sessions-allowed}

並行來賓會話的數量限制為每個組織的用戶配額總量的10%。 這表示，對於使用者配額為200的組織，最多可同時使用20位來賓使用者。 第21位用戶被拒絕訪問，並且僅當20位活動來賓用戶的會話結束時才能作為來賓訪問。

## Guest使用者與品牌入口網站的互動 {#guest-user-interaction-with-brand-portal}

### 訪客UI導覽

在以來賓身分進入品牌入口網站時，使用者可以看到所有公 [開共用的資產和資料夾](../using/brand-portal-sharing-folders.md#sharefolders) ，或只與來賓使用者共用。 此檢視是僅限內容的檢視，會在卡片、清單或欄版面中顯示資產。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理員已啟用「啟用資料夾層次結構」配置，來賓用戶在登錄到Brand Portal時會看到資料夾樹（從根資料夾開始）和在各自父資料夾內排列的共用資料夾 [](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) 。

這些父資料夾是虛擬資料夾，不能對其執行任何操作。 You can recognize these virtual folders with a lock icon.

No action tasks are visible on hovering or selecting them in Card View, unlike the shared folders. [!UICONTROL Overview button is shown on selecting a virtual folder in Column View and List View.]

>[!NOTE]
>
>Note that the default thumbnail of the virtual folders is the thumbnail image of the first shared folder.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL 「檢視設定] 」選項可讓訪客使用者調整「卡片檢視」中的卡片大小， [!UICONTROL 或欄位可顯示] 在「清單檢視」中 。

![](assets/nav-guest-user.png)

「內 [!UICONTROL 容」樹狀結構] ，可讓您在資產階層中移動。

![](assets/guest-login-ui.png)

品牌入口網站 [!UICONTROL 提供] 「概述」選項給來賓用戶， [!UICONTROL 以檢視所選資產] /資料夾的資產屬性。 「概 [!UICONTROL 述] 」選項可見：

* 在頂端的工具列中，選取資產／資料夾時。
* 在下拉式清單中，選取「軌道選擇器」。
在選取資 [!UICONTROL 產] /資料夾時選取「概述」選項時，使用者可以看到資產建立的標題、路徑和時間。 但是，在資產詳細資料頁面上，選取「 [!UICONTROL 概述] 」選項可讓使用者查看資產的中繼資料。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL 左側導覽]** (Navigation)選項可讓使用者從檔案導覽至系列，然後在來賓工作階段中返回，讓使用者瀏覽檔案或系列中的資產。

**[!UICONTROL Filter option allows guest users to filter asset files and folders using search predicates set by the administrator.]**

### 來賓用戶功能

訪客使用者可以存取品牌入口網站上的公開資產，也沒有進一步討論的限制。

來賓用戶可以：

* 存取所有品牌入口網站使用者專用的公開資料夾和系列。
* 瀏覽成員、詳細資料頁，並擁有所有公共資料夾和集合成員的完整資產視圖。
* 搜尋公共資料夾和系列中的資產。
* 將資產新增至燈箱集合。 系列的這些變更會在工作階段期間持續存在。
* download assets directly or through lightbox collection.

Guest users cannot:

* 建立系列和儲存的搜尋，或進一步共用。
* access folder and collections settings.
* share assets as links.

### 在來賓作業階段中下載資產

Guest users can directly download assets shared publically or exclusively with guest users on Brand Portal. 來賓使用者也可以將資產新增至 [!UICONTROL Lightbox] （公開系列），並在工作階段過期前下載 [!UICONTROL Lightbox] 系列。

若要下載資產和系列，請使用下列網址的下載圖示：

* 快速動作縮圖，此縮圖會顯示在暫留在資產或系列上
* 工具列，此工具列會出現在選取資產或系列時

![](assets/download-on-guest.png)

在「 **[!UICONTROL 下載]** 」對話方 [!UICONTROL 塊中選取「啟用下載加速] 」，可 [以增強下載效能](../using/accelerated-download.md)。

## 退出來賓會話 {#exit-guest-session}

要退出來賓會話，請使用 **[!UICONTROL 標題中可用選項的「結束會話]** 」。 不過，如果訪客作業使用的瀏覽器標籤不作用中，則作業會在閒置兩小時後自動過期。

![](assets/end-guest-session.png)

## 監控來賓用戶活動 {#monitoring-guest-user-activities}

管理員可監控訪客使用者與品牌入口網站的互動。 在品牌入口網站中產生的報表可提供訪客使用者活動的關鍵見解。 例如，「 **[!UICONTROL 下載]** 」報表可用來追蹤訪客使用者下載的資產計數。 **[!UICONTROL 「使用者登入]** 」報表可通知訪客使用者上次登入入口網站的時間，以及指定期間內的登入頻率。
