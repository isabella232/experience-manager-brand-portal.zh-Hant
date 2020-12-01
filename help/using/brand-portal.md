---
title: AEM Assets品牌入口網站概觀
seo-title: AEM Assets品牌入口網站概觀
description: AEM Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部人士和內部企業使用者，並跨裝置發佈。
seo-description: AEM Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部人士和內部企業使用者，並跨裝置發佈。
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '1524'
ht-degree: 8%

---


# AEM Assets品牌入口網站簡介{#overview-of-aem-assets-brand-portal}

身為行銷人員，您有時需要與通路合作夥伴和內部商業使用者共同作業，以快速建立、管理並傳遞相關的數位內容給客戶。 在整個客戶歷程中及時傳遞相關內容，對於推動更大的需求、轉化、參與度和客戶忠誠度至關重要。

但是，開發解決方案以支援與延伸內部團隊、合作夥伴和經銷商有效且安全地分享經核准的品牌標誌、准則、宣傳資產或產品像片，是一項挑戰。

**Adobe Experience Manager(AEM)Assets Brand** Portal著重於行銷人員需要透過提供資產分發和資產貢獻功能，與全球分散的Brand Portal使用者有效協作。

資產分發可讓您輕鬆取得、控制並安全地透過各種裝置將經過核准的創意資產分發給外部人士和內部商業使用者。 但是，資產貢獻可讓品牌入口網站使用者將資產上傳至品牌入口網站並發佈至AEM資產，而不需存取作者環境。 貢獻功能稱為&#x200B;**品牌入口網站中的資產來源補充**。 此外，它可改善資產分發的整體品牌入口網站體驗，並從品牌入口網站使用者（外部機構／團隊）獲得貢獻，加速資產上市時間，並降低不合規和未授權存取的風險。
請參閱[品牌入口網站中的資產來源補充](brand-portal-asset-sourcing.md)。

以瀏覽器為基礎的入口網站環境可讓您以核准的格式輕鬆上傳、瀏覽、搜尋、預覽和匯出資產。

## 使用 Brand Portal 設定 AEM Assets {#configure-brand-portal}

Adobe Experience Manager(AEM)Assets是透過Adobe Developer Console設定品牌入口網站，該網站會購買IMS Token以授權您的品牌入口網站租用戶。

>[!NOTE]
>
>AEM Assets是雲端服務、AEM Assets 6.3及更新版本，支援透過Adobe Developer Console以品牌入口網站設定AEM Assets。

### 使用品牌入口網站{#prerequisites}設定AEM資產的必要條件

您需要下列項目才能使用 Brand Portal 設定 AEM Assets：

* 啟動並執行AEM Assets例項。
* Brand Portal 租用戶 URL。
* 在 Brand Portal 租用戶的 IMS 組織具有系統管理員權限的使用者。

如需詳細資訊，請參閱「設定AEM資產與品牌門戶[」。](../using/configure-aem-assets-with-brand-portal.md)

## 品牌入口網站{#Personas}中的使用者角色

品牌入口網站支援下列使用者角色：

* 來賓用戶
* 檢視者
* 編輯者
* 管理員

下表列出了這些角色中的用戶可以執行的任務：

|  | **瀏覽** | **搜尋** | **下載** | **共用資料夾** | **共用集合** | **以連結方式共用資產** | **存取管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **來賓用戶** | ý* | ý* | ý* | x | x | x | x |
| **檢視者** | ý | ý | ý | x | x | x | x |
| **編輯者** | ý | ý | ý | ý | ý | ý | x |
| **管理員** | ý | ý | ý | ý | ý | ý | ý |

*訪客使用者只能瀏覽、存取和搜尋公用資料夾和系列中的資產。

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### 來賓用戶{#guest-user}

任何未經驗證而對品牌入口網站上資產有限存取的使用者皆為訪客使用者。 來賓會話允許用戶訪問公共資料夾和集合。 身為來賓用戶，您可以瀏覽資產詳細資訊，並擁有公共資料夾和系列成員的完整資產視圖。 您可以搜尋、下載公共資產並新增至[!UICONTROL Lightbox]系列。

不過，來賓作業會限制您建立系列和已儲存的搜尋，並進一步共用。 來賓作業中的使用者無法存取資料夾和系列設定，也無法將資產共用為連結。 以下是來賓用戶可以執行的任務清單：

