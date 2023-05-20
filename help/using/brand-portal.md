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
source-git-commit: fb2ce4d39fd9e7aa69ba541bd48a6b9cddd3b4c5
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 6%

---

# Experience Manager AssetsBrand Portal概述 {#overview-of-aem-assets-brand-portal}

作為營銷人員，您有時需要與渠道合作夥伴和內部業務用戶協作，以快速建立、管理和向客戶交付相關數字內容。 在整個客戶過程中及時交付相關內容對於推動更大的需求、轉換、接洽和客戶忠誠度至關重要。

但是，開發支援與擴展的內部團隊、合作夥伴和轉銷商高效、安全地共用經批准的品牌標誌、准則、活動資產或產品快照的解決方案是一項挑戰。

**Adobe Experience Manager(AEMAssets Brand Portal)** 重點強調營銷商通過提供資產分配和資產貢獻能力與全球分佈的Brand Portal用戶進行有效協作的需要。

資產分配使您能夠方便地獲得、控制和安全地將經批准的創造性資產分散到外部各方和跨設備的內部業務用戶。 不過，資產貢獻可讓品牌入口網站使用者上傳資產品牌入口網站和發佈，而不需要存取作者 Experience Manager。 貢獻特徵稱為 **Brand Portal資產採購**。 同時，它提高了資產發佈的整體品牌入口網站體驗，以及來自品牌入口網站使用者（外部代理/團隊）的貢獻，加速了上市時間的資產，並降低了違反管理法規和未授權存取的風險。[請參閱品牌入口網站 ](brand-portal-asset-sourcing.md) 中的資產來源。

以瀏覽器為基礎的 portal 環境可讓您輕鬆上傳、流覽、搜尋、預覽和匯出已核准格式的資產。

## 透過 Brand Portal 設定 Experience Manager Assets {#configure-brand-portal}

將Adobe Experience Manager資產配置為Brand Portal可為Brand Portal用戶啟用資產發佈、資產分配和資產貢獻功能。

>[!NOTE]
>
>在Experience Manager Assetsas a Cloud Service、Experience Manager Assets6.3及更高版本上支援將Experience Manager Assets配置為Brand Portal。

Experience Manager Assetsas a Cloud Service通過從雲管理器激活Brand Portal自動配置為Brand Portal。 激活工作流在後端建立所需的配置，並在與Experience Manager Assetsas a Cloud Service實例相同的IMS組織上激活Brand Portal。

然而，Experience Manager Assets（內部和托管服務）使用Adobe Developer控制台手動配置為Brand Portal，該控制台為Brand Portal租戶授權採購AdobeIdentity Management服務(IMS)令牌。

