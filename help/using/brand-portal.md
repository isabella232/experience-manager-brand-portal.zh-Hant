---
title: Experience Manager AssetsBrand Portal概述
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager AssetsBrand Portal可幫助您輕鬆獲得、控制和安全地將經批准的創意資產分散給外部各方和跨設備的內部業務用戶。
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 72a303082c1456b98143f740c228c73926f2fb3e
workflow-type: tm+mt
source-wordcount: '1558'
ht-degree: 6%

---

# Experience Manager AssetsBrand Portal概述 {#overview-of-aem-assets-brand-portal}

作為營銷人員，您有時需要與渠道合作夥伴和內部業務用戶協作，以快速建立、管理和向客戶交付相關數字內容。 在整個客戶過程中及時交付相關內容對於推動更大的需求、轉換、接洽和客戶忠誠度至關重要。

但是，開發支援與擴展的內部團隊、合作夥伴和轉銷商高效、安全地共用經批准的品牌標誌、准則、活動資產或產品快照的解決方案是一項挑戰。

**Adobe Experience Manager(AEMAssets Brand Portal)** 重點強調營銷商通過提供資產分配和資產貢獻能力與全球分佈的Brand Portal用戶進行有效協作的需要。

資產分配使您能夠方便地獲得、控制和安全地將經批准的創造性資產分散到外部各方和跨設備的內部業務用戶。 然而，資產貢獻使Brand Portal用戶能夠將資產上傳到Brand Portal並發佈到Experience Manager Assets，而無需訪問作者環境。 貢獻特徵稱為 **Brand Portal資產採購**。 而且，它共同改善了Brand Portal在資產分配方面的總體經驗和Brand Portal用戶（外部機構/團隊）的貢獻，加快了資產上市的時間，並降低了不遵守法規和未經授權的訪問的風險。
看， [Brand Portal資產來源補充](brand-portal-asset-sourcing.md)。

通過基於瀏覽器的門戶環境，您可以輕鬆地以批准的格式上載、瀏覽、搜索、預覽和導出資產。

## 透過 Brand Portal 設定 Experience Manager Assets {#configure-brand-portal}

將Adobe Experience Manager資產配置為Brand Portal可為Brand Portal用戶啟用資產發佈、資產分配和資產貢獻功能。

>[!NOTE]
>
>在Experience Manager Assetsas a Cloud Service、Experience Manager Assets6.3及更高版本上支援將Experience Manager Assets配置為Brand Portal。

Experience Manager Assetsas a Cloud Service通過從雲管理器激活Brand Portal自動配置為Brand Portal。 激活工作流在後端建立所需的配置，並在與Experience Manager Assetsas a Cloud Service實例相同的IMS組織上激活Brand Portal。

然而，Experience Manager Assets（內部和托管服務）使用Adobe Developer控制台手動配置為Brand Portal，該控制台為Brand Portal租戶授權採購AdobeIdentity Management服務(IMS)令牌。

