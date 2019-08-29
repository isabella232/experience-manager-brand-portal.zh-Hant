---
title: 將資產共用為連結
seo-title: 將資產共用為連結
description: AEM Assets Brand Portal管理員可以與授權內部使用者和外部實體(包括合作夥伴和廠商)共用多個資產的連結。編輯人員只能檢視和共用與他們共用的資產。
seo-description: AEM Assets Brand Portal管理員可以與授權內部使用者和外部實體(包括合作夥伴和廠商)共用多個資產的連結。編輯人員只能檢視和共用與他們共用的資產。
uuid: 8889ac24-c56 d-4a47-b792-80c34 ffb5 c3 f
contentOwner: bdhar
content-type: 引用
topic-tags: 共用
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: f3573319-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 將資產共用為連結 {#share-assets-as-a-link}

[!DNL AEM Assets Brand Portal] 管理員可以與授權內部使用者和外部實體共用多個資產連結，包括合作夥伴和廠商。編輯人員只能檢視和共用與他們共用的資產。

透過連結共用資產是方便外部廠商使用的便利方式，因為接收者不需要登入才能 [!DNL Brand Portal] 存取資產。

連結共用存取權僅限於編輯器和管理員。如需詳細資訊，請參閱 [管理使用者、群組和使用者角色](../using/brand-portal-adding-users.md#manage-user-roles)。

>[!NOTE]
>
>允許使用高達5GB的郵遞區號下載功能 [!DNL brand portal]。

若要將資產共用為連結，請遵循下列步驟：

1. 按一下左側的覆蓋圖示，然後選擇 **「導覽**」。

   ![](assets/siderail.png)

2. 從左側的側邊圖，按一下 **「檔案** 」以共用資料夾或影像。若要共用系列，請按一下 **[!UICONTROL 系列]**。

   ![](assets/navigationrail.png)

3. 選取您要共用為連結的資料夾或系列。

   ![](assets/asset-link-share.png)

4. 從上方的工具列，按一下 **「共用連結** 」圖示。

   **「連結共用」** 對話方塊隨即出現。

   ![](assets/link-sharing.png)

   >[!NOTE]
   >
   >**「共用連結** 」欄位會顯示自動建立的資產連結。此連結的預設過期時間為天。您可以複製連結並與使用者分開共用，或從 **「連結分享」** 對話方塊共用該連結。

5. 在電子郵件地址方塊中，輸入您要與其共用連結的使用者的電子郵件ID。您可以將連結與多個使用者共用。

   如果使用者是貴組織的成員，請從出現在下拉式清單中的建議中選擇其電子郵件ID。如果使用者是外部使用者，請輸入完整的電子郵件ID，然後按 **Enter**；電子郵件ID會新增至使用者清單。

   ![](assets/link-sharing-text.png)

6. 在 **「主旨** 」方塊中，輸入您要共用之資產的主旨。
7. 在 **「訊息** 」方塊中，視需要輸入訊息。
8. 在 **「過期」** 欄位中，使用日期選擇器指定連結的到期日和時間。根據預設，過期日期會設為您共用連結當日的天。

   透過連結共用的資產會在跨越 **「過期」** 欄位中指定的日期和時間後過期。如需有關過期資產的行為以及根據使用者 [!DNL Brand Portal]角色的權限活動變更的詳細資訊，請參閱 [管理資產數位權利](../using/manage-digital-rights-of-assets.md#asset-expiration)。

9. 按一下&#x200B;**「共用」**。會將訊息確認為與使用者共用連結。使用者會收到包含連結的電子郵件。

   ![](assets/link-sharing-email.png)

   >[!NOTE]
   >
   >管理員可以自訂電子郵件訊息，其中包括自訂標誌、說明和頁尾，並加上 [品牌](../using/brand-portal-branding.md) 功能。

## 從共用連結下載資產 {#download-assets-from-shared-links}

按一下電子郵件中的連結，即可檢視共用資產。[!DNL AEM] 「連結共用」頁面隨即開啓。

若要下載共用資產：

1. 按一下資產，然後按一下 **工具列中的「下載** 」圖示。

   ![](assets/assets-shared-link.png)

   >[!NOTE]
   >
   >目前，您只能針對特定資產產生預覽和縮圖，視檔案格式而定。如需支援檔案格式的詳細資訊，請參閱 [「預覽和縮圖支援資產格式](#preview-thumbnail-support)」。

   >[!NOTE]
   >
   >如果您下載的資產也包含授權資產，則會重新導向 **至「版權管理** 」頁面。在本頁中，選取授權資產，按一下 **「同意」**，然後按一下 **「下載**」。如果您選擇不同意，則只會下載未授權的資產。\
   >受授權保護的資產具有 [附加](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 的授權合約，可透過設定資產 [的中繼資料屬性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 來完成 [!DNL AEM Assets]。

   ![](assets/licensed-asset-download.png)

   **「下載」** 對話方塊隨即出現。
   ![](assets/download-linkshare.png)

   * 若要加快共用為連結的資產檔案下載，請選取 **「啓用下載加速** 選項」並 [遵循精靈](../using/accelerated-download.md#download-workflow-using-file-accelerator)。如需更多有關快速下載資產 [!DNL Brand Portal] 的參考 [指南，請參閱指南以加速下載[！DNL品牌入口網站]](../using/accelerated-download.md)。

2. 若要下載資產的轉譯以及共用連結的資產，請選取 **「轉譯」** 選項。當您這麼做時， **會顯示「排除系統轉譯** 」選項，預設會選取此選項。如此可防止下載立即可用的轉譯以及已核准資產或其自訂轉譯。

   不過，若要允許自動產生的轉譯連同自訂轉譯一起下載，請取消選取 **「排除系統轉譯** 」選項。

   >[!NOTE]
   >
   >如果共用資產的使用者未獲得管理員 [授權存取原始轉譯](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges)，則不會使用共用連結下載原始轉譯。

   ![](assets/download-linkshare-autoren.png)

3. 點選/按一下 **「下載**」。資產(若選取的話)會下載為ZIP檔案至您的本機資料夾。不過，如果下載單一資產而不使用任何轉譯，則不會建立郵遞區號，因此可確保快速下載。

>[!NOTE]
>
>[!DNL Brand Portal] 限制下載大小大於GB的檔案大小。

## 預覽和縮圖支援資產格式 {#preview-thumbnail-support}

下列矩陣列出 [!DNL Brand Portal] 支援縮圖和預覽的資產格式：

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
| PM* | 不適用 | 不適用 |
| PSD | ✓ | ✕ |
| EPS | 不適用 | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| OT* | ✕ | ✕ |
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
| EPUB | ✓ | ✕ |
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

下列圖例說明矩陣中使用的符號：

| 符號符號 | 意謂意義 |
|---|---|
| ✓ | 此檔案格式支援此功能 |
| ✕ | 此檔案格式不支援此功能 |
| 不適用 | 此功能不適用於此檔案格式 |
| * | 此功能需要在作者實例上 [!DNL AEM] 附加這個檔案格式的附加支援，而不是 [!DNL Brand Portal] 在資產發佈至 [!DNL Brand Portal] |

## 取消共用共用為連結的資產 {#unshare-assets-shared-as-a-link}

若要將先前共用資產取消共用為連結，請執行下列動作：

1. 若要檢視您共用的資產作為連結，請按一下左側的覆蓋圖示，然後選擇 **「導覽」**。

   ![](assets/siderail.png)

2. 從側邊圖中，按一下 **共用連結**。

   ![](assets/navigationrail.png)

3. 檢閱您從顯示的清單中共用的連結。
4. 若要取消共用清單中的連結，請選取該連結並按一下連結項目旁的bin圖示，或上方工具列上的 **「取消共用** 」圖示。

   ![](assets/unshare-links.jpg)

   >[!NOTE]
   >
   >共用連結的顯示為使用者專屬。此功能不會顯示所有用戶的所有使用者共用的連結。

5. 在警告訊息方塊中，按一下 **「繼續」** 確認取消共用。連結的項目會從共用連結清單中移除。
