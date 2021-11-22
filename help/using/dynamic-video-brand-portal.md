---
title: Brand Portal 上的動態視訊支援
seo-title: Dynamic video support on Brand Portal
description: Brand Portal 上的動態視訊支援
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 7128c71576ae938a49f9bff0b95b98b7fc480f69
workflow-type: tm+mt
source-wordcount: '1256'
ht-degree: 3%

---

# Brand Portal 上的動態視訊支援 {#dynamic-video-support-on-brand-portal}

透過Dynamic Media支援，在Brand Portal上自適應地預覽和播放影片。 也會從入口網站和共用連結下載動態轉譯。
Brand Portal使用者可以：

* 在「資產詳細資料」頁面、「卡片檢視」和「連結共用預覽」頁面中預覽影片。
* 播放視訊會在「資產詳細資料」頁面上編碼。
* 在「資產詳細資料」頁面的「轉譯」標籤中檢視動態轉譯。
* 下載視訊會對包含視訊的資料夾進行編碼。

>[!NOTE]
>
>若要處理影片並將影片發佈至Brand Portal，請確定您的Experience Manager製作例項是在Dynamic Media混合模式或Dynamic Media上設定 **[!DNL Scene7]** 模式。

若要預覽、播放和下載影片，Brand Portal會向管理員公開下列兩項設定：

