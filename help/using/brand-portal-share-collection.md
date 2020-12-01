---
title: 共用集合
seo-title: 共用集合
description: AEM Assets品牌入口網站管理員可以與授權使用者共用或取消共用系列或智慧型系列。 編輯人員只能檢視和共用由他們建立、與他們共用的系列，以及公開的系列。
seo-description: AEM Assets品牌入口網站管理員可以與授權使用者共用或取消共用系列或智慧型系列。 編輯人員只能檢視和共用由他們建立、與他們共用的系列，以及公開的系列。
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: a587061bc8afe250a88b4a02b42b6acd9ef6bbeb
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---


# 共用系列{#share-collections}

系列代表一組儲存在Adobe Experience Manager Assets品牌入口網站中的相關資產。 使用者可透過[套用搜尋或Facet搜尋來建立智慧型系列，以篩選出相關資產](brand-portal-searching.md)並將它們儲存在一起，以方便存取並進一步與其他品牌入口網站使用者共用。

管理員可以與授權品牌入口網站使用者共用及取消共用系列。 編輯人員和檢視者可檢視並共用由他們建立、與他們共用的系列，以及公開的系列。

>[!NOTE]
>
>編輯者無法將公開系列變更為非公開的系列，因此&#x200B;**[!UICONTROL 系列設定]**&#x200B;對話方塊中沒有&#x200B;**[!UICONTROL 公開系列]**&#x200B;核取方塊。

## 共用集合 {#share-collection}

以下是與授權品牌入口網站使用者共用系列的步驟：

1. 登入您的品牌入口網站租用戶。 依預設，會開啟&#x200B;**[!UICONTROL 檔案]**&#x200B;檢視，其中包含所有已發佈的資產和資料夾。

1. 在頂端的快速導覽中，按一下「系列」****。

1. 從&#x200B;**[!UICONTROL Collections]**&#x200B;控制台，執行下列任一操作：

   * 將指標暫留在您要共用的系列上。 從系列的快速動作縮圖中，按一下「設定」**[!UICONTROL 圖示。]**

      ![](assets/settings-icon.png)

   * 選取您要共用的系列。 在頂部的工具欄上，按一下「**[!UICONTROL 設定]**」。

      ![](assets/collection-console.png)

1. 在&#x200B;**[!UICONTROL 系列設定]**&#x200B;對話方塊中，選取您要與其共用系列的使用者，並選取使用者的角色，以符合其全域角色。 例如，將編輯器角色分配給全局編輯器，將查看器角色分配給全局查看器。

   或者，若要讓系列可供所有使用者使用，而不論其群組成員資格和角色為何，請選取「公用系列」核取方塊，將其公開。****

   >[!NOTE]
   >
   >不過，非管理員使用者可能無法建立公用系列，以避免擁有大量公用系列，以節省系統空間。 組織可以停用「管理工具」面板中「允許從&#x200B;**[!UICONTROL 一般]**&#x200B;設定建立公用系列」。****

   ![](assets/collection_sharingadduser.png)

   編輯者無法將公開系列變更為非公開的系列，因此在&#x200B;**[!UICONTROL 系列設定]**&#x200B;對話方塊中沒有&#x200B;**[!UICONTROL 公開系列]**&#x200B;核取方塊。

   ![](assets/collection-setting-editor.png)

1. 按一下&#x200B;**[!UICONTROL 添加]**&#x200B;按鈕添加用戶，然後按一下&#x200B;**[!UICONTROL 保存]**。 系列會與使用者共用。

   >[!NOTE]
   >
   >使用者的角色控制對系列內資產和資料夾的存取。 如果使用者沒有資產的存取權，則會與使用者共用空的系列。 此外，使用者的角色也會控制系列的可用動作。

## 取消共用系列{#unshare-a-collection}

若要取消共用先前共用的系列，請執行下列動作：

1. 從&#x200B;**[!UICONTROL Collections]**&#x200B;主控台中，選取您要取消共用的系列。

   在頂部的工具欄上，按一下「**[!UICONTROL 設定]**」。

   ![](assets/collection_settings.png)

1. 在&#x200B;**[!UICONTROL 系列設定]**&#x200B;對話方塊的&#x200B;**[!UICONTROL 成員]**&#x200B;區段下，按一下使用者旁的&#x200B;**[!UICONTROL x]**&#x200B;符號，將它們從可存取系列的使用者清單中移除。

   ![](assets/unshare_collection.png)

1. 出現警告訊息。 按一下&#x200B;**[!UICONTROL 確認]**&#x200B;取消共用系列。

1. 按一下&#x200B;**[!UICONTROL 保存]**&#x200B;以應用更改。

   從共用清單移除使用者後，非共用的系列就會從使用者的&#x200B;**[!UICONTROL Collections]**&#x200B;主控台移除。

<!--
1. Click the overlay icon on the left, and choose **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. From the siderail on the left, click **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

1. From the **[!UICONTROL Collections]** console, do one of the following:

    * Hover the pointer over the collection you want to share. From the quick action thumbnails available for the collection, click the **[!UICONTROL Settings]** icon.

   ![](assets/settings_thumbnail.png)

    * Select the collection you want to share. From the toolbar at the top, click **[!UICONTROL Settings]**.
    
   ![](assets/collection-sharing.png)

1. In the [!UICONTROL Collection Settings] dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. For example, assign the Editor role to a global editor, the Viewer role to a global viewer.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **[!UICONTROL Public Collection]** check-box.

   >[!NOTE]
   >
   >However, non-admin users can be restricted from creating public collections, to avoid having numerous public collections so that system space can be saved. Organizations can disable the **[!UICONTROL Allow public collections creation]** configuration from [!UICONTROL General] settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **[!UICONTROL Public Collection]** check-box available in **[!UICONTROL Collection Settings]** dialog.

   ![](assets/collection-setting-editor.png)

1. Select **[!UICONTROL Add]**, and then **[!UICONTROL Save]**. The collection is shared with the chosen users.

   >[!NOTE]
   >
   >A user's role governs access to the assets and folders inside a collection. If a user does not have access to assets, an empty collection is shared with the user. Also, a user's role governs the actions available for collections.

## Unshare a collection {#unshare-a-collection}

To unshare a previously shared collection, do the following:

1. From the **[!UICONTROL Collections]** console, select the collection you want to unshare.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. On the **[!UICONTROL Collection Settings]** dialog box, under **[!UICONTROL Members]**, click the **[!UICONTROL x]** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. In the warning message box, click **[!UICONTROL Confirm]** to confirm unshare.

   Click **[!UICONTROL Save]**.

1. Log in to Brand Portal with the credentials of the user you removed from the shared list. The collection is removed from the **[!UICONTROL Collections]** console.
-->