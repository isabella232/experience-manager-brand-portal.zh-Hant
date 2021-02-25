---
title: 使用報表
seo-title: 使用報表
description: AEM Assets品牌入口網站管理員可以檢視品牌入口網站使用情況的報表，並建立、管理及檢視透過品牌入口網站分享的資產下載、過期、發佈及連結相關的報表。
seo-description: AEM Assets品牌入口網站管理員可以檢視品牌入口網站使用情況的報表，並建立、管理及檢視透過品牌入口網站分享的資產下載、過期、發佈及連結相關的報表。
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
translation-type: tm+mt
source-git-commit: 0e26e6ae38d7b62576bc1751965a71168ad8faf5
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 2%

---


# 使用報表 {#work-with-reports}

報告功能有助於評估品牌入口網站的使用情況，並瞭解內部和外部使用者如何與核准的資產互動。 管理員可以檢視「品牌入口網站使用狀況」報表，該報表一律可在「資產報表」頁面上使用。 不過，使用者登入和透過連結下載、過期、發佈和共用資產的報表可從「資產報表」頁面產生和檢視。 這些報表有助於分析資產部署，可讓您衍生關鍵成功度量，以評估組織內外已核准資產的接受度。

報表管理介面是直覺式的，包含存取儲存報表的精細選項和控制項。 您可以從「資產報表」頁面檢視、下載或刪除報表，其中會列出所有先前產生的報表。

## 檢視報表{#view-reports}

若要檢視報表，請依照下列步驟進行：

1. 從頂端的工具列，點選／按一下AEM標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下「建立／管理報表」]**以開啟「資產報表」]**&#x200B;頁面。**[!UICONTROL **[!UICONTROL 

   ![](assets/access-asset-reports.png)

1. 存取「資產報表」頁面中的&#x200B;**[!UICONTROL 使用]**&#x200B;報表和其他產生的報表。

   >[!NOTE]
   >
   >使用狀況報表是在品牌入口網站中產生的預設報表。 無法建立或刪除。 不過，您可以建立、下載和刪除「下載」、「過期」、「發佈」、「連結共用」和「使用者登入」報表。

   若要檢視報表，請按一下報表連結。 或者，選取報表，並從工具列點選／按一下「檢視」圖示。

   **[!UICONTROL 使用]** 狀況報表會顯示有效品牌入口網站使用者人數、所有資產佔用的儲存空間，以及品牌入口網站中資產總計的相關資訊。未指派給管理控制台中任何產品設定檔的品牌入口網站使用者被視為非作用中使用者，不會反映在&#x200B;**[!UICONTROL 使用狀況報表]**中。
報表也會顯示每個資訊度量的允許容量。

   ![](assets/usage-report.png)

   **[!UICONTROL 「使]** 用者登入」報表會提供有關登入品牌入口網站之使用者的資訊。報表會顯示每個使用者的顯示名稱、電子郵件ID、角色（管理員、檢視器、編輯器、訪客）、群組、上次登入、活動狀態，以及從Brand Portal 6.4.2部署到產生報表時的登入計數。

   ![](assets/user-logins.png)

   **[!UICONTROL 下]** 載報表會列出特定日期和時間範圍內下載的所有資產的詳細資訊。

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >資產&#x200B;**[!UICONTROL Download]**&#x200B;報表只會顯示個別選取並從品牌入口網站下載的資產。 如果使用者已下載包含資產的檔案夾，報表不會顯示該檔案夾或該檔案夾內的資產。

   **[!UICONTROL 「到]** 期報告」會列出並詳細說明在特定時間範圍內到期的所有資產。

   ![](assets/expiration-report.png)

   **[!UICONTROL 「發]** 布報表」會列出並提供在指定時段內從AEM發佈至品牌入口網站的所有資產的相關資訊。

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >「發佈報表」不會顯示內容片段的相關資訊，因為內容片段無法發佈至品牌入口網站。

   **[!UICONTROL 「連結共用」]** 報表會列出在特定時段內，透過品牌入口網站介面的連結共用的所有資產。報表也會通知透過連結共用資產的時間、使用者、連結的到期時間，以及租用戶（及共用資產連結的使用者）的共用連結數。 無法自訂「連結共用報表」欄。

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >「連結共用報表」不會顯示有權存取透過連結分享之資產或已透過連結下載資產的使用者。
   >
   >若要追蹤透過共用連結的下載，您必須在&#x200B;**[!UICONTROL 建立報表]**&#x200B;頁面上選取「僅連結共用下載」選項後，產生下載報表。 ****&#x200B;不過，在本例中，使用者（下載者）是匿名的。

