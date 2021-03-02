---
title: '設定並發佈從AEM Assets到品牌入口網站的貢獻資料夾 '
seo-title: 設定並發佈從AEM Assets到品牌入口網站的貢獻資料夾
description: 深入瞭解如何從AEM Assets設定及發佈貢獻資料夾至品牌入口網站。
seo-description: 深入瞭解如何從AEM Assets設定及發佈貢獻資料夾至品牌入口網站。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 4221199d874ce63a936e5e6e02a16ee95cab4499
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 0%

---


# 在AEM Assets{#configure-contribution-folder}中設定貢獻資料夾

對於協作資產採購，AEM用戶（具有權限的管理員和非管理員用戶）可以建立「資產貢獻」類型&#x200B;**的新資料夾，確保建立的新資料夾可以由品牌門戶用戶提交資產。**&#x200B;這會自動觸發在新建立的&#x200B;**Contribution**&#x200B;資料夾中建立另外兩個子資料夾的工作流程，名為&#x200B;**SHARED**&#x200B;和&#x200B;**NEW**。

然AEM後，使用者會將應新增至貢獻資料夾的資產類型以及一組基準資產的簡介上傳至&#x200B;**SHARED**&#x200B;資料夾，以確保品牌入口網站使用者擁有所需的資訊，以定義資產需求。 然後，管理員可以先授與作用中的品牌入口網站使用者對貢獻資料夾的存取權，再將新建立的貢獻資料夾發佈至品牌入口網站。

以下視訊示範如何在AEM Assets設定「貢獻」檔案夾：

