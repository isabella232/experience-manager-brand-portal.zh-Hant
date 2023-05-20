---
title: 上載資產並發佈從Brand Portal到Experience Manager Assets的Contribution資料夾
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: 深入瞭解上載新資產和發佈從Brand Portal到Experience Manager Assets的稿件資料夾。
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 606f4389780025f5cf92b11bf8cac464e36be44a
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# 將稿資料夾發佈到Experience Manager Assets {#using-asset-souring-in-bp}

具有適當權限的Brand Portal用戶可以將多個資產或包含多個資產的資料夾上載到貢獻資料夾。 但是，Brand Portal用戶只能將資產上傳到 **新建** 的子菜單。 **共用** 資料夾適用于建立新的貢獻資產時，品牌入口網站使用者可使用的基準資產（參照內容）。

Brand Portal用戶具有訪問貢獻資料夾的權限，可以執行以下活動：

* [下載資產要求](#download-asset-requirements)
* [將新資產上載到貢獻資料夾](#uplad-new-assets-to-contribution-folder)
* [將稿資料夾發佈到Experience Manager Assets](#publish-contribution-folder-to-aem)

## 下載資產要求 {#download-asset-requirements}

當「貢獻」資料夾由 Experience Manager Assets 用戶共用時，品牌入口網站使用者會自動接收電子郵件/脈衝通知，並允許他們下載的摘要資產（參考檔） **** ，以確保他們瞭解下載需求。

品牌入口網站用戶執行下列活動下載資產需求：

* **下載簡要** ：下載附加至「貢獻」資料夾的簡短（資產要求檔），該檔案包含資產相關資訊按讚類型的資產、用途、支援的格式、最大資產大小等。
* **下載基線資產** ：下載可用於瞭解所需資產類型的基線資產。 品牌入口網站使用者可以使用這些資產作為參考，為貢獻建立新的資產。

Brand Portal儀表板反映允許Brand Portal用戶使用的所有現有資料夾以及新共用的貢獻資料夾。 在此示例中，Brand Portal用戶僅有權訪問新建立的貢獻資料夾，沒有其他現有資料夾與用戶共用。

**若要下載資產要求：**

1. 登入您的品牌入口網站執行個體。
1. 從品牌入口網站控制台中選取貢獻資料夾。
1. 按一下 **[!UICONTROL 屬性]** 。 包含貢獻資料夾詳細資訊的屬性視窗開啟。

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. **[!UICONTROL 按一下下載簡短]** 選項，以下載您的本機電腦檔的資產需求。

   ![](assets/download.png)

1. 返回品牌入口網站控制台。
1. 按一下以開啟「貢獻」資料夾，您可以在貢獻資料夾中看到兩個子資料夾（ **[!UICONTROL 共用]** 和 **[!UICONTROL 新增]** ）。 共用資料夾包含管理員共用的所有基準資產（參照內容）。
1. 您可以下載包含您的本機電腦上所有基準資產的 **[!UICONTROL 共用]** 資料夾。或者，您可以開啟 **[!UICONTROL 共用]** 資料夾，然後按一下 **「下載** 」圖示以下載個別檔案/資料夾。

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

瀏覽簡介（資產需求文檔）並參考基準資產以瞭解資產需求。 現在，您可以建立新的貢獻資產，並將其上傳至「貢獻」資料夾。。


## 上傳資產至貢獻檔案夾 {#upload-new-assets-to-contribution-folder}

完成資產需求後，品牌入口網站使用者可以建立新的貢獻資產，並將其上傳至貢獻資料夾中的新資料夾。 用戶可以上傳多個資產至資產貢獻資料夾。 不過，一次只能建立一個檔案夾。

>[!NOTE]
>
>品牌入口網站使用者可以上傳資產（每個檔案大小最多 **2** GB）至新資料夾。
>
>任何品牌入口網站租戶的最大上傳限制為 **10** GB，累積應用於所有貢獻資料夾。
>
>上載到Brand Portal的資產不會處理格式副本，也不包含預覽。

>[!NOTE]
>
>建議在將貢獻資料夾發佈到Experience Manager Assets後釋放上載空間，以便其他Brand Portal用戶可以獲得貢獻。
>
>如果需要將您的Brand Portal租戶的上載限制擴展到 **10** GB，聯繫客戶支援，指定要求。


**要上載新資產，請執行以下操作：**

1. 登錄到您的Brand Portal實例。
Brand Portal儀表板反映允許Brand Portal用戶使用的所有現有資料夾以及新共用的稿件資料夾。

1. 選擇貢獻資料夾，然後按一下將其開啟。 貢獻資料夾包含兩個子資料夾 —  **[!UICONTROL 共用]** 和 **[!UICONTROL 新建]**。

1. 按一下 **[!UICONTROL 新建]** 的子菜單。

   ![](assets/upload-new-assets4.png)

1. 按一下 **[!UICONTROL 建立]** > **[!UICONTROL 檔案]** 上載包含多個資產的單個檔案或資料夾(.zip)。

   ![](assets/upload-new-assets5.png)

1. 瀏覽資產（檔案或資料夾）並將其上載到 **[!UICONTROL 新建]** 的子菜單。

   ![](assets/upload-asset4.png)

將所有資產或資料夾上載到NEW資料夾後，將貢獻資料夾發佈到Experience Manager Assets。


## 將稿資料夾發佈到Experience Manager Assets {#publish-contribution-folder-to-aem}

品牌入口網站使用者可以發佈「貢獻」資料夾來 Experience Manager Assets，而無需存取 Experience Manager 作者執行個體。

請確定您已完成資產需求，並上傳「貢獻」資料夾內新 **檔案夾中** 新建立的資產。

**若要發佈貢獻資料夾。。**

1. 登入您的品牌入口網站執行個體。

1. 從品牌入口網站控制台中選取貢獻資料夾。
1. 按一下 **[!UICONTROL 發佈到AEM]**。

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

在發佈工作流的不同階段向Brand Portal用戶和管理員發送電子郵件/脈衝通知：

1. **已排隊**  — 在Brand Portal觸發發佈工作流時，會向Brand Portal用戶和Brand Portal管理員發送通知。

1. **完成**  — 當貢獻資料夾成功發佈到Brand Portal時，會向Brand Portal用戶和管理員發送通知。

將新建立的資產發佈到Experience Manager Assets後，Brand Portal用戶可以從NEW資料夾中刪除這些資產。 但是，Brand Portal管理員可以從NEW和SHARED資料夾中刪除資產。

一旦實現建立貢獻資料夾的目標，Brand Portal管理員可以刪除貢獻資料夾以釋放其他用戶的上載空間。

## 發佈作業狀態 {#publishing-job-status}

管理員可以使用兩個報告來查看從Brand Portal發佈到Experience Manager Assets的資產貢獻資料夾的狀態。

* 在Brand Portal，導航到 **[!UICONTROL 工具]** > **[!UICONTROL 資產貢獻狀態]**。 此報表反映發佈工作流不同階段的所有發佈作業的狀態。

   ![](assets/contribution-folder-status-v2.png)

* 在Experience Manager Assets（內部或托管服務），導航至 **[!UICONTROL 資產]** > **[!UICONTROL 作業]**。 此報表反映所有發佈作業的最終狀態（成功或錯誤）。

   ![](assets/publishing-status.png)

* 在Experience Manager Assetsas a Cloud Service，導航到 **[!UICONTROL 資產]** > **[!UICONTROL 作業]**。

   或者，您可以直接導航到 **[!UICONTROL 作業]** 的上界。

   此報告反映所有發佈作業的最終狀態（成功或錯誤），包括將資產從Brand Portal導入Experience Manager Assetsas a Cloud Service。

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->

## 自動從Contribution資料夾刪除發佈到Experience Manager Assets的資產 {#automatically-delete-published-assets-from-contribution-folder}

品牌入口網站現在每12小時執行一次自動作業，掃描所有貢獻資料夾並刪除所有發佈至 AEM 的資產。 因此，您不需要手動刪除「貢獻」資料夾中的資產，以將資料夾大小保持在 [閾值限制](#upload-new-assets-to-contribution-folder)。 您還可以監視在過去七天內自動執行的刪除作業的狀態。 作業的報表提供以下詳細資訊：

* 作業開始時間
* 作業結束時間
* 作業狀態
* 作業中包括的總資產
* 工作中成功刪除的資產總數
* 因工作執行而提供的儲存總數

   ![刪除報告](assets/deletion-reports.png)

您還可以進一步追溯以查看刪除作業中包括的每個資產的詳細資訊。 報表中包括資產標題、大小、作者、刪除狀態和刪除時間等詳細資訊。

![刪除報告詳細資訊](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * 客戶可以請求 Adobe Systems 客戶支援來停用和重新啟用自動刪除工作功能，或變更其執行的頻率。
> * 此功能適用于 Experience Manager 6.5.13.0 及更高版本。


### 檢視和下載刪除報表 {#view-delete-jobs}

若要視圖和下載刪除工作的報表：

1. 在品牌入口網站中，導覽至 **[!UICONTROL 工具]** > **[!UICONTROL 資產貢獻狀態]** > **[!UICONTROL 刪除報表]** 選項。

1. 選取工作，然後按一下 **[!UICONTROL 檢視]** 以視圖報表。

   檢視刪除工作中包含的每個資產的詳細資料。 報表中包含資產標題、大小、作者、刪除狀態和刪除時間等詳細資訊。 按一下 **[!UICONTROL 下載]** 以下載 CSV 格式中的工作報表。

   報表中資產的刪除狀態可具有下列可能值：

   * **已刪除** -已成功從貢獻資料夾中刪除資產。

   * **找** 不到-品牌入口網站找不到貢獻資料夾中的資產。 已手動從檔案夾中刪除資產。

   * **略過** -品牌入口網站略過資產刪除，因為「貢獻」資料夾中的資產目前尚未發佈至 Experience Manager。

   * **失敗** -品牌入口網站無法刪除資產。 有三個重試嘗試刪除具有 `Failed` 刪除狀態的資產。 如果資產第三次嘗試刪除失敗，則需要手動刪除資產。

### 刪除報告

品牌入口網站也可讓您選擇一或多個報表並手動刪除。

若要刪除報告：

1. 導航到 **[!UICONTROL 工具]**>**[!UICONTROL 資產貢獻狀態]**>**[!UICONTROL 刪除報告]** 的雙曲餘切值。

1. 選擇一個或多個報告，然後按一下 **[!UICONTROL 刪除]**。