有關詳細資訊，請參見 [配置Experience Manager Assets和Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。

## Personas在Brand Portal {#Personas}

Brand Portal支援以下用戶角色：

* 來賓用戶
* 檢視者
* 編輯者
* 管理員

下表列出了這些角色中的用戶可以執行的任務：

|  | **瀏覽** | **搜尋** | **下載** | **共用資料夾** | **共用集合** | **以連結方式共用資產** | **訪問管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **來賓用戶** | ✓* | ✓* | ✓* | x | x | x | x |
| **檢視者** | ✓ | ✓ | ✓ | x | x | x | x |
| **編輯者** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理員** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>來賓用戶只能瀏覽、訪問和搜索公用資料夾和集合中的資產。

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 來賓用戶 {#guest-user}

對Brand Portal上的資產具有有限訪問權限而無需進行身份驗證的任何用戶都是來賓用戶。 來賓會話允許用戶訪問公共資料夾和集合。 作為來賓用戶，您可以瀏覽資產詳細資訊並查看公用資料夾和集合成員的完整資產視圖。 您可以搜索、下載和添加公共資產到 [!UICONTROL 燈箱] 的下界。

但是，來賓會話會限制您建立集合和保存的搜索，並進一步共用它們。 來賓會話中的用戶無法訪問資料夾和集合設定，並且不能將資產作為連結共用。 以下是來賓用戶可以執行的任務清單：

* [瀏覽和訪問公共資產](browse-assets-brand-portal.md)

* [搜索公共資產](brand-portal-searching.md)

* [下載公共資產](brand-portal-download-assets.md)

* [將資產添加到 [!UICONTROL 燈箱]](brand-portal-light-box.md#add-assets-to-lightbox)

### 檢視者 {#viewer}

Brand Portal的標準用戶通常是具有Viewer角色的用戶。 具有此角色的用戶可以訪問允許的資料夾、集合和資產。 用戶還可以瀏覽、預覽、下載和導出資產（原始或特定格式副本）、配置帳戶設定以及搜索資產。 以下是查看器可執行的任務清單：

* [瀏覽資產](browse-assets-brand-portal.md)

* [搜索資產](brand-portal-searching.md)

* [下載資產](brand-portal-download-assets.md)

### 編輯者 {#editor}

具有編輯器角色的用戶可以執行查看器可以執行的所有任務。 此外，編輯器還可以查看管理員共用的檔案和資料夾。 具有編輯器角色的用戶還可以與其他用戶共用內容（檔案、資料夾、集合）。

除了查看器可以執行的任務外，編輯器還可以執行以下附加任務：

* [共用資料夾](brand-portal-sharing-folders.md)

* [共用集合](brand-portal-share-collection.md)

* [以連結方式共用資產](brand-portal-link-share.md)

### 管理員 {#administrator}

管理員包括在中標籤為系統管理員或Brand Portal產品管理員的用戶 [!UICONTROL Admin Console]。 管理員可以添加和刪除系統管理員和用戶、定義預設、向用戶發送電子郵件以及查看門戶使用情況和儲存報告。

>[!NOTE]
>
>在Brand Portal，在 [!UICONTROL Admin Console] 具有與系統管理員相同的權限。

管理員可以執行編輯器可以執行的所有任務。 以下是管理員可以執行的其他任務：

* [管理使用者、群組和使用者角色](brand-portal-adding-users.md)

* [自定義牆紙、頁眉和電子郵件](brand-portal-branding.md)

* [使用自訂搜尋 Facet](brand-portal-search-facets.md)

* [使用中繼資料結構表單](brand-portal-metadata-schemas.md)

* [套用影像預設集或動態轉譯](brand-portal-image-presets.md)

* [使用報表](brand-portal-reports.md)

除上述任務外，AEM Assets的作者還可以執行以下任務：

* [使用 Brand Portal 設定 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

* [將資料夾發佈至 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [將集合發佈至 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Brand PortalURL的替代別名 {#tenant-alias-for-portal-url}

Brand Portal6.4.3以後，組織可以有一個備用（別名）URL，用於其Brand Portal租戶的現有URL。 別名URL可通過在URL中具有備用前置詞來建立。\
請注意，只能自定義Brand PortalURL的前置詞，而不能自定義整個URL。 例如，具有現有域的組織 `geomettrix.brand-portal.adobe.com` 能 `geomettrixinc.brand-portal.adobe.com` 已根據請求建立。

但是，AEM作者實例可以 [配置](../using/configure-aem-assets-with-brand-portal.md) 僅具有租戶ID URL，而不具有租戶別名（備用）URL。

>[!NOTE]
>
>要獲取現有門戶URL中租戶名稱的別名，組織需要使用新的租戶別名建立請求與客戶支援部門聯繫。 通過首先檢查別名是否可用，然後建立別名來處理此請求。
>
>要替換舊別名或刪除舊別名，需要執行相同的進程。

## 請求訪問Brand Portal {#request-access-to-brand-portal}

用戶可以從登錄螢幕請求訪問Brand Portal。 這些請求將發送給Brand Portal管理員，這些管理員通過Adobe授予用戶訪問權限 [!UICONTROL Admin Console]。 授予訪問權限後，用戶將收到通知電子郵件。

要請求訪問，請執行以下操作：

1. 在Brand Portal登錄頁中，選擇 **[!UICONTROL 按一下這裡]** 對應 **[!UICONTROL 需要訪問？]**. 但是，要輸入來賓會話，請選擇 **[!UICONTROL 按一下這裡]** 對應 **[!UICONTROL 來賓訪問？]**。

   ![Brand Portal登錄螢幕](assets/bp-login-requestaccess.png)

   的 [!UICONTROL 請求訪問] 的上界。

1. 要請求訪問組織的Brand Portal，您必須具有 [!UICONTROL Adobe ID]。 [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]。

   在 [!UICONTROL 請求訪問] 頁面，使用ID登錄（方案1）或建立 [!UICONTROL Adobe ID] （場景2）:

   ![[!UICONTROL 請求訪問]](assets/bplogin_request_access_2.png)

   **方案1**

   1. 如果你有 [!UICONTROL Adobe ID]。 [!UICONTROL Enterprise ID]或 [!UICONTROL Federated ID]按一下 **[!UICONTROL 登錄]**。
的 [!UICONTROL 登錄] 的上界。

   1. 提供 [!UICONTROL Adobe ID] 按一下 **[!UICONTROL 登錄]**。

      ![Adobe登錄](assets/bplogin_request_access_3.png)
   您被重定向到 [!UICONTROL 請求訪問] 的子菜單。

   **方案2**

   1. 如果你沒有 [!UICONTROL Adobe ID]，按一下 **[!UICONTROL 找個Adobe ID]** 從 [!UICONTROL 請求訪問] 的子菜單。
的 [!UICONTROL 登錄] 的上界。
   1. 按一下 **[!UICONTROL 找個Adobe ID]**。
的 [!UICONTROL 註冊] 的上界。
   1. 輸入您的姓名、電子郵件ID和密碼。
   1. 選擇 **[!UICONTROL 註冊]**。

      ![](assets/bplogin_request_access_5.png)
   您被重定向到 [!UICONTROL 請求訪問] 的子菜單。

1. 下一頁顯示您的名稱和用於請求訪問的電子郵件ID。 為管理員留下注釋，然後按一下 **[!UICONTROL 提交]**。

   ![](assets/bplogin-request-access.png)

## 產品管理員授予訪問權限 {#grant-access-to-brand-portal}

Brand Portal產品管理員在其Brand Portal通知區域和收件箱中通過電子郵件接收訪問請求。

![訪問請求的通知](assets/bplogin_request_access_7.png)

要授予訪問權限，產品管理員需要按一下Brand Portal通知區中的相關通知，然後按一下 **[!UICONTROL 授予訪問權限]**。
或者，產品管理員可以按照訪問請求電子郵件中提供的連結訪問Adobe [!UICONTROL Admin Console] 並將用戶添加到相關產品配置中。

您被重定向到 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 的子菜單。 使用Adobe [!UICONTROL Admin Console] 建立用戶並將其分配給產品配置檔案（以前稱為產品配置），這些配置檔案在Brand Portal顯示為組。 有關在中添加用戶的詳細資訊 [!UICONTROL Admin Console]，請參閱 [添加用戶](brand-portal-adding-users.md#add-a-user) （按照步驟4-7添加用戶）。

## Brand Portal語 {#brand-portal-language}

你可以把Brand Portal語從Adobe [!UICONTROL Experience Cloud設定]。

![訪問請求的通知](assets/BPLang.png)

要更改語言：

1. 選擇 [!UICONTROL 用戶] > [!UICONTROL 編輯配置檔案] 的上界。

   ![編輯設定檔](assets/EditBPProfile.png)

1. 開 [!UICONTROL Experience Cloud設定] 的子菜單。 [!UICONTROL 語言] 的下界。

## Brand Portal維護通知 {#brand-portal-maintenance-notification}

在Brand Portal計畫停機進行維護之前，您登錄Brand Portal後，將顯示一條通知作為橫幅。 示例通知：

![](assets/bp_maintenance_notification.png)

您可以取消此通知並繼續使用Brand Portal。 此通知將出現在每個新會話中。

## 發佈和系統資訊 {#release-and-system-information}

* [新功能](whats-new.md)
* [發行說明](brand-portal-release-notes.md)
* [支援的檔案格式](brand-portal-supported-formats.md)

## 相關資源 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [論AEM壇](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
