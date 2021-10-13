---
title: Experience Manager Assets Brand Portal概述
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal可協助您輕鬆取得、控制並安全地跨裝置將經過核准的創意資產發佈給外部人士和內部企業使用者。
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: ec52e1900e4ac9ec664d88c4b5fb492df4d4a32f
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 6%

---

# Experience Manager Assets Brand Portal概述 {#overview-of-aem-assets-brand-portal}

身為行銷人員，您有時需要與通路合作夥伴和內部業務使用者共同合作，以快速建立、管理相關數位內容，並將其提供給客戶。 在整個客戶歷程中及時傳遞相關內容，對於推動更大的需求、轉換、參與和客戶忠誠度至關重要。

但是，要開發能支援與擴大的內部團隊、合作夥伴和經銷商高效且安全地共用已核准品牌標誌、准則、行銷活動資產或產品快照的解決方案，將是一項挑戰。

**Adobe Experience Manager(AEM)Assets品牌** 入口網站著重於行銷人員需要透過提供資產發佈和資產貢獻功能，與分散於全球各地的Brand Portal使用者有效協作。

資產發佈可讓您輕鬆取得、控制並安全地跨裝置將經過核准的創意資產發佈給外部方和內部業務使用者。 但是，資產貢獻可讓Brand Portal使用者將資產上傳至Brand Portal並發佈至Experience Manager Assets，而不需存取製作環境。 貢獻功能稱為&#x200B;**Brand Portal中的Assets Sourcing**。 同時，它還能改進Brand Portal資產分銷的整體體驗，並改善Brand Portal使用者（外部機構/團隊）的貢獻，加快資產上市時間，並降低不合規和未授權存取的風險。
請參閱[Brand Portal中的Asset Sourcing](brand-portal-asset-sourcing.md)。

瀏覽器入口網站環境可讓您輕鬆上傳、瀏覽、搜尋、預覽和匯出已核准格式的資產。

## 透過 Brand Portal 設定 Experience Manager Assets {#configure-brand-portal}

使用Brand Portal設定Adobe Experience Manager資產，可為Brand Portal使用者啟用資產發佈、資產分發和資產貢獻功能。

>[!NOTE]
>
>Experience Manager Assetsas a Cloud Service、Experience Manager Assets 6.3及更新版本均支援使用Brand Portal設定Experience Manager Assets。

Experience Manager Assetsas a Cloud Service會透過從Cloud Manager啟動Brand Portal自動透過Brand Portal進行設定。 啟動工作流程會在後端建立必要的設定，並在與Experience Manager Assetsas a Cloud Service例項相同的IMS組織上啟動Brand Portal。

然而，Experience Manager Assets（內部部署和托管服務）是使用Brand Portal Developer Console手動設定，其會擷取AdobeIdentity Management服務(IMS)代號，以授權Brand Portal租用戶。

如需詳細資訊，請參閱[使用Brand Portal設定Experience Manager Assets](../using/configure-aem-assets-with-brand-portal.md)。

## Brand Portal中的使用者角色 {#Personas}

Brand Portal支援下列使用者角色：

* 來賓用戶
* 檢視者
* 編輯者
* 管理員

下表列出這些角色中的使用者可執行的任務：

