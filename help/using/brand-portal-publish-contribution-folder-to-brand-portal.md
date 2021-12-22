---
title: '設定貢獻資料夾並從Experience Manager Assets發佈至Brand Portal '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: 深入了解如何設定及發佈從Experience Manager Assets到Brand Portal的貢獻資料夾。
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 3845d9fa17e75d59493383303ca0978349ca0401
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# 在Experience Manager Assets中設定貢獻資料夾 {#configure-contribution-folder}

針對協作資產來源補充，Experience Manager Assets使用者（管理員和非擁有權限的管理員使用者）可以建立新的資料夾類型 **資產貢獻**，確保已建立的新資料夾可供Brand Portal使用者提交資產時開啟。  這會自動觸發建立額外兩個子資料夾(稱為 **共用** 和 **新增**，在新建立的 **貢獻** 檔案夾。

Experience Manager Assets使用者接著會上傳應新增至貢獻資料夾的資產類型簡介，以及一組基準資產，至 **共用** 資料夾，確保Brand Portal使用者擁有所需資訊。 然後，管理員可先授與作用中Brand Portal使用者對貢獻資料夾的存取權，再將新建立的貢獻資料夾發佈至Brand Portal。

下列影片示範如何在Experience Manager Assets中設定「貢獻」資料夾：

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets使用者在設定貢獻資料夾時執行下列活動：

* [建立貢獻資料夾](#create-contribution-folder)
* [上傳資產需求並指派貢獻者](#configure-contribution-folder-properties)
* [上傳基線資產](#uplad-new-assets-to-contribution-folder)
* [將貢獻資料夾從Experience Manager Assets發佈至Brand Portal](#publish-contribution-folder-to-brand-portal)

## 建立貢獻資料夾 {#create-contribution-folder}


Experience Manager Assets管理員和非擁有建立新資料夾權限的使用者，可以在Experience Manager Assets中建立貢獻資料夾。
若要建立貢獻資料夾，請建立「資產貢獻」類型的新資料夾，確保已建立的新資料夾可供Brand Portal使用者提交資產。  這會自動觸發工作流程，在貢獻資料夾內建立另外兩個子資料夾，稱為SHARED和NEW。


>[!NOTE]
>
>管理員可以在資料夾內建立多個資產貢獻資料夾。
>
>資產貢獻資料夾包含用於資產散布和貢獻的NEW和SHARED資料夾。 請勿在貢獻資料夾內建立資產、資料夾或貢獻資料夾。


您可以在建立貢獻資料夾時個別設定貢獻資料夾屬性。 在此範例中，我們會個別設定屬性。

**若要建立貢獻資料夾：**

1. 登入您的Experience Manager Assets執行個體。

1. 導覽至 **[!UICONTROL 資產]** > **[!UICONTROL 檔案]**. 它會列出Experience Manager Assets存放庫中的所有現有資料夾。

1. 按一下 **[!UICONTROL 建立]** 來建立新資料夾。 **[!UICONTROL 建立資料夾]** 對話框開啟。

1. 輸入 **[!UICONTROL 標題]** 和 **[!UICONTROL 名稱]** ，然後選取 **[!UICONTROL 資產貢獻]** 框。
建議使用小寫字母而不含任何空格來命名資料夾。

1. 按一下&#x200B;**[!UICONTROL 建立]**。您可以在Experience Manager Assets存放庫中看到列出的貢獻資料夾。

   >[!NOTE]
   >
   >非管理員使用者可以建立和共用資產貢獻資料夾，但無法修改或刪除。


   ![](assets/create-contribution-folder.png)

1. 按一下以開啟貢獻資料夾，您會看到兩個子資料夾 — **[!UICONTROL 共用]** 和 **[!UICONTROL 新增]** 會在貢獻資料夾中自動建立。

   ![](assets/contribution-folder.png)


## 設定貢獻資料夾屬性 {#configure-contribution-folder-properties}

Experience Manager Assets管理員在設定貢獻資料夾的屬性時，會執行下列活動。

* **新增說明**:提供貢獻資料夾的高階說明。
* **上傳簡報**:上傳包含資產相關資訊的資產需求檔案。
* **新增貢獻者**:新增Brand Portal使用者，以授與他們對貢獻資料夾的存取權。

資產需求是指管理員為協助貢獻者(Brand Portal使用者)了解貢獻資料夾的需求和需求而提供的詳細資訊。 管理員上傳資產需求檔案，其中包含應新增至貢獻資料夾的資產類型及資產相關資訊（例如用途、影像類型、最大大小等）的簡介。

**若要設定貢獻資料夾屬性：**

1. 登入您的Experience Manager Assets執行個體。

1. 導覽至 **[!UICONTROL 資產>檔案]** 並找出貢獻資料夾。
1. 選取貢獻資料夾，然後按一下 **[!UICONTROL 屬性]** 開啟「資料夾屬性」窗口。

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. 導覽至 **[!UICONTROL 資產貢獻]** 標籤。
1. 進入高級 **[!UICONTROL 說明]** 的下一頁。
1. 按一下 **[!UICONTROL 上傳簡報]** 從本機電腦瀏覽並上傳 **資產需求單據**.

   ![](assets/upload.png)

1. 在 **[!UICONTROL 添加用戶]** 欄位中，新增您要與其共用貢獻資料夾的Brand Portal使用者。 這些使用者可使用Brand Portal介面存取內容，並上傳至貢獻資料夾。
1. 按一下「**[!UICONTROL 儲存]**」。

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>搜尋結果以Experience Manager Assets中設定的Brand Portal使用者清單為基礎。 確定您有更新的Brand Portal使用者清單。

管理員可以下載 `user.csv` 檔案 [!DNL Admin Console] 並作為新增Brand Portal使用者的基礎範本。 前往 [!UICONTROL 使用者] 並按一下 [!UICONTROL 將使用者清單匯出為csv] 下載選項 `users.csv` 檔案。 下列範例使用者清單詳細說明新增使用者所需的屬性。 使用者項目的唯一必要屬性是 `Email` 而所有其他屬性則為選用。

[取得檔案](assets/users.csv)

## 上傳資產至貢獻資料夾 {#uplad-new-assets-to-contribution-folder}

Experience Manager Assets使用者上傳一組基準資產至 **共用** 資料夾，確保Brand Portal使用者具備所需資訊。

**若要上傳基準資產：**

1. 登入您的Experience Manager Assets執行個體。

1. 導覽至 **[!UICONTROL 資產>檔案]** 並找出貢獻資料夾。

1. 選取貢獻資料夾，然後按一下以開啟它。

1. 按一下 **[!UICONTROL 新增]** 檔案夾。

   ![](assets/upload-new-assets1.png)

1. 按一下 **[!UICONTROL 建立]** > **[!UICONTROL 檔案]** 上傳包含多個資產的個別檔案或資料夾(.zip)。

   ![](assets/upload-new-assets2.png)

1. 瀏覽資產（檔案或資料夾）並上傳至 **[!UICONTROL 新增]** 檔案夾。

   ![](assets/upload-asset4.png)

將所有資產或資料夾上傳至NEW資料夾後，將貢獻資料夾發佈至Experience Manager Assets。


## 將貢獻資料夾發佈至Brand Portal {#publish-contribution-folder-to-brand-portal}

設定貢獻資料夾後，Experience Manager Assets使用者（管理員/非管理員使用者）就可以將貢獻資料夾從Experience Manager Assets發佈至Brand Portal。 擁有存取貢獻資料夾權限的Brand Portal使用者會在完成發佈動作時收到電子郵件/脈衝通知。


**若要發佈貢獻資料夾：**

1. 登入您的Experience Manager Assets執行個體。

1. 導覽至 **[!UICONTROL 資產>檔案]** 並找出您要發佈至Brand Portal的貢獻資料夾。
1. 選取貢獻資料夾，然後按一下 **[!UICONTROL 快速發佈]** > **[!UICONTROL 發佈至Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   貢獻資料夾發佈至Brand Portal後，您會收到成功訊息。

會傳送電子郵件/脈衝通知給指派給貢獻資料夾的Brand Portal使用者。 Brand Portal使用者可以存取貢獻資料夾並開始貢獻。 看， [上傳資產至貢獻資料夾並發佈至Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
