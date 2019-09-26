---
title: AEM Assets品牌入口網站概觀
seo-title: AEM Assets品牌入口網站概觀
description: AEM Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部人士和內部企業使用者，並跨裝置發佈。
seo-description: AEM Assets Brand Portal可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部人士和內部企業使用者，並跨裝置發佈。
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: 引用
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: 簡介
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: f9397850937a5adb01ec41bc3b60afa712a4ddc3

---


# AEM Assets品牌入口網站概觀 {#overview-of-aem-assets-brand-portal}

身為行銷人員，您有時需要與通路合作夥伴和內部商業使用者共同作業，以快速建立、管理並傳遞相關的數位內容給客戶。 在整個客戶歷程中及時傳遞相關內容，對於推動更大的需求、轉化、參與度和客戶忠誠度至關重要。

但是，開發解決方案以支援與延伸內部團隊、合作夥伴和經銷商有效且安全地分享經核准的品牌標誌、准則、宣傳資產或產品像片，是一項挑戰。

**Adobe Experience Manager(AEM)Assets Brand Portal** ，可協助您輕鬆取得、控制並安全地將經過核准的創意資產發佈給外部廠商和跨裝置的內部商業使用者。 它有助於提高資產共用的效率，加快資產上市時間，並降低不合規和未授權存取的風險。

以瀏覽器為基礎的入口網站環境可讓您以核准的格式輕鬆上傳、瀏覽、搜尋、預覽和匯出資產。

## 品牌入口網站中的使用者角色 {#Personas}

品牌入口網站支援下列使用者角色：

* Guest user
* 檢視者
* 編輯者
* 管理員

下表列出了這些角色中的用戶可以執行的任務：

|  | **瀏覽** | **搜尋** | **下載** | **共用資料夾** | **共用系列** | **將資產共用為連結** | **存取管理工具** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Guest user** | ✓* | ✓* | ✓* | x | x | x | x |
| **檢視者** | ✓ | ✓ | ✓ | x | x | x | x |
| **編輯者** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **管理員** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

*訪客使用者只能瀏覽、存取和搜尋公用資料夾和系列中的資產。

### Guest user {#guest-user}

任何未經驗證而對品牌入口網站上資產有限存取的使用者皆為訪客使用者。 來賓會話允許用戶訪問公共資料夾和集合。 身為來賓用戶，您可以瀏覽資產詳細資訊，並擁有公共資料夾和系列成員的完整資產視圖。 您可以搜尋、下載公共資產並新增至 [!UICONTROL Lightbox] 集合。

However, guest session restricts you from creating collections and saved searches, and share them further. Users in a guest session cannot access folder and collections settings, and cannot share assets as link. 以下是來賓用戶可以執行的任務清單：

[Browse and access public assets](browse-assets-brand-portal.md)

[Search public assets](brand-portal-searching.md)

[Download public assets](brand-portal-download-users.md)

