---
title: 管理使用者、群組和使用者角色
seo-title: 管理使用者、群組和使用者角色
description: 管理員可以使用Adobe Admin Console來建立AEM Assets品牌入口網站使用者和產品設定檔，並使用品牌入口網站使用者介面來管理其角色。 檢視器和編輯者無法使用此權限。
seo-description: 管理員可以使用Adobe Admin Console來建立AEM Assets品牌入口網站使用者和產品設定檔，並使用品牌入口網站使用者介面來管理其角色。 檢視器和編輯者無法使用此權限。
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
role: 管理員
translation-type: tm+mt
source-git-commit: 263653916e4bc183827c197c3beb137c9e59ccb1
workflow-type: tm+mt
source-wordcount: '2210'
ht-degree: 0%

---


# 管理用戶、組和用戶角色{#manage-users-groups-and-user-roles}

管理員可以使用Adobe Admin Console來建立AEM Assets品牌入口網站使用者和產品設定檔，並使用品牌入口網站使用者介面來管理其角色。 檢視器和編輯者無法使用此權限。

在[[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)中，您可以檢視與您組織相關的所有產品。 產品可以是任何Experience Cloud解決方案，例如Adobe Analytics、Adobe Target或品AEM牌入口網站。 您必須選擇AEMBrand Portal產品，並建立產品設定檔。

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

這些產品設定檔會每8小時與品牌入口網站使用者介面同步，並顯示為品牌入口網站中的群組。 在您新增使用者並建立產品設定檔，以及將使用者新增至這些產品設定檔後，您就可以在Brand Portal中為使用者和群組指派角色。

>[!NOTE]
>
>若要在品牌入口網站中建立群組，請從Adobe[!UICONTROL Admin Console]，使用「產品>產品描述檔&#x200B;]**」，而非「**[!UICONTROL &#x200B;使用者頁面>使用者群組&#x200B;]**」。**[!UICONTROL  Adobe[!UICONTROL Admin Console]中的產品設定檔可用於在品牌入口網站中建立群組。

## 添加用戶{#add-a-user}

如果您是產品管理員，請使用Adobe[[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)來建立使用者，並將他們指派至產品設定檔（*先前稱為產品設定*），這些設定檔會在品牌入口網站中顯示為群組。 您可以使用群組來執行大量作業，例如角色管理和資產共用。

>[!NOTE]
>
>沒有品牌入口網站存取權的新使用者可以從品牌入口網站的登入畫面要求存取權。 如需詳細資訊，請參閱[要求存取品牌入口網站](../using/brand-portal.md#request-access-to-brand-portal)。 在通知區域收到訪問請求通知後，按一下相關通知，然後按一下&#x200B;**[!UICONTROL 授予訪問權]**。 或者，請依照收到的存取要求電子郵件中的連結進行。 接下來，要通過[Adobe[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)添加用戶，請遵循以下步驟中的步驟4-7。

>[!NOTE]
>
>您可以直接或從品牌入口網站登入[Adobe[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)。 如果您直接登入，請依照下列程式中的步驟4-7新增使用者。

1. 從頂AEM端的工具列，按一下Adobe標誌以存取管理工具。

   ![AEM logo](assets/aemlogo.png)

1. 從管理工具面板中，按一下&#x200B;**[!UICONTROL 用戶]**。

   ![管理工具面板](assets/admin-tools-panel-5.png)

1. 在[!UICONTROL 使用者角色]頁面中，按一下&#x200B;**[!UICONTROL 管理]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL 啟動Admin Console]**。

   ![要啟動的用戶角色Admin Console](assets/launch_admin_console.png)

1. 在Admin Console中，執行下列操作之一以建立新用戶：

   * 在頂部的工具欄上，按一下&#x200B;**[!UICONTROL 概述]**。 在[!UICONTROL 概述]頁面中，按一下品牌入口網站產品卡上的&#x200B;**[!UICONTROL 指派使用者]**。

   ![Admin Console概觀](assets/admin_console_overviewadduser.png)

   * 在頂部的工具欄中，按一下&#x200B;**[!UICONTROL 用戶]**。 在[!UICONTROL Users]頁面中，預設會選取左側導軌中的[!UICONTROL Users]。 按一下&#x200B;**[!UICONTROL 添加用戶]**。

   ![Admin Console新增使用者](assets/admin_console_adduseruserpage.png)

1. 在「新增使用者」對話方塊中，輸入您要新增之使用者的電子郵件ID，或從您輸入時顯示的建議清單中選取使用者。

   ![將使用者新增至品牌入口網站](assets/add_user_to_aem_bp.png)

1. 將使用者指派至少一個產品設定檔（先前稱為產品設定），讓使用者可以存取品牌入口網站。 從&#x200B;**[!UICONTROL Please select a profile for this product]**&#x200B;欄位中選擇適當的產品設定檔。
1. 按一下「**[!UICONTROL 儲存]**」。歡迎電子郵件會傳送給您新增的使用者。 受邀的使用者可以按一下歡迎電子郵件中的連結，並使用[!UICONTROL Adobe ID]登入，以存取品牌入口網站。 如需詳細資訊，請參閱[首次登入體驗](../using/brand-portal-onboarding.md)。

   >[!NOTE]
   >
   >如果使用者無法登入品牌入口網站，組織的管理員應造訪Adobe[!UICONTROL Admin Console]，並檢查使用者是否存在且已新增至至少一個產品描述檔。

   有關授予用戶管理權限的資訊，請參閱[為用戶提供管理員權限](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers)。

## 新增產品設定檔{#add-a-product-profile}

[!UICONTROL Admin Console]中的產品設定檔（先前稱為產品設定）用於在品牌入口網站中建立群組，以便您在品牌入口網站中執行大量作業，例如角色管理和資產共用。 **Brand** Portalis，預設產品設定檔；您可以建立更多產品設定檔，並將使用者新增至新的產品設定檔。

>[!NOTE]
>
>您可以直接或從品牌入口網站登入[[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)。 如果您直接登入[!UICONTROL Admin Console]，請依照下列步驟步驟4-7新增產品設定檔。

1. 從頂AEM端的工具列，按一下Adobe標誌以存取管理工具。

   ![標AEM志](assets/aemlogo.png)

1. 從管理工具面板中，按一下&#x200B;**[!UICONTROL 用戶]**。

   ![管理工具面板](assets/admin-tools-panel-6.png)

1. 在[!UICONTROL 使用者角色]頁面中，按一下&#x200B;**[!UICONTROL 管理]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL 啟動Admin Console]**。

   ![啟動Admin Console](assets/launch_admin_console.png)

1. 在頂部的工具欄上，按一下&#x200B;**[!UICONTROL 產品]**。
1. 在[!UICONTROL 產品]頁面中，預設會選取[!UICONTROL 產品描述檔]。 按一下「**[!UICONTROL 新建配置檔案]**」。

   ![新增產品設定檔](assets/admin_console_addproductprofile.png)

1. 在[!UICONTROL 建立新描述檔]頁面中，提供描述檔名稱、顯示名稱、描述檔說明，並選擇當使用者新增至描述檔或從描述檔移除時，您要透過電子郵件通知使用者。

   ![建立產品設定檔](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. 按一下&#x200B;**[!UICONTROL Done]**。 產品設定群組（例如&#x200B;**[!UICONTROL Sales group]**）會新增至品牌入口網站。

   ![產品設定檔](assets/admin_console_productprofileadded.png)

## 將用戶添加到產品配置檔案{#add-users-to-a-product-profile}

若要將使用者新增至品牌入口網站群組，請將使用者新增至[!UICONTROL Admin Console]中的對應產品設定檔（先前稱為產品設定）。 您可以個別或大量新增使用者。

>[!NOTE]
>
>您可以直接或從品牌入口網站登入[[!UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)。 如果您直接登入Admin Console，請依照下列程式中的步驟4-7，將使用者新增至產品設定檔。

1. 從頂AEM端的工具列，按一下Adobe標誌以存取管理工具。

   ![標AEM志](assets/aemlogo.png)

1. 從管理工具面板中，按一下&#x200B;**[!UICONTROL 用戶]**。

   ![管理工具面板](assets/admin-tools-panel-7.png)

1. 在[!UICONTROL 使用者角色]頁面中，按一下&#x200B;**[!UICONTROL 管理]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL 啟動Admin Console]**。

   ![啟動 [!DNL Admin Console]](assets/launch_admin_console.png)

1. 在頂部的工具欄上，按一下&#x200B;**[!UICONTROL 產品]**。
1. 在[!UICONTROL 產品]頁面中，預設會選取[!UICONTROL 產品描述檔]。 開啟您要新增使用者的產品設定檔，例如[!UICONTROL 銷售群組]。

   ![產品設定檔](assets/admin_console_productprofileadded.png)

1. 若要將個別使用者新增至產品設定檔，請執行下列動作：

   * 按一下&#x200B;**[!UICONTROL 添加用戶]**。

   ![群組以在品牌入口網站中對應產品描述檔](assets/admin_console_productprofilesalesgroup.png)

   * 在[!UICONTROL 新增使用者至銷售群組]頁面中，輸入您要新增之使用者的電子郵件ID，或從您鍵入時顯示的建議清單中選取使用者。

   ![新增使用者至群組](assets/admin_console_addusertosalesgroup.png)

   * 按一下「**[!UICONTROL 儲存]**」。



1. 若要將大量使用者新增至產品設定檔，請執行下列動作：

   * 選擇&#x200B;**[!UICONTROL 省略號(...)> 「依CSV新增使用者」。]**

   ![大量新增使用者](assets/admin_console_addbulkusers.png)

   * 在&#x200B;**[!UICONTROL 「依CSV新增使用者」頁面中，下載CSV範本或拖放CSV檔案。]**

   ![依csv新增使用者](assets/admin_console_addbulkuserscsv.png)

   * 按一下&#x200B;**[!UICONTROL Upload]**。
   如果您將使用者新增至預設的產品設定檔（即品牌入口網站），歡迎電子郵件會傳送至您新增使用者的電子郵件ID。 受邀的使用者可以按一下歡迎電子郵件中的連結，並使用[!UICONTROL Adobe ID]登入，以存取品牌入口網站。 如需詳細資訊，請參閱[首次登入體驗](../using/brand-portal-onboarding.md)。

   新增至自訂或新產品設定檔的使用者不會收到電子郵件通知。

## 為用戶{#provide-administrator-privileges-to-users}提供管理員權限

您可以為品牌入口網站使用者提供系統管理員或產品管理員權限。 請勿提供[!UICONTROL Admin Console]中提供的其他管理權限，如產品配置檔案管理員、用戶組管理員和支援管理員。 要瞭解有關這些角色的更多資訊，請參閱[管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html)。

>[!NOTE]
>
>您可以直接或從品牌入口網站登入[[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)。 如果您直接登入[!UICONTROL Admin Console]，請依照下列程式中的步驟4-8將使用者新增至產品設定檔。

1. 從頂AEM端的工具列，按一下Adobe標誌以存取管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 從管理工具面板中，按一下&#x200B;**[!UICONTROL 用戶]**。

   ![管理工具面板](assets/admin-tools-panel-8.png)

1. 在[!UICONTROL 使用者角色]頁面中，按一下&#x200B;**[!UICONTROL 管理]**&#x200B;標籤，然後按一下&#x200B;**[!UICONTROL 啟動Admin Console]**。

   ![啟動Admin Console](assets/launch_admin_console.png)

1. 在頂部的工具欄中，按一下&#x200B;**[!UICONTROL 用戶]**。
1. 在[!UICONTROL Users]頁面中，預設會選取左側導軌中的[!UICONTROL Users]。 按一下要向其提供管理員權限的用戶的用戶名。

   ![在Admin Console中添加用戶](assets/admin_console_adduseruserpage.png)

1. 在使用者設定檔頁面中，找到底部的&#x200B;**[!UICONTROL 管理權限]**&#x200B;區段，然後選擇&#x200B;**[!UICONTROL 省略號(...)>編輯管理權限]**。
   ![Admin Console中的管理權限](assets/admin_console_editadminrights.png)

1. 在[!UICONTROL 編輯管理員]頁面中，選擇系統管理員或產品管理員。

   ![在Admin Console中編輯管理員權限](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >品牌入口網站僅支援系統管理員和產品管理員角色。
   >
   >Adobe建議您避免使用系統管理員角色，因為它授予組織內所有產品的管理員權限。 例如，組織的系統管理員（包括3種Marketing Cloud產品）擁有這3種產品的完整權限集。 只有系統管理員可以設定AEM Assets，讓資產可以從AEM Assets發佈至品牌入口網站。 如需詳細資訊，請參閱[使用品牌入口網站設定AEM Assets。](../using/configure-aem-assets-with-brand-portal.md)
   >
   >相反地，「產品管理員」角色僅授予特定產品的管理員權限。 如果您想要在品牌入口網站中實施更精細的存取控制，請使用產品管理員角色並選取產品作為品牌入口網站。

   >[!NOTE]
   >
   >品牌入口網站不支援產品設定檔管理員（舊稱組態管理員）權限。 避免將產品描述檔管理員權限指派給使用者。

1. 查看管理類型選擇並按一下&#x200B;**[!UICONTROL 保存]**。

   >[!NOTE]
   >
   >要撤銷用戶的管理員權限，請在&#x200B;**[!UICONTROL 編輯管理員]**&#x200B;頁中進行相應的更改，然後按一下&#x200B;**[!UICONTROL 保存]**。


## 管理用戶角色{#manage-user-roles}

管理員可修改品牌入口網站中使用者的角色。

除了管理員角色外，品牌入口網站還支援下列角色：

* [!UICONTROL 檢視器]:具有此角色的用戶可以查看管理員與他們共用的檔案和資料夾。檢視器也可以搜尋及下載資產。 不過，檢視器無法與其他使用者共用內容（檔案、檔案夾、[!UICONTROL 系列]）。
* [!UICONTROL 編輯器]:具有此角色的使用者擁有檢視器的所有權限。此外，編輯人員可與其他使用者共用內容（資料夾、[!UICONTROL 系列]、連結）。

1. 從頂AEM端的工具列，按一下Adobe標誌以存取管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 從管理工具面板中，按一下&#x200B;**[!UICONTROL 用戶]**。

   ![管理工具面板](assets/admin-tools-panel-9.png)

1. 在[!UICONTROL 用戶角色]頁中，預設選擇[!UICONTROL 用戶]頁籤。 對於要更改角色的用戶，從&#x200B;**[!UICONTROL 角色]**&#x200B;下拉式清單中選擇&#x200B;**[!UICONTROL Editor]**&#x200B;或&#x200B;**[!UICONTROL Viewer]**。

   ![修改用戶角色](assets/modify_user_role.png)

   要同時修改多個用戶的角色，請選擇用戶並從&#x200B;**[!UICONTROL 角色]**&#x200B;下拉式清單中選擇相應的角色。

   >[!NOTE]
   >
   >管理員用戶的[!UICONTROL 角色]清單被禁用。 您無法選擇這些用戶來修改其角色。


   >[!NOTE]
   >
   >如果用戶是編輯器組的成員，則用戶角色也會被禁用。 若要撤銷使用者的編輯權限，請將使用者從「編輯器」群組中移除，或將整個群組的角色變更為「檢視器」。


1. 按一下「**[!UICONTROL 儲存]**」。將為相應用戶修改角色。 如果您選擇了多個用戶，則會同時修改所有用戶的角色。

   >[!NOTE]
   >
   >使用者權限的變更只有在使用者重新登入品牌入口網站後，才會反映在&#x200B;**[!UICONTROL 使用者角色]**&#x200B;頁面中。

## 管理組角色和權限{#manage-group-roles-and-privileges}

管理員可以將特定權限與品牌入口網站上的[group](../using/brand-portal-adding-users.md#main-pars-title-278567577)使用者建立關聯。 **[!UICONTROL 用戶角色]**&#x200B;頁上的&#x200B;**[!UICONTROL 組]**&#x200B;頁籤允許管理員：

* 將角色分配給用戶組
* 限制使用者群組從Brand Portal下載影像檔案(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-rgb、x-xbitmap、x-icon、image/photoshop、image/x-photoshop、.psd、image/vnd.adobe.photoshop)的原始轉譯本。

>[!NOTE]
>
>對於共用為連結的資產，會根據共用資產的使用者權限，套用存取影像檔案原始轉譯的權限。

要修改角色並有權訪問特定組成員的原始轉譯，請執行以下步驟：

1. 在&#x200B;**[!UICONTROL 用戶角色]**&#x200B;頁上，導航至&#x200B;**[!UICONTROL 組]**&#x200B;頁籤。
1. 選擇要更改角色的組。
1. 從&#x200B;**[!UICONTROL 角色]**&#x200B;下拉式清單中選擇適當的角色。

   允許群組成員存取影像檔案的原始轉譯(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-portable-pixmap、x-rgb、x-xbitmap、x-icon、image/photoshop、.pshop、image/vnd.adobe.poshop)從入口網站或共用連結下載，請保留該群組的&#x200B;**[!UICONTROL 存取原稿]**&#x200B;選項。 預設情況下，會為所有用戶選擇「訪問原稿」選項。 ****&#x200B;若要防止使用者群組存取原始轉譯，請取消選取該群組對應的選項。

   ![用戶組角色](assets/access-original-rend.png)

   >[!NOTE]
   >
   >如果將使用者新增至多個群組，且其中一個群組有限制，則限制將套用至該使用者。
   >
   >此外，管理員即使是受限制群組的成員，也無法存取影像檔案的原始轉譯的限制。


1. 按一下「**[!UICONTROL 儲存]**」。將修改相應組的角色。

   >[!NOTE]
   >
   >使用者對群組的關聯或使用者的群組成員資格，每8小時會同步至品牌入口網站。 對用戶或組角色的更改在下次同步作業運行後生效。

