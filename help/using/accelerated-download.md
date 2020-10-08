---
title: 加速品牌入口網站下載
seo-title: 加速品牌入口網站下載
description: 增強品牌入口網站和共用連結的下載效能。
seo-description: 增強品牌入口網站和共用連結的下載效能。
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 2%

---


# 加速品牌入口網站下載 {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal與IBM Aspera Connect整合，讓大型資產檔案的下載效能得以提升，後者是隨選安裝應用程式。 該應用程式使用專有技術來消除TCP開銷，並幫助提高資產檔案的傳輸速度。 此整合可確保增強的下載體驗。

>[!NOTE]
>
>下載速度因網路頻寬、伺服器延遲和用戶端地理位置等因素而異。

預設 **[!UICONTROL 會啟用「快速下載]** 」設定，這可大幅降低從品牌入口網站下載所需資產檔案所花的時間。

![](assets/download-configuration.png)

## 加速檔案下載的必要條件 {#prerequisites-to-accelerate-file-download}

若要更快速下載檔案，請確定下列事項：

* 導覽至「 **[!UICONTROL 工具]** >下載 **[!UICONTROL 」，並確認「下載設定」中已啟]** 用「快速下載 **[!UICONTROL 」]******&#x200B;設定。
* 埠33001（TCP和UDP）在防火牆上開啟。 如需先決條件的詳細資訊，請參 [閱Aspera Connect用戶端檔案](https://downloads.asperasoft.com/en/documentation/8)。
* 使用管理員權限安裝Aspera Connect。
* 如需Aspera傳輸用戶端的平台支援，請參 [閱Aspera Connect平台支援表](https://www.asperasoft.com/company/support/transfer-clients/)。

## 下載網域 {#download-domains}

以下是不同地理位置的下載網域：

| 地區代碼 | 網域 |
|---|---|
| 不適用或1 | downloads-na1.brand-portal.adobe.com |
| 北美VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| 亞太SIN2 | downloads-apac1.brand-portal.adobe.com |

## 使用檔案加速器的下載效能範例 {#expected-download-performance-using-file-accelerator}

下表顯示使用Aspera Connect檔案下載加速器的2 GB檔案下載效能：

*觀察到的結果會因網路頻寬、伺服器延遲和用戶端位置等因素而有所不同，因為Brand Portal伺服器位於俄勒岡（美國）。*

| 用戶端位置 | 客戶端與伺服器之間的延遲（毫秒） | 使用Aspera Connect檔案傳輸加速器(MBps)加速 | 下載含Aspera檔案傳輸加速器的2 GB檔案所花的時間（秒） |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| 美國西部（北美）加州) | 18 | 36 | 57 |
| 美國西部（俄勒岡） | 42 | 36 | 57 |
| 美國東部(N.維吉尼亞) | 85 | 35 | 58 |
| 亞太地區（東京） | 124 | 36 | 57 |
| Noida（印度） | 275 | 13.36 | 153 |
| 雪梨 | 175 | 29 | 70 |
| 倫敦 | 179 | 35 | 58 |
| 新加坡 | 196 | 34 | 60 |

## 使用檔案加速器下載工作流程 {#download-workflow-using-file-accelerator}

若要更快速地從品牌入口網站下載資產：

1. 使用支援的瀏覽器登入品牌入口網站。
1. 瀏覽並選取您要下載的檔案夾或資產。 從頂端的工具列，按一下「下 **[!UICONTROL 載]** 」圖示。 此時 **[!UICONTROL 會出現]** 「下載」對話方塊，並依預設選取「資 **[!UICONTROL 產]** 」和「 **** 啟用下載加速」核取方塊。

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >目前不支援傳送電子郵件通知及下載資產連結的功能，同時啟用更快速的下載。

   ![](assets/fast-download-emailchk.png)

1. 按一 **[!UICONTROL 下下載]**。

   若要加速品牌入口網站租用戶帳戶的下載體驗，您必須在瀏覽器的擴充功能中安裝Aspera Connect用戶端應用程式。

1. **下載Aspera Connect用戶端**

   如果您的系統未安裝Aspera Connect用戶端，或現有Aspera Connect用戶端已過時，瀏覽器頁面上會顯示提示，您可從此處選取「下載最新版本」來下載系統特定的Aspera Connect用戶端 ****。

   ![](assets/aspera-not-launched.png)

   若要從https://downloads.asperasoft.com/connect2/下載最新版Aspera Connect [，請選取「](https://downloads.asperasoft.com/connect2/)Download Now **[!UICONTROL (立即下載]** )」並依照指示進行。

1. **安裝Aspera Connect客戶端**

   要安裝IBM Aspera Connect客戶端設定，請從IBM Aspera Connect客戶端應用程式的。msi檔案運行設定，然後遵循安裝嚮導。

1. 成功安裝客戶機後，請刷新瀏覽器頁面並再次啟動下載步驟。

   首次使用Aspera Connect時，瀏覽器會提示使用 **[!UICONTROL IBM Aspera Connect開啟連結]**。 若要在未來略過此對話方塊，請啟 **[!UICONTROL 用「記住我對FASP連結的選擇」]**。

   >[!NOTE]
   >
   >這則訊息在不同的瀏覽器上不同。

1. 對話框確認是否繼續傳輸。 選擇 **[!UICONTROL 允許]** ，開始。
要在將來跳過此對話框，請啟 **[!UICONTROL 用「使用我的選項來連接此主機」]**。
下載開始。 對話方塊顯示下載進度。 使用對話方塊 **[!UICONTROL 暫停]**、繼 **[!UICONTROL 續]**&#x200B;或 **[!UICONTROL 取消]** 下載。
Aspera Connect應用程式提供系統上的「活動視窗」，讓使用者可檢視和管理所有傳輸作業。 如需詳細資訊，請參 [閱Aspera Connect用戶端檔案](https://downloads.asperasoft.com/en/documentation/8)。

![](assets/aspera-activity-window.png)

成功完成下載後，對話方塊會顯示資產下載至使用者系統的位置。 如果發生故障，則顯示錯誤。

>[!NOTE]
>
>Aspera Connect用戶端應用程式有已知的限制，如果在「偏好設定」的標籤「傳輸」下啟用「永遠詢問我要將下載的檔案儲存在何處 **[!UICONTROL 」，就不會出現選取下載位置的提示]**********。 在開始下載之前，請在「將下載的檔案儲存至」文字方塊中 **[!UICONTROL 提供位置]**。

## 在Microsoft Edge瀏覽器上使用檔案加速器 {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge以增強保護模式(EPM)運行，在同一專用網路或受信任站點上，防止與Aspera Connect伺服器通信。 因此，每次建立與伺服器的連線時，都會出現快顯視窗。

![](assets/switchapps-msedge.png)

若要在Microsoft Edge上使用加速下載功能，請從受信任的網站清單中移除品牌入口網站。

1. 開啟「控制面板」(**[!UICONTROL 視窗鍵+ X]**，然後選 **[!UICONTROL 取「控制面板]**」)。
1. 前往「網 **[!UICONTROL 路與網際網路]** >網 **[!UICONTROL 際網路選項」]**。 按一下「安 **[!UICONTROL 全性]** 」標籤。
1. 按一下「受 **[!UICONTROL 信任的網站]**」區域，然後按 **[!UICONTROL 一下「網站]**」。
1. 從清單中移除品牌入口網站。

## Aspera Connect用戶端偏好設定 {#aspera-connect-client-preferences}

在IBM Aspera Connect Client偏好設定中，可以使用滑鼠右鍵按一下圖示並選取「偏好設定」，來設定一些有用的 **[!UICONTROL 偏好設定]**。

![](assets/download_assets_frombrandportalimg19.png)

您可以設定預設的下載位置。

![](assets/aspera-preferences.png)

此外，Aspera Connect用戶端也可以標籤為在系統啟動時自動啟動，如此連線用戶端就會執行，並可供下載，開始更快速。

![](assets/aspera-automaticallylaunch.png)

## 疑難排解下載加速的問題 {#troubleshoot-issues-with-download-acceleration}

如果下載加速無法為您運作，請依照下列步驟進行疑難排解：

1. 請從您的機器造訪https://test-connect.asperasoft.com，以檢查 [是否未封鎖](https://test-connect.asperasoft.com/) 埠。

   如果埠不正常，請聯繫您的網路團隊，並確保Ports 33001（包括TCP和UDP）未在防火牆中被阻止。

1. 如果埠正常，則使用https://www.speedtest.net/測量可用頻寬，檢查網路是否不 [慢](https://www.speedtest.net/)。

   如果頻寬為幾(1-10 Mbps)或Kbps，則使用Aspera偏好設定並嘗試限制等於可用頻寬的頻寬。

1. 若要確認從Aspera示範伺服器下載是否正常運作，請使用https://demo.asperasoft.com/aspera/user [](https://demo.asperasoft.com/aspera/user)。\
   (登入： asperweb，密碼： 德摩斯佩拉

1. 如果上述疑難排解步驟無法運作，請取消選取「啟用下載加速」選項，然後使用一般下載。