## 產生報告{#generate-reports}

管理員可以生成並管理以下標準報告，生成後，這些報告將保存為[稍後訪問](../using/brand-portal-reports.md#main-pars-header):

* 使用者登入
* 下載
* 過期
* 發佈
* 連結共用

您可自訂「下載」、「過期」和「發佈」報表中的欄供檢視。 若要產生報表，請依照下列步驟進行：

1. 從頂端的工具列，點選／按一下AEM標誌以存取管理工具。

1. 在管理工具面板中，點選／按一下「建立／管理報表」]**以開啟「資產報表」]**&#x200B;頁面。**[!UICONTROL **[!UICONTROL 

   ![](assets/asset-reports.png)

1. 在「資產 報表」頁面 ，點選/按一下「 **[!UICONTROL 建立」]**。
1. 從&#x200B;**[!UICONTROL 建立報表]**&#x200B;頁面中，選取要建立的報表，並點選／按一下&#x200B;**[!UICONTROL 下一步]**。

   ![](assets/crete-report.png)

1. 設定報表詳細資訊。 指定&#x200B;**[!UICONTROL Download]**、**[!UICONTROL Expiration]**&#x200B;和&#x200B;**[!UICONTROL Publish]**&#x200B;報表的標題、說明、資料夾結構（其中報表需要執行並產生統計資料）和日期範圍。

   ![](assets/create-report-page.png)

   但是，**[!UICONTROL 連結共用報表]**&#x200B;只需要標題、說明和日期範圍參數。

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >報表產生時，報表標題中的特殊字元#和%會以連字型大小(-)取代。

1. 點選／按一下&#x200B;**[!UICONTROL Next]**，以設定「下載」、「過期」和「發佈」報表的欄。
1. 根據需要選擇或取消選擇相應的複選框。 例如，若要在&#x200B;**[!UICONTROL Download]**&#x200B;報表中檢視使用者（下載資產）的名稱，請選取&#x200B;**[!UICONTROL Downloaded By]**。 下圖說明在「下載」報表中選取預設欄。

   ![](assets/createdownloadreport.png)

   您也可以新增自訂欄至這些報表，以顯示更多符合您自訂需求的資料。

   若要新增自訂欄至「下載」、「發佈」或「有效期」報表，請依照下列步驟執行：

   1. 若要顯示自訂欄，請點選／按一下[!UICONTROL 自訂欄]中的&#x200B;**[!UICONTROL Add]**。
   1. 在&#x200B;**[!UICONTROL 欄名稱]**&#x200B;欄位中指定欄的名稱。
   1. 使用屬性選擇器，選擇列需要映射到的屬性。

      ![](assets/property-picker.png)
或者，在屬性路徑欄位中鍵入路徑。

      ![](assets/property-path.png)

      若要新增更多自訂欄，請點選／按一下「新增&#x200B;****」，然後重複步驟2和3。

1. 點選／按一下&#x200B;**[!UICONTROL Create]**。 訊息會通知報表產生已開始。

## 下載報告{#download-reports}

若要將報表儲存並下載為。csv檔案，請執行下列其中一項作業：

* 在「資產報表」頁面上選取報表，然後從頂端的工具列點選／按一下「下載&#x200B;**[!UICONTROL 」。]**

![](assets/download-asset-report.png)

* 從「資產報表」頁面，開啟報表。 從報表頁面頂端選擇&#x200B;**[!UICONTROL 下載]**&#x200B;選項。

![](assets/download-report-fromwithin.png)

## 刪除報告{#delete-reports}

若要刪除現有報表，請從&#x200B;**[!UICONTROL 資產報表]**&#x200B;頁面選擇報表，並從頂端的工具列點選／按一下&#x200B;**[!UICONTROL 刪除]**。

>[!NOTE]
>
>**[!UICONTROL 無]** 法刪除「使用」報表。
