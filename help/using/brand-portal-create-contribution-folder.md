---
title: 建立貢獻資料夾
seo-title: 建立貢獻資料夾
description: '深入瞭解如何在AEM Assets中建立貢獻資料夾。 '
seo-description: 深入瞭解如何在AEM Assets中建立貢獻資料夾。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 92961850279ad5a676ec0bc655d3a16f0497b024
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}

AEM管理員和擁有建立新檔案夾權限的非管理員使用者可以在AEM Assets中建立 **Contribution** 檔案夾。
若要建立 **Contribution** 檔案夾，請建立新的「資產貢獻」檔案夾 ****，確保建立的新檔案夾可由Brand Portal使用者提交資產。  這會自動觸發在新建立的「貢獻」檔案夾中建立另外兩個子檔案夾( **SHARED** 和 **NEW**)的 **** 工作流程。

**若要建立新貢獻資料夾：**
1. 登入您的AEM作者例項預設URL: http:// localhost:4502/aem/start.html
1. 導覽至「 **[!UICONTROL 資產>檔案]**」。它會列出AEM Assets存放庫中的所有現有檔案夾。
1. Click **[!UICONTROL Create]** to create a new folder. 「建立資料夾」(Create Folder)彈出窗口開啟。
1. 輸入資 **[!UICONTROL 料夾的]** 標題 **[!UICONTROL 和名稱]** ，並勾選核取方塊「資產貢 **[!UICONTROL 獻」]**。
建議使用沒有空格的小字母來命名資料夾。
1. 按一下&#x200B;**[!UICONTROL 建立]**。
   ![](assets/create-contribution-folder.png)
1. 您可以在AEM Assets儲存庫中看到新建立的貢獻資料夾。
1. 按一下以開啟貢獻資料夾，您會看到兩個子資料夾-**[!UICONTROL SHARED]****[!UICONTROL 和NEW]** -會自動在貢獻資料夾中建立。\
   ![](assets/contribution-folder.png)

您現在可以設定「貢獻」檔案夾屬性。 請參閱「設 [定貢獻資料夾屬性](brand-portal-configure-contribution-folder-properties.md)」。

>[!NOTE]
>
>非管理員使用者只能建立及共用資產貢獻資料夾。 建立貢獻資料夾後，非管理員使用者便無法修改或刪除它。
>
>不支援資產貢獻檔案夾巢狀。 您可以在資料夾中建立多個貢獻資料夾，但不得在其他貢獻資料夾中建立貢獻資料夾。