[Add assets to [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### 檢視者 {#viewer}

A standard user in Brand Portal is typically a user with the role of Viewer. A user with this role can access permitted folders, collections, and assets. The user can also browse, preview, download, and export assets (original or specific renditions), configure account settings, and search for assets. Here is a list of tasks that a Viewer can perform:

[Browse assets](browse-assets-brand-portal.md)

[Search for assets](brand-portal-searching.md)

[Download assets](brand-portal-download-users.md)

### 編輯者 {#editor}

A user with the role of Editor can perform all tasks that a Viewer can perform. In addition, and Editor can view the files and folders that an administrator shares. 具有編輯器角色的使用者也可以與其他人共用內容（檔案、檔案夾、系列）。

除了檢視器可執行的工作外，編輯器還可執行下列其他工作：

[共用資料夾](brand-portal-sharing-folders.md)

[Share a collection](brand-portal-share-collection.md)

[將資產共用為連結](brand-portal-link-share.md)

### 管理員 {#administrator}

管理員在 [!UICONTROL Admin Console中包含標示為系統管理員或品牌入口網站產品管理員的]使用者。 管理員可以新增和移除系統管理員和使用者、定義預設集、傳送電子郵件給使用者，以及檢視入口網站的使用情況和儲存報告。

管理員可以執行編輯器可以執行的所有任務，以執行以下附加任務：

[管理使用者、群組和使用者角色](brand-portal-adding-users.md)

[自訂壁紙、頁首和電子郵件](brand-portal-branding.md)

[使用自訂搜尋Facet](brand-portal-search-facets.md)

[使用中繼資料結構表單](brand-portal-metadata-schemas.md)

[套用影像預設集或動態轉譯](brand-portal-image-presets.md)

[使用報表](brand-portal-reports.md)

除了上述工作外，AEM Assets中的「作者」也可以執行下列工作：

[設定與品牌入口網站的AEM資產整合](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Publish folders to Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publish collections to Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## 品牌入口網站URL的替代別名 {#tenant-alias-for-portal-url}

品牌入口網站6.4.3版之後，組織可以有一個替代（別名）URL供其品牌入口網站的現有URL使用。 別名URL可以通過在URL中具有備用前置詞來建立。\
請注意，只能自訂品牌入口網站URL的首碼，而不能自訂整個URL。 例如，現有網域 **[!UICONTROL geometrix.brand-portal.adobe.com的組織可取得]** geomettrixinc.brand-portal.adobe.com **** 。

不過，AEM Author例項只能以租 [用戶ID](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) URL設定，而不能以租用戶別名（替代）URL設定。

>[!NOTE]
>
>若要在現有入口網站URL中取得租用戶名稱的別名，組織必須向Adobe支援部門提出新的租用戶別名建立要求。 首先檢查別名是否可用，然後建立別名，即可處理此請求。
>
>要替換舊別名或刪除舊別名，必須執行相同的進程。

## 要求存取品牌入口網站 {#request-access-to-brand-portal}

使用者可從登入畫面要求存取品牌入口網站。 這些請求會傳送至品牌入口網站管理員，這些管理員會透過Adobe [!UICONTROL Admin Console授與使用者存取權]。 在授予存取權後，使用者會收到通知電子郵件。

若要申請存取權，請執行下列動作：

1. From the Brand Portal login page, select Click here corresponding to Need Access?********. However, to enter the guest session, select the Click here corresponding to Guest Access?.********

   ![Brand Portal login screen](assets/bp-login-requestaccess.png)

   The Request Access page opens.

2. To request access to an organization’s Brand Portal, you must have a valid Adobe ID, Enterprise ID, or Federated ID.

   In the Request Access page, sign in using your ID (scenario 1) or create an Adobe ID (scenario 2):
   ![[!UICONTROL Request access]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. If you have an Adobe ID, Enterprise ID, or Federated ID, click Sign In.
**** The Sign in page opens.
   2. Provide your Adobe ID credentials and click Sign in.****<br />
   ![Adobe sign in](assets/bplogin_request_access_3.png)

   You are redirected to the Request Access page.
   **Scenario 2**
   1. If you do not have an Adobe ID, to create one, click Get an Adobe ID from the Request Access page.
****The Sign in page opens.
   2. Click **[!UICONTROL Get an Adobe ID]**.
「注 [!UICONTROL 冊] 」頁面隨即開啟。
   3. 輸入您的名字和姓氏、電子郵件ID和密碼。
   4. 選擇 **[!UICONTROL 註冊]**。<br />
   ![](assets/bplogin_request_access_5.png)

   您會被重新導向至「請 [!UICONTROL 求存取] 」頁面。

3. 下一頁會顯示您的姓名和電子郵件ID，以要求存取權。 保留管理員的注釋，然後按一下「提 **[!UICONTROL 交」]**。

   ![](assets/bplogin-request-access.png)

## 產品管理員授與存取權 {#grant-access-to-brand-portal}

品牌入口網站產品管理員會在其品牌入口網站通知區域，以及透過其收件匣中的電子郵件，收到存取要求。

![存取要求的通知](assets/bplogin_request_access_7.png)

若要授與存取權，產品管理員必須按一下品牌入口網站通知區中的相關通知，然後按一下「授 **[!UICONTROL 與存取權]**」。
或者，產品管理員可依存取要求電子郵件中提供的連結，造訪Adobe [!UICONTROL Admin Console] ，並將使用者新增至相關的產品設定。
![](assets/bplogin_request_access_8.png)

您會被重新導向 [至Adobe [!UICONTROL管理控制台]](https://adminconsole.adobe.com/enterprise/overview) 首頁。 使用Adobe [!UICONTROL Admin Console] ，建立使用者並將他們指派至產品設定檔（先前稱為產品設定），這些設定檔在品牌入口網站中顯示為群組。 如需有關在 [!UICONTROL Admin Console中新增使用者的詳細資訊]，請參閱 [](brand-portal-adding-users.md#add-a-user) 新增使用者（請依照新增使用者的程式中的步驟4-7）。

## 品牌入口網站語言 {#brand-portal-language}

您可以從「Adobe [!UICONTROL Experience Cloud設定」變更品牌入口]網站語言。

![存取要求的通知](assets/BPLang.png)

要更改語言，請執行以下操作：

1. 從頂 [!UICONTROL 部菜單中選] 擇「用戶  」&gt;「編輯配置檔案」。
   ![編輯設定檔](assets/EditBPProfile.png)

2. 在「 [!UICONTROL Experience cloud設定] 」頁面上，從「語言  」下拉式選單中選取語言。

## 品牌入口網站維護通知 {#brand-portal-maintenance-notification}

在計畫關閉品牌入口網站以進行維護之前，當您登入品牌入口網站後，通知會顯示為橫幅。 範例通知：

![](assets/bp_maintenance_notification.png)

您可以關閉此通知並繼續使用品牌入口網站。 此通知會顯示在每個新作業中。

## 發行和系統資訊 {#release-and-system-information}

<!--* [What's new](../using/whats-new.md)-->
* [發行說明](brand-portal-release-notes.md)
* [支援的檔案格式](brand-portal-supported-formats.md)

## 相關資源 {#related-resources}

* [Adobe客戶服務](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [AEM論壇](https://www.adobe.com/go/aod_forums_en)