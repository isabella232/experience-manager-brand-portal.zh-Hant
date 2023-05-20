---
title: 管理使用者、群組和使用者角色
seo-title: Manage users, groups, and user roles
description: 管理員可以使用Adobe Admin Console建立Brand Portal用戶和產品配置檔案，並使用Brand Portal用戶介面管理其角色。 此權限不可供查看者和編輯使用。
seo-description: Administrators can use Adobe Admin Console to create Brand Portal users and product profiles, and manage their roles using the Brand Portal user interface. This privilege is not available to Viewers and Editors.
uuid: 0dc1867c-6d1b-4d0d-a25e-0df207c269b8
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557e22b
role: Admin
exl-id: 35b1fd75-f9e4-4145-80bd-84de091f8b2b
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '2185'
ht-degree: 0%

---

# 管理使用者、群組和使用者角色 {#manage-users-groups-and-user-roles}

管理員可以使用 Adobe Admin Console 來建立 Experience Manager Assets 品牌入口網站使用者和產品設定檔，並使用管理品牌入口網站介面用戶其角色。 檢視器和編輯器不可使用此許可權。

在 Admin Console ] ](https://adminconsole.adobe.com/enterprise/overview) 中 [[!UICONTROL  ，您可以視圖與您的組織相關的所有產品。產品可以是任何 Experience Cloud 解決方案，例如 Adobe Analytics、Adobe Target 或 Experience Manager Assets 品牌入口網站。 您必須選擇 AEM 品牌入口網站產品，並建立產品設定檔。

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

這些產品設定檔會每8個小時與品牌入口網站用戶介面同步，並在品牌入口網站中顯示為群組。 添加用戶並建立產品配置檔案，以及將用戶添加到這些產品配置檔案後，您就可以將角色分配給Brand Portal的用戶和組。

>[!NOTE]
>
>若要從 Adobe Systems [!UICONTROL  Admin Console ] 品牌入口網站中建立群組，請使用 **[!UICONTROL 產品 > 產品設定檔]** ，而非 **[!UICONTROL 使用者頁面 > 使用者群組]** 。 Adobe Systems [!UICONTROL  Admin Console ] 中的產品設定檔用於在品牌入口網站中建立群組。

## 新增用戶 {#add-a-user}

如果您是產品管理員，請使用 Adobe Systems [[!UICONTROL  Admin Console ] ](https://adminconsole.adobe.com/enterprise/overview) 來建立使用者，並將其指派至產品設定檔（ *先前稱為產品* 設定），在品牌入口網站中顯示為群組。您可以使用群組執行大量操作，例如角色管理和資產共用。

>[!NOTE]
>
>新無法存取品牌入口網站的使用者，可請求品牌入口網站的登入畫面中的存取權。 有關詳細資訊，請參閱 [請求訪問Brand Portal](../using/brand-portal.md#request-access-to-brand-portal)。 在通知區域中接收訪問請求通知後，按一下相關通知，然後按一下 **[!UICONTROL 授予訪問權限]**。 或者，追隨接收的存取請求電子郵件中的連結。 接下來，通過 [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview)，請按照以下步驟4-7操作。

>[!NOTE]
>
>您可以登入 [ 直接或從品牌入口網站 Adobe Systems [!UICONTROL  Admin Console ] ](https://adminconsole.adobe.com/enterprise/overview) 。如果您直接登入，請追隨以下程式中的步驟4-7 以新增用戶。

1. 在頂部的 AEM 工具列中，按一下 Adobe Systems 標誌以存取管理工具。

   ![AEM 標誌](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 用戶]**。

   ![「管理工具」面板](assets/admin-tools-panel-5.png)

1. 在 [!UICONTROL 用戶角色] 的 **[!UICONTROL 管理]** ，然後按一下 **[!UICONTROL 啟動Admin Console]**。

   ![要啟動的用戶角色Admin Console](assets/launch_admin_console.png)

1. 在Admin Console中，執行下列操作之一以建立新用戶：

   * 在頂部的工具欄中，按一下 **[!UICONTROL 概述]**。 在 [!UICONTROL 概述] 的 **[!UICONTROL 分配用戶]** 從Brand Portal產品卡上。

   ![Admin Console概述](assets/admin_console_overviewadduser.png)

   * 在頂部的工具欄中，按一下 **[!UICONTROL 用戶]**。 在 [!UICONTROL 用戶] 頁面， [!UICONTROL 用戶] 的下界。 按一下 **[!UICONTROL 添加用戶]**。

   ![Admin Console添加用戶](assets/admin_console_adduseruserpage.png)

1. 在「增加用戶」對話方塊中，輸入您要新增的用戶的電子郵件 ID，或從您鍵入的建議清單中選擇用戶。

   ![將用戶新增至品牌入口網站](assets/add_user_to_aem_bp.png)

1. 將用戶分配到至少一個產品配置檔案（以前稱為產品配置），以便用戶可以訪問Brand Portal。 從 **[!UICONTROL 請為此產品選擇配置檔案]** 的子菜單。
1. 按一下「**[!UICONTROL 儲存]**」。向新添加的用戶發送歡迎電子郵件。 受邀用戶可以按一下歡迎電子郵件中的連結訪問Brand Portal。 用戶可以使用電子郵件ID登錄([!UICONTROL Adobe ID]。 [!UICONTROL Enterprise ID]或 [!UICONTROL 虛擬ID])在Admin Console中配置。 有關詳細資訊，請參見 [首次登錄體驗](../using/brand-portal-onboarding.md)。

   >[!NOTE]
   >
   >如果用戶無法登錄到Brand Portal，則組織管理員應訪問Adobe [!UICONTROL Admin Console] 並檢查用戶是否存在以及是否已添加到至少一個產品配置檔案中。

   有關向用戶授予管理權限的資訊，請參見 [為用戶提供管理員權限](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers)。

## 添加產品配置檔案 {#add-a-product-profile}

中的產品配置檔案（以前稱為產品配置） [!UICONTROL Admin Console] 用於在Brand Portal建立組，以便您可以在Brand Portal執行批量操作，如角色管理和資產共用。 **Brand Portal** 是可用的預設產品配置檔案；您可以建立更多產品配置檔案並將用戶添加到新產品配置檔案中。

>[!NOTE]
>
>您可以登錄到 [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 或直接從Brand Portal。 如果登錄到 [!UICONTROL Admin Console] 請直接按照以下步驟中的步驟4-7添加產品配置檔案。

1. 在頂部AEM的工具欄中，按一下Adobe徽標以訪問管理工具。

   ![標AEM志](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 用戶]**。

   ![「管理工具」面板](assets/admin-tools-panel-6.png)

1. 在頁面的使用者角色 ] 中，按一下 **[!UICONTROL 管理]** 標籤，然後按一下 **[!UICONTROL Launch Admin Console]** 。 [!UICONTROL 

   ![Launch Admin Console](assets/launch_admin_console.png)

1. 在頂部的工具欄中，按一下 **[!UICONTROL 產品]**。
1. 在 [!UICONTROL 產品] 頁面， [!UICONTROL 產品配置檔案] 的下界。 按一下 **[!UICONTROL 新建配置檔案]**。

   ![添加新產品配置檔案](assets/admin_console_addproductprofile.png)

1. 在 [!UICONTROL 建立新配置檔案] 頁中，提供配置檔案名稱、顯示名稱、配置檔案說明，並選擇是否要在將用戶添加到配置檔案或從配置檔案中刪除時通過電子郵件通知用戶。

   ![建立產品配置檔案](assets/admin_console_addaproductprofilecreatenewprofile.png)

1. 按一下 **[!UICONTROL 完成]**。 例如，產品配置組 **[!UICONTROL 銷售組]**&#x200B;的子菜單。

   ![產品設定檔](assets/admin_console_productprofileadded.png)

## 將用戶添加到產品配置檔案 {#add-users-to-a-product-profile}

要將用戶添加到Brand Portal組，請將其添加到中的相應產品配置檔案（以前稱為產品配置） [!UICONTROL Admin Console]。 您可以單獨或批量添加用戶。

>[!NOTE]
>
>您可以登錄到 [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 或直接從Brand Portal。 如果直接登錄到Admin Console，請按照下面步驟中的步驟4-7將用戶添加到產品配置檔案中。

1. 在頂部的工具欄中，按一下Experience Manager徽標以訪問管理工具。

   ![標AEM志](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 用戶]**。

   ![管理工具面板](assets/admin-tools-panel-7.png)

1. 在頁面的使用者角色 ] 中，按一下 **[!UICONTROL 管理]** 標籤，然後按一下 **[!UICONTROL Launch Admin Console]** 。 [!UICONTROL 

   ![啟動 [!DNL Admin Console]](assets/launch_admin_console.png)

1. 從頂部的工具列中按一下 **[!UICONTROL 產品]** 。
1. [!UICONTROL 在產品 ] 頁面中， [!UICONTROL  預設會選取產品設定檔 ] 。開啟要新增用戶的產品設定檔，例如 [!UICONTROL  「銷售群組 ] 」。

   ![產品設定檔](assets/admin_console_productprofileadded.png)

1. 若要將個別使用者新增至產品設定檔，請執行下列操作：

   * 按一下 **[!UICONTROL 「新增使用者]** 」。

   ![要在品牌入口網站中映射產品設定檔的群組](assets/admin_console_productprofilesalesgroup.png)

   * [!UICONTROL 在「將使用者新增至銷售群組 ] 頁面中，鍵入您要新增的用戶的電子郵件 ID，或從顯示的建議清單中選擇用戶。

   ![將用戶添加到組](assets/admin_console_addusertosalesgroup.png)

   * 按一下「**[!UICONTROL 儲存]**」。



1. 若要將大量使用者新增至產品設定檔，請執行下列操作：

   * 選擇 **[!UICONTROL 省略號（...） > 依 CSV]** 新增使用者。

   ![大量新增使用者](assets/admin_console_addbulkusers.png)

   * **[!UICONTROL 在「新增使用者依據 CSV]** 頁面中，下載 CSV 範本或拖放 CSV 檔案。

   ![按csv添加用戶](assets/admin_console_addbulkuserscsv.png)

   * 按一下 **[!UICONTROL 上載]**。
   如果將用戶添加到預設產品配置檔案，即Brand Portal，則歡迎電子郵件將發送到您添加的用戶的電子郵件ID。 邀請的用戶可以通過按一下歡迎電子郵件中的連結並使用 [!UICONTROL Adobe ID]。 有關詳細資訊，請參見 [首次登錄體驗](../using/brand-portal-onboarding.md)。

   添加到自定義或新產品配置檔案的用戶不會收到電子郵件通知。

## 為用戶提供管理員權限 {#provide-administrator-privileges-to-users}

您可以向Brand Portal用戶提供系統管理員或產品管理員權限。 不提供中提供的其他管理權限 [!UICONTROL Admin Console]，如產品配置檔案管理員、用戶組管理員和支援管理員。 要瞭解這些角色的詳細資訊，請參閱 [管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html)。

>[!NOTE]
>
>您可以登錄到 [[!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 或直接從Brand Portal。 如果登錄到 [!UICONTROL Admin Console] 請直接按照以下步驟中的步驟4-8將用戶添加到產品配置檔案。

1. 在頂部AEM的工具欄中，按一下Adobe徽標以訪問管理工具。

   ![AEMLogo](assets/aemlogo.png)

1. 在「管理工具」面板中，按一下 **[!UICONTROL 使用者]** 。

   ![管理工具面板](assets/admin-tools-panel-8.png)

1. 在頁面的使用者角色 ] 中，按一下 **[!UICONTROL 管理]** 標籤，然後按一下 **[!UICONTROL Launch Admin Console]** 。 [!UICONTROL 

   ![Launch Admin Console](assets/launch_admin_console.png)

1. 從頂部的工具列中按一下 **[!UICONTROL 使用者]** 。
1. 在 [!UICONTROL 用戶] 頁面， [!UICONTROL 用戶] 的下界。 按一下要向其提供管理員權限的用戶的用戶名。

   ![在Admin Console中添加用戶](assets/admin_console_adduseruserpage.png)

1. 在用戶配置檔案頁中，找到 **[!UICONTROL 管理權]** 的 **[!UICONTROL 省略號(...)>編輯管理員權限]**。
   ![Admin Console中的管理權限](assets/admin_console_editadminrights.png)

1. 在 [!UICONTROL 編輯管理員] 頁面，選擇「系統管理員」或「產品管理員」。

   ![編輯Admin Console中的管理員權限](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   >
   >Brand Portal僅支援系統管理員和產品管理員角色。
   >
   >Adobe建議您避免使用「系統管理員」角色，因為它授予組織範圍內所有組織產品的管理員權限。 例如，包含三個營銷雲產品的組織的系統管理員對所有三個產品都擁有全部權限集。 只有系統管理員才能配置Experience Manager Assets，以便從Experience Manager Assets到Brand Portal發佈資產。 有關詳細資訊，請參見 [將Experience Manager Assets配置為Brand Portal](../using/configure-aem-assets-with-brand-portal.md)。
   >
   >相反，「產品管理員」角色僅授予特定產品的管理員權限。 若要在品牌入口網站中實施更詳細的存取控制，請使用產品管理員角色，然後選取「產品」做為「品牌入口網站」。

   >[!NOTE]
   >
   >品牌入口網站不支援產品設定檔管理員（先前稱為設定管理員）許可權。 避免將產品設定檔管理員權利指派給用戶。

1. 查看管理類型選擇，然後按一下 **[!UICONTROL 保存]**。

   >[!NOTE]
   >
   >要撤消用戶的管理員權限，請在 **[!UICONTROL 編輯管理員]** ，然後按一下 **[!UICONTROL 保存]**。


## 管理用戶角色 {#manage-user-roles}

管理員可以修改Brand Portal用戶的角色。

除管理員角色外，Brand Portal還支援以下角色：

* [!UICONTROL 查看器]:具有此角色的用戶可以查看管理員與他們共用的檔案和資料夾。 查看者還可以搜索和下載資產。 但是，查看器無法共用內容(檔案、資料夾、 [!UICONTROL 集合])。
* [!UICONTROL 編輯器]:具有此角色的用戶具有查看器的所有權限。 此外，編輯員可以共用內容(資料夾、 [!UICONTROL 集合]，連結)。

1. 在頂部AEM的工具欄中，按一下Adobe徽標以訪問管理工具。

   ![阿莫爾奧戈](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 用戶]**。

   ![「管理工具」面板](assets/admin-tools-panel-9.png)

1. 在 [!UICONTROL 用戶角色] 頁 [!UICONTROL 用戶] 頁籤 對於要更改其角色的用戶，請選擇 **[!UICONTROL 編輯器]** 或 **[!UICONTROL 查看器]** 從 **[!UICONTROL 角色]** 下拉。

   ![修改使用者角色](assets/modify_user_role.png)

   若要同時修改多個使用者的角色，請選取使用者並從角色 ]**下拉式清單中**[!UICONTROL  選擇適當的角色。

   >[!NOTE]
   >
   >管理員使用者的 [!UICONTROL  角色 ] 清單已停用。 您無法選取這些使用者來修改其角色。


   >[!NOTE]
   >
   >如果用戶是編輯器群組的成員，也會停用用戶角色。 若要撤銷用戶的編輯許可權，請從編輯器中移除用戶群組或將整個群組的角色變更為檢視器。


1. 按一下「**[!UICONTROL 儲存]**」。為相應用戶修改角色。 如果選擇了多個用戶，則同時修改所有用戶的角色。

   >[!NOTE]
   >
   >只有在使用者重新登入至品牌入口網站後， **[!UICONTROL 才會在使用者頁面角色]** 中反映用戶許可權的變更。

## 管理群組角色與許可權 {#manage-group-roles-and-privileges}

管理員可以將特定許可權與 [ 品牌入口網站上的使用者群組 ](../using/brand-portal-adding-users.md#main-pars-title-278567577) 關聯。 使用者角色 ]**上**[!UICONTROL  標籤的 **[!UICONTROL 群組]** 頁面允許管理員：

* 將角色指派給用戶群組
* 限制用戶組從Brand Portal下載影像檔案(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-rgb、x-xbitmap、x-icon、image/photoshop、.psd、image/vnd.adobe.photoshop)的原始格式副本。

>[!NOTE]
>
>對於作為連結共用的資產，訪問影像檔案原始格式副本的權限將根據共用資產的用戶的權限應用。

若要修改角色和許可權以存取特定群組成員的原始轉譯，請追隨以下步驟：

1. 在頁面的 **[!UICONTROL 使用者角色]** 上，導覽至 **[!UICONTROL 群組]** 標籤。
1. 選取您要變更角色的群組。
1. 從 **[!UICONTROL 角色]** 的子菜單。

   允許組成員訪問影像檔案的原始格式副本(.jpeg、.tiff、.png、.bmp、.gif、.pjpeg、x-portable-anymap、x-portable-bitmap、x-portable-graymap、x-rgb、x-xbitmap、x-icon、image/photoshop、.psd、image/vnd.adobe.p)從入口或共用連結下載的，保留 **[!UICONTROL 訪問原始]** 的子菜單。 預設情況下， **[!UICONTROL 為所有使用者選取「存取原始]** 」選項。 若要防止消費者群組存取原始轉譯，請取消選取對應于該群組的選項。

   ![使用者群組角色](assets/access-original-rend.png)

   >[!NOTE]
   >
   >如果將用戶新增至多個群組，且其中一個群組有限制，則限制會套用至該用戶。
   >
   >此外，存取影像檔案原始轉譯的限制不適用於管理員平均，儘管他們是受限制群組的成員。


1. 按一下「**[!UICONTROL 儲存]**」。針對對應群組修改角色。

   >[!NOTE]
   >
   >用戶-群組關聯或用戶的群組成員資格同步至每8小時品牌入口網站。 用戶或群組角色的變更會在下一個同步工作執行後生效。
