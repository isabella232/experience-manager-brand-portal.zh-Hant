---
title: 常見問答
seo-title: null
description: 在 Adobe Experience Manager Assets 品牌入口網站中分析常見問題。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# 常見問答 {#frequently-asked-questions}

品牌入口網站常見問題著重于使用最新 Experience Manager Assets 品牌入口網站6.4.6 發行版本或較早版本時可能遇到的終端使用者查詢和問題。


## Brand Portal6.4.6常見問題  {#faqs-bp646}

**克斯。 現有舊OAuth終結點(`https://legacy-oauth.cloud.adobe.io/login`)不工作。 可能的原因是什麼？**

**安。** 不建議使用舊式OAuth配置。 您必須將Experience Manager Assets作者實例升級到最新的Service Pack，並通過Adobe Developer控制台進行配置。 請參閱 [將Experience Manager Assets配置為Brand Portal](configure-aem-assets-with-brand-portal.md) 的雙曲餘切值。 不過，若要讓舊版 OAuth 設定在升級之前運作，請將舊版 OAuth 端點更新為 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/` 。

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. 升級至 Assets 開發人員主控台後，我無法發佈「貢獻」資料夾的資產從品牌入口網站至 Experience Manager Adobe Systems。 我的作者執行個體位於 Experience Manager Assets 6.5.4 上。可能有什麼原因？**

**自動化.** 是的，發佈貢獻資料夾的資產時，若要透過 Adobe Systems 開發者控制台 Experience Manager Assets 6.5.4，就有一個已知問題。

Experience Manager Assets 6.5.5 已修正此問題。您可以將 Experience Manager Assets 執行個體升級至最新的 service pack，並 [ 在 Adobe Systems 開發人員控制台上升級您 ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 的設定。

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Ques. 在 Experience Manager Assets 中看不到「貢獻」資料夾的品牌入口網站內容。 可能有什麼原因？**

**自動化.** 請聯絡您的 Experience Manager Assets 管理員驗證設定，並確保您的品牌入口網站租戶僅使用一個 Experience Manager Assets author 執行個體。

當您在多個 Experience Manager Assets 作者例上設定品牌入口網站租戶時，可能會發生此問題。 例如，管理員在測試和生產環境的 Experience Manager Assets 作者執行個體上設定相同的品牌入口網站。 在這種情況下，資產發佈品牌入口網站中的觸發器，但 Experience Manager Assets 作者執行個體無法匯入資產 coz。


**Ques. 我無法發佈從 Experience Manager Assets 到品牌入口網站的資產。 複製記錄檔指出連線超時。 是否有快速修正？**

**自動化.** 如果在複製佇列中有多個掛起的請求，發佈通常會失敗並出現逾時錯誤。 若要解決此問題，請確保將複製代理程式設定為避免超時。

執行下列步驟以設定「複製代理」：

1. 登入您的 Experience Manager Assets 作者執行個體。
1. **在工具** 面板中，導覽至 **[!UICONTROL 「部署]** > **[!UICONTROL 」複製]** 。
1. 在「複製頁面中，按一下 **[!UICONTROL 作者]** 的代理。 您可以查看品牌入口網站租戶的四個複製代理程式。
1. 按一下「複製代理」 URL 以開啟代理詳細資料。
1. 按一下 **[!UICONTROL 編輯]** 以修改複製代理程式設定。
1. 在代理設定中，按一下 **[!UICONTROL 擴展]** 頁籤。
1. 選擇 **[!UICONTROL 關閉連接]** 的子菜單。
1. 重複步驟4至7以配置所有四個複製代理。
1. 重新啟動伺服器並驗證連接。


## Brand Portal6.4.5常見問題  {#faqs-bp645}

**克斯。 品牌入口網站6.4.5 發行的主要變更是什麼？**

**自動化.** Experience Manager AssetsBrand Portal6.4.5是一個功能發佈版，它允許Brand Portal用戶從Brand Portal實例內上傳內容，並將貢獻資料夾發佈回Experience Manager Assets，而無需管理員權限。
有關詳細資訊，請參見 [Brand Portal資產來源補充](brand-portal-asset-sourcing.md)。



**克斯。 我是否會失去對我建立的任何現有資產、功能或配置的訪問權限？**

**安。** 所有現有功能和配置都保持不變。 您的終端使用者不受影響，您的內容保持不變。



**Ques. 何時移至新版本的品牌入口網站？**

**自動化.** 2019年10月發行品牌入口網站6.4.5。 而下一品牌入口網站版本預期會在第 3 2020 季度發行。對於更新和版本變更，建議在品牌入口網站中追蹤 [ 版本資訊 ](brand-portal-release-notes.md) 和 [ 新。 ](whats-new.md)



**Ques. 我的用戶會受到影響嗎？**

**安。** Brand Portal6.4.5版僅在Brand Portal內，因此對您的最終用戶沒有影響。



**克斯。 作為Brand Portal用戶，我是否需要執行任何操作？**

**安。** Brand Portal6.4.5版附帶了一個名為「資產來源補充」的新功能。 管理員必須配置Experience Manager Assets的資產採購功能，以便為Brand Portal用戶啟用該功能。 如需詳細資訊，請參閱 [ 啟用資產來源 ](brand-portal-asset-sourcing.md) 。



**Ques. 誰可以建立貢獻資料夾？**

**安。** 任何具有在Experience Manager Assets建立新資料夾權限的Experience Manager Assets用戶都可以 **貢獻** 的子菜單。 建立 **貢獻** 資料夾，建立新類型的資料夾 **資產貢獻**。
此資料夾與活動的Brand Portal用戶共用，以便進行貢獻。



**克斯。 貢獻資料夾包含什麼？**

**自動化.****貢獻** 資料夾包含兩個子資料夾 **新增** 和 **共用** 。最初，新資料夾為空白，共用資料夾包含品牌入口網站使用者的參考內容（可重複使用的資產）。品牌入口網站使用者存取 **貢獻** 資料夾，並在新 **資料夾中** 上傳內容。



**Ques.  我可以修改現有貢獻資料夾的名稱嗎？**

**自動化.** **否**，不能修改現有名稱 **貢獻** 的子菜單。



**克斯。 資產需求與RT的貢獻是什麼？**

**安。** 的 **簡介** 附加到的文檔 **貢獻** 資料夾和上載到 **共用** folder可幫助Brand Portal用戶瞭解作為貢獻者的貢獻和期望的需要，並統稱為資產要求。



**克斯。 我可以上傳資產至任何允許的資料夾嗎？**

**自動化.** 並非所有允許的資料夾。 品牌入口網站用戶僅 **能上傳內容的「貢獻** 」資料夾中，Experience Manager Assets 或品牌入口網站管理員共用。



**Ques. 如何存取貢獻資料夾？**

**自動化.**&#x200B;只有在已與您共用貢獻 **資料夾時，您才能存取** 它。只要共用貢獻資料夾，您就會收到電子郵件/脈衝通知。 您可以透過電子郵件中連結的「共用」來存取「貢獻」資料夾，或登入至您的品牌入口網站執行個體並導覽至 notfication 的鈴聲圖示，以存取貢獻資料夾。

>[!NOTE]
>
>如果您不是現有的品牌入口網站用戶，請請求 Experience Manager Assets 管理員在「管理控制台」中建立您的用戶，並將您的設定檔新增到用戶使用者品牌入口網站中的清單設定檔中。

**Ques. 用戶匯入的 CSV 檔案格式如何？**

**自動化.** 格式與大量用戶匯入的 Admin Console 支援相同。 必須填寫電子郵件、姓氏和姓氏。



**Ques. 什麼是在「資產貢獻用戶」下拉式清單中填入使用者（品牌入口網站貢獻者）的清單？**

**自動化.** 下拉式清單中的使用者會從 Experience Manager Assets 中上載的品牌入口網站用戶設定（.csv）檔案中填入。



**Ques. 我可以在何處看到匯入和發佈工作的狀態？**

**自動化.**&#x200B;在 Experience Manager Assets 中，您可以在非同步 **工作頁面中查看匯入** 的狀態。在品牌入口網站中，您可以在工具 > 資產貢獻狀態 ]**中**[!UICONTROL  查看發佈工作的狀態。



**Ques. 在 Experience Manager 中週期性執行的匯入工作頻率是什麼？**

**自動化.** 在 Experience Manager Assets 中，輪詢的每5分鐘執行一次。



**Ques. 資料夾可從品牌入口網站發佈到 Experience Manager Assets 的次數是否有 threashold？**

**自動化.** 不，所有資產 **新建** 資料夾將發佈到Experience Manager Assets，而不管其早先發佈。 每次a **貢獻** 資料夾從Brand Portal發佈到Experience Manager Assets，它會覆蓋 **新建** 的子菜單。



**克斯。 如何在「貢獻」資料夾中上載新資產？**

**安。** 請參閱詳細文檔，瞭解 [正在將資產上載到貢獻資料夾](brand-portal-publish-contribution-folder-to-brand-portal.md)。



**克斯。 我看不到由Brand Portal用戶上載到NEW資料夾的資產的縮略圖/預覽？**

**自動化.** 其設計方式如下： coz 不會在品牌入口網站結尾執行工作流程。



**Ques. 如果資料夾從 Experience Manager Assets 發佈至 flux 中的品牌入口網站會發生什麼事？**

**自動化.** 在 Experience Manager Assets 中，每次發佈資料夾至品牌入口網站時，都會維護記錄。 發佈時，所有未發佈到品牌入口網站的資產都放在一個複製佇列中。 觸發發佈工作後新增至資料夾的任何資產都不會發佈到品牌入口網站。 當 Experience Manager Assets 用戶再次發佈檔案夾時，只會發佈先前未發佈的資產（現有的複製佇列）。這適用于從 Experience Manager Assets 到品牌入口網站，以及在貢獻資料夾中共用資料夾的任何檔案夾。

**Ques. 我該如何聯絡問題？**

**自動化.** 請聯絡您的 Adobe Systems 帳戶管理員或客戶支援。

>[!NOTE]
>
>發行計畫為暫定，可能會變更。 請聯絡您的 Adobe Systems 客戶經理或客戶支援以取得更新的發行排程。


## 產品訪問和支援（受限站點） {#product-access-and-support-restricted-sites}

這些站點僅可供客戶使用。 如果您是客戶並需要訪問，請與Adobe客戶經理聯繫。

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
