---
title: 品牌入口網站上的動態視訊支援
seo-title: 品牌入口網站上的動態視訊支援
description: 品牌入口網站上的動態視訊支援
seo-description: 品牌入口網站上的動態視訊支援
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: Mgulati
products: SG_ PERIENCENCENAGER/Brand_ Portal
content-type: 引用
topic-tags: 下載安裝
discoiquuid: e18d992a-a3 b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 品牌入口網站上的動態視訊支援 {#dynamic-video-support-on-brand-portal}

[!DNL Brand Portal] 使用動態媒體支援，輕鬆預覽和播放影片。也可以從入口網站和共用連結下載動態轉譯。
[!DNL Brand Portal] 使用者可以：

* 在「資產詳細資料」頁面、「卡片檢視」和連結共用預覽頁面中預覽影片。
* 在「資產詳細資料」頁面上播放視訊Encode。
* 在「資產詳細資料」頁面上，檢視「轉譯」索引標籤中的動態轉譯。
* 下載包含視訊的視訊編碼和檔案夾。

>[!NOTE]
>
>若要處理影片並將它們發佈， [!DNL Brand Portal]請確定 [!DNL AEM] 您的作者實例已設定在動態媒體混合模式或動態媒體 [!DNL Scene 7] 模式上。

若要預覽、播放和下載視訊， [!DNL Brand Portal] 請對管理員顯示下列兩種組態：

* [動態媒體混合設定](#configure-dm-hybrid-settings)： [!DNL AEM] 如果作者實例執行動態媒體混合模式。
* [Dynamic Media[！DNL Scene]設定，](#configure-dm-scene7-settings)如果 [!DNL AEM] 作者實例正在動態媒體[!DNL Scene 7] 模式上執行。
根據您在 [!DNL AEM] 作者執行個體中設定的設定，設定上述任 [!DNL Brand Portal] 一設定。

>[!NOTE]
>
>在Scene Connect執行模式上執行 [!DNL Brand Portal] 的Author與 [!DNL AEM] Author整合時，不 [!UICONTROL 支援動態] 影片。

## 動態影片如何播放？ {#how-are-dynamic-videos-played}

![視訊Encode是從雲端擷取](assets/VideoEncodes.png)

如果動態媒體設定([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[DNL Scene]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 設定已設定， [!DNL Brand Portal]動態轉譯會從 [!DNL Scene 7] 伺服器擷取。因此，視訊編碼的預覽和播放不會延遲，而且品質也會扭曲。

由於視訊編碼不會儲存 [!DNL Brand Portal] 在存放庫中並從 [!DNL Scene 7] 伺服器擷取，因此請確定「作者實例」 [!DNL AEM] 上的「動態媒體」設定 [!DNL Brand Portal] 相同。

>[!NOTE]
>
>不支援視訊檢視器和檢視器預設集 [!DNL Brand Portal]。預覽視訊並在預設檢視器上播放 [!DNL Brand Portal]。

## 必備條件 {#prerequisites}

若要處理動態影片， [!DNL Brand Portal]請務必：

* **在DM(動態媒體)模式上啓動[!DNL AEM]作者(動態媒體)模式**[!DNL AEM] 在 [!DNL Brand Portal][動態媒體混合模式](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 或 [動態媒體上啓動作者實例(已整合)DNL Scene]模式](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)。
* **根據「Author」(動態媒體)模式[!DNL AEM]Author**&#x200B;上的「Dynamic Media」(動態媒體)模式 [!DNL AEM] ，設定Dynamic
Media雲端服務，設定任 [一Dynamic Media Cloud服務](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 或 [[！來自工具的DNL](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) [!DNL AEM]**Scene]雲端服務** | **雲端服務** | **動態媒體**。
* **根據Author上的動態媒體雲端設定在品牌入口網站**&#x200B;上設定動態 [!DNL AEM] 媒體，設定 [動態媒體設定](#configure-dm-hybrid-settings) 或 [[！管理工具的DNL](#configure-dm-scene7-settings) [!DNL Brand Portal] Scene]設定。
確定 [個別[！如果您使用Dynamic](#separate-tenants) Media Mixed和Dynamic Media S的功能，DNL品牌入口網站會使用 [!DNL AEM] Dynamic Media Mixed和Dynamic Media [!UICONTROL Scene] 模式設定的「作者」實例 。
* **發佈套用至品牌入口網站的視訊編碼資料夾**&#x200B;套用 [視訊編碼](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) ，並將包含多媒體資產的 [!DNL AEM] 檔案夾發佈 [!DNL Brand Portal]至「作者」實例。
* **Whitelist在SPS中啓用IPS(如果使用Dynamic** Media啓用安全預覽)，如果使用Dynamic Media([!DNL Scene 7] 針對 [公司啓用](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 安全預覽)，建議 [!DNL Scene 7] 公司管理員 [白名單使用](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) SPS([!UICONTROL Scene] Publishing System) flash UI的公開匯出IP。
Egries IP如下：

| **區域** | **Egries IP** |
|--- |--- |
| 不適用 | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| 亞太地區 | 63.140.44.54 |

若要將ePS的其中一個帳戶列入白名單，請參閱 [準備您的帳戶以取得安全測試服務](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳實務

為確保動態視訊資產已成功預覽、播放及下載( [!DNL Brand Portal] 和共用連結)，請遵循下列實務：

### 動態媒體混合和動態媒體Scene模式的不同租用戶 {#separate-tenants}

如果您同時使用Dynamic Media [!DNL Scene 7] 和Dynamic Media Mixed功能，建議您使用Dynamic [!DNL Brand Portal][!DNL AEM] Media混合和動態媒體 [!DNL Scene 7] 模式設定的「作者」實例使用不同的租用戶。
![作者和BP一到一個對應](assets/BPDynamicMedia.png)

### AEM作者實例與品牌入口網站的組態詳細資訊

確定組態詳細資訊-例如標題、註冊ID、Video Service URL(在動態媒體混合)和標題、憑證(電子郵件和密碼)、地區、公司(在動態媒體中 [!DNL Scene 7])都是相同的in [!DNL Brand Portal][!DNL AEM] and Cloud組態。

### 將IP用於動態媒體Scene模式的白名單

如果Dynamic Media Scene-has [Secure preview](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)Enabled-is used to service assets to [!DNL Brand Portal]，then Scene7 create asp專用Image Server for starting environment or internal applications.對此伺服器的任何要求都會檢查來源IP位址。如果傳入請求未在核准的IP位址清單內，則會傳回失敗回應。
因此，Scene-7公司管理員會透過SPS(Scene-7Publishing System) flash UI，為其公司的安全測試環境設定已核准的IP位址清單。請確定您所屬地區(來自下列)的退出IP已新增至核准清單。
若要將ePS的其中一個帳戶列入白名單，請參閱 [準備您的帳戶以取得安全測試服務](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
退出IP如下：

| **區域** | **Egries IP** |
|--- |--- |
| 不適用 | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| 亞太地區 | 63.140.44.54 |

## 設定動態媒體(混合)設定 {#configure-dm-hybrid-settings}

[!DNL AEM] 如果Author實例執行於動態媒體混合模式，則可從管理工具面板使用視訊方塊來設定動態媒體閘道設定。
>[!NOTE]
>
>[視訊編碼設定檔](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 不會發佈到， [!DNL Brand Portal]而是從Scene伺服器擷取。因此，若要成功在視訊編碼中 [!DNL Brand Portal]播放，請確定設定詳細資訊與您的「作者」例項中 [的Scene雲端設定](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)[!DNL AEM] 相同。
若要設定 [!DNL Brand Portal] 租用戶的動態媒體設定：

1. 從上方的工具列選取 [!DNL AEM] 用來存取管理工具的標誌 [!DNL Brand Portal]。

2. 從管理工具面板，選取 **「視訊** 」圖標。
   ![品牌入口網站上的動態媒體混合設定](assets/DMHybrid-Video.png)
   **「編輯動態媒體設定** 」頁面隨即開啓。
   ![品牌入口網站上的動態媒體混合設定](assets/edit-dynamic-media-config.png)

3. 指定 **註冊ID** 和 **視訊服務URL** (DM-閘道URL)。請確定這些詳細資訊與「 **工具** &gt; **雲端服務** 」中的「 [!DNL AEM] 工具」&gt;「雲端服務」相同。

4. 選擇 **「儲存** 」以儲存設定。

## 設定Dynamic Media Scene設定 {#configure-dm-scene7-settings}

[!DNL AEM] 如果作者實例執行於Dynamic Media- [!UICONTROL Scene] 模式，則可從管理工具面板使用 **Dynamic Media Configuration** 方塊來設定 [!UICONTROL Scene] 伺服器設定。

若要設定租用戶的Dynamic Media [!UICONTROL Scene][!DNL Brand Portal] 設定：

1. 從上方的工具列選取 [!DNL AEM] 用來存取管理工具的標誌 [!DNL Brand Portal]。

2. 從管理工具面板，選取 **「動態媒體設定** 」圖標。
   ![「編輯動態媒體設定」 [!DNL Brand Portal]](assets/DMS7-Tile.png)頁面上的DM Scene設定開啓。
   ![Scene設定上的 [!DNL Brand Portal]](assets/S7Config.png)

3. 提供：
   * 標題
   * 存取Scene伺服器的憑證(電子郵件ID和密碼)
   * 地區請確定這些值與 [!DNL AEM] 「作者」例項中的值相同。

4. Select **Connect to Dynamic Media**.

5. 提供 **公司名稱**， **並儲存** 設定。
