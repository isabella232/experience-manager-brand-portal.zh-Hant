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
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 品牌入口網站上的動態視訊支援 {#dynamic-video-support-on-brand-portal}

使用Dynamic Media支援在品牌入口網站上預覽和播放視訊。也可以從入口網站和共用連結下載動態轉譯。
品牌入口網站使用者可以：

* 在「資產詳細資料」頁面、「卡片檢視」和連結共用預覽頁面中預覽影片。
* 在「資產詳細資料」頁面上播放視訊Encode。
* 在「資產詳細資料」頁面上，檢視「轉譯」索引標籤中的動態轉譯。
* 下載包含視訊的視訊編碼和檔案夾。

>[!NOTE]
>
>若要處理視訊並將它們發佈至品牌入口網站，請確定您的AEM作者實例已設定在動態媒體混合模式或動態媒體 [!DNL Scene 7] 模式上。

若要預覽、播放和下載視訊，品牌入口網站會對管理員顯示下列兩種設定：

* [動態媒體混合設定](#configure-dm-hybrid-settings)如果AEM作者實例執行於動態媒體混合模式。
* [Dynamic Media[！DNL Scene]設定](#configure-dm-scene7-settings)：如果AEM作者實例執行於動態媒體[!DNL Scene 7] 模式上。
根據您在AEM Author實例中設定的組態，設定其中任一組態，並複製品牌入口網站租用戶。

>[!NOTE]
>
>在 [!UICONTROL Scene Connect] 執行模式上執行的AEM Author與AEM Author整合時，不支援動態視訊。

## 動態影片如何播放？ {#how-are-dynamic-videos-played}

![視訊Encode是從雲端擷取](assets/VideoEncodes.png)

如果動態媒體設定([混合](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) 或 [[DNL Scene]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) 設定是在品牌入口網站上設定的，動態轉譯會從 [!DNL Scene 7] 伺服器擷取。因此，視訊編碼的預覽和播放不會延遲，而且品質也會扭曲。

由於視訊編碼不會儲存在Brand Portal存放庫中並從 [!DNL Scene 7] 伺服器擷取，因此請確定AEM作者實例和品牌入口網站上的動態媒體設定相同。

>[!NOTE]
>
>品牌入口網站不支援視訊檢視器和檢視器預設集。「品牌入口網站」中的預設檢視器會預覽視訊並播放。

## 必備條件 {#prerequisites}

若要在品牌入口網站上使用動態視訊，請務必：

* **在DM(動態媒體)模式啓動AEM作者(動態媒體)模式**&#x200B;從 [Dynamic
Media混合模式](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) 或 [Dynamic Media[！DNL Scene]模式](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)。
* **在AEM Author**上設定動態媒體雲端服務AEM
Author on the Dynamic Media模式AEM Author is running on [Dynamic Media Cloud services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) or [[！來自工具的AEM Author雲端服務](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) 雲端 **服務** | **雲端服務** | **動態媒體**。
* **根據AEM Author上的動態媒體雲端設定在品牌入口網站**&#x200B;上設定動態媒體，設定 [動態媒體設定](#configure-dm-hybrid-settings) 或 [[！來自品牌入口網站管理工具的DNL Scene]設定](#configure-dm-scene7-settings) 。
如果您使用Dynamic Media Mixed和Dynamic Media S的功能，請確定 [個別的品牌入口網站租件](#separate-tenants) 會使用於AEM Author實例，並使用Dynamic Media Hybrid和Dynamic Media [!UICONTROL Scene] 模式 。
* **將資料夾發佈至品牌入口網站**&#x200B;套用視訊編碼套用 [至品牌入口網站套用視訊編碼](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) ，並將包含豐富媒體資產的檔案夾發佈至品牌入口網站。
* **Whitelist在SPS中啓用IPS(如果使用Dynamic** Media啓用安全預覽)，如果使用Dynamic Media([!DNL Scene 7] 針對 [公司啓用](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 安全預覽)，建議 [!DNL Scene 7] 公司管理員 [白名單使用](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) SPS([!UICONTROL Scene] Publishing System) flash UI的公開匯出IP。
Egries IP如下：

| **區域** | **Egries IP** |
|--- |--- |
| 不適用 | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| 亞太地區 | 63.140.44.54 |

若要將ePS的其中一個帳戶列入白名單，請參閱 [準備您的帳戶以取得安全測試服務](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳實務

為確保動態視訊資產已成功預覽、播放並從品牌入口網站(和共用連結)下載，請遵循下列實務：

### 動態媒體混合和動態媒體Scene模式的不同租用戶 {#separate-tenants}

如果您同時使用Dynamic Media [!DNL Scene 7] 和Dynamic Media Mixed功能，建議您針對使用Dynamic Media混合和動態媒體 [!DNL Scene 7] 模式設定的AEM作者實例使用不同的品牌入口保留期。
![作者和BP一到一個對應](assets/BPDynamicMedia.png)

### AEM作者實例與品牌入口網站的組態詳細資訊

請確定設定詳細資訊-品牌入口網站和AEM雲端設定中的 [!UICONTROL 「標題]」、 [!UICONTROL 「註冊ID]」、 [!UICONTROL 「視訊服務URL」(] 位於 [!UICONTROL 動態媒體混合])和 [!UICONTROL 「標題]」、「認證」([!UICONTROL 電子郵件] 和「密碼」)、 [!UICONTROL 「地區]」、 [!UICONTROL 「公司] 」(位於動態媒體 [!DNL Scene 7][!UICONTROL )都相同]。

### 將IP用於動態媒體Scene模式的白名單

如果Dynamic Media Scene-has [Secure preview-](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)has used-is used to service assets to Brand Portal， [!UICONTROL 則Scene] 會為測試環境或內部應用程式建立專用的影像伺服器。對此伺服器的任何要求都會檢查來源IP位址。如果傳入請求未在核准的IP位址清單內，則會傳回失敗回應。
因此 [!UICONTROL ，Scene-7] 公司管理員會透過SPS(Scene-7Publishing System) flash UI，為其公司 [!UICONTROL 的安全測試] 環境 [!UICONTROL 設定] 已核准的IP位址清單。請確定您所屬地區(來自下列)的退出IP已新增至核准清單。
若要將ePS的其中一個帳戶列入白名單，請參閱 [準備您的帳戶以取得安全測試服務](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
退出IP如下：

| **區域** | **Egries IP** |
|--- |--- |
| 不適用 | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| 亞太地區 | 63.140.44.54 |

## 設定動態媒體(混合)設定 {#configure-dm-hybrid-settings}

如果AEM作者實例執行於動態媒體混合模式，則可從管理工具面板使用 [!UICONTROL 視訊] 方塊來設定動態媒體閘道設定。
>[!NOTE]
>
>[視訊編碼設定檔](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 不會發佈至品牌入口網站，而是從 [!UICONTROL Scene] 伺服器擷取。因此，若要在品牌入口網站中成功播放視訊編碼，請確定組態詳細資訊與[ [！UICOHTROL Scene雲端設定]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) ，位於您的AEM作者實例中。
若要在品牌入口網站租件上設定動態媒體設定：

1. 從品牌入口網站上方的工具列中，選取AEM logo以便存取管理工具。

2. 從管理工具面板，選取 **[!UICONTROL 「視訊]** 」圖標。

![品牌入口網站上的動態媒體混合設定](assets/DMHybrid-Video.png)

**[!UICONTROL 「編輯動態媒體設定]** 」頁面隨即開啓。

![品牌入口網站上的動態媒體混合設定](assets/edit-dynamic-media-config.png)

3. 指定 **[!UICONTROL 註冊ID]** 和 **[!UICONTROL 視訊服務URL]** (DM-閘道URL)。請確定這些詳細資料與 **[!UICONTROL 「工具&gt;雲端服務]** 」中的「AEM作者」例項相同。

4. 選擇 **「儲存** 」以儲存設定。

## 設定Dynamic Media Scene設定 {#configure-dm-scene7-settings}

如果AEM作者實例執行於Dynamic Media- [!UICONTROL Scene] 模式，則可從管理工具面板使用 **[!UICONTROL Dynamic Media Configuration]** 方塊來設定 [!UICONTROL Scene] 伺服器設定。

若要在品牌入口網站租件上設定Dynamic Media [!UICONTROL Scene] 設定：

1. 從品牌入口網站上方的工具列中，選取AEM logo以便存取管理工具。

2. 從管理工具面板，選取 **[!UICONTROL 「動態媒體設定]** 」圖標。
   ![品牌入口網站上的DM [!UICONTROL Scene] 設定](assets/DMS7-Tile.png)

[!UICONTROL 「編輯動態媒體設定] 」頁面隨即開啓。

![品牌入口網站上的Scene設定](assets/S7Config.png)

3. 提供：
   * [!UICONTROL 標題]
   * 存取Scene伺服器的憑證([!UICONTROL 電子郵件ID] 和 [!UICONTROL 密碼])
   * [!UICONTROL 地區]請確定這些值與AEM作者實例中的值相同。

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. 提供 **[!UICONTROL 公司名稱]**， **[!UICONTROL 並儲存]** 設定。
