---
title: Brand Portal 上的動態視訊支援
seo-title: Brand Portal 上的動態視訊支援
description: Brand Portal 上的動態視訊支援
seo-description: Brand Portal 上的動態視訊支援
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 3%

---


# Brand Portal 上的動態視訊支援 {#dynamic-video-support-on-brand-portal}

運用動態媒體支援，在品牌入口網站上自適應地預覽和播放視訊。 也可從入口網站和共用連結下載動態轉譯。
品牌入口網站使用者可以：

* 在「資產詳細資料」頁面、「卡片檢視」和連結共用預覽頁面中預覽影片。
* 在「資產詳細資料」頁面上播放視訊編碼。
* 在「資產詳細資料」頁面的「轉譯」索引標籤中檢視動態轉譯。
* 下載視訊編碼和包含視訊的資料夾。

>[!NOTE]
>
>若要處理視訊並將其發佈至品牌入口網站，請確定您的AEM Author例項已設定在動態媒體混合模式或動態媒體&#x200B;**[!DNL Scene 7]**&#x200B;模式。

若要預覽、播放和下載視訊，品牌入口網站會向管理員公開下列兩種設定：

* [動態媒體混合](#configure-dm-hybrid-settings)
設定如果AEM Author例項是在動態媒體混合模式上執行。
* [動態 [!DNL Scene 7] ](#configure-dm-scene7-settings)
媒體設定如果AEM Author例項在動態媒體模式上**[!DNL Scene 7]** 執行。根據您在AEM Author實例中設定的設定來設定其中一個設定，此實例會複製品牌入口網站租用戶。

>[!NOTE]
>
>動態視訊不受品牌入口網站租戶支援，這些租戶已設定AEM Author，並在&#x200B;**[!UICONTROL Scene7Connect]**&#x200B;執行模式中執行。

## 動態視訊如何播放？{#how-are-dynamic-videos-played}

![從雲端擷取視訊編碼](assets/VideoEncodes.png)

如果在品牌入口網站上設定動態媒體組態（[Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings)或[[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)組態），則會從&#x200B;**[!DNL Scene 7]**&#x200B;伺服器擷取動態轉譯。 因此，視訊編碼是預覽和播放時不會延遲和品質失真。

由於視訊編碼不會儲存在品牌入口網站儲存庫中，而且會從&#x200B;**[!DNL Scene 7]**&#x200B;伺服器擷取，請確定AEM作者實例和品牌入口網站上的動態媒體設定是相同的。

>[!NOTE]
>
>品牌入口網站不支援視訊檢視器和檢視器預設集。 視訊會在品牌入口網站的預設檢視器上預覽和播放。

## 必備條件 {#prerequisites}

若要在品牌入口網站上處理動態視訊，請確定：

* **在DM（動態媒體）模式上啟動AEM Author（動態媒體）**
在 [Dynamic Media Hybrid ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) mode或 [Dynamic  [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)上啟動AEM Author例項（已設定品牌入口網站）。
* **在AEM**
Author上配置Dynamic Cloud服務基於Media模式AEM Author在 [Dynamic Media ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Cloud Services或 [[!DNL Scene 7] Cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Services on  **Dynamic Media Cloud Services的組上運行，從Dynamic Media Cloud Cloud Servicesoud Servicesoud Services**  ****  ****| Sum Services作者開發出的DD Dy Dy Dy Dy Dy Med Med Med Med Memid Med Med Med Media Media Media Media
* **在品牌入口網站上設**
定動態媒體根據AEM作者上的Dynamic Media cloud設定，從品牌入口網站管理工具 [設定](#configure-dm-hybrid-settings) 動態媒 [[!DNL Scene 7] ](#configure-dm-scene7-settings)  體設定或設定。如果您使用動態媒體混合與動態媒體混合的功能，請確定[個別品牌入口網站租戶](#separate-tenants)用於AEM Author執行個體，這些執行個體已設定為動態媒體混合與動態媒體&#x200B;**[!UICONTROL Scene7]**&#x200B;模式。****
* **使用視訊編碼發佈檔案夾套用至品牌**
入口網站套 [用視](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) 訊編碼，並將包含豐富型媒體資產的檔案夾從AEM作者例項發佈至品牌入口網站。
* **Allowlist Egress IPs if**
secure preview **[!DNL Scene 7]**  [enabled如果使用Dynamic Media-](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) （具有為公司啟用的安全預覽功能），則建議 **[!DNL Scene 7]**  [company administrator allowlist the public egressIpProbushing System(Flash Publishing Sy Sy Sy Sy Sy Sy Sy Stem)，為各自的地區建立公共出口](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) ****  IN.出口IP如下：

| **區域** | **出口IP** |
|--- |--- |
| 不適用 | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

要允許列出其中一個出口IP，請參閱[準備您的帳戶以用於安全測試服務](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。

## 最佳作法

若要確保您的動態視訊資產能夠從品牌入口網站（和共用連結）成功預覽、播放和下載，請遵循下列實務：

### 動態媒體混合與動態媒體場景7模式的不同租戶{#separate-tenants}

如果您同時使用Dynamic Media **[!DNL Scene 7]**&#x200B;和Dynamic Media Hybrid功能，建議您針對使用Dynamic Media Hybrid和Dynamic Media **[!DNL Scene 7]**&#x200B;模式設定的AEM Author例項，使用不同的品牌入口網站租戶。<br />

![作者與BP一對一映射](assets/BPDynamicMedia.png)

### 在AEM Author例項和品牌入口網站的設定詳細資訊相同

確保配置詳細資訊——如&#x200B;**[!UICONTROL Title]**、**[!UICONTROL 註冊ID]**、**[!UICONTROL 視頻服務URL]**（在&#x200B;**[!UICONTROL 動態媒體混合體]**&#x200B;中）和&#x200B;**[!UICONTROL Title]**、憑據（**[!UICONTROL 電子郵件]**&#x200B;和密碼）、**[!UICONTROL 地區]**、**[!UICONTROL 公司]**（在動態媒體&#x200B;**[!DNL Scene 7]**&#x200B;中）-在品牌入口網站和&#x200B;**[!UICONTROL AEM雲端設定]**&#x200B;中是相同的。

### 允許列出動態媒體場景7模式的公開出口IP

如果使用Dynamic Media **[!UICONTROL Scene 7]**-具有[啟用安全預覽的](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-來將視訊資產提供至品牌入口網站，則&#x200B;**[!UICONTROL Scene 7]**會建立專用的影像伺服器，以用於測試環境或內部應用程式。 對此伺服器的任何請求都會檢查源IP地址。 如果傳入請求不在已核准的IP位址清單中，則會傳回失敗回應。
因此，**[!UICONTROL Scene-7]**&#x200B;公司管理員會透過&#x200B;**[!UICONTROL SPS]**(Scene-7 Publishing System)flash UI，為公司的&#x200B;**[!UICONTROL 安全測試]**環境設定核准的IP位址清單。 請確定您各自地區的出口IP（來自下列）已新增至核准清單。
要允許列出其中一個出口IP，請參閱[準備您的帳戶以用於安全測試服務](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)。
出口IP如下：

| **區域** | **出口IP** |
|--- |--- |
| 不適用 | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## 設定動態媒體(Hybrid)設定{#configure-dm-hybrid-settings}

如果AEM Author例項是在動態媒體混合模式上執行，則從管理工具面板使用&#x200B;**[!UICONTROL Video]**&#x200B;圖格來設定動態媒體閘道設定。

>[!NOTE]
>
>[視訊編碼設定檔](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html)不會發佈至品牌入口網站，而是從&#x200B;**[!UICONTROL Scene 7]**&#x200B;伺服器擷取。 因此，若要在品牌入口網站中成功播放視訊編碼，請確定設定詳細資訊與AEM作者例項中的[[!UICONTROL Scene7雲端設定]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices)相同。

若要在品牌入口網站租戶上設定動態媒體設定：

1. 選取AEM標誌，從品牌入口網站頂端的工具列存取管理工具。
1. 從管理工具面板中，選擇&#x200B;**[!UICONTROL Video]**&#x200B;表徵圖。

   ![品牌入口網站上的動態媒體混合配置](assets/DMHybrid-Video.png)

   **[!UICONTROL 「編輯動態媒體]** 設定」頁面隨即開啟。

   ![品牌門戶上的動態媒體混合配置](assets/edit-dynamic-media-config.png)

1. 指定&#x200B;**[!UICONTROL 註冊ID]**&#x200B;和&#x200B;**[!UICONTROL 視訊服務URL]**（DM-閘道URL）。 請確定這些詳細資訊與您AEM Author例項中的&#x200B;**[!UICONTROL 工具>雲端服務]**&#x200B;相同。
1. 選擇&#x200B;**保存**&#x200B;以保存配置。

## 設定動態媒體Scene7設定{#configure-dm-scene7-settings}

如果AEM Author例項是在動態媒體- **[!UICONTROL 場景7]**&#x200B;模式上執行，則從管理工具面板使用&#x200B;**[!UICONTROL 動態媒體設定]**&#x200B;圖格來設定&#x200B;**[!UICONTROL 場景7]**&#x200B;伺服器設定。

若要在品牌入口網站租戶上設定動態媒體&#x200B;**[!UICONTROL Scene 7]**&#x200B;組態：

1. 選取AEM標誌，從品牌入口網站頂端的工具列存取管理工具。

2. 從管理工具面板中，選擇&#x200B;**[!UICONTROL 動態媒體配置]**&#x200B;表徵圖。<br />
   ![品牌 [!UICONTROL 入口網] 站上的DM Scene 7設定](assets/DMS7-Tile.png)
   **[!UICONTROL 「編輯動態媒體]** 設定」頁面隨即開啟。<br />
   ![品牌入口網站上的Scene 7設定](assets/S7Config.png)

3. 提供：
   * **[!UICONTROL 標題]**
   * 存取Scene 7伺服器的認證（**[!UICONTROL 電子郵件ID]**&#x200B;和&#x200B;**[!UICONTROL 密碼]**）
   * **[!UICONTROL 地]**
區：請確定這些值與AEM Author例項中的值相同。

4. 選擇&#x200B;**[!UICONTROL 連接到動態媒體]**。

5. 提供&#x200B;**[!UICONTROL 公司名稱]**&#x200B;和&#x200B;**[!UICONTROL 保存]**&#x200B;配置。
