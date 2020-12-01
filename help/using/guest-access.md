---
title: Brand Portal 的訪客存取
seo-title: Brand Portal 的訪客存取
description: 允許來賓訪問，並節省大量無需驗證的用戶上線的工作。
seo-description: 允許來賓訪問，並節省大量無需驗證的用戶上線的工作。
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 1a8658a3ced4fd211a1c1606a80bb51920ca8be1
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 1%

---


# Brand Portal 的訪客存取 {#guest-access-to-brand-portal}

AEM Brand入口網站可讓訪客存取入口網站。 訪客使用者不需要憑證即可進入入口網站，並可存取入口網站的公用資產（和系列）。 來賓作業中的使用者可將資產新增至燈箱（私人系列）並下載資產，直到其作業持續為止，除非來賓使用者選擇[[!UICONTROL 結束作業]](#exit-guest-session)，否則從作業開始算起2小時。

訪客存取功能可讓組織快速地將核准的資產[與預期的對象大規模共用，而不需上線。 ](../using/brand-portal-sharing-folders.md#how-to-share-folders)Brand Portal 6.4.2版之後，已配備為多個並行來賓用戶提供服務，這是每個組織的用戶配額總量的10%。 允許訪客存取可節省管理和載入大量需要在品牌入口網站上使用有限功能的使用者的時間。\
組織可以使用管理工具面板中的&#x200B;**[!UICONTROL 存取]**&#x200B;設定中的&#x200B;**[!UICONTROL 允許來賓存取]**&#x200B;選項，啟用（或停用）組織品牌入口帳戶的來賓存取。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 開始來賓會話{#begin-guest-session}

若要匿名輸入品牌入口網站，請選擇&#x200B;**[!UICONTROL 按一下此處**[!UICONTROL &#x200B;訪客存取？]**]** 在品牌入口網站歡迎畫面上。輸入catcha安全性檢查，以授與使用品牌入口網站的存取權。

![](assets/bp-login-screen.png)

## 來賓會話持續時間{#guest-session-duration}


來賓用戶會話保持活動狀態15分鐘。
這表示**[!UICONTROL 燈箱]**&#x200B;的狀態會從工作階段開始時間保留15分鐘，並在此之後，目前的來賓會話重新啟動，因此燈箱狀態會丟失。

例如，訪客使用者於15時登入品牌入口網站，並將資產新增至&#x200B;**[!UICONTROL Lightbox]**，於15:05時下載。 如果使用者未在15:15小時（登入後15分鐘內）之前下載&#x200B;**[!UICONTROL Lightbox]**&#x200B;系列（或其資產），使用者就必須重新啟動工作階段。 **[!UICONTROL 燈箱]**&#x200B;將會是空的，這表示如果作業遺失，已上傳的資產將不再可用。

## 允許的併發來賓會話{#concurrent-guest-sessions-allowed}

並行來賓會話的數量限制為每個組織的用戶配額總量的10%。 這表示，對於使用者配額為200的組織，最多可同時使用20位來賓使用者。 第21位用戶被拒絕訪問，並且僅當20位活動來賓用戶的會話結束時才能作為來賓訪問。

## 訪客使用者與品牌入口網站的互動{#guest-user-interaction-with-brand-portal}

### 訪客UI導覽

當以來賓身分進入品牌門戶時，用戶可以公開查看所有[資產和共用的資料夾](../using/brand-portal-sharing-folders.md#sharefolders)或僅與來賓用戶共用。 此檢視是僅限內容的檢視，會在卡片、清單或欄版面中顯示資產。

![](assets/disabled-folder-hierarchy1.png)

但是，如果管理員已啟用[啟用資料夾層次](../using/brand-portal-general-configuration.md#main-pars-header-1621071021)配置，則來賓用戶在登錄到Brand Portal時會看到資料夾樹（從根資料夾開始）和在各自父資料夾內排列的共用資料夾。

這些父資料夾是虛擬資料夾，不能對其執行任何操作。 您可以使用鎖定表徵圖來識別這些虛擬資料夾。

與共用資料夾不同，當懸停或在&#x200B;**[!UICONTROL 卡片視圖]**&#x200B;中選擇操作任務時，不會顯示任何操作任務。 **[!UICONTROL 在「]** 列視圖」和「清單視圖」中選擇虛擬資料夾時， **[!UICONTROL 將]** 顯示「概述 **[!UICONTROL 」按鈕]**。

>[!NOTE]
>
>虛擬資料夾的預設縮略圖是第一個共用資料夾的縮略圖。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL 「檢視]** 設定」選項可讓訪客使用者調整「卡片檢視」欄中的 **[!UICONTROL 卡]** 片大小，以便顯示在「清單 **[!UICONTROL 檢視」中]**。

![](assets/nav-guest-user.png)

**[!UICONTROL 內容樹狀結構]**&#x200B;可讓您在資產階層中移動。

![](assets/guest-login-ui.png)

品牌入口網站提供&#x200B;**[!UICONTROL 概述]**&#x200B;選項給來賓用戶以查看所選資產／資料夾的&#x200B;**[!UICONTROL 資產屬性]**。 顯示&#x200B;**[!UICONTROL 概述]**&#x200B;選項：

* 在頂端的工具列中，選取資產／資料夾時。
* 在下拉式清單中，選取「軌道選擇器」。
在選取資產／資料夾時選取**[!UICONTROL 概述]**&#x200B;選項時，使用者可以看到資產建立的標題、路徑和時間。 但是，在資產詳細資料頁面上，選取&#x200B;**[!UICONTROL 概述]**&#x200B;選項可讓使用者查看資產的中繼資料。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL 左側導]** 覽選項可讓使用者從檔案導覽至系列，然後在來賓作業階段中返回，讓使用者瀏覽檔案或系列中的資產。

**[!UICONTROL 篩選]** 功能可讓來賓用戶使用管理員設定的搜索謂語來篩選資產檔案和資料夾。

### 來賓用戶功能

訪客使用者可以存取品牌入口網站上的公開資產，也沒有進一步討論的限制。

**來賓用戶可以**:

* 存取所有品牌入口網站使用者專用的公開資料夾和系列。
* 瀏覽成員、詳細資料頁，並擁有所有公共資料夾和集合成員的完整資產視圖。
* 在公共資料夾和系列間搜尋資產。
* 將資產新增至燈箱集合。 系列的這些變更會在工作階段期間持續存在。
* 直接下載資產或透過燈箱集合。

**來賓用戶不能**:

* 建立系列和已儲存的搜尋，或進一步共用。
* 存取檔案夾和系列設定。
* 將資產共用為連結。

### 在來賓作業階段中下載資產

來賓使用者可直接在品牌入口網站上公開或獨家下載與來賓使用者共用的資產。 來賓使用者也可以將資產新增至&#x200B;**[!UICONTROL Lightbox]**（公開系列），並在工作階段過期前下載&#x200B;**[!UICONTROL Lightbox]**&#x200B;系列。

若要下載資產和系列，請使用下列網址的下載圖示：

* 快速動作縮圖，此縮圖會顯示在暫留在資產或系列上
* 頂端的工具列，在選取資產或系列時會出現

![](assets/download-on-guest.png)

選擇&#x200B;**[!UICONTROL 在[!UICONTROL 下載]對話方塊上啟用下載加速]**，可讓您[增強下載效能](../using/accelerated-download.md)。

## 退出來賓會話{#exit-guest-session}

要退出來賓會話，請從標題中可用的選項使用&#x200B;**[!UICONTROL 結束會話]**。 不過，如果訪客作業使用的瀏覽器標籤不作用中，則作業會在閒置兩小時後自動過期。

![](assets/end-guest-session.png)

## 監視來賓用戶活動{#monitoring-guest-user-activities}

管理員可監控訪客使用者與品牌入口網站的互動。 在品牌入口網站中產生的報表可提供訪客使用者活動的關鍵見解。 例如，**[!UICONTROL Download]**&#x200B;報表可用來追蹤訪客使用者下載的資產計數。 **[!UICONTROL 使用]** 者登入報表可通知訪客使用者上次登入入口網站的時間，以及指定期間的登入頻率。
