---
title: 發佈至「貢獻」檔案夾至AEM資產
seo-title: 發佈至「貢獻」檔案夾至AEM資產
description: 深入瞭解在品牌入口網站中將貢獻檔案夾發佈至AEM Assets。
seo-description: 深入瞭解在品牌入口網站中將貢獻檔案夾發佈至AEM Assets。
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 8e08fdfb95686d28960c0fd440754b90c22ae557
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# 將貢獻資料夾發佈至AEM Assets {#publish-contribution-folder-to-aem}

品牌入口網站使用者可以將貢獻檔案夾發佈至AEM Assets，而不需存取AEM作者實例。

請確定您已完成[資產需求](brand-portal-download-asset-requirements.md)，並在貢獻檔案夾的&#x200B;**NEW**&#x200B;資料夾中上傳新建立的資產。 請參閱[將資產上傳至貢獻資料夾](brand-portal-upload-assets-to-contribution-folder.md)。

**若要發佈貢獻資料夾：**

1. 登入您的品牌入口網站例項。

1. 從「品牌入口網站」控制面板選取貢獻資料夾。
1. 按一下「發佈至AEM **[!UICONTROL 」。]**

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

在發佈工作流程的不同階段，會傳送電子郵件／脈衝通知給品牌入口網站使用者和管理員：
1. **已佇列** -當品牌入口網站中觸發發佈工作流程時，會傳送通知給品牌入口網站使用者和品牌入口網站管理員。

1. **完成** -當貢獻資料夾成功發佈至AEM Assets時，會傳送通知給品牌入口網站使用者和品牌入口網站管理員。


**發佈工作狀態**

管理員可使用兩個報表來檢視從Brand Portal發佈至AEM Assets的資產貢獻資料夾狀態。

* 在品牌入口網站中，導覽至「工具&#x200B;**** > **[!UICONTROL 資產貢獻狀態]**」。 此報告會反映所有發佈工作的狀態，包括發佈工作流程的不同階段（已佇列和完成）。

* 在AEM Assets作者例項中，導覽至&#x200B;**[!UICONTROL Tools]** > **[!UICONTROL Jobs]**。 此報表只反映處於待定狀態的發佈作業。