有關詳細資訊，請參見 [配置Experience Manager Assets和Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。

## 品牌入口網站中的使用者角色 {#Personas}

品牌入口網站支援下列用戶角色：

* 訪客用戶
* 檢視者
* 編輯者
* 管理員

下表列出這些角色中的使用者可以執行的工作：

|  | **瀏覽** | **搜尋** | **下載** | **共用資料夾** | **共用集合** | **以連結方式共用資產** | **訪問管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **來賓用戶** | ✓* | ✓* | ✓* | x | x | x | x |
| **檢視者** | ✓ | ✓ | ✓ | x | x | x | x |
| **編輯器** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
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

Experience Manager AssetsBrand Portal [來賓訪問](#request-access-to-brand-portal) Brand Portal。 來賓用戶不需要憑據即可進入門戶，並且可以訪問公共資料夾和集合。 作為來賓用戶，您可以瀏覽資產詳細資訊並查看公用資料夾和集合成員的完整資產視圖。 您可以搜索、下載和添加公共資產到 [!UICONTROL 燈箱] 的下界。

不過，「訪客」會話會限制您建立集合和儲存的搜尋，並進一步分享。 來賓會話中的用戶無法訪問資料夾和集合設定，並且不能將資產作為連結共用。 以下是訪客用戶可以執行的工作清單：

* [瀏覽和存取公開資產](browse-assets-brand-portal.md)

* [Search 公開資產](brand-portal-searching.md)

* [下載公開資產](brand-portal-download-assets.md)

* [將資產添加到 [!UICONTROL 燈箱]](brand-portal-light-box.md#add-assets-to-lightbox)

有關詳細資訊，請參見 [來賓可訪問Brand Portal](../using/guest-access.md)。

### 檢視者 {#viewer}

Brand Portal用戶定義 [!DNL Admin Console] 可以以查看者的身份訪問Brand Portal。 具有此角色的用戶可以登錄Brand Portal並訪問允許的資料夾、集合和資產。 用戶還可以瀏覽、預覽、下載和導出資產（原始或特定格式副本）、配置帳戶設定以及搜索資產。 以下是查看器可執行的任務清單：

* [瀏覽資產](browse-assets-brand-portal.md)

* [Search 資產](brand-portal-searching.md)

* [下載資產](brand-portal-download-assets.md)

### 編輯者 {#editor}

具有編輯器角色的用戶可以執行檢視器可以執行的所有工作。 此外，也可視圖管理員共用的檔案和檔案夾。 使用編輯器角色的用戶也可以與其他人共用內容（檔案、資料夾、集合）。

除了檢視器可以執行的工作外，編輯器還可以執行下列其他工作：

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

* [自訂牆紙、頁面標題和電子郵件](brand-portal-branding.md)

* [使用自訂搜尋 Facet](brand-portal-search-facets.md)

* [使用中繼資料結構表單](brand-portal-metadata-schemas.md)

* [套用影像預設集或動態轉譯](brand-portal-image-presets.md)

* [使用報表](brand-portal-reports.md)

除了上述工作外，AEM Assets 中作者可以執行下列工作：

* [使用 Brand Portal 設定 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

* [將資料夾發佈至 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [將集合發佈至 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## 品牌入口網站 url 的備用別名 {#tenant-alias-for-portal-url}

品牌入口網站6.4.3，組織可以為其品牌入口網站租戶的現有 URL 擁有一個備用（別名） URL。 可透過在 URL 中使用備用首碼來建立別名 URL。\
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

1. 在Brand Portal登錄頁中，選擇 **[!UICONTROL 按一下這裡]** 對應 **[!UICONTROL 需要訪問？]**。但是，要輸入來賓會話，請選擇 **[!UICONTROL 按一下這裡]** 對應 **[!UICONTROL 來賓訪問？]**。

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

   1. 如果您沒有 Adobe ID ] ，請按一下 **[!UICONTROL 從要求存取 ] 頁面中 [!UICONTROL  取得 Adobe ID]** 。 [!UICONTROL 的 [!UICONTROL 登錄] 的上界。
   1. 按一下 **[!UICONTROL 「獲取 Adobe ID]** 。[!UICONTROL 註冊 ] 頁面開啟。
   1. 輸入您的姓氏和姓氏、電子郵件 ID 和密碼。
   1. 選取 **[!UICONTROL 註冊]** 。

      ![](assets/bplogin_request_access_5.png)
   您被重定向到 [!UICONTROL 請求訪問] 的子菜單。

1. 下一頁顯示您的名稱和用於請求訪問的電子郵件ID。 為管理員留下注釋，然後按一下 **[!UICONTROL 提交]**。

   ![](assets/bplogin-request-access.png)

## 產品管理員授予訪問權限 {#grant-access-to-brand-portal}

Brand Portal產品管理員在其Brand Portal通知區域和收件箱中通過電子郵件接收訪問請求。

![訪問請求的通知](assets/bplogin_request_access_7.png)

若要授權存取，產品管理員需按一下品牌入口網站通知區域中的相關通知，然後按一下 **[!UICONTROL 授予存取權]** 。或者，產品管理員可以追隨存取請求電子郵件中提供的連結，以造訪 Adobe Systems [!UICONTROL  Admin Console ] 並將用戶新增至相關產品設定。

您已重新導向至 [ Adobe Systems [!UICONTROL  Admin Console ] ](https://adminconsole.adobe.com/enterprise/overview) 首頁。使用 Adobe Systems [!UICONTROL  Admin Console ] 來建立使用者並將其指派至產品設定檔（先前稱為產品設定），在品牌入口網站中顯示為群組。 如需在 Admin Console ] 中 [!UICONTROL  新增使用者的詳細資訊，請參閱 [ 新增用戶 ](brand-portal-adding-users.md#add-a-user) （追隨步驟4-7 以新增用戶）。

## 品牌入口網站語言 {#brand-portal-language}

您可以從 Adobe Systems [!UICONTROL  Experience Cloud 設定 ] 變更品牌入口網站語言。

![存取請求的通知](assets/BPLang.png)

要更改語言：

1. 從頂部功能表中選擇 [!UICONTROL  使用者 ] > [!UICONTROL  編輯設定檔 ] 。

   ![編輯設定檔](assets/EditBPProfile.png)

1. 在 Experience Cloud 設定 ] 頁面上 [!UICONTROL  ，從語言 ] 下拉式功能表中 [!UICONTROL  選擇語言。

## 品牌入口網站維護通知 {#brand-portal-maintenance-notification}

在Brand Portal計畫停機進行維護之前，您登錄Brand Portal後，將顯示一條通知作為橫幅。 示例通知：

![](assets/bp_maintenance_notification.png)

您可以取消此通知並繼續使用Brand Portal。 此通知將出現在每個新會話中。

## 發佈和系統資訊 {#release-and-system-information}

* [新增功能](whats-new.md)
* [發行說明](brand-portal-release-notes.md)
* [支援的檔案格式](brand-portal-supported-formats.md)

## 相關資源 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM 論壇](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