* [Dynamic Media混合配置](#configure-dm-hybrid-settings)
如果「Experience Manager製作」例項在「動態媒體混合」模式中執行。
* [Dynamic Media [!DNL Scene7] 配置](#configure-dm-scene7-settings)
如果Experience Manager製作例項在動態媒體上執行 — **[!DNL Scene7]** 模式。
根據您在複製Brand Portal租戶的「Experience Manager製作」例項中設定的設定，來設定其中一項設定。

>[!NOTE]
>
>設定了「Experience Manager作者」且在上執行的Brand Portal租戶不支援動態影片 **[!UICONTROL Scene7Connect]** 運行模式。

## 如何播放動態影片？ {#how-are-dynamic-videos-played}

![從雲端擷取視訊編碼](assets/VideoEncodes.png)

如果Dynamic Media設定([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 設定)，則會從擷取動態轉譯 **[!DNL Scene7]** 伺服器。 因此，視頻編碼是預視和播放的，在質量上沒有延遲和失真。

由於視訊編碼不會儲存在Brand Portal存放庫中，因此會擷取 **[!DNL Scene7]** 伺服器上，請確定Adobe Experience Manager製作執行個體和Brand Portal上的Dynamic Media設定相同。

>[!NOTE]
>
>Brand Portal不支援視訊檢視器和檢視器預設集。 影片會在Brand Portal的預設檢視器中預覽及播放。

## 必備條件 {#prerequisites}

若要在Brand Portal上使用動態影片，請務必：

* **在Dynamic Media模式上啟動Experience Manager作者**
啟動Experience Manager製作例項(已設定Brand Portal)，位於 [Dynamic Media - [!DNL Scene7] 模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 或 [Dynamic Media — 混合模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 或
* **在Experience Manager作者上設定Dynamic MediaCloud Services**
根據Dynamic Media模式(Scene7模式或混合模式)Experience Manager作者正在執行，請設定 [Dynamic MediaCloud Services([!DNL Scene7] 模式)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) 或 [Dynamic MediaCloud Services（混合模式）](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) Experience Manager作者來源 **工具** | **Cloud Services** | **Dynamic Media**.
* **在Brand Portal上設定Dynamic Media**
根據Dynamic Media雲端設定在Experience Manager作者上，設定 [Dynamic Media設定](#configure-dm-hybrid-settings) 或 [[!DNL Scene7] 設定](#configure-dm-scene7-settings)  從Brand Portal管理工具。
確保 [獨立Brand Portal租戶](#separate-tenants) 用於在Dynamic Media中設定的Experience Manager製作例項 —  **[!UICONTROL Scene7]** 模式和Dynamic Media — 混合模式。 尤其是使用Dynamic Media功能時 **[!UICONTROL S7]** 和Dynamic Media混合。
* **套用視訊編碼的發佈資料夾至Brand Portal**
套用 [視訊編碼](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 和從「Experience Manager製作」例項將包含多媒體資產的資料夾發佈至Brand Portal。
* **允許清單在啟用安全預覽時在SPS中輸出IP**
若使用Dynamic Media -**[!DNL Scene7]** ( [已啟用安全預覽](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) )，則建議 **[!DNL Scene7]** 公司管理員 [允許列出公開輸出IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 針對使用SPS的個別區域(**[!UICONTROL Scene7]** 發佈系統)flash UI。
輸出IP如下：

| **區域** | **輸出IP** |
|--- |--- |
| 不適用 | 130.248.160.68, 20.94.203.130 |
| 歐洲、中東和非洲 | 185.34.189.3, 51.132.146.75 |
| APAC | 63.140.44.54 |

若要允許列出其中一個輸出IP，請參閱 [準備安全測試服務的帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## 最佳作法

若要確保您的動態視訊資產能從Brand Portal（和共用連結）成功預覽、播放和下載，請遵循下列實務：

### Dynamic Media的獨立租戶 — Scene7和Dynamic Media — 混合模式 {#separate-tenants}

如果您同時使用Dynamic Media - **[!DNL Scene7]** 模式和Dynamic Media — 混合模式功能，針對使用Dynamic Media設定的「Experience Manager作者」例項，使用不同的Brand Portal租戶 —  **[!DNL Scene7]** 和Dynamic Media — 混合模式。


![作者與BP一對一映射](assets/BPDynamicMedia.png)

### 與Experience Manager製作例項和Brand Portal的設定詳細資料相同

確保Brand Portal和 **[!UICONTROL Experience Manager雲端設定]**. 相同的設定詳細資訊包括下列項目：

* **[!UICONTROL 標題]**
* **[!UICONTROL 註冊 ID]**
* **[!UICONTROL 視訊服務URL]** in **[!UICONTROL Dynamic Media — 混合模式]**
* **[!UICONTROL 標題]**
* 憑據(**[!UICONTROL 電子郵件]** 和密碼)
* **[!UICONTROL 區域]**
* **[!UICONTROL 公司]** 在Dynamic Media- **[!DNL Scene7]** 模式

### 允許列出Dynamic Media Scene7模式的公用輸出IP

如果Dynamic Media **[!UICONTROL Scene7]**-having [已啟用安全預覽](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) — 用於將視訊資產提供給Brand Portal，然後 **[!UICONTROL Scene7]** 為測試環境或內部應用程式建立專用的映像伺服器。 對此伺服器的任何請求都會檢查來源IP位址。 如果傳入的請求不在核准的IP位址清單內，則會傳回失敗回應。
此 **[!UICONTROL Scene7]** 因此，公司管理員會為其公司的 **[!UICONTROL 安全測試]** 環境，透過 **[!UICONTROL SPS]** (Scene7 Publishing System)flash UI。 請確定已將您各自地區的輸出IP（來自下列）新增至該已核准清單。
若要允許列出其中一個輸出IP，請參閱 [準備安全測試服務的帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
輸出IP如下：

| **區域** | **輸出IP** |
|--- |--- |
| 不適用 | 130.248.160.66, 52.151.32.108 |
| 歐洲、中東和非洲 | 185.34.189.1 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media（混合）設定 {#configure-dm-hybrid-settings}

如果Experience Manager製作例項在動態媒體混合模式上執行，請使用 **[!UICONTROL 影片]** 從「管理工具」面板平鋪，以配置Dynamic Media閘道設定。

>[!NOTE]
>
>此 [視訊編碼設定檔](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 不會發佈至Brand Portal，而是會從 **[!UICONTROL Scene7]** 伺服器。 因此，若要讓視訊編碼在Brand Portal中成功播放，請確定設定詳細資訊與 [Dynamic MediaCloud Services([!DNL Scene7] 模式)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-scene7-mode/config-dms7.html?lang=en#configuring-dynamic-media-cloud-services) 在Experience Manager製作例項中。

若要在Brand Portal租戶上設定Dynamic Media設定：

1. 選取Experience Manager標誌，以便從Brand Portal頂端的工具列存取管理工具。
1. 從管理工具面板中，選取 **[!UICONTROL 影片]** 方塊。

   ![Dynamic Media Brand Portal上的混合設定](assets/DMHybrid-Video.png)

   **[!UICONTROL 編輯Dynamic Media設定]** 頁面開啟。

   ![Dynamic Media Brand Portal上的混合設定](assets/edit-dynamic-media-config.png)

1. 指定 **[!UICONTROL 註冊ID]** 和 **[!UICONTROL 視訊服務URL]** （DM — 閘道URL）。 請確定這些詳細資料與 **[!UICONTROL 工具>Cloud Services]** 在Experience Manager製作例項中。
1. 選擇 **儲存** 以儲存設定。

## 配置Dynamic Media Scene7設定 {#configure-dm-scene7-settings}

如果Experience Manager製作例項在Dynamic Media上執行 —  **[!UICONTROL Scene7]** 模式，然後使用 **[!UICONTROL Dynamic Media設定]** 從「管理工具」面板建立磁貼以配置 **[!UICONTROL Scene7]** 伺服器設定。

設定Dynamic Media **[!UICONTROL Scene7]** Brand Portal租戶的設定：

1. 選取Experience Manager標誌，以便從Brand Portal頂端的工具列存取管理工具。

2. 從管理工具面板中，選取 **[!UICONTROL Dynamic Media設定]** 方塊。

   ![DM [!UICONTROL 場景7] Brand Portal的設定](assets/DMS7-Tile.png)

   **[!UICONTROL 編輯Dynamic Media設定]** 頁面開啟。

   ![Brand Portal上的Scene 7設定](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 標題]**
   * 憑據(**[!UICONTROL 電子郵件ID]** 和 **[!UICONTROL 密碼]**)以存取Scene7伺服器
   * **[!UICONTROL 區域]**

   請確定這些值與您在Experience Manager製作例項中找到的值相同。

4. 選擇 **[!UICONTROL 連線至Dynamic Media]**.

5. 提供 **[!UICONTROL 公司名稱]**，和 **[!UICONTROL 儲存]** 設定。
