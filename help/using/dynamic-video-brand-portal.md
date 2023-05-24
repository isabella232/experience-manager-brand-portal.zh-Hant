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
source-git-commit: f56918ea8eb14ba04b7e141f4f1cae318e532512
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 4%

---

# Brand Portal 上的動態視訊支援 {#dynamic-video-support-on-brand-portal}

在Dynamic Media支援下，在Brand Portal自適應地預覽和播放視頻。 還可以從門戶和共用連結下載動態格式副本。
Brand Portal用戶可以：

* 在「資產詳細資訊」頁、「卡視圖」和連結共用預覽頁中預覽視頻。
* 在「資產詳細資訊」頁面上播放視頻編碼。
* 在「資產詳細資訊」頁面的「格式副本」頁籤中查看動態格式副本。
* 下載視頻編碼和包含視頻的資料夾。

>[!NOTE]
>
>要處理視頻並將其發佈到Brand Portal，請確保您的「Experience Manager作者」實例已在Dynamic Media混合模式或Dynamic Media上設定 **[!DNL Scene7]** 的子菜單。

要預覽、播放和下載視頻，Brand Portal向管理員公開以下兩種配置：

* [Dynamic Media混合配置](#configure-dm-hybrid-settings)
如果Experience Manager作者實例在動態媒體混合模式下運行。
* [Dynamic Media [!DNL Scene7] 配置](#configure-dm-scene7-settings)
如果Experience Manager作者實例正在動態媒體上運行 — **[!DNL Scene7]** 的子菜單。
根據您在Experience Manager作者實例中設定的複製Brand Portal租戶的配置，設定這些配置中的任意一個。

>[!NOTE]
>
>在配置了Experience Manager作者的Brand Portal租戶上不支援動態視頻 **[!UICONTROL Scene7]** 運行模式。

## 動態視頻如何播放？ {#how-are-dynamic-videos-played}

![從雲中獲取視頻編碼](assets/VideoEncodes.png)

如果Dynamic Media配置([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 配置)，在Brand Portal上設定，動態格式副本從 **[!DNL Scene7]** 伺服器。 因此，視頻編碼是預覽和播放的，沒有延遲和質量失真。

由於視頻編碼不儲存在Brand Portal儲存庫中，因此從 **[!DNL Scene7]** 伺服器，確保Adobe Experience Manager作者實例和Brand Portal上的Dynamic Media配置相同。

>[!NOTE]
>
>Brand Portal不支援視頻查看器和查看器預設。 視頻在Brand Portal的預設觀看者上預覽和播放。

## 必備條件 {#prerequisites}

要處理Brand Portal上的動態視頻，請確保：

* **在Dynamic Media模式下啟動Experience Manager作者**
啟動Experience Manager作者實例(配置了Brand Portal) [Dynamic Media [!DNL Scene7] 模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) 或 [Dynamic Media — 混合模式](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) 或
* **配置Dynamic MediaCloud Services的Experience Manager作者**
基於Dynamic Media模式(Scene7模式或混合模式)Experience Manager作者正在運行，請設定 [Dynamic MediaCloud Services([!DNL Scene7] 模式)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=zh-Hant#configuring-dynamic-media-cloud-services) 或 [Dynamic MediaCloud Services（混合模式）](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) 關於Experience Manager作者 **工具** | **Cloud Services** | **Dynamic Media**。
* **在Brand Portal配置Dynamic Media**
根據Experience Manager作者上的Dynamic Media雲配置，配置 [Dynamic Media設定](#configure-dm-hybrid-settings) 或 [[!DNL Scene7] 設定](#configure-dm-scene7-settings) 從Brand Portal的行政工具中。
確保 [獨立的Brand Portal租戶](#separate-tenants) 用於在Dynamic Media配置的Experience Manager作者實例 —  **[!UICONTROL Scene7]** 模式和Dynamic Media — 混合模式。 特別是如果你使用Dynamic Media **[!UICONTROL S7]** 和Dynamic Media混血車。
* **發佈應用於Brand Portal的帶視頻編碼的資料夾**
應用 [視頻編碼](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 將包含富媒體資產的資料夾從Experience Manager作者實例發佈到Brand Portal。
* **如果啟用了安全預覽，則允許列出SPS中的出口IP**
如果使用Dynamic Media。**[!DNL Scene7]** ( [啟用安全預覽](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) )，則建議 **[!DNL Scene7]** 公司管理員 [允許列出公用出口IP](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) 針對使用SPS的各個區域(**[!UICONTROL Scene7]** 發佈系統)快閃記憶體UI。
出口IP如下：

| **區域** | **出口IP** |
|--- |--- |
| 不適用 | 130.248.160.68,  20.94.203.130 |
| 歐洲、中東和非洲 | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

要允許列出其中一個出口IP，請參見 [準備安全測試服務帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳做法

要確保您的動態視頻資產從Brand Portal（和共用連結）成功預覽、播放和下載，請遵循以下操作：

### Dynamic Media-Scene7和Dynamic Media — 混合模式的獨立租戶 {#separate-tenants}

如果你同時使用Dynamic Media。 **[!DNL Scene7]** 模式和Dynamic Media — 混合模式功能，使用不同的Brand Portal租戶來Experience Manager作者實例，配置為Dynamic Media- **[!DNL Scene7]** 和Dynamic Media — 混合模式。


![作者與BP一對一映射](assets/BPDynamicMedia.png)

### Experience Manager作者實例和Brand Portal的配置詳細資訊相同

確保配置詳細資訊在Brand Portal和 **[!UICONTROL Experience Manager雲配置]**。 相同的配置詳細資訊包括：

* **[!UICONTROL 標題]**
* **[!UICONTROL 註冊 ID]**
* **[!UICONTROL 視頻服務URL]** 在 **[!UICONTROL Dynamic Media — 混合模式]**
* **[!UICONTROL 標題]**
* 憑據(**[!UICONTROL 電子郵件]** 和密碼)
* **[!UICONTROL 區域]**
* **[!UICONTROL 公司]** 在Dynamic Media。 **[!DNL Scene7]** 模式

### 允許列出Dynamic MediaScene7模式的公共出口IP

如果Dynamic Media **[!UICONTROL Scene7]** — 有 [啟用安全預覽](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) — 用於向Brand Portal提供視頻資產， **[!UICONTROL Scene7]** 為臨時環境或內部應用程式建立專用的映像伺服器。 對此伺服器的任何請求都檢查源IP地址。 如果傳入請求不在批准的IP地址清單中，則返回失敗響應。
的 **[!UICONTROL Scene7]** 因此，公司管理員為其公司配置經批准的IP地址清單 **[!UICONTROL 安全測試]** 環境，通過 **[!UICONTROL SPS]** (Scene7發佈系統)flash UI。 確保將您各自區域的出口IP（來自下面）添加到該批准清單。
要允許列出其中一個出口IP，請參見 [準備安全測試服務帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
輸出IP如下：

| **區域** | **出口IP** |
|--- |--- |
| 不適用 | 130.248.160.66, 20.94.203.130 |
| 歐洲、中東和非洲 | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media（混合）設定 {#configure-dm-hybrid-settings}

如果Experience Manager作者實例在動態媒體混合模式下運行，則使用 **[!UICONTROL 視頻]** 從管理工具面板中拼貼以配置Dynamic Media網關設定。

>[!NOTE]
>
>的 [視頻編碼配置檔案](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) 不發表給Brand Portal，而是從 **[!UICONTROL Scene7]** 伺服器。 因此，對於在Brand Portal成功播放的視頻編碼，請確保配置細節與 [Dynamic MediaCloud Services([!DNL Scene7] 模式)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=zh-Hant#configuring-dynamic-media-cloud-services) 你的Experience Manager作者案。

要在Brand Portal租戶上設定Dynamic Media配置：

1. 選擇Experience Manager徽標，以便您可以從頂部的工具欄(位於Brand Portal)訪問管理工具。
1. 從管理工具面板中，選擇 **[!UICONTROL 視頻]** 平鋪。

   ![Dynamic Media混合配置在Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL 編輯Dynamic Media配置]** 的上界。

   ![Dynamic Media混合配置在Brand Portal](assets/edit-dynamic-media-config.png)

1. 指定 **[!UICONTROL 註冊ID]** 和 **[!UICONTROL 視頻服務URL]** （DM — 網關URL）。 確保這些詳細資訊與 **[!UICONTROL 工具>Cloud Services]** 你的Experience Manager作者案。
1. 選擇 **保存** 的子菜單。

## 配置Dynamic MediaScene7設定 {#configure-dm-scene7-settings}

如果Experience Manager作者實例正在Dynamic Media上運行 —  **[!UICONTROL Scene7]** 模式，然後使用 **[!UICONTROL Dynamic Media配置]** 從管理工具面板中平鋪以配置 **[!UICONTROL Scene7]** 伺服器設定。

設定Dynamic Media **[!UICONTROL Scene7]** Brand Portal租戶的配置：

1. 選擇Experience Manager徽標，以便您可以從頂部的工具欄(位於Brand Portal)訪問管理工具。

2. 從管理工具面板中，選擇 **[!UICONTROL Dynamic Media配置]** 平鋪。

   ![DM [!UICONTROL 場景7] Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL 編輯Dynamic Media配置]** 的上界。

   ![場景7Brand Portal配置](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 標題]**
   * 憑據(**[!UICONTROL 電子郵件ID]** 和 **[!UICONTROL 密碼]**)訪問Scene7伺服器
   * **[!UICONTROL 區域]**

   確保這些值與在Experience Manager作者實例中找到的值相同。

4. 選擇 **[!UICONTROL 連接到Dynamic Media]**。

5. 提供 **[!UICONTROL 公司名稱]**, **[!UICONTROL 保存]** 配置。
