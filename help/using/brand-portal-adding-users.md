---
title: 管理使用者、群組和使用者角色
seo-title: 管理使用者、群組和使用者角色
description: 管理員可以使用Adobe Admin Console來建立AEM Assets Brand Portal使用者和產品描述檔，並使用品牌入口網站使用者介面管理其角色。檢視器和編輯器無法使用此權限。
seo-description: 管理員可以使用Adobe Admin Console來建立AEM Assets Brand Portal使用者和產品描述檔，並使用品牌入口網站使用者介面管理其角色。檢視器和編輯器無法使用此權限。
uuid: 0dc1867c-6d1b-4d0d-a25 e-0df207 c269 b8
content-type: 引用
topic-tags: 管理
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: ba468e80-d077-4af6-b782-238fc557 e22 b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 管理使用者、群組和使用者角色 {#manage-users-groups-and-user-roles}

管理員可以使用Adobe Admin Console來建立AEM Assets Brand Portal使用者和產品描述檔，並使用品牌入口網站使用者介面管理其角色。檢視器和編輯器無法使用此權限。

In [[！UICOHTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)，您可以檢視所有與您組織相關聯的產品。產品可能是任何Experience Cloud解決方案，例如Adobe Analytics、Adobe Target或AEM品牌入口網站。您必須選擇AEM品牌入口網站產品，並建立產品描述檔。

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

這些產品設定檔每小時都會與品牌入口網站使用者介面同步，並顯示為品牌入口網站中的群組。新增使用者並建立產品描述檔，並新增使用者至這些產品設定檔後，您可以在品牌入口網站中指派角色給使用者和群組。

>[!NOTE]
>
>若要在品牌入口網站中建立群組，請 [!UICONTROL 使用]**[!UICONTROL 「產品&gt;產品描述檔]**」，而非 **[!UICONTROL 「使用者」頁面&gt;「使用者群組]**」。Adobe [!UICONTROL Admin Console] 中的產品描述檔可用來建立品牌入口網站中的群組。

## 新增使用者 {#add-a-user}

如果您是產品管理員，請使用Adobe [[！UICOHTROL Admin Console可](http://adminconsole.adobe.com/enterprise/overview) 建立使用者並指派給產品描述檔(*先前稱為產品設定*)，在品牌入口網站中顯示為群組。您可以使用群組執行大量作業，例如角色管理和資產共用。

>[!NOTE]
無權存取品牌入口網站的新使用者可以從品牌入口網站的登入畫面要求存取權。如需詳細資訊，請參閱 [「品牌入口網站」的「請求存取](../using/brand-portal.md#request-access-to-brand-portal)權」。在通知區域收到存取要求通知後，按一下相關通知，然後按一下 **[!UICONTROL 「授予存取權]**」。或者，請依照收到的存取要求電子郵件中的連結進行。接著，透過 [Adobe[！UICOHTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview)，請依照以下程序的步驟進行4-7。

>[!NOTE]
您可以登入 [Adobe[！UICOHTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) 直接或從品牌入口網站取得。如果您直接登入，請依照下列程序中的步驟來新增使用者。

1. 從上方的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![AEM logo](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 「使用者]**」。

   ![管理工具面板](assets/admin-tools-panel-5.png)

3. 在 [!UICONTROL 「使用者角色] 」頁面中，按一下「 **[!UICONTROL 管理]** 」標籤，然後按一下 **[!UICONTROL 「啓動管理控制台]**」。

   ![啓動Admin Console的使用者角色](assets/launch_admin_console.png)

4. 在管理控制台中，執行下列其中一項建立新使用者：

   * 從上方的工具列，按一下 **[!UICONTROL 「概述]**」。在 [!UICONTROL 「概述] 」頁面中，按一下 **[!UICONTROL 品牌入口網站產品卡中的指派使用者]** 。
   ![管理控制台概述](assets/admin_console_overviewadduser.png)

   * 從上方的工具列，按一下 **[!UICONTROL 「使用者]**」。在 [!UICONTROL 「使用者] 」頁面中，預設會選取左側導軌中的 [!UICONTROL 使用者] 。按一下 **[!UICONTROL 「新增使用者]**」。
   ![管理控制台新增使用者](assets/admin_console_adduseruserpage.png)

5. 在新增使用者對話方塊中，輸入使用者的電子郵件ID，您可以從顯示時出現的建議清單中新增或選取使用者。

   ![新增使用者至品牌入口網站](assets/add_user_to_aem_bp.png)

6. 將使用者指派至少一個產品描述檔(先前稱為產品設定)，讓使用者可以存取品牌入口網站。從 **[!UICONTROL 「請為此產品]** 欄位選取描述檔」中選擇適當的產品設定檔。
7. Click **[!UICONTROL Save]**. 歡迎電子郵件會傳送給您新增的使用者。受邀的使用者可以按一下歡迎電子郵件中的連結，並使用 [!UICONTROL Adobe ID登入，以存取品牌入口網站]。如需詳細資訊，請參閱 [首次登入體驗](../using/brand-portal-onboarding.md)。

   >[!NOTE]
   如果使用者無法登入品牌入口網站，組織的管理員應造訪Adobe [!UICONTROL Admin Console] 並檢查使用者是否存在並已新增至至少一個產品描述檔。

   如需有關授予使用者管理權限的詳細資訊，請參閱 [為使用者提供管理員權限](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers)。

## 新增產品描述檔 {#add-a-product-profile}

[!UICONTROL 「管理控制台」中的產品描述檔(先前稱為產品設定)] 可用來在品牌入口網站中建立群組，以便您能夠在品牌入口網站中執行大量作業，例如角色管理和資產共用。**品牌入口網站** 是可用的預設產品設定檔；您可以建立更多的產品設定檔，並新增使用者至新的產品設定檔。

>[!NOTE]
您可以登入 [[！UICOHTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) 直接或從品牌入口網站取得。如果您直接登入 [!UICONTROL Admin Console] ，請依照下列程序中的步驟來新增產品描述檔。

1. 從上方的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![AEM標誌](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 「使用者]**」。

   ![管理工具面板](assets/admin-tools-panel-6.png)

3. 在 [!UICONTROL 「使用者角色] 」頁面中，按一下「 **[!UICONTROL 管理]** 」標籤，然後按一下 **[!UICONTROL 「啓動管理控制台]**」。

   ![啓動Admin Console](assets/launch_admin_console.png)

4. 從上方的工具列，按一下 **[!UICONTROL 「產品]**」。
5. 在 [!UICONTROL 「產品」] 頁面中，預設會選取 [!UICONTROL 「產品描述檔] 」。按一下 **[!UICONTROL 「新增描述檔]**」。

   ![新增產品描述檔](assets/admin_console_addproductprofile.png)

6. 在 [!UICONTROL 「建立新描述檔] 」頁面中，提供描述檔名稱、顯示名稱、描述檔描述，並選擇是否要透過電子郵件將使用者新增至或從描述檔中移除。

   ![建立產品描述檔](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. 按一下 **[!UICONTROL 完成]**。產品設定群組(例如 **[!UICONTROL 銷售群組]**)會新增至品牌入口網站。

   ![產品設定檔](assets/admin_console_productprofileadded.png)

## 新增使用者至產品描述檔 {#add-users-to-a-product-profile}

若要新增使用者至品牌入口網站群組，請在 [!UICONTROL 「管理控制台]」中新增至對應的產品設定檔(先前稱為產品設定)。您可以個別或大量新增使用者。

>[!NOTE]
您可以登入 [[！UICOHTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) 直接或從品牌入口網站取得。如果您直接登入Admin Console，請依照下列程序中的步驟來新增使用者至產品描述檔。

1. 從上方的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![AEM標誌](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 「使用者]**」。

   ![管理工具面板](assets/admin-tools-panel-7.png)

3. 在 [!UICONTROL 「使用者角色] 」頁面中，按一下「 **[!UICONTROL 管理]** 」標籤，然後按一下 **[!UICONTROL 「啓動管理控制台]**」。

   ![Launch [!DNL Admin Console]](assets/launch_admin_console.png)

4. 從上方的工具列，按一下 **[!UICONTROL 「產品]**」。
5. 在 [!UICONTROL 「產品」] 頁面中，預設會選取 [!UICONTROL 「產品描述檔] 」。開啓您要新增使用者的產品設定檔，例如 [!UICONTROL 銷售群組]。

   ![產品設定檔](assets/admin_console_productprofileadded.png)

6. 若要新增個別使用者至產品描述檔，請執行下列動作：

   * 按一下 **[!UICONTROL 「新增使用者]**」。
   ![在品牌入口網站中映射產品描述檔的群組](assets/admin_console_productprofilesalesgroup.png)

   * 在 [!UICONTROL 「新增使用者至銷售」群組] 頁面中，輸入您要在輸入時出現的建議清單中新增或選取使用者的電子郵件ID。
   ![新增使用者至群組](assets/admin_console_addusertosalesgroup.png)

   * Click **[!UICONTROL Save]**.



7. 若要新增大量使用者至產品描述檔，請執行下列動作：

   * 選擇橢圓形(...)**[!UICONTROL &gt;使用CSV新增使用者]**。
   ![大量新增使用者](assets/admin_console_addbulkusers.png)

   * 在「依CSV **[!UICONTROL 新增使用者」]** 頁面中，下載CSV範本或拖放CSV檔案。
   ![透過csv新增使用者](assets/admin_console_addbulkuserscsv.png)

   * 按一下 **[!UICONTROL 「上傳]**」。
   如果您新增使用者至預設產品描述檔，則會將歡迎電子郵件傳送給您新增的使用者的電子郵件ID。受邀的使用者可以按一下歡迎電子郵件中的連結，並使用 [!UICONTROL Adobe ID登入，以存取品牌入口網站]。如需詳細資訊，請參閱 [首次登入體驗](../using/brand-portal-onboarding.md)。

   新增至自訂或新產品描述檔的使用者不會收到電子郵件通知。

## 為使用者提供管理員權限 {#provide-administrator-privileges-to-users}

您可以為品牌入口網站使用者提供系統管理員或產品管理員權限。請勿提供 [!UICONTROL Admin Console中可用的其他管理權限]，例如產品設定檔管理員、使用者群組管理員以及支援管理員。若要深入瞭解這些角色，請參閱 [管理角色](https://helpx.adobe.com/enterprise/using/admin-roles.html)。

>[!NOTE]
您可以登入 [[！UICOHTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) 直接或從品牌入口網站取得。如果您直接登入 [!UICONTROL Admin Console] ，請依照下列程序中的步驟來新增使用者至產品描述檔。

1. 從上方的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![AEMlogo](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 「使用者]**」。

   ![管理工具面板](assets/admin-tools-panel-8.png)

3. 在 [!UICONTROL 「使用者角色] 」頁面中，按一下「 **[!UICONTROL 管理]** 」標籤，然後按一下 **[!UICONTROL 「啓動管理控制台]**」。

   ![啓動Admin Console](assets/launch_admin_console.png)

4. 從上方的工具列，按一下 **[!UICONTROL 「使用者]**」。
5. 在 [!UICONTROL 「使用者] 」頁面中，預設會選取左側導軌中的 [!UICONTROL 使用者] 。按一下您要提供管理員權限之使用者的使用者名稱。

   ![在Admin Console中新增使用者](assets/admin_console_adduseruserpage.png)

6. 在使用者描述檔頁面中，找出底部的 **[!UICONTROL 「管理權限]** 」區段，並選擇「橢圓」(**[!UICONTROL …&gt;編輯管理權限]**。
   ![管理控制台中的管理員權限](assets/admin_console_editadminrights.png)

7. 在 [!UICONTROL 「編輯管理] 」頁面中，選取系統管理員或產品管理員。

   ![在管理控制台中編輯管理權限](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   品牌入口網站僅支援系統管理員和產品管理員角色。
   Adobe建議您避免使用系統管理員角色，因為它授予組織所有產品的全組織管理員權限。例如，組織的系統管理員包含三個Marketing Cloud產品的完整權限集，這三個產品都有一組權限。只有系統管理員可以設定AEM Assets，以便將資產從AEM Assets發佈至品牌入口網站。如需詳細資訊，請參閱 [「設定AEM資產與品牌入口網站](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)的整合」。
   相反地，產品管理員角色僅授予特定產品的管理員權限。如果您想要在Brand Portal內執行更精細的存取控制，請使用產品管理員角色，然後選取產品作為品牌入口網站。

   >[!NOTE]
   品牌入口網站不支援產品設定檔管理員(先前稱為設定管理員)權限。避免指派產品描述檔管理員權限給使用者。

8. 檢閱管理類型選擇，然後按一下 **[!UICONTROL 「儲存]**」。

   >[!NOTE]
   若要撤銷使用者的管理員權限，請在 [!UICONTROL 「編輯管理] 」頁面中進行適當的變更，然後按一下 **[!UICONTROL 「儲存]**」。

## 管理使用者角色 {#manage-user-roles}

管理員可以修改品牌入口網站中使用者的角色。

除了管理員角色外，品牌入口網站還支援下列角色：

* [!UICONTROL 檢視器]：具有此角色的使用者可以檢視管理員與他們分享的檔案和資料夾。檢視者也可以搜尋和下載資產。不過，觀眾無法與其他使用者共用內容(檔案、資料夾、 [!UICONTROL 系列])。
* [!UICONTROL 編輯器]：具有此角色的使用者擁有檢視器的所有權限。此外，編輯器可與其他使用者共用內容(資料夾、 [!UICONTROL 系列]、連結)。

1. 從上方的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![AEMlogo](assets/aemlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 「使用者]**」。

   ![管理工具面板](assets/admin-tools-panel-9.png)

3. 在 [!UICONTROL 「使用者角色] 」頁面中，預設會選取 [!UICONTROL 「使用者] 」索引標籤。對於想要變更角色的使用者，請從「角色」下拉式清單中選取 **[!UICONTROL 「編輯者]** 」或 **[!UICONTROL 「檢視器]****** 」。

   ![修改使用者角色](assets/modify_user_role.png)

   若要同時修改多位使用者的角色，請選取使用者並從 **[!UICONTROL 角色]** 下拉式清單中選擇適當角色。

   >[!NOTE]
   管理員使用者的 [!UICONTROL 角色] 清單已停用。您無法選取這些使用者來修改其角色。

   >[!NOTE]
   如果使用者是Editor群組的成員，也會停用使用者角色。若要撤銷使用者的編輯權限，請從「編輯器」群組移除使用者，或將整個群組的角色變更為「檢視器」。

4. Click **[!UICONTROL Save]**. 已針對對應的使用者修改角色。如果您選取多個使用者，則會同時修改所有使用者的角色。

   >[!NOTE]
   只有在使用者重新登入品牌入口網站後，使用者權限的變更才會反映在 [!UICONTROL 使用者角色] 頁面中。

## 管理群組角色和權限 {#manage-group-roles-and-privileges}

管理員可以將特定權限與品牌入口網站上的一組 [](../using/brand-portal-adding-users.md#main-pars-title-278567577) 使用者建立關聯。「使用者角色」頁面上的「 [!UICONTROL 群組] 」標籤可讓管理員：

* 指派角色給使用者群組
* 限制使用者群組下載影像檔案的原始轉譯(.jpeg、. tiff、. png、. bmp、. gif、. pjpg、x-able-any map、x-portable-bitmap、x-portable-any map、x-domable-pitmap、x-domable-pitmap、x-clip-premap、x-publish-pimap、x-publishine、x-clip、image/photoshop、image/x-photoshop/vnd. adobe. photoshop) from Brand Portal。

>[!NOTE]
對於共用為連結的資產，會根據共用資產的使用者權限，套用存取影像檔案原始轉譯的權限。

若要修改角色並有權存取特定群組成員的原始轉譯，請遵循下列步驟：

1. 在 [!UICONTROL 「使用者角色] 」頁面上，導覽至 **[!UICONTROL 「群組]** 」標籤。
2. 選取您要變更角色的群組。
3. 從 [!UICONTROL 「角色」] 下拉式清單中選擇適當的角色。

   若要允許群組成員存取原始影像檔案(.jpeg、. tiff、. png、. bmp、. gif、. pjpeg、x-able-any map、x-portable-bitmap、x-portable-any map、x-domable-any map、x-domable-pitmap、x-browsing-graymap、x-clip、image/photoshop、image/x-photoshop shop、. psd、 [!UICONTROL image/vnd. adobe. photoshop從入口網站或共用連結下載，會保留該群組中選取的「存取原始」] 選項。依預設，會為所有使用者選取 [!UICONTROL 「存取原始] 」選項。若要防止使用者群組存取原始轉譯，請取消選取對應該群組的選項。

   ![使用者群組角色](assets/access-original-rend.png)

   >[!NOTE]
   如果使用者新增至多個群組，如果其中一個群組有限制，限制將適用於該使用者。
   此外，存取影像檔案的原始轉譯限制並不適用於管理員，即使他們是受限制群組成員亦然。

4. Click **[!UICONTROL Save]**. 已針對對應群組修改角色。

   >[!NOTE]
   使用者對群組關聯或使用者群組成員資格每個小時都會同步至品牌入口網站。使用者或群組角色的變更會在下次同步工作執行後生效。