[瀏覽及存取公共資產](browse-assets-brand-portal.md)

[搜尋公共資產](brand-portal-searching.md)

[下載公用資產](brand-portal-download-assets.md)

[將資產新增至 [!UICONTROL 燈箱]](brand-portal-light-box.md#add-assets-to-lightbox)

### 檢視者 {#viewer}

品牌入口網站中的標準使用者通常是具有檢視器角色的使用者。 具有此角色的使用者可以存取允許的資料夾、系列和資產。 使用者也可以瀏覽、預覽、下載和匯出資產（原始或特定轉譯）、設定帳戶設定，以及搜尋資產。 以下是檢視器可執行的工作清單：

[瀏覽資產](browse-assets-brand-portal.md)

[搜尋資產](brand-portal-searching.md)

[下載資產](brand-portal-download-assets.md)

### 編輯者 {#editor}

具有編輯器角色的使用者可以執行檢視器可以執行的所有工作。 此外，編輯器還可以查看管理員共用的檔案和資料夾。 具有編輯器角色的使用者也可以與其他人共用內容（檔案、檔案夾、系列）。

除了檢視器可執行的工作外，編輯器還可執行下列其他工作：

[共用資料夾](brand-portal-sharing-folders.md)

[共用集合](brand-portal-share-collection.md)

[以連結方式共用資產](brand-portal-link-share.md)

### 管理員 {#administrator}

管理員在[!UICONTROL 管理控制台]中包含標示為系統管理員或品牌入口網站產品管理員的使用者。 管理員可以新增和移除系統管理員和使用者、定義預設集、傳送電子郵件給使用者，以及檢視入口網站的使用情況和儲存報告。

管理員可以執行編輯器可以執行的所有任務，以執行下列其他任務：

[管理使用者、群組和使用者角色](brand-portal-adding-users.md)

[自訂壁紙、頁首和電子郵件](brand-portal-branding.md)

[使用自訂搜尋 Facet](brand-portal-search-facets.md)

[使用中繼資料結構表單](brand-portal-metadata-schemas.md)

[套用影像預設集或動態轉譯](brand-portal-image-presets.md)

[使用報表](brand-portal-reports.md)

除了上述工作外，AEM Assets中的「作者」也可以執行下列工作：

[使用 Brand Portal 設定 AEM Assets](../using/configure-aem-assets-with-brand-portal.md)

[將資料夾發佈至 Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[將集合發佈至 Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## 品牌入口網站URL的替代別名{#tenant-alias-for-portal-url}

品牌入口網站6.4.3版之後，組織可以有一個替代（別名）URL供其品牌入口網站的現有URL使用。 別名URL可以通過在URL中具有備用前置詞來建立。\
請注意，只能自訂品牌入口網站URL的首碼，而不能自訂整個URL。 例如，現有網域為&#x200B;**[!UICONTROL geometrix.brand-portal.adobe.com]**&#x200B;的組織可取得依要求建立的&#x200B;**[!UICONTROL geomettrixinc.brand-portal.adobe.com]**。

不過，AEM Author例項可以[設定](../using/configure-aem-assets-with-brand-portal.md)，但只能使用租用戶ID URL，而不能使用租用戶別名（替代）URL。

>[!NOTE]
>
>若要在現有入口網站URL中取得租用戶名稱的別名，組織必須向Adobe支援部門提出新的租用戶別名建立要求。 首先檢查別名是否可用，然後建立別名，即可處理此請求。
>
>要替換舊別名或刪除舊別名，必須執行相同的進程。

## 要求存取品牌入口網站{#request-access-to-brand-portal}

使用者可從登入畫面要求存取品牌入口網站。 這些請求會傳送給品牌入口網站管理員，這些管理員會透過Adobe [!UICONTROL 管理控制台]授與使用者存取權。 在授予存取權後，使用者會收到通知電子郵件。

若要申請存取權，請執行下列動作：

1. 在品牌入口網站登入頁面中，選擇&#x200B;**[!UICONTROL 按一下此處]**&#x200B;對應於&#x200B;**[!UICONTROL 需要存取？]**. 但是，要進入來賓會話，請選擇&#x200B;**[!UICONTROL 按一下這裡]**&#x200B;與&#x200B;**[!UICONTROL 來賓訪問？]**&#x200B;對應。

   ![品牌入口網站登入畫面](assets/bp-login-requestaccess.png)

   將開啟[!UICONTROL 請求訪問]頁。

1. 若要申請存取組織的品牌入口網站，您必須擁有有效的[!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL Federated ID]。

   在[!UICONTROL 請求存取]頁面中，使用您的ID登入（藍本1）或建立[!UICONTROL Adobe ID]（藍本2）:<br />
   ![[!UICONTROL 請求存取]](assets/bplogin_request_access_2.png)

   **方案1**
   1. 如果您有[!UICONTROL Adobe ID]、[!UICONTROL Enterprise ID]或[!UICONTROL Federated ID]，請按一下「登入&#x200B;**[!UICONTROL 」。]**[!UICONTROL 登入]頁面隨即開啟。
   1. 提供您的[!UICONTROL Adobe ID]認證，然後按一下「登入&#x200B;**[!UICONTROL 」。<br />]**

   ![Adobe登入](assets/bplogin_request_access_3.png)

   您會被重新導向至「請求存取[!UICONTROL 」頁面。<br />]
   **方案2**
   1. 如果您沒有[!UICONTROL Adobe ID]，請按一下&#x200B;**[!UICONTROL 從[!UICONTROL 請求存取]頁面取得Adobe ID]**。
[!UICONTROL 登入]頁面隨即開啟。
   1. 按一下「取得Adobe ID ]**」。**[!UICONTROL [!UICONTROL 註冊]頁面隨即開啟。
   1. 輸入您的名字和姓氏、電子郵件ID和密碼。
   1. 選擇&#x200B;**[!UICONTROL 註冊]**。<br />

   ![](assets/bplogin_request_access_5.png)

   您會被重新導向至「請求存取[!UICONTROL 」頁面。]

1. 下一頁會顯示您的姓名和電子郵件ID，以要求存取權。 留下管理員的注釋，然後按一下&#x200B;**[!UICONTROL Submit]**。<br />

   ![](assets/bplogin-request-access.png)

## 產品管理員授予{#grant-access-to-brand-portal}存取權

品牌入口網站產品管理員會在其品牌入口網站通知區域，以及透過其收件匣中的電子郵件，收到存取要求。

![存取要求的通知](assets/bplogin_request_access_7.png)

若要授予存取權，產品管理員必須按一下品牌入口網站通知區中的相關通知，然後按一下&#x200B;**[!UICONTROL 授予存取權]**。
或者，產品管理員可依存取要求電子郵件中提供的連結，造訪Adobe [!UICONTROL 管理控制台]，並將使用者新增至相關的產品設定。

您會被重新導向至「Adobe [!UICONTROL 管理控制台]](https://adminconsole.adobe.com/enterprise/overview)」首頁。 [使用Adobe [!UICONTROL Admin Console]來建立使用者並指派給產品設定檔（先前稱為產品設定），這些設定檔在品牌入口網站中顯示為群組。 有關在[!UICONTROL 管理控制台]中添加用戶的詳細資訊，請參閱[添加用戶](brand-portal-adding-users.md#add-a-user)（按照添加用戶過程中的步驟4-7操作）。

## 品牌入口網站語言{#brand-portal-language}

您可以從Adobe [!UICONTROL Experience Cloud設定]變更品牌入口網站語言。

![存取要求的通知](assets/BPLang.png)

要更改語言，請執行以下操作：

1. 從頂部菜單中選擇[!UICONTROL User] > [!UICONTROL 編輯配置檔案]。<br />

   ![編輯設定檔](assets/EditBPProfile.png)

1. 在「[!UICONTROL Experience Cloud設定]」頁面上，從「[!UICONTROL 語言]」下拉式選單中選取語言。

## 品牌入口網站維護通知{#brand-portal-maintenance-notification}

在計畫關閉品牌入口網站以進行維護之前，當您登入品牌入口網站後，通知會顯示為橫幅。 範例通知：

![](assets/bp_maintenance_notification.png)

您可以關閉此通知並繼續使用品牌入口網站。 此通知會顯示在每個新作業中。

## 發行和系統資訊{#release-and-system-information}

* [新功能](whats-new.md)
* [發行說明](brand-portal-release-notes.md)
* [支援的檔案格式](brand-portal-supported-formats.md)

## 相關資源{#related-resources}

* [Adobe客戶服務](https://helpx.adobe.com/tw/marketing-cloud/contact-support.html)
* [AEM論壇](https://www.adobe.com/go/aod_forums_en)