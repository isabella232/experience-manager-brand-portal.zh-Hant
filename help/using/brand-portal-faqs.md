---
title: 常見問題
seo-title: null
description: 深入瞭解Adobe Experience Manager Assets品牌入口網站中的常見問題。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ac5952c318baae8400928592d9a372ab966191cf
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---


# 常見問題 {#frequently-asked-questions}

品牌入口網站常見問答集主要針對使用者在使用最新AEM Assets Brand Portal 6.4.6版或更舊版本時可能遇到的查詢和問題。


## 品牌入口網站6.4.6常見問答集  {#faqs-bp646}

**客戶。 現有的舊式OAuth端點(`https://legacy-oauth.cloud.adobe.io/login`)無法運作。 可能的原因是什麼？**

**Ans。** 舊版OAuth設定已過時。 您必須將AEM Assets作者例項升級至最新的Service Pack，並透過Adobe Developer Console加以設定。 如需詳 [細資訊，請參閱「設定AEM資產與品牌入口網站](configure-aem-assets-with-brand-portal.md) 」。 不過，若要讓舊版OAuth設定在升級前運作，請將舊版OAuth端點更新為 `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

**客戶。 升級至Adobe Developer Console後，我無法將貢獻資料夾的資產從品牌入口網站發佈至AEM資產。 我的作者實例位於AEM 6.5.4。 可能的原因是什麼？**

**Ans。** 是的，透過Adobe Developer Console將貢獻資料夾的資產發佈至AEM 6.5.4上的AEM Assets時，有已知問題。

AEM 6.5.5中的問題已修正。 您可以在Adobe Developer Console上將AEM Assets實例升級至最新的Service Pack AEM 6.5.5, [並升級您的組態](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) 。

如需AEM 6.5.4的立即修正，建議您下載 [修補程式](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) ，並安裝在AEM作者實例上。

**客戶。 在AEM Assets中，我看不到從品牌入口網站發佈的貢獻資料夾內容。 可能的原因是什麼？**

**Ans。** 請連絡您的AEM Assets管理員以驗證設定，並確定您的品牌入口網站租用戶僅設定一個AEM Assets作者例項。

當您在多個AEM Assets作者例項上設定品牌入口網站租用戶時，可能會發生此問題。 例如，管理員會在AEM Assets作者執行個體的測試與生產環境上設定相同的品牌入口租用戶。 在此案例中，資產發佈會在Brand Portal中觸發，但AEM Assets作者例項無法匯入資產coz，複製代理程式不會收到請求的Token。


**客戶。 我無法將資產從AEM Assets發佈至品牌入口網站。 複製日誌表示連接超時。 有速效藥嗎？**

**Ans。** 如果複製佇列中有多個待審請求，發佈通常會失敗並出現逾時錯誤。 要解決此問題，請確保將複製代理配置為避免超時。

執行以下步驟以配置複製代理：
1. 登入您的AEM Assets作者實例。
1. 從「工 **具** 」面板，導覽至「部 **[!UICONTROL 署]** >復 **[!UICONTROL 制」]**。
1. 在「複製」頁中，按一下「作 **[!UICONTROL 者上的代理」]**。 您可以看到您的品牌門戶租用戶的四個複製代理。
1. 按一下複製代理URL以開啟代理詳細資訊。
1. 按一下 **[!UICONTROL 編輯]** ，修改複製代理設定。
1. 在「代理設定」中，按一下「 **[!UICONTROL Extended]** 」頁籤。
1. 啟用「關 **[!UICONTROL 閉連接]** 」複選框。
1. 重複步驟4到7 ，以配置所有四個複製代理。
1. 重新啟動伺服器並驗證連接。


## 品牌入口網站6.4.5常見問答集  {#faqs-bp645}

**客戶。 品牌入口網站6.4.5版的主要變更為何？**

**Ans。** AEM Assets Brand Portal 6.4.5是一項功能發行，可讓品牌入口網站使用者從品牌入口網站例項內上傳內容，並將「貢獻」檔案夾發佈回AEM Assets，而不需要管理員權限。
如需詳細資訊，請參 [閱品牌入口網站中的資產來源補充](brand-portal-asset-sourcing.md)。



**客戶。 我是否會失去對已建立的任何現有資產、功能或設定的存取權？**

**Ans。** 您現有的所有功能和組態都保持不變。 您的使用者不受影響，而且您的內容仍保持不變。



**客戶。 我何時要改用新版的Brand Portal?**

**Ans。** 品牌入口網站6.4.5已於2019年10月推出生產。 下一個品牌入口網站版本預計將於2020年第3季度推出。
如需更新和版本變更，建議您追蹤 [版本注意事項](brand-portal-release-notes.md)[和品牌入口網站的新功能](whats-new.md)。



**客戶。 我的使用者是否會受到影響？**

**Ans。** 品牌入口網站6.4.5版僅限於品牌入口網站，因此對您的使用者沒有影響。



**客戶。 身為品牌入口網站使用者，我需要執行什麼動作？**

**Ans。** Brand Portal 6.4.5版隨附一項名為「資產來源補充」的新功能。 AEM管理員必須在AEM Assets中設定「資產來源補充」功能，才能為品牌入口網站使用者啟用此功能。 如需詳細資訊，請參閱「啟 [用資產來源補充](brand-portal-configure-asset-sourcing.md)」。



**客戶。 誰可以建立貢獻資料夾？**

**Ans。** 任何擁有在AEM Assets中建立新檔案夾權限的AEM使用者，都可以建立「貢 **獻** 」檔案夾。 若要建立「貢 **獻** 」檔案夾 **，請建立「資產貢獻」類型的**新檔案夾。
此資料夾會與作用中的品牌入口網站使用者共用，以取得貢獻。



**客戶。 「貢獻」檔案夾包含哪些內容？**

**Ans。** **Contribution** （貢獻）資料夾包含兩個子資 **料夾** NEW **（新）**和SHARED（共用）。 一開始，NEW檔案夾是空白的，而SHARED檔案夾包含品牌入口網站使用者的參考內容（可重複使用的資產）。
品牌入口網站使用者會存取 **Contribution** 檔案夾，並上傳 **NEW檔案夾中的** 內容。



**客戶。  我可以修改現有貢獻資料夾的名稱嗎？**

**Ans。** **否**，您無法修改現有貢獻資料 **夾的** 名稱。



**客戶。 資產需求w.r.t的貢獻為何？**

**Ans。** 附 **加至「貢獻** 」檔案夾的Brief **檔案及上傳至** SHARED **** 檔案夾的參考內容（可重複使用的資產）可協助品牌入口網站使用者瞭解貢獻和期望作為貢獻者的需求，並統稱為資產需求。



**客戶。 我是否可將資產上傳至任何允許的資料夾？**

**Ans。** 並非所有允許的資料夾。 品牌入口網站使用者只能將內容上傳至AEM或 **品牌入口網站** 管理員共用的「貢獻」檔案夾。



**客戶。 如何存取「貢獻」檔案夾？**

**Ans。** 只有已與您共 **用「貢獻** 」資料夾時，您才可以存取它。 每當您共用「貢獻」檔案夾時，都會收到電子郵件／脈衝通知。 您可以透過電子郵件中共用的連結存取「貢獻」檔案夾，或登入您的品牌入口網站例項，並導覽至鈴形圖示，以取得「貢獻」檔案夾的通知。

>[!NOTE]
>
>如果您不是現有的品牌入口網站使用者，請要求AEM管理員在AEM管理控制台中建立您的使用者，並將您的個人檔案新增至品牌入口網站使用者清單中的使用者設定檔案。 請參閱「 [新增品牌入口網站使用者](brand-portal-configure-asset-sourcing.md)」。




**客戶。 使用者匯入的CSV檔案格式為何？**

**Ans。** 格式與Admin Console支援的大量使用者匯入格式相同。 電子郵件、名字和姓氏是必填的。



**客戶。 「資產貢獻」使用者下拉式清單中填入的使用者清單（品牌入口網站參與者）為何？**

**Ans。** 下拉式清單中的使用者會從AEM中上傳的品牌入口網站使用者設定(.csv)檔案中填入。



**客戶。 我可以在哪裡看到匯入和發佈工作的狀態？**

**Ans。** 在AEM中，您可以在非同步工作頁面中看到匯 **入** 的狀態。 在品牌入口網站中，您可以在「工具>資產貢獻」狀態中 **[!UICONTROL 看到發佈工作的狀態]**。



**客戶。 在AEM中定期執行的匯入工作頻率為何？**

**Ans。** 在AEM中，投票每5分鐘執行一次。



**客戶。 資料夾可從品牌入口網站發佈至AEM Assets的次數是否有任何原因？**

**Ans。** 否。 **NEW** Assets檔案夾中的所有資產都會發佈至AEM Assets，不論這些資產先前已發佈的事實為何。 每當從 **Brand Portal發佈** 「貢獻」檔案夾至AEM Assets時，它都會覆寫 **NEW** 檔案夾的內容。



**客戶。 如何上傳「貢獻」檔案夾中的新資產？**

**Ans。** 請參閱上傳資產至貢獻資 [料夾的詳細檔案](brand-portal-upload-assets-to-contribution-folder.md)。



**客戶。 品牌入口網站使用者上傳至NEW檔案夾的資產上沒有縮圖／預覽？**

**Ans。** 它如設計般，品牌入口網站端不會執行工作流程。



**客戶。 如果資料夾從AEM Assets發佈至動態的品牌入口網站，會發生什麼情況？**

**Ans。** 在AEM中，每次將資料夾發佈至品牌入口網站時，都會保留記錄檔。 在發佈時，所有未發佈至品牌入口網站的資產都會放入複製佇列。 觸發發佈工作後新增至資料夾的任何資產都不會發佈至品牌入口網站。 當AEM使用者再次發佈資料夾時，只有先前未發佈的資產（存在於複製佇列中）才會發佈至品牌入口網站。
從AEM Assets發佈至品牌入口網站的任何資料夾，以及「貢獻」資料夾中的SHARED資料夾，都適用此點。



**客戶。 我要與誰聯絡有問題？**

**Ans。** 請聯絡您的Adobe客戶經理或客戶支援。


>[!NOTE]
>
>發行時間表尚未確定，可能會有所變更。 請連絡您的Adobe客戶經理或客戶支援以取得更新的發行計畫。





## 產品存取與支援（受限制的網站） {#product-access-and-support-restricted-sites}

這些網站僅提供給客戶使用。 如果您是客戶且需要存取權，請連絡您的Adobe客戶經理。

* [](https://daycare.day.com) [產品存取](https://login.marketing.adobe.com)

* [Adobe客戶服務](https://helpx.adobe.com/contact.html)