>[!VIDEO](https://video.tv.adobe.com/v/30547)

使用AEM者在設定貢獻資料夾時執行下列活動：

* [建立貢獻資料夾](#create-contribution-folder)
* [上傳資產需求並指派參與者](#configure-contribution-folder-properties)
* [上傳基準資產](#uplad-new-assets-to-contribution-folder)
* [將貢獻資料夾從AEM Assets發佈至品牌入口網站](#publish-contribution-folder-to-brand-portal)

## 建立貢獻資料夾{#create-contribution-folder}


擁有建AEM立新資料夾權限的管理員和非管理員使用者，可以在AEM Assets建立貢獻資料夾。
若要建立貢獻檔案夾，請建立新的「資產貢獻」類型檔案夾，以確保建立的新檔案夾可由品牌入口網站使用者提交資產。  這會自動觸發工作流程，此工作流程會在貢獻資料夾中建立另外兩個子資料夾，稱為SHARED和NEW。

>[!NOTE]
>
>您可以在資料夾中建立多個貢獻資料夾。 請勿在其他貢獻資料夾內建立貢獻資料夾。

**要建立貢獻資料夾：**
1. 登入您的AEM Assets實例。

1. 導覽至「**[!UICONTROL 資產]** > **[!UICONTROL 檔案]**」。 它列出了AEM Assets儲存庫中的所有現有資料夾。

1. 按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以建立新資料夾。 **[!UICONTROL 「建立文]** 件夾」(Create Folder)對話框開啟。

1. 輸入資料夾的&#x200B;**[!UICONTROL Title]**&#x200B;和&#x200B;**[!UICONTROL Name]** ，然後選擇&#x200B;**[!UICONTROL 資產貢獻]**複選框。
建議您使用小寫字母，而不需任何空格來命名資料夾。

1. 按一下&#x200B;**[!UICONTROL 建立]**。您可以在AEM Assets儲存庫中看到列出的貢獻資料夾。

   >[!NOTE]
   >
   >非管理員使用者可以建立和共用資產貢獻資料夾，但無法修改或刪除它。


   ![](assets/create-contribution-folder.png)

1. 按一下以開啟貢獻資料夾，您會看到兩個子資料夾-**[!UICONTROL SHARED]**&#x200B;和&#x200B;**[!UICONTROL NEW]**&#x200B;會自動在貢獻資料夾中建立。

   ![](assets/contribution-folder.png)

您也可以在建立貢獻資料夾時設定貢獻資料夾屬性。

## 設定貢獻資料夾屬性{#configure-contribution-folder-properties}

管AEM理員在配置貢獻資料夾屬性時執行以下活動。

* **添加說明**:提供貢獻資料夾的高階說明。
* **上傳簡介**:上傳包含資產相關資訊的資產需求檔案。
* **新增參與者**:新增品牌入口網站使用者，以授與他們對貢獻資料夾的存取權。

資產需求是指管理員提供的詳細資訊，以協助參與者（品牌入口網站使用者）瞭解貢獻資料夾的需求和需求。 管理員上傳資產需求檔案，其中包含應新增至貢獻檔案夾的資產類型及資產相關資訊的簡介，例如用途、影像類型、最大大小等。

**若要設定貢獻資料夾屬性：**

1. 登入您的AEM Assets實例。

1. 導覽至「**[!UICONTROL 資產>檔案]**」，並找出貢獻資料夾。
1. 選擇貢獻資料夾並按一下&#x200B;**[!UICONTROL 屬性]**&#x200B;以開啟資料夾屬性窗口。

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. 導覽至「資產貢獻&#x200B;**[!UICONTROL 」標籤。]**
1. 輸入貢獻資料夾的高階&#x200B;**[!UICONTROL 說明]**。
1. 按一下「上傳簡報」，從本機電腦瀏覽並上傳「資產需求檔案」。********

   ![](assets/upload.png)

1. 在&#x200B;**[!UICONTROL 新增使用者]**&#x200B;欄位中，新增您要與其共用貢獻資料夾的品牌入口網站使用者。 這些使用者可以使用品牌入口網站介面存取內容並上傳至貢獻資料夾。
1. 按一下「**[!UICONTROL 儲存]**」。

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>搜尋結果以在AEM Assets設定的品牌入口網站使用者清單為基礎。 請確定您有更新的品牌入口網站使用者清單。

## 上傳資產至貢獻資料夾{#uplad-new-assets-to-contribution-folder}

品牌入口網站使用者可以下載資產需求，以瞭解貢獻的需求。
然後，他們可以建立新的貢獻資產，並將其上傳至貢獻檔案夾中的NEW檔案夾。

>[!NOTE]
>
>品牌入口網站使用者只能將資產上傳至NEW檔案夾。
>
>任何品牌入口網站租用戶的上傳上限為&#x200B;**10** GB，累計會套用至所有貢獻資料夾。


將新建立的資產發佈至AEM Assets後，品牌入口網站使用者可以從NEW檔案夾中刪除這些資產。 但是，品牌入口網站管理員可以從NEW和SHARED資料夾刪除資產。

當建立貢獻資料夾的目標達成後，品牌入口網站管理員可以刪除貢獻資料夾，以釋放其他使用者的上傳空間。

>[!NOTE]
>
>建議在將貢獻資料夾發佈至AEM Assets後釋放上傳空間，以便讓其他品牌入口網站使用者可使用該資料夾進行貢獻。
>
>如果您需要將品牌入口網站的上傳限制擴充至&#x200B;**10** GB以外，請連絡Adobe支援，指定此需求。


**若要上傳新資產：**

1. 登入您的品牌入口網站例項。
「品牌入口網站」控制面板會反映品牌入口網站使用者允許使用的所有現有資料夾，以及新共用的貢獻資料夾。

1. 選取貢獻資料夾，然後按一下以開啟它。 貢獻資料夾包含兩個子資料夾- **[!UICONTROL SHARED]**&#x200B;和&#x200B;**[!UICONTROL NEW]**。

1. 按一下&#x200B;**[!UICONTROL NEW]**&#x200B;資料夾。

   ![](assets/upload-new-assets1.png)

1. 按一下「建立&#x200B;**[!UICONTROL >]** > **[!UICONTROL 檔案]**」，上傳包含多個資產的個別檔案或檔案夾(.zip)。

   ![](assets/upload-new-assets2.png)

1. 瀏覽資產（檔案或檔案夾）並上傳至&#x200B;**[!UICONTROL NEW]**&#x200B;檔案夾。

   ![](assets/upload-new-assets3.png)

將所有資產或檔案夾上傳至NEW檔案夾後，將貢獻檔案夾發佈至AEM Assets。


## 將貢獻資料夾發佈至品牌入口網站{#publish-contribution-folder-to-brand-portal}

配置貢獻資料夾後，使AEM用者（管理員／非管理員使用者）就可將貢獻資料夾從AEM Assets發佈至品牌入口網站。 擁有存取貢獻檔案夾權限的品牌入口網站使用者會在發佈動作完成時收到電子郵件／脈衝通知。


**若要發佈貢獻資料夾：**

1. 登入您的AEM Assets實例。

1. 導覽至「**[!UICONTROL 資產>檔案]**」，並找出您要發佈至品牌入口網站的貢獻資料夾。
1. 選取貢獻資料夾，然後按一下「快速發佈」**[!UICONTROL >>「發佈至品牌入口網站」]**。]****[!UICONTROL 

   ![](assets/publish-contribution-folder-to-bp.png)

   貢獻資料夾發佈至品牌入口網站後，您會收到成功訊息。

電子郵件／脈衝通知會傳送給指派給貢獻資料夾的品牌入口網站使用者。 品牌入口網站使用者可以存取貢獻資料夾並開始貢獻。 請參閱[將資產上傳至貢獻資料夾並發佈至AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)。
