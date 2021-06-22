---
title: 加速Brand Portal下載
seo-title: 加速Brand Portal下載
description: 提升從Brand Portal和共用連結的下載效能。
seo-description: 提升從Brand Portal和共用連結的下載效能。
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
exl-id: cf28df58-c6dd-4b12-8279-01351892009f
source-git-commit: 6e6d771e93a3b76f72548f1a3cc61d75e31342ad
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 2%

---

# 加速Brand Portal下載{#guide-to-accelerate-downloads-from-brand-portal}

Adobe Experience Manager Assets Brand Portal可與IBM Aspera Connect（隨需安裝應用程式）整合，以增強大型資產檔案的下載效能。 應用程式使用專有技術來消除TCP開銷，並幫助提高資產檔案的傳輸速度。 此整合可確保增強的下載體驗。

>[!NOTE]
>
>下載速度因網路頻寬、伺服器延遲和客戶端地理位置等因素而異。

預設會啟用&#x200B;**[!UICONTROL 快速下載]**&#x200B;設定，大幅縮短從Brand Portal下載所需資產檔案所花的時間。

![](assets/download-settings-new.png)

## 加速檔案下載的先決條件{#prerequisites-to-accelerate-file-download}

若要更快下載檔案，請確定下列事項：

* 導覽至&#x200B;**[!UICONTROL Tools]** > **[!UICONTROL Download]**&#x200B;並確認&#x200B;**[!UICONTROL Fast Download]**&#x200B;組態已在&#x200B;**[!UICONTROL Download Settings]**&#x200B;中啟用。
* 確保在防火牆上開啟埠33001（TCP和UDP）。 有關先決條件的詳細資訊，請參閱[ IBM Aspera Connect Client文檔](https://downloads.asperasoft.com/en/documentation/8)。
* [使用管理員權限在瀏覽器的擴充功能中安裝IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) 。
* 有關Aspera傳輸客戶端的平台支援，請參閱[ IBM Aspera Connect平台支援矩陣](https://www.asperasoft.com/company/support/transfer-clients/)。

## 下載域{#download-domains}

以下是不同地理位置的下載網域：

| 地區代碼 | 網域 |
|---|---|
| NA或1 | downloads-na1.brand-portal.adobe.com |
| 不適用VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## 使用檔案加速器{#expected-download-performance-using-file-accelerator}的下載效能示例

下表顯示使用Aspera Connect檔案下載加速器的2 GB檔案下載效能：

*由於Brand Portal伺服器位於奧勒岡州（美國），觀察到的結果確實會因網路頻寬、伺服器延遲和用戶端位置等因素而有所不同。*

| 用戶端位置 | 客戶端和伺服器之間的延遲（毫秒） | 使用Aspera連接檔案傳輸加速器(MBps)實現速度 | 下載具有Aspera檔案傳輸加速器的2 GB檔案所花的時間（秒） |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| 美國西部（加利福尼亞北） | 18 | 36 | 57 |
| 美國西部（俄勒岡） | 42 | 36 | 57 |
| 美國東（維吉尼亞北） | 85 | 35 | 58 |
| APAC（東京） | 124 | 36 | 57 |
| 諾伊達（印度） | 275 | 13.36 | 153 |
| 雪梨 | 175 | 29 | 70 |
| 倫敦 | 179 | 35 | 58 |
| 新加坡 | 196 | 34 | 60 |

## 使用檔案加速器{#download-workflow-using-file-accelerator}下載工作流

若要更快從Brand Portal下載資產：

1. 登入您的Brand Portal租用戶。 依預設，會開啟&#x200B;**[!UICONTROL 檔案]**&#x200B;檢視，其中包含所有已發佈的資產和資料夾。

   執行下列任一操作：

   * 選取您要下載的資產或資料夾。 從頂端的工具列按一下&#x200B;**[!UICONTROL Download]**&#x200B;圖示。

      ![select-multiple assets](assets/select-assets-new.png)

   * 若要下載資產的特定資產轉譯，請將指標暫留在資產上，然後按一下快速動作縮圖中可用的&#x200B;**[!UICONTROL 下載]**&#x200B;圖示。

      ![select-asset](assets/select-asset.png)

1. 會開啟&#x200B;**[!UICONTROL 下載]**&#x200B;對話方塊，列出所有選取的資產。

   若要在下載資產時保留Brand Portal資料夾階層，請選取「為每個資產建立個別資料夾」核取方塊。****

   下載按鈕會反映所選項目的計數。 套用完規則後，按一下「**[!UICONTROL 下載項目]**」。 若要進一步了解如何套用規則，請參閱[下載資產](../using/brand-portal-download-assets.md#download-assets)。

   ![下載對話](assets/download-dialog-box-new.png)

1. 預設情況下，在&#x200B;**[!UICONTROL 下載設定]**&#x200B;中啟用了&#x200B;**[!UICONTROL 快速下載]**&#x200B;設定。 因此，確認方塊會顯示為使用IBM Aspera Connect下載資產。

   如果您是第一次下載資產，且瀏覽器中未安裝IBM Aspera Connect，或現有版本已過期，系統會提示您[安裝Aspera下載加速器](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html)。

   ![](assets/aspera-not-launched.png)

1. **安裝Aspera Connect Client**

   要安裝IBM Aspera Connect客戶端安裝程式，請從IBM Aspera Connect客戶端應用程式的.msi檔案中運行安裝程式，並遵循安裝嚮導。

   ![](assets/aspera-download-1.png)

1. 成功安裝用戶端後，請重新整理瀏覽器頁面並重新開始下載步驟。

1. 若要繼續使用&#x200B;**[!UICONTROL 快速下載]**，請按一下&#x200B;**[!UICONTROL 允許]**。 所有選定的轉譯都使用IBM Aspera Connect下載到zip資料夾中。

   下載成功後，對話方塊會顯示資產下載至使用者系統的位置。

   ![](assets/aspera-download-2.png)

   如果您不想使用IBM Aspera Connect，請按一下&#x200B;**[!UICONTROL Deny]**。 如果拒絕或失敗&#x200B;**[!UICONTROL 快速下載]**，系統會填入錯誤訊息。 按一下&#x200B;**[!UICONTROL 一般下載]**&#x200B;按鈕以繼續下載資產。

>[!NOTE]
>
>如果管理員關閉了&#x200B;**[!UICONTROL Fast Download]**&#x200B;設定，則選定的格式副本將直接下載到zip資料夾中，而不使用IBM Aspera Connect。

<!-- 
On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.


1. Log in to Brand Portal using a supported browser.
1. Browse and select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon. the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** and **[!UICONTROL Enable download acceleration]** check boxes selected by default. 

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >The functionality to send email notification with the link to download assets is presently not supported while faster downloads are enabled.

   ![](assets/fast-download-emailchk.png)

1. Click **[!UICONTROL Download]**.

   To speed up the download experience on your Brand Portal tenant account, you need to have Aspera Connect client application installed in your browser's extension.

1. **Download Aspera Connect Client**

   If Aspera Connect client is not installed on your system or the existing Aspera Connect client is out of date, a prompt is displayed on the browser page from where you can download the system-specific Aspera Connect client by selecting **[!UICONTROL Download Latest Version]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

1. **Install Aspera Connect Client**

   To install IBM Aspera Connect client setup, run the setup from  .msi  file of IBM Aspera Connect client application and follow the installation wizard.

1. Once the client is successfully installed, refresh the browser page and initiate the download steps again.

   When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. To skip this dialog in future, enable **[!UICONTROL Remember my choice for FASP links]**.

   >[!NOTE]
   >
   >This message is different on the different browsers.

1. A dialog box confirms whether to proceed the transfer or not. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Download begins. A dialog box shows the progress of the download. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
Aspera Connect application provides an Activity Window on the system where user can view and manage all transfer sessions. For more information, refer [Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.
-->

## 在Microsoft Edge瀏覽器{#using-file-accelerator-on-microsoft-edge-browser}上使用檔案加速器

Microsoft Edge在增強保護模式(EPM)下運行，在同一專用網路或受信任站點上，該模式阻止與Aspera Connect伺服器通信。 因此，每次與伺服器建立連線時，都會顯示快顯視窗。

![](assets/switchapps-msedge.png)

若要在Microsoft Edge上使用加速下載功能，請從受信任的網站清單中移除Brand Portal網站。

1. 開啟「控制面板」（**[!UICONTROL Window key + X]**，然後選擇&#x200B;**[!UICONTROL 「控制面板」]**）。
1. 轉至&#x200B;**[!UICONTROL 網路和Internet]** > **[!UICONTROL Internet選項]**。 按一下&#x200B;**[!UICONTROL Security]**&#x200B;標籤。
1. 按一下&#x200B;**[!UICONTROL 受信任站點區域]**，然後按一下&#x200B;**[!UICONTROL 站點]**。
1. 從清單中移除Brand Portal網站。

## Aspera連接客戶端首選項{#aspera-connect-client-preferences}

通過按一下右鍵表徵圖並選擇&#x200B;**[!UICONTROL 首選項]**，可以在IBM Aspera連接客戶端首選項中設定一些有用的首選項。

![](assets/download_assets_frombrandportalimg19.png)

您可以設定預設的下載位置。

![](assets/aspera-preferences.png)

此外，Aspera Connect客戶端可標籤為在系統啟動時自動啟動，以便連接客戶端正在運行，並且可供下載以更快開始。

![](assets/aspera-automaticallylaunch.png)

## 下載加速{#troubleshoot-issues-with-download-acceleration}的疑難排解問題

如果下載加速無法供您使用，請依照下列步驟進行疑難排解：

1. 通過從電腦訪問[https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/)檢查埠是否未被阻止。

   如果埠不正常，請聯繫您的網路團隊，確保防火牆中沒有阻止埠33001（TCP和UDP）。

1. 如果埠正常，則使用[https://www.speedtest.net/](https://www.speedtest.net/)測量可用頻寬來檢查網路是否不慢。

   如果頻寬為幾(1-10 Mbps)或以每秒位元組數表示，則使用Aspera首選項並嘗試將頻寬限制為等於可用頻寬。

1. 若要確認來自Aspera示範伺服器的下載是否正常運作，請使用[https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user)。\
   （登入） asperaweb ，密碼： demoaspera)

1. 如果上述疑難排解步驟皆無法運作，請取消選取「啟用下載加速」選項，然後使用一般下載。
