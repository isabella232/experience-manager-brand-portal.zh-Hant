---
title: 以連結方式共用資產
seo-title: Share assets as a link
description: Adobe Experience Manager Assets Brand Portal管理員可與授權的內部使用者和外部實體（包括合作夥伴和廠商）共用多個資產的連結。 編輯人員只能檢視和共用與他們共用的資產。
seo-description: Adobe Experience Manager Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: e3e35ad4be5c082ad7bac7bed8ea20a186d245ad
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 5%

---

# 以連結方式共用資產 {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal管理員可與授權的內部使用者及外部實體（包括合作夥伴和廠商）共用多個資產的連結。 編輯人員只能檢視和共用與他們共用的資產。

透過連結共用資產是讓外部使用者能使用的便利方式，因為接收者不必登入Brand Portal即可存取資產。

<!-- Link sharing access is restricted to editors and administrators. 
-->

如需詳細資訊，請參閱 [管理使用者、群組和使用者角色](../using/brand-portal-adding-users.md#manage-user-roles).


以下是以連結形式共用資產的步驟：

1. 登入您的Brand Portal租用戶。 依預設， **[!UICONTROL 檔案]** 「檢視」隨即開啟，其中包含所有已發佈的資產和資料夾。

1. 選取您要共用的資產或資料夾，或導覽至 **[!UICONTROL 集合]** 檢視來共用您已建立的集合。

   ![select-multiple assets](assets/select-assets-new.png)

1. 在頂端的工具列中，按一下 **[!UICONTROL 共用連結]** 表徵圖。

   此 **[!UICONTROL 連結共用]** 對話框。

   ![](assets/link-sharing.png)

   * 在電子郵件地址方塊中，輸入您要共用連結之使用者的電子郵件ID。 您可以與多個使用者共用連結。 如果使用者是您組織的成員，請從下拉式清單中顯示的建議中選取其電子郵件ID。 如果使用者為外部，請輸入完整的電子郵件ID，然後按 **[!UICONTROL 輸入]**;電子郵件ID會新增至使用者清單。

      ![](assets/link-sharing-text.png)

   * 在 **[!UICONTROL 主旨]** 方塊中，輸入您要共用資產的主旨。
   * 在 **[!UICONTROL 訊息]** 框中，視需要鍵入消息。
   * 在 **[!UICONTROL 過期]** 欄位中，使用日期選擇器來指定連結的到期日期和時間。 依預設，到期日會設為自您共用連結的日期起7天。
   * 啟用 **[!UICONTROL 允許下載原始檔案]** 核取方塊，讓收件者下載原始轉譯。

   透過連結共用的資產，會在超過 **[!UICONTROL 過期]** 欄位。 如需Brand Portal中過期資產的行為以及根據使用者角色允許的活動進行哪些變更的相關資訊，請參閱 [管理資產的數位版權](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >連結的預設過期時間為7天。 連結必須以電子郵件傳送給使用者，使用 **[!UICONTROL 連結共用]** ，請勿分別複製和共用連結。

1. 按一下&#x200B;**[!UICONTROL 「共用」]**。訊息會確認連結已與使用者共用。 使用者會收到包含共用連結的電子郵件。

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >管理員可以自訂電子郵件訊息，包括使用自訂標誌、說明和頁尾 [品牌推廣](../using/brand-portal-branding.md) 功能。

## 從共用連結下載資產 {#download-assets-from-shared-links}

按一下電子郵件中的連結，以存取共用資產。 「 AEM連結共用」頁面隨即開啟。

若要下載共用資產：

1. 按一下資產或資料夾，然後按一下 **[!UICONTROL 下載]** 圖示。

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >目前，您只能根據檔案格式，針對特定資產產生預覽和縮圖。 有關支援的檔案格式的詳細資訊，請參見 [資產格式的預覽和縮圖支援](#preview-thumbnail-support).

1. 此 **[!UICONTROL 下載]** 對話框。

   ![下載對話](assets/download-dialog-box-new.png)

1. 依預設， **[!UICONTROL 快速下載]** 中的 **[!UICONTROL 下載設定]**. 因此，確認方塊似乎會繼續使用IBM Aspera Connect下載。

   若要繼續使用 **[!UICONTROL 快速下載]**，按一下 **[!UICONTROL 允許]**.

   所有選取的轉譯都會下載至zip資料夾中，其中包含每個資產的個別資料夾。

   >[!NOTE]
   >
   >從共用連結下載資產時，系統會為每個資產建立個別的資料夾。
   >
   >如果選取要下載的資料夾、集合或超過20個資產， **[!UICONTROL 下載]** 會略過對話方塊，而使用者可存取的所有資產轉譯（排除動態轉譯）會下載至zip資料夾，其中包含每個資產的個別資料夾。

   >[!NOTE]
   >
   >如果以連結形式共用資產的使用者並未使用共用連結，則不會使用共用連結下載原始轉譯 [授權管理員存取原始轉譯](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).


>[!NOTE]
>
>Brand Portal會限制使用連結共用來下載大小超過5 GB的資料夾或資產。

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

-->

## 資產格式的預覽和縮圖支援 {#preview-thumbnail-support}

下列矩陣列出Brand Portal支援縮圖和預覽的資產格式：

| 資產格式 | 縮圖支援 | 預覽支援 |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| PNM* | 不適用 | 不適用 |
| PGM* | 不適用 | 不適用 |
| PBM* | 不適用 | 不適用 |
| PPM* | 不適用 | 不適用 |
| PSD | ✓ | ✕ |
| EPS | 不適用 | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| ePub | ✓ | ✕ |
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
| JAR | ✓ | ✕ |
| RAR | 不適用 | ✕ |
| TAR | 不適用 | ✕ |
| ZIP | ✓ | ✕ |

下圖說明矩陣中使用的符號：

| 符號 | 意義 |
|---|---|
| ✓ | 此檔案格式支援此功能 |
| ✕ | 此檔案格式不支援此功能 |
| 不適用 | 此功能不適用於此檔案格式 |
| &#42; | 此功能需要AEM製作例項上此檔案格式的附加支援，但在資產發佈至Brand Portal後，不需要在Brand Portal上支援 |

## 取消共用以連結形式共用的資產 {#unshare-assets-shared-as-a-link}

若要取消共用先前共用的資產作為連結，請執行下列動作：

1. 登入Brand Portal時， **[!UICONTROL 檔案]** 視圖預設會開啟。 若要檢視您以連結形式共用的資產，請導覽至 **[!UICONTROL 共用連結]** 檢視。

1. 從顯示的清單中檢閱您共用的連結。

   ![](assets/shared-links.png)

1. 若要從清單中取消共用連結，請選取該連結，然後按一下 **[!UICONTROL 取消共用]** 圖示。

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >共用連結的顯示是使用者專屬的。 此功能不會顯示租用戶的所有使用者共用的所有連結。

1. 在警告訊息方塊中，按一下 **[!UICONTROL 繼續]** 確認取消共用。 連結的項目會從共用連結清單中移除。
