---
title: 以連結方式共用資產
seo-title: 以連結方式共用資產
description: AEM Assets品牌入口網站管理員可與授權的內部使用者和外部實體（包括合作夥伴和廠商）共用多個資產的連結。 編輯人員只能檢視並共用與他們共用的資產。
seo-description: AEM Assets品牌入口網站管理員可與授權的內部使用者和外部實體（包括合作夥伴和廠商）共用多個資產的連結。 編輯人員只能檢視並共用與他們共用的資產。
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: fab0855e8d30e7b6ddf9b4ae5b2ce1fb627c81ce
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 5%

---


# 以連結方式共用資產 {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal管理員可與授權的內部使用者和外部實體（包括合作夥伴和廠商）共用多個資產的連結。 編輯人員只能檢視並共用與他們共用的資產。

透過連結分享資產是讓外部人士也能使用的便利方式，因為接收者不需要登入品牌入口網站即可存取資產。

<!-- Link sharing access is restricted to editors and administrators. 
-->

如需詳細資訊，請參閱[管理使用者、群組和使用者角色](../using/brand-portal-adding-users.md#manage-user-roles)。

>[!NOTE]
>
>品牌入口網站上的連結共用功能允許下載高達5GB的郵遞區號。


以下是將資產共用為連結的步驟：

1. 登入您的品牌入口網站租用戶。 依預設，會開啟&#x200B;**[!UICONTROL 檔案]**&#x200B;檢視，其中包含所有已發佈的資產和資料夾。

1. 選擇要共用的資產或檔案夾，或導覽至&#x200B;**[!UICONTROL 系列]**&#x200B;檢視，以共用您建立的系列。

   ![select-multiple-assets](assets/select-assets-new.png)

1. 在頂端的工具列中，按一下「共用連結」圖示。****

   將顯示&#x200B;**[!UICONTROL 鏈路共用]**&#x200B;對話框。

   ![](assets/link-sharing.png)

   * 在電子郵件地址方塊中，輸入您要與其共用連結之使用者的電子郵件ID。 您可以與多位使用者共用連結。 如果使用者是您組織的成員，請從下拉式清單中顯示的建議中選取其電子郵件ID。 如果用戶是外部用戶，請鍵入完整的電子郵件ID，然後按&#x200B;**[!UICONTROL Enter]**;電子郵件ID會新增至使用者清單。

      ![](assets/link-sharing-text.png)

   * 在&#x200B;**[!UICONTROL Subject]**&#x200B;方塊中，輸入您要共用之資產的主旨。
   * 在&#x200B;**[!UICONTROL Message]**&#x200B;框中，如有必要，鍵入消息。
   * 在&#x200B;**[!UICONTROL Expiration]**&#x200B;欄位中，使用日期選擇器指定連結的到期日期和時間。 依預設，到期日會從您共用連結的日期開始設為7天。
   * 啟用「允許下載原始檔案&#x200B;]**」核取方塊，讓收件者下載原始轉譯。**[!UICONTROL 

   透過連結共用的資產會在超過&#x200B;**[!UICONTROL 到期]**&#x200B;欄位中指定的日期和時間後過期。 如需有關過期資產行為以及基於品牌入口網站使用者角色之允許活動變更的資訊，請參閱[管理資產的數位權限](../using/manage-digital-rights-of-assets.md#asset-expiration)。

   >[!NOTE]
   >
   >連結的預設過期時間為7天。 必須使用&#x200B;**[!UICONTROL 連結共用]**&#x200B;對話方塊，以電子郵件方式將連結傳送給使用者，請勿個別複製和共用連結。

1. 按一下&#x200B;**[!UICONTROL 「共用」]**。訊息會確認連結已與使用者共用。 使用者會收到包含共用連結的電子郵件。

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >管理員可以自訂電子郵件訊息，包括使用[品牌](../using/brand-portal-branding.md)功能自訂標誌、說明和頁尾。

## 從共用連結下載資產{#download-assets-from-shared-links}

按一下電子郵件中的連結，以存取共用資產。 「AEM連結共用」頁面隨即開啟。

若要下載共用資產：

1. 按一下資產或資料夾，然後按一下工具列上的&#x200B;**[!UICONTROL 下載]**&#x200B;圖示。

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >目前，您只能針對特定資產產生預覽和縮圖，視檔案格式而定。 如需支援檔案格式的詳細資訊，請參閱[資產格式的預覽和縮圖支援](#preview-thumbnail-support)。

1. 出現&#x200B;**[!UICONTROL Download]**&#x200B;對話框。

   ![下載對話](assets/download-dialog-box-new.png)

1. 依預設，**[!UICONTROL 快速下載]**&#x200B;設定會在&#x200B;**[!UICONTROL 下載設定]**&#x200B;中啟用。 因此，使用IBM Aspera Connect時，會出現確認方塊繼續下載。

   若要繼續使用&#x200B;**[!UICONTROL 快速下載]**，請按一下&#x200B;**[!UICONTROL 允許]**。

   所有選取的轉譯都會下載在包含每個資產個別資料夾的Zip檔案夾中。

   >[!NOTE]
   >
   >如果選取了檔案夾、系列或超過20個資產供下載，則會略過&#x200B;**[!UICONTROL 下載]**&#x200B;對話方塊，而使用者可存取的所有資產轉譯（不包括動態轉譯）會下載在zip檔案夾中。 會為zip檔案夾內的每個資產建立個別的檔案夾。

   >[!NOTE]
   >
   >如果管理員未授權將資產共用為連結的使用者[存取原始轉譯，則不會使用共用連結來下載原始轉譯。](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges)


>[!NOTE]
>
>品牌入口網站限制每個檔案大小下載超過5GB的資產。

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

>[!NOTE]
>
>Brand Portal restricts downloading assets larger than 5GB per file size.
-->

## 資產格式的預覽和縮圖支援{#preview-thumbnail-support}

下列矩陣列出品牌入口網站支援縮圖和預覽的資產格式：

| 資產格式 | 縮圖支援 | 預覽支援 |
|--------------|-------------------|-----------------|
| PNG | ý | ý |
| GIF | ý | ý |
| TIFF | ý | ✕ |
| JPEG | ý | ý |
| BMP | ý | ✕ |
| PNM* | 不適用 | 不適用 |
| PGM* | 不適用 | 不適用 |
| PBM* | 不適用 | 不適用 |
| PPM* | 不適用 | 不適用 |
| PSD | ý | ✕ |
| EPS | 不適用 | ✕ |
| DNG | ý | ✕ |
| PICT | ý | ✕ |
| PSB* | ý | ✕ |
| JPG | ý | ý |
| AI | ý | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ý | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ý | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ý | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ý | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| EPUB | ý | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| MPG | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | 不適用 | ✕ |
| JAR | ý | ✕ |
| RAR | 不適用 | ✕ |
| TAR | 不適用 | ✕ |
| ZIP | ý | ✕ |

下圖說明矩陣中使用的符號：

| 符號 | 意義 |
|---|---|
| ý | 此檔案格式支援此功能 |
| ✕ | 此檔案格式不支援此功能 |
| 不適用 | 此功能不適用於此檔案格式 |
| * | 這項功能需要AEM作者例項上此檔案格式的附加支援，但是在資產發佈至品牌入口網站後，不需要在品牌入口網站上支援 |

## 取消共用資產作為連結{#unshare-assets-shared-as-a-link}共用

若要取消共用先前共用的資產做為連結，請執行下列動作：

1. 當您登入品牌入口網站時，預設會開啟&#x200B;**[!UICONTROL 檔案]**&#x200B;檢視。 若要檢視您共用為連結的資產，請導覽至「共用連結」**[!UICONTROL 檢視。]**

1. 檢視您從顯示的清單中共用的連結。

   ![](assets/shared-links.png)

1. 若要從清單中取消共用連結，請選取該連結，然後按一下頂端工具列上的「取消共用&#x200B;****」圖示。

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >共用連結的顯示是使用者專屬的。 此功能不會顯示租用戶所有使用者共用的所有連結。

1. 在警告訊息方塊中，按一下「繼續&#x200B;**[!UICONTROL 」以確認取消共用。]**&#x200B;連結的項目會從共用連結清單中移除。