|  | **瀏覽** | **搜尋** | **下載** | **共用資料夾** | **共用集合** | **以連結方式共用資產** | **存取管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **來賓用戶** | ✓* | ✓* | ✓* | x | x | x | x |
| **檢視者** | ✓ | ✓ | ✓ | x | x | x | x |
| **編輯者** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理員** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>訪客使用者只能瀏覽、存取和搜尋公用資料夾和集合中的資產。

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 來賓用戶 {#guest-user}

任何使用者只要在未進行驗證的情況下，對Brand Portal上的資產有有限的存取權，即為訪客使用者。 來賓會話允許用戶訪問公用資料夾和集合。 身為來賓使用者，您可以瀏覽資產詳細資訊，並擁有公用資料夾和集合成員的完整資產檢視。 您可以搜尋、下載和新增公用資產至[!UICONTROL Lightbox]集合。

不過，來賓工作階段會限制您建立集合和已儲存的搜尋，並進一步共用。 來賓工作階段中的使用者無法存取資料夾和集合設定，且無法以連結形式共用資產。 以下是來賓用戶可執行的任務清單：

* [瀏覽及存取公共資產](browse-assets-brand-portal.md)

* [搜尋公用資產](brand-portal-searching.md)

* [下載公開資產](brand-portal-download-assets.md)

* [將資產新增至[!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### 檢視者 {#viewer}

Brand Portal中的標準使用者通常是具有檢視器角色的使用者。 具有此角色的使用者可以存取允許的資料夾、集合和資產。 使用者也可以瀏覽、預覽、下載和匯出資產（原始或特定轉譯）、設定帳戶設定，以及搜尋資產。 以下是檢視器可執行的工作清單：

* [瀏覽資產](browse-assets-brand-portal.md)

* [搜尋資產](brand-portal-searching.md)

* [下載資產](brand-portal-download-assets.md)

### 編輯者 {#editor}

具有編輯者角色的使用者可以執行檢視器可執行的所有工作。 此外，和編輯器還可以查看管理員共用的檔案和資料夾。 具有編輯者角色的使用者也可以與其他人共用內容（檔案、資料夾、集合）。

除了檢視器可執行的工作之外，編輯器還可執行下列其他工作：

* [共用資料夾](brand-portal-sharing-folders.md)

* [共用集合](brand-portal-share-collection.md)

* [以連結方式共用資產](brand-portal-link-share.md)

### 管理員 {#administrator}

管理員包括在[!UICONTROL Admin Console]中標籤為系統管理員或Brand Portal產品管理員的用戶。 管理員可以添加和刪除系統管理員和用戶、定義預設集、向用戶發送電子郵件，以及查看門戶使用情況和儲存報告。

管理員可以執行編輯器可以執行的所有任務：

* [管理使用者、群組和使用者角色](brand-portal-adding-users.md)

* [自訂壁紙、頁面標題和電子郵件](brand-portal-branding.md)

* [使用自訂搜尋 Facet](brand-portal-search-facets.md)

* [使用中繼資料結構表單](brand-portal-metadata-schemas.md)

* [套用影像預設集或動態轉譯](brand-portal-image-presets.md)

* [使用報表](brand-portal-reports.md)

除了上述工作，AEM Assets中的作者還可執行下列工作：

* [使用 Brand Portal 設定 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

* [將資料夾發佈至 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [將集合發佈至 Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Brand Portal url的替代別名 {#tenant-alias-for-portal-url}

Brand Portal 6.4.3之後，組織可以有一個替代（別名）URL供其Brand Portal租用戶的現有URL使用。 別名URL可借由在URL中有替代首碼來建立。\
請注意，只能自訂Brand Portal URL的首碼，不能自訂整個URL。 例如，現有網域`geomettrix.brand-portal.adobe.com`的組織可依請求建立`geomettrixinc.brand-portal.adobe.com`。

不過，AEM Author例項只能使用租用戶ID URL來設定[](../using/configure-aem-assets-with-brand-portal.md)，而不能使用租用戶別名（替代）URL。

>[!NOTE]
>
>若要在現有入口URL中取得租用戶名稱的別名，組織需要透過新的租用戶別名建立請求，聯絡客戶支援。 首先檢查別名是否可用，然後建立別名，即可處理此請求。
>
>要替換舊別名或刪除舊別名，必須執行相同的進程。

## 要求存取Brand Portal {#request-access-to-brand-portal}

使用者可從登入畫面要求存取Brand Portal。 這些要求會傳送給Brand Portal管理員，這些管理員會透過[!UICONTROL Admin Console]Adobe授與使用者的存取權。 授予存取權後，使用者會收到通知電子郵件。

要請求訪問，請執行以下操作：

1. 從Brand Portal登入頁面中，選取&#x200B;**[!UICONTROL 按一下這裡]**&#x200B;並對應於&#x200B;**[!UICONTROL 需要存取？]**. 但是，要進入來賓會話，請選擇與&#x200B;**[!UICONTROL 來賓訪問？]**&#x200B;對應的&#x200B;**[!UICONTROL 按一下這裡]**。

   ![Brand Portal登入畫面](assets/bp-login-requestaccess.png)

   將開啟「[!UICONTROL 請求訪問]」頁。

1. 若要要求存取組織的Brand Portal，您必須具備有效的[!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL Federated ID]。

   在[!UICONTROL 要求存取]頁面中，使用您的ID（案例1）登入或建立[!UICONTROL Adobe ID]（案例2）:

   ![[!UICONTROL 要求存取]](assets/bplogin_request_access_2.png)

   **方案1**

   1. 如果您有[!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL Federated ID]，請按一下&#x200B;**[!UICONTROL 登入]**。
[!UICONTROL 登入]頁面隨即開啟。

   1. 提供您的[!UICONTROL Adobe ID]憑證，然後按一下&#x200B;**[!UICONTROL 登入]**。

      ![Adobe登入](assets/bplogin_request_access_3.png)
   系統會將您重新導向至[!UICONTROL 要求存取]頁面。

   **方案2**

   1. 若您沒有[!UICONTROL Adobe ID]，若要建立此變數，請從[!UICONTROL 請求存取]頁面按一下&#x200B;**[!UICONTROL 取得Adobe ID]**。
[!UICONTROL 登入]頁面隨即開啟。
   1. 按一下「**[!UICONTROL 取得Adobe ID]**」。
將開啟[!UICONTROL 註冊]頁面。
   1. 輸入您的名字和姓氏、電子郵件ID和密碼。
   1. 選擇&#x200B;**[!UICONTROL 註冊]**。

      ![](assets/bplogin_request_access_5.png)
   系統會將您重新導向至[!UICONTROL 要求存取]頁面。

1. 下一頁會顯示您的名稱，以及用於要求存取權的電子郵件ID。 留下管理員的注釋，然後按一下&#x200B;**[!UICONTROL Submit]**。

   ![](assets/bplogin-request-access.png)

## 產品管理員授予存取權 {#grant-access-to-brand-portal}

Brand Portal產品管理員會在其Brand Portal通知區域和透過收件匣的電子郵件接收存取要求。

![訪問請求的通知](assets/bplogin_request_access_7.png)

若要授與存取權，產品管理員必須按一下Brand Portal通知區域中的相關通知，然後按一下&#x200B;**[!UICONTROL 授與存取權]**。
或者，產品管理員可以遵循存取請求電子郵件中提供的連結，瀏覽Adobe[!UICONTROL Admin Console]，並將使用者新增至相關產品設定。

系統會將您重新導向至[Adobe[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)首頁。 使用Adobe[!UICONTROL Admin Console]來建立使用者，並將其指派給產品設定檔（舊稱為產品設定檔），這些設定檔在Brand Portal中顯示為群組。 有關在[!UICONTROL Admin Console]中添加用戶的詳細資訊，請參閱[添加用戶](brand-portal-adding-users.md#add-a-user)（按照過程中的步驟4-7添加用戶）。

## Brand Portal語 {#brand-portal-language}

您可以從「Adobe[!UICONTROL Experience Cloud設定]」變更Brand Portal語言。

![訪問請求的通知](assets/BPLang.png)

若要變更語言：

1. 從頂部菜單中選擇「[!UICONTROL 用戶] > [!UICONTROL 編輯配置檔案]」。

   ![編輯設定檔](assets/EditBPProfile.png)

1. 在[!UICONTROL Experience Cloud設定]頁面，從[!UICONTROL 語言]下拉式選單中選取語言。

## Brand Portal維護通知 {#brand-portal-maintenance-notification}

在排程Brand Portal進行維護之前，您登入Brand Portal後，通知會顯示為橫幅。 範例通知：

![](assets/bp_maintenance_notification.png)

您可以關閉此通知，然後繼續使用Brand Portal。 此通知會顯示在每個新工作階段中。

## 發行和系統資訊 {#release-and-system-information}

* [新功能](whats-new.md)
* [發行說明](brand-portal-release-notes.md)
* [支援的檔案格式](brand-portal-supported-formats.md)

## 相關資源 {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [AEM論壇](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
