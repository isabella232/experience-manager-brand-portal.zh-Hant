---
title: 訪客存取品牌入口網站
seo-title: 訪客存取品牌入口網站
description: 允許來賓存取並儲存許多不需要驗證的使用者。
seo-description: 允許來賓存取並儲存許多不需要驗證的使用者。
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: Mgulati
topic-tags: 簡介
content-type: 引用
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 訪客存取品牌入口網站 {#guest-access-to-brand-portal}

[!DNL AEM Brand portal] 讓來賓存取入口網站。訪客使用者不需要認證才能進入入口網站，並且可以存取入口網站的公用資產(和系列)。來賓作業中的使用者可將資產新增至其燈箱(私人系列)，並下載相同的內容直到作業階段持續，直到訪客使用者選擇 [結束工作階段](#exit-guest-session)為止，直到工作階段期間為止。

客戶存取功能可讓組織 [快速地將核准的資產](../using/brand-portal-sharing-folders.md#how-to-share-folders) 與目標對象分享，而不需加以安排。[!DNL Brand Portal] 6.4.2附件可提供多名同時使用的來賓使用者，佔每個組織使用者配額的10%。允許來賓存取可節省管理和展示需要使用有限功能的使用者的時間 [!DNL Brand Portal]。\
組織可以使用管理工具面板中存取 [!DNL Brand Portal] 權設定的 **「允許使用者存取」** 選項，啓用(或 **停用** )客戶對組織帳戶的存取權。

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## 開始來賓作業 {#begin-guest-session}

若要匿名進入品牌入口網站，請按一下此處 **** 按一下 **[!UICONTROL 與「訪客存取權」對應的「按一下這裡」嗎？]**[!DNL Brand Portal] 歡迎畫面。使用者不需要存取存取權並等待管理員驗證他們是否授與存取權 [!DNL Brand Portal]。

![](assets/bp-login-screen.png)

## 訪客作業期間 {#guest-session-duration}

來賓使用者工作階段會持續運作小時。這表示 [!UICONTROL 燈箱] 的狀態會保留到工作階段開始時間的小時，而在小時後，目前的來賓作業會重新啓動，因此燈箱狀態會遺失。\
例如，來賓使用者登入1500 [!DNL Brand Portal] 小時，並在16：50小時內將資產新增至燈箱。如果使用者未在17：00小時前下載 [!UICONTROL 燈箱系列(] 或其資產)， [!UICONTROL 燈箱] 將變成空白，因為使用者必須在小時結束時重新啓動工作階段(這是1700小時)。

## 允許的並行訪客作業 {#concurrent-guest-sessions-allowed}

並行來賓作業的數目限制為每個組織的10%使用者配額。也就是說，對於擁有200位使用者配額的組織，最多可同時使用20位使用者。21位使用者被拒絕存取，且只有當20名作用中來賓使用者結束時，才能夠以來賓身分存取。

## 訪客與品牌入口網站的互動 {#guest-user-interaction-with-brand-portal}

### 訪客UI導覽

在輸入 [!DNL Brand Portal] 做為來賓時，使用者可以看到公開共用 [](../using/brand-portal-sharing-folders.md#sharefolders) 的所有資產和資料夾，或僅與來賓使用者共用。此檢視僅為內容檢視，可在卡片、清單或欄版面中顯示資產。

![](assets/disabled-folder-hierarchy1.png)

不過，如果管理員啓用 [!DNL Brand Portal][「Enable Folder階層」(啓用檔案夾階層](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) )配置，「訪客使用者」會看到資料夾樹狀結構(從根資料夾開始)和共用資料夾，這些資料夾會排列在其各自的父資料夾中。

這些父資料夾是虛擬資料夾，無法執行任何動作。您可以使用鎖定圖示辨識這些虛擬資料夾。

與共用資料夾不同的是，在「卡片檢視」中不會顯示任何動作任務，也不會顯示任何動作任務。「概述」按鈕會顯示在選取「欄檢視」和「清單檢視」中的虛擬資料夾。

>[!NOTE]
>
>請注意，虛擬檔案夾的預設縮圖是第一個共用資料夾的縮圖影象。

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

「檢視設定」選項可讓來賓使用者調整卡片檢視或欄中的卡片大小，以顯示在「清單檢視」中。

![](assets/nav-guest-user.png)

「內容」樹狀結構可讓您瀏覽資產階層。

![](assets/guest-login-ui.png)

[!DNL Brand Portal] 提供 **「概述」** 選項給「訪客」使用者，檢視所選資產/檔案夾的資產屬性。「概述」選項可顯示：

1. 位於上方的工具列中，選取資產/檔案夾。
2. 在下拉式清單中，選取「邊欄選擇器」。

在選取資產/資料夾時選取「概述」選項時，使用者可以查看資產建立的標題、路徑和時間。而在資產詳細資料頁面選取「概述」選項時，使用者可查看資產的中繼資料。

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL 左側導軌中的導覽]** 選項可讓您從檔案中導覽至 [!UICONTROL 系列] ，並在來賓作業中返回，如此使用者就可瀏覽檔案或 [!UICONTROL 系列]中的資產。

**篩選** 選項可讓來賓使用者使用管理員設定的搜尋預期詞來篩選資產檔案和資料夾。

### 客群使用者功能

客戶使用者可以存取 [!DNL Brand Portal]公開資產，也沒有其他限制。

來賓使用者可以：

* 存取所有的公開資料夾和 [!UICONTROL 系列][!DNL Brand Portal] 。
* 瀏覽成員、詳細資料頁面，以及所有公開資料夾和 [!UICONTROL 系列成員的完整資產檢視]。
* 在公用資料夾和 [!UICONTROL 系列中搜尋資產]。
* 新增資產至燈箱 [!UICONTROL 集合]。這些 [!UICONTROL 對系列的變更會] 在工作階段期間持續存在。
* 直接下載資產或透過燈箱 [!UICONTROL 集合下載]。

訪客使用者無法：

* 建立 [!UICONTROL 系列] 和儲存的搜尋，或進一步共用。
* 存取資料夾和 [!UICONTROL 系列] 設定。
* 將資產共用為連結。

### 下載來賓作業中的資產

賓客使用者可以直接下載共用的資產，或僅供賓客使用 [!DNL Brand Portal]。來賓使用者也可以將資產新增至 [!UICONTROL Lightbox] (公開 [!UICONTROL 系列])，並在作業過期之前下載 [!UICONTROL 燈箱系列] 。

若要下載資產和 [!UICONTROL 系列]，請從下列位置使用下載圖示：

* 快速動作縮圖，會顯示在資產或 [!UICONTROL 系列上的停留上]
* 上方的工具列，顯示在選取資產或 [!UICONTROL 系列上]

![](assets/download-on-guest.png)

選取 **「在下載上啓用下載加速** 」對話框可讓您 [增強下載效能](../using/accelerated-download.md)。

## 退出來賓作業 {#exit-guest-session}

若要退出來賓作業，請使用標題中可用選項的 **「結束工作階段** 」。不過，如果訪客工作階段使用的瀏覽器標籤為非活動狀態，則作業會在兩小時無活動後自動過期。

![](assets/end-guest-session.png)

## 監控來賓使用者活動 {#monitoring-guest-user-activities}

管理員可以監控來賓使用者與 [!DNL Brand Portal]其互動。產生的 [!DNL Brand Portal] 報表可為來賓使用者活動提供重要見解。例如 **，下載** 報告可用來追蹤來賓使用者下載的資產計數。**使用者登入** 報告可在訪客上次登入入口網站和指定持續時間登入頻率時通知。
