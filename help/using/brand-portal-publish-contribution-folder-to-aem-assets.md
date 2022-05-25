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

具有適當權限的Brand Portal用戶可以將多個資產或包含多個資產的資料夾上載到貢獻資料夾。 但是，Brand Portal用戶只能將資產上傳到 **新建** 的子菜單。 的 **共用** 資料夾用於分發基準資產（參考內容），這些資產可供Brand Portal用戶使用，同時建立新資產供捐助。

Brand Portal用戶具有訪問貢獻資料夾的權限，可以執行以下活動：

* [下載資產要求](#download-asset-requirements)
* [將新資產上載到貢獻資料夾](#uplad-new-assets-to-contribution-folder)
* [將稿資料夾發佈到Experience Manager Assets](#publish-contribution-folder-to-aem)

## 下載資產要求 {#download-asset-requirements}

Brand Portal用戶在Experience Manager Assets用戶共用一個貢獻資料夾時自動接收電子郵件/脈衝通知，允許他們下載簡介（資產要求）文檔，並從 **共用** 資料夾，以確保他們瞭解資產要求。

Brand Portal用戶執行以下活動以下載資產要求：

* **下載簡介**:下載附加到繳費資料夾的簡介（資產需求文檔），該資料夾包含資產類型、用途、支援的格式、最大資產大小等與資產相關的資訊。
* **下載基準資產**:下載可用於瞭解所需資產類型的基準資產。 Brand Portal用戶可以使用這些資產作為參考，以建立新的資產作貢獻。

Brand Portal儀表板反映允許Brand Portal用戶使用的所有現有資料夾以及新共用的貢獻資料夾。 在此示例中，Brand Portal用戶僅有權訪問新建立的貢獻資料夾，沒有其他現有資料夾與用戶共用。

**要下載資產要求，請執行以下操作：**

1. 登錄到您的Brand Portal實例。
1. 從「Brand Portal」儀表板中選擇「貢獻」資料夾。
1. 按一下 **[!UICONTROL 屬性]**。 將開啟包含貢獻資料夾詳細資訊的屬性窗口。

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. 按一下 **[!UICONTROL 下載簡介]** 選項，在本地電腦上下載資產需求文檔。

   ![](assets/download.png)

1. 回到Brand Portal儀表板。
1. 按一下以開啟稿資料夾，您可以看到兩個子資料夾 — **[!UICONTROL 共用]** 和 **[!UICONTROL 新建]** 的子菜單。 SHARED資料夾包含管理員共用的所有基線資產（參考內容）。
1. 您可以下載 **[!UICONTROL 共用]** 包含本地電腦上所有基線資產的資料夾。
或者，你可以開啟 **[!UICONTROL 共用]** 資料夾，然後按一下 **下載** 表徵圖，可下載單個檔案/資料夾。

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

瀏覽簡介（資產需求文檔）並參考基準資產以瞭解資產需求。 現在，您可以建立新資產供稿，並將其上載到稿件資料夾。


## 將資產上載到貢獻資料夾 {#upload-new-assets-to-contribution-folder}

通過資產要求後，Brand Portal用戶可以建立新資產供捐贈，並將其上載到捐贈資料夾中的NEW資料夾。 用戶可以將多個資產上載到資產貢獻資料夾。 但是，一次只能建立一個資料夾。

>[!NOTE]
>
>Brand Portal用戶可以上傳資產(最大 **2** GB（每檔案大小）到NEW資料夾。
>
>任何Brand Portal租戶的最大上載限制為 **10**&#x200B;累計應用於所有貢獻資料夾的GB。
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

Brand Portal用戶可以將貢獻資料夾發佈到Experience Manager Assets，而無需訪問Experience Manager作者實例。

確保您已完成資產要求並將新建立的資產上載到 **新建** 資料夾。

**要發佈稿件資料夾：**

1. 登錄到您的Brand Portal實例。

1. 從「Brand Portal」儀表板中選擇「貢獻」資料夾。
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

Brand Portal現在每十二小時執行一次自動作業，以掃描所有Contribution資料夾並刪除發佈到的所有AEM資產。 因此，您不需要手動刪除「貢獻」資料夾中的資產，以將資料夾大小保持在 [閾值限制](#upload-new-assets-to-contribution-folder)。 您還可以監視在過去七天內自動執行的刪除作業的狀態。 作業的報表提供以下詳細資訊：

* 作業開始時間
* 作業結束時間
* 作業狀態
* 作業中包括的總資產
* 作業中已成功刪除的資產總數
* 作業運行後可用的總儲存

   ![刪除報告](assets/deletion-reports.png)

您還可以進一步追溯以查看刪除作業中包括的每個資產的詳細資訊。 報表中包括資產標題、大小、作者、刪除狀態和刪除時間等詳細資訊。

![刪除報告詳細資訊](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * 客戶可以請求Adobe客戶支援禁用並重新啟用自動刪除作業功能或更改其執行頻率。
> * 此功能可隨6.5.13.0和更高版本一起使用。


### 查看和下載刪除報告 {#view-delete-jobs}

要查看和下載刪除作業的報告，請執行以下操作：

1. 在Brand Portal，導航到 **[!UICONTROL 工具]**>**[!UICONTROL 資產貢獻狀態]**>**[!UICONTROL 刪除報告]** 的雙曲餘切值。

1. 選擇作業並按一下 **[!UICONTROL 視圖]** 按鈕

   查看刪除作業中包含的每個資產的詳細資訊。 報表中包括資產標題、大小、作者、刪除狀態和刪除時間等詳細資訊。 按一下 **[!UICONTROL 下載]** 以CSV格式下載作業的報告。

   報表中資產的刪除狀態可以具有以下可能值：

   * **已刪除**  — 資產已成功從「貢獻」資料夾中刪除。

   * **未找到** -Brand Portal在「貢獻」資料夾中找不到資產。 資產已手動從資料夾中刪除。

   * **已跳過** -Brand Portal跳過了資產刪除，因為「貢獻」資料夾中有可用於資產的新版本，但尚未發佈到Experience Manager。

   * **失敗** -Brand Portal未能刪除資產。 有三次重試嘗試刪除具有 `Failed` 刪除狀態。 如果資產第三次重試刪除嘗試失敗，則需要手動刪除資產。

### 刪除報表

Brand Portal還允許您選擇一個或多個報告並手動刪除它們。

要刪除報表：

1. 導航到 **[!UICONTROL 工具]**>**[!UICONTROL 資產貢獻狀態]**>**[!UICONTROL 刪除報告]** 的雙曲餘切值。

1. 選擇一個或多個報告，然後按一下 **[!UICONTROL 刪除]**。


