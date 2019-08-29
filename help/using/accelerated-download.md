---
title: 加速從品牌入口網站下載的指南
seo-title: 加速從品牌入口網站下載的指南
description: 從品牌入口網站和共用連結增強下載效能。
seo-description: 從品牌入口網站和共用連結增強下載效能。
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: Mgulati
topic-tags: 下載安裝
content-type: 引用
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bc145 zed0 c0
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 加速從品牌入口網站下載的指南 {#guide-to-accelerate-downloads-from-brand-portal}

品牌入口網站支援透過整合IBM Assa Connect(這是隨選應用程式)來加速大型資產檔案的下載。此應用程式使用專利技術來移除TCP覆蓋，並有助於改善檔案傳輸速度，進而確保下載體驗。分布各地的使用者若遇到延遲，也可以從這項功能中獲益。

>[!NOTE]
>
>IBM Assera Connect可讓您快速從品牌入口網站和共用連結下載大型資產檔案，但下載速度可能視不同因素(例如網路頻寬、伺服器延遲和客戶地理位置)而有所不同。

若要設定加速檔案下載的特定租件，管理員 **[!UICONTROL 可從管理工具]** 面板中 **的一般設定** 啓用「下載加速」(依預設停用)。

如果啓用此功能，品牌入口網站使用者可透過安裝Assera Connect用戶端，大幅降低從品牌入口網站或透過共用連結下載所需資產檔案的時間。

![](assets/enable-fast-file-download.png)

## 加速檔案下載的必要條件 {#prerequisites-to-accelerate-file-download}

若要使用更快速的檔案下載功能，請確定：

* 連接埠33001(TCP&amp; UDP)由管理員在防火牆中開啓。如需使用IBM Assera Connect的必要條件，請參閱 [Assera Connect用戶端文件](https://downloads.asperasoft.com/en/documentation/8)。

   以下是不同地理區域的下載網域：

   | 區域 | 網域 |
   |---|---|
   | 北美或北美 | downloads-na1.brand-portal.adobe.com |
   | 北美VA5 | downloads-na2.brand-portal.adobe.com |
   | EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
   | APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

* 系統管理員權限會用來下載IBM AsPera Connect安裝程式套件，因為您無法在「來賓」帳戶下安裝Assera Connect。

### 系統和瀏覽器需求 {#system-and-browser-requirements}

AsPera Connect3.8.0的系統和瀏覽器需求如下：

| ﻿OS | OS版本 | 瀏覽器 |  | 必要程式庫 |
|----------------|----------------------------------------|-------------------|-------|--------------------------|
| Windows | Windows7、8、10 | Chrome | 64-66 |  |
|  | Windows Server2008，R2，2012R2，2016 | Firefox | 57-60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Internet Explorer | 11 |  |
|  |  | Microsoft Edge | 39-42 |  |
| macOS作業系統 | 10.11 - 10.13 | Chrome | 64-66 |  |
|  |  | Firefox | 57-60 |  |
|  |  | Firefox ESR | 52 |  |
|  |  | Safari | 11 |  |
| Linux(64位元) | RHEL-7 | Chrome | 64-66 | OpenSSL1.0.2g或更新版本 |
|  | CentOS-7 |  |  | Mesa EGL |
|  | Debian-9 |  |  | glib2.28或更新版本 |
|  | SLES11-12 |  |  |  |
|  | Fedora26-27 |  |  |  |
|  | openSUSE42.3 | Firefox | 57-60 |  |
|  | Ubuntu14-17 | Firefox ESR | 52 |  |

如需不同版本Assera傳輸用戶端的平台支援矩陣，請參閱 [Assera Connect平台支援矩陣](https://www.asperasoft.com/company/support/transfer-clients/)。

## 使用檔案加速器預期下載效能 {#expected-download-performance-using-file-accelerator}

在不同用戶端位置使用Assera Connect檔案下載加速器的2GB檔案下載效能如下：在美國奧勒崗，考慮品牌入口網站伺服器：

| 用戶端位置 | 用戶端與伺服器之間的延遲 | 使用Assera檔案傳輸加速器加快速度 | 使用Assera檔案傳輸加速器下載2GB檔案的時間 |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| U.S. West(N. California) | 18毫秒 | 36MB/s | 57秒 |
| U.S. West(Oregon) | 42毫秒 | 36MB/s | 57秒 |
| U.S. 東部(N. Virginia) | 85毫秒 | 35MB/s | 58秒 |
| 亞太地區(東京) | 124毫秒 | 36MB/s | 57秒 |
| Noida | 275毫秒 | 13.36MB/s | 153秒 |
| 雪梨 | 175毫秒 | 29MB/s | 70秒 |
| 倫敦 | 179毫秒 | 35MB/s | 58秒 |
| 新加坡 | 196毫秒 | 34MB/s | 60秒 |

>[!NOTE]
>
>引用的資料是根據實驗室中進行的測試而定，僅供指示。觀察到的結果因網路頻寬、伺服器延遲和用戶端位置等因素而異。

## 使用檔案加速器下載工作流程 {#download-workflow-using-file-accelerator}

若要更快從品牌入口網站下載資產：

1. 透過偏好的瀏覽器登入品牌入口網站。
2. 瀏覽並選取要下載的資產檔案、資料夾或系列。點選/點選下載選項。
「下載」對話方塊會出現，並選取 [「啓用下載加速] 」選項。
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >目前不支援傳送內含下載資產連結的電子郵件通知，同時啓用更快速的下載。

   ![](assets/fast-download-emailchk.png)

3. 點選/按一下 **「下載**」。
若要加速您的品牌入口用戶帳戶上的下載體驗，您必須在系統上安裝Assera Connect用戶端應用程式。

4. **下載AsPera Connect用戶端：**如果您的系統未安裝AsPera
Connect用戶端，或已安裝的AsPera Connect用戶端過期，則瀏覽器頁面上會出現提示，您可以從下載系統特定的AsPera Connect用戶端下載 **最新版本**。

   ![](assets/aspera-not-launched.png)

   若要從 [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/)下載最新版本的AsPera Connect，請選取 **「立即下載」** 並依照指示進行。

5. **安裝Assera Connect用戶端**若要安裝IBM
Assa Connect用戶端設定，請從IBM AsPera Connect用戶端應用程式的. msi檔案執行設定，然後遵循安裝精靈。

6. 成功安裝用戶端後，重新整理瀏覽器頁面並重新啓動下載步驟，或選取「 **在** 資產 **下載中重新啓動」** 對話方塊(步驟#2)。
第一次使用Assera Connect時，瀏覽器會提示您使用 **IBM Assera Connect開啓連結**。若要在未來跳過此對話方塊，請記住 **我的FASP連結選擇**。

   >[!NOTE]
   >
   >此訊息在不同瀏覽器上不同。

7. 對話方塊會確認是否繼續傳輸。選取 **「允許** 」開始。
若要在未來略過此對話方塊，請啓用 **此主機**的所有連線。
下載開始。對話方塊會顯示下載進度。使用對話方塊 **暫停**、 **繼續**&#x200B;或 **取消** 下載。
Assera Connect應用程式提供系統上的「活動視窗」，使用者可檢視並管理所有傳輸工作階段。如需詳細資訊，請參閱 [AsPera Connect用戶端文件](https://downloads.asperasoft.com/en/documentation/8)。

![](assets/aspera-activity-window.png)

在下載完成後，對話方塊會顯示下載資產至使用者系統的位置。如果發生失敗，則會顯示錯誤。

>[!NOTE]
>
>在「偏好設定」中，如果 **「永遠詢問我儲存下載檔案的位置** 」位於 **「偏好設定」中的標籤** Transmissions**下方，您**&#x200B;就不會出現Asperia Connect用戶端應用程式的已知限制。在任何下載開始之前，請在文字方塊中提供位置，將下載的檔案 **儲存**&#x200B;至。

## 在Microsoft Edge瀏覽器上使用檔案加速器 {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge可在增強保護模式(EPM)中執行，防止與Aspera Connect伺服器通訊，同時在同一個私人網路或受信任網站上進行通訊。因此，每次與伺服器連線時，就會顯示快顯視窗。

![](assets/switchapps-msedge.png)

若要在Microsoft Edge上使用加速下載功能，請從受信任的網站清單移除品牌入口網站。

1. 開啓「控制台」(按 **視窗鍵+ X**，然後選取 **「控制台」**)。
2. 前往 **網路和網際網路&gt;網際網路選項**。按一下 **「安全性** 」標籤。
3. 按一下 **受信任網站區域**，然後按一下 **網站**。
4. 從清單中移除品牌入口網站網站。

## Assera Connect用戶端偏好設定 {#aspera-connect-client-preferences}

有一些有用的偏好設定可在IBM AsPera Connect用戶端偏好設定中設定，方法是按一下圖示並選取 **偏好設定**。

![](assets/download_assets_frombrandportalimg19.png)

您可以設定預設下載位置。

![](assets/aspera-preferences.png)

此外，Assera Connect用戶端可標示為在系統啓動時自動啓動，讓連線用戶端執行並可供下載開始更快。

![](assets/aspera-automaticallylaunch.png)

## 疑難排解下載加速問題 {#troubleshoot-issues-with-download-acceleration}

如果下載加速無法供您使用，請依照下列步驟進行疑難排解：

1. 請從電腦瀏覽 [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) ，檢查連接埠是否未被封鎖。

   如果連接埠不確定，請聯絡您的網路團隊，並確定連接埠33001(TCP&amp; UDP)不會在防火牆中封鎖。

2. 如果連接埠是「確定」，則請使用 [https://www.speedtest.net/測量可用頻寬，檢查網路是否緩慢](https://www.speedtest.net/)。

   如果頻寬為少數(1-10Mbps)或Kbps，則使用Assera Preferences並嘗試限制頻寬等於可用頻寬。

3. 若要確認從Assera展示伺服器下載是否正常運作，請使用 [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user)。\
   (登入：asperaweb，password：demasperia)

4. 如果上述疑難排解步驟沒有作用，請取消選取「啓用下載加速」選項並使用正常下載。
