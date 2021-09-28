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
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 2%

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
>若要處理影片並將影片發佈至Brand Portal，請確定您的AEM Author例項已設定在Dynamic Media混合模式或Dynamic Media **[!DNL Scene 7]**&#x200B;模式。

若要預覽、播放和下載影片，Brand Portal會向管理員公開下列兩項設定：

* [Dynamic Media混](#configure-dm-hybrid-settings)
合設定如果AEM Author例項在Dynamic Media混合模式上執行。
* [動態 [!DNL Scene 7] ](#configure-dm-scene7-settings)
媒體設定如果AEM製作執行個體在動態媒體模式中**[!DNL Scene 7]** 執行。根據您在複製Brand Portal租用戶的AEM Author例項中設定的設定，設定其中一項設定。

>[!NOTE]
>
>設定在&#x200B;**[!UICONTROL Scene7Connect]**&#x200B;執行模式上執行之AEM Author的Brand Portal租戶不支援動態影片。

## 如何播放動態影片？ {#how-are-dynamic-videos-played}

![從雲端擷取視訊編碼](assets/VideoEncodes.png)

若已在Brand Portal上設定Dynamic Media設定（[ Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)或[[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)設定），則會從&#x200B;**[!DNL Scene 7]**&#x200B;伺服器擷取動態轉譯。 因此，視頻編碼是預視和播放的，在質量上沒有延遲和失真。

由於視訊編碼不會儲存在Brand Portal存放庫中，且會從&#x200B;**[!DNL Scene 7]**&#x200B;伺服器擷取，因此請確定AEM製作執行個體和Brand Portal上的Dynamic Media設定相同。

>[!NOTE]
>
>Brand Portal不支援視訊檢視器和檢視器預設集。 影片會在Brand Portal的預設檢視器中預覽及播放。

## 必備條件 {#prerequisites}

若要在Brand Portal上使用動態影片，請務必：

* **在DM(Dynamic Media)模式上啟動AEM Author**
在Dynamic Media Hybrid模式或動態媒體模式上啟動AEM Author例項(已設定 [Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) ) [ [!DNL Scene 7] (](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode))。
* **在AEM上設定Dynamic Media雲**
端服務根據Dynamic Media模式，AEM Author正在執行，請在「工具」的AEM  [Author上](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) 設定一個Dynamic Media雲端服務，或 [[!DNL Scene 7] 在](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Author上設定 **雲端服務** |  **Cloud Services** |  **Dynamic Media**。
* **在Brand Portal上設**
定Dynamic Media根據AEM作者上的Dynamic Media雲端設定，從 [Brand Portal管理工具](#configure-dm-hybrid-settings)  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  設定Dynamic Media設定或設定。如果您使用Brand Portal Hybrid和Dynamic Media **[!UICONTROL S7]**&#x200B;的功能，請務必將[個別的Dynamic Media租戶](#separate-tenants)用於以Dynamic Media Hybrid和Dynamic Media **[!UICONTROL Scene7]**&#x200B;模式設定的AEM Author例項。
* **使用視訊編碼發佈資料夾(套用至**
Brand Portal)套 [用視](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 訊編碼，並將包含AEM製作例項多媒體資產的資料夾發佈至Brand Portal。
* **允許清單在啟用安全預**
覽的情況下在SPS中輸出IP如果使用Dynamic Media **[!DNL Scene 7]** -  [(為公司啟用安全](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) 預覽)，建議公司管理員允許列 **[!DNL Scene 7]** 出使用SPS( [Scene 7 ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) Publishing System)快閃記憶體UI之個別地區的公開&#x200B;**** 輸出IP。輸出IP如下：

| **區域** | **輸出IP** |
|--- |--- |
| 不適用 | 130.248.160.66, 52.151.32.108 |
| 歐洲、中東和非洲 | 185.34.189.1 |
| APAC | 63.140.44.54 |

若要允許列出其中一個輸出IP，請參閱[為安全測試服務準備您的帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳作法

若要確保您的動態視訊資產能從Brand Portal（和共用連結）成功預覽、播放和下載，請遵循下列實務：

### Dynamic Media Hybrid和Dynamic Media Scene 7模式的不同租戶 {#separate-tenants}

如果您同時使用Dynamic Media **[!DNL Scene 7]**&#x200B;和Dynamic Media Hybrid功能，建議針對以Dynamic Media Hybrid和Dynamic Media **[!DNL Scene 7]**&#x200B;模式設定的AEM Author例項，使用不同的Brand Portal租戶。


![作者與BP一對一映射](assets/BPDynamicMedia.png)

### 與AEM Author例項和Brand Portal的設定詳細資料相同

確保配置詳細資訊(如&#x200B;**[!UICONTROL Title]**、**[!UICONTROL 註冊ID]**、**[!UICONTROL 視頻服務URL]**(在&#x200B;**[!UICONTROL Dynamic Media Hybrid]**&#x200B;中)和&#x200B;**[!UICONTROL Title]**、憑證（**[!UICONTROL Email]**&#x200B;和密碼）、**[!UICONTROL Region]**、**[!UICONTROL 中的Dynamic Media公司(a15/)**[!DNL Scene 7]**) — 在Brand Portal和**[!UICONTROL  AEM雲端設定&#x200B;]**中相同。]**

### 允許列出Dynamic Media Scene 7模式的公開輸出IP

如果使用Dynamic Media **[!UICONTROL Scene 7]**-having [secure preview enabled](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) — 來將視訊資產提供給Brand Portal，則&#x200B;**[!UICONTROL Scene 7]**會為預備環境或內部應用程式建立專用的影像伺服器。 對此伺服器的任何請求都會檢查來源IP位址。 如果傳入的請求不在核准的IP位址清單內，則會傳回失敗回應。
因此， **[!UICONTROL Scene-7]**&#x200B;公司管理員會透過&#x200B;**[!UICONTROL SPS]**(Scene-7 Publishing System)快閃記憶體UI，為其公司的&#x200B;**[!UICONTROL Secure Testing]**環境設定已核准的IP位址清單。 請確定已將您各自地區的輸出IP（來自下列）新增至該已核准清單。
若要允許列出其中一個輸出IP，請參閱[為安全測試服務準備您的帳戶](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
輸出IP如下：

| **區域** | **輸出IP** |
|--- |--- |
| 不適用 | 130.248.160.66, 52.151.32.108 |
| 歐洲、中東和非洲 | 185.34.189.1 |
| APAC | 63.140.44.54 |

## 配置Dynamic Media（混合）設定 {#configure-dm-hybrid-settings}

如果AEM製作執行個體在動態媒體混合模式上執行，請從管理工具面板使用&#x200B;**[!UICONTROL Video]**&#x200B;圖磚，以設定Dynamic Media閘道設定。

>[!NOTE]
>
>[視訊編碼設定檔](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html)不會發佈至Brand Portal，而是從&#x200B;**[!UICONTROL Scene 7]**&#x200B;伺服器擷取。 因此，若要讓視訊編碼在Brand Portal中成功播放，請確定設定詳細資訊與AEM Author例項中的[[!UICONTROL Scene7雲端設定]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)相同。

若要在Brand Portal租戶上設定Dynamic Media設定：

1. 從頂端的Brand Portal工具列選取AEM標誌以存取管理工具。
1. 從管理工具面板中，選擇&#x200B;**[!UICONTROL Video]**&#x200B;圖磚。

   ![Dynamic Media Brand Portal上的混合設定](assets/DMHybrid-Video.png)

   **[!UICONTROL 編輯Dynamic Media]** 設定頁面隨即開啟。

   ![Dynamic Media Brand Portal上的混合設定](assets/edit-dynamic-media-config.png)

1. 指定&#x200B;**[!UICONTROL 註冊ID]**&#x200B;和&#x200B;**[!UICONTROL 視訊服務URL]**（DM — 網關URL）。 請確定這些詳細資料與AEM Author例項中&#x200B;**[!UICONTROL Tools > Tails > Authors]** Cloud Services的相同。
1. 選擇&#x200B;**保存**&#x200B;以保存配置。

## 配置Dynamic Media Scene7設定 {#configure-dm-scene7-settings}

如果AEM製作執行個體在Dynamic Media- **[!UICONTROL Scene 7]**&#x200B;模式中執行，請從管理工具面板使用&#x200B;**[!UICONTROL Dynamic Media設定]**&#x200B;圖磚，以設定&#x200B;**[!UICONTROL Scene 7]**&#x200B;伺服器設定。

若要在Brand Portal租戶上設定Dynamic Media **[!UICONTROL Scene 7]**&#x200B;設定：

1. 從頂端的Brand Portal工具列選取AEM標誌以存取管理工具。

2. 從管理工具面板中，選擇&#x200B;**[!UICONTROL Dynamic Media Configuration]**&#x200B;磁貼。

   ![Brand Portal [!UICONTROL 上的DM Scene 7] 設定](assets/DMS7-Tile.png)

   **[!UICONTROL 編輯Dynamic Media]** 設定頁面隨即開啟。

   ![Brand Portal上的Scene 7設定](assets/S7Config.png)

3. 提供：

   * **[!UICONTROL 標題]**
   * 訪問Scene 7伺服器的憑據（**[!UICONTROL 電子郵件ID]**&#x200B;和&#x200B;**[!UICONTROL 密碼]**）
   * **[!UICONTROL 區域]**

   請確定這些值與您AEM Author例項中的值相同。

4. 選擇&#x200B;**[!UICONTROL 連接到Dynamic Media]**。

5. 提供&#x200B;**[!UICONTROL 公司名稱]**&#x200B;和&#x200B;**[!UICONTROL 儲存]**&#x200B;設定。
