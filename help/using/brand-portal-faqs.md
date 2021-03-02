---
title: 常見問題
seo-title: null
description: 深入瞭解Adobe Experience Manager資產品牌入口網站中的常見問題。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 4983e2e160b5cfb213e249f731e1858fab2cf972
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 2%

---


# 常見問題 {#frequently-asked-questions}

品牌入口網站常見問答集主要針對使用者在使用最新的AEM Assets品牌入口網站6.4.6版或更舊版本時可能遇到的查詢和問題。


## 品牌入口網站6.4.6常見問答集{#faqs-bp646}

**客戶。現有的舊式OAuth端點(`https://legacy-oauth.cloud.adobe.io/login`)無法運作。 可能的原因是什麼？**

**Ans。** 舊版OAuth設定已過時。您必須將AEM Assets作者實例升級至最新的Service Pack，並透過Adobe開發人員主控台進行設定。 如需詳細資訊，請參閱[使用品牌入口網站設定AEM Assets。 ](configure-aem-assets-with-brand-portal.md)不過，若要讓舊版OAuth設定在升級前運作，請將舊版OAuth端點更新為`https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**客戶。升級至「Adobe開發人員主控台」後，我無法將貢獻資料夾的資產從品牌入口網站發佈至AEM Assets。 我的作者例項AEM是6.5.4。可能的原因是什麼？**

**Ans。** 是的，透過Adobe開發人員主控台將貢獻資料夾的資產發佈至AEM Assets的AEM6.5.4時，有已知問題。

此問題已在AEM6.5.5中修正。您可以將AEM Assets實例升級至最新的Service Pack AEM 6.5.5和[，以升級Adobe開發人員控制台上的配置](https://docs.adobe.com/content/help/zh-Hant/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。

如需6.AEM5.4的立即修正，建議您下載Hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041)並安裝在您的作AEM者例項上。[

**客戶。我看不到貢獻資料夾的內容，這些內容是從AEM Assets的Brand Portal發佈的。 可能的原因是什麼？**

**Ans。** 請連絡您的AEM Assets管理員以驗證設定，並確保您的品牌入口網站租用戶僅設定一個AEM Assets作者例項。

當您在多個AEM Assets作者例項上設定品牌入口網站租戶時，可能會發生此問題。 例如，管理員在AEM Assets的測試與生產環境作者實例上設定相同的品牌入口租用戶。 在這種情況下，Brand Portal中會觸發資產發佈，但AEM Assets作者實例無法匯入資產coz，複製代理不會收到請求的Token。


**客戶。我無法將資產從AEM Assets發佈至品牌入口網站。 複製日誌表示連接超時。 有快速修正嗎？**

**Ans。** 如果複製佇列中有多個待審請求，發佈通常會失敗並出現逾時錯誤。要解決此問題，請確保將複製代理配置為避免超時。

執行以下步驟以配置複製代理：
1. 登入您的AEM Assets作者實例。
1. 從&#x200B;**工具**&#x200B;面板，導航至&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 複製]**。
1. 在「複製」頁中，按一下&#x200B;**[!UICONTROL 作者上的代理]**。 您可以看到您的品牌門戶租用戶的四個複製代理。
1. 按一下複製代理URL以開啟代理詳細資訊。
1. 按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;以修改複製代理設定。
1. 在「代理設定」中，按一下&#x200B;**[!UICONTROL Extended]**&#x200B;頁籤。
1. 選中&#x200B;**[!UICONTROL 關閉連接]**&#x200B;複選框。
1. 重複步驟4到7 ，以配置所有四個複製代理。
1. 重新啟動伺服器並驗證連接。


## 品牌入口網站6.4.5常見問答集{#faqs-bp645}

**客戶。品牌入口網站6.4.5版的主要變更為何？**

**Ans。** AEM Assets品牌入口網站6.4.5是功能發行，可讓品牌入口網站使用者從品牌入口網站例項內上傳內容，並將貢獻資料夾發佈回AEM Assets，毋需擁有管理員權限。如需詳細資訊，請參閱品牌入口網站中的[資產來源補充](brand-portal-asset-sourcing.md)。



**客戶。我是否會失去對已建立的任何現有資產、功能或組態的存取權？**

**Ans。** 您現有的所有功能和組態都保持不變。您的使用者不受影響，而且您的內容仍保持不變。



**客戶。我何時要移至新版的品牌入口網站？**

**Ans。** 品牌入口網站6.4.5已於2019年10月推出生產。下一個品牌入口網站版本預計將於2020年第3季度推出。
對於更新和版本變更，建議您追蹤[發行說明](brand-portal-release-notes.md)和[品牌入口網站的新增功能](whats-new.md)。



**客戶。我的使用者是否會受到影響？**

**Ans。** 品牌入口網站6.4.5版僅限於品牌入口網站，因此對您的使用者沒有影響。



**客戶。身為品牌入口網站使用者，我需要執行什麼動作？**

**Ans。** Brand Portal 6.4.5版隨附一項名為「資產來源補充」的新功能。管AEM理員必須在AEM Assets設定「資產來源補充」功能，才能為品牌入口網站使用者啟用此功能。 有關詳細資訊，請參閱[啟用資產來源補充](brand-portal-asset-sourcing.md)。



**客戶。誰可以建立貢獻資料夾？**

**Ans。** 任何AEM擁有在AEM Assets建立新資料夾權限的使用者，都可以建立 **** Contribution資料夾。若要建立&#x200B;**Contribution**&#x200B;檔案夾，請建立類型&#x200B;**Asset Contribution**的新檔案夾。
此資料夾會與作用中的品牌入口網站使用者共用，以取得貢獻。



**客戶。「貢獻」資料夾包含哪些內容？**

**Ans。** **Contribution** 資料夾包含兩個子資料 **** 夾NEW **和SHARED**。一開始，NEW檔案夾是空白的，而SHARED檔案夾包含品牌入口網站使用者的參考內容（可重複使用的資產）。
品牌入口網站使用者會存取**Contribution**&#x200B;資料夾，並上傳&#x200B;**NEW**&#x200B;資料夾中的內容。



**客戶。我可以修改現有貢獻資料夾的名稱嗎？**

**Ans。** **否**，您無法修改現有Contribution資料夾的 **** 名稱。



**客戶。什麼是資產需求w.r.t貢獻？**

**Ans。** 附 **** 加至 **** Contribution資料夾的簡報檔案以及 **** SHARED資料夾中上傳的參考內容（可重複使用的資產）可協助品牌入口網站使用者瞭解作為貢獻者的貢獻和期望，並統稱為資產需求。



**客戶。我是否可將資產上傳至任何允許的資料夾？**

**Ans。** 並非所有允許的資料夾。品牌入口網站使用者只能將內容上傳至由或品牌入口網站管理員共用的&#x200B;**貢獻** AEM資料夾。



**客戶。如何存取「貢獻」檔案夾？**

**Ans。** 只有已與您共 **** 用Contribution資料夾時，您才能存取它。每當您共用「貢獻」檔案夾時，都會收到電子郵件／脈衝通知。 您可以透過電子郵件中共用的連結存取「貢獻」檔案夾，或登入您的品牌入口網站例項，並導覽至鈴形圖示，以取得「貢獻」檔案夾的通知。

>[!NOTE]
>
>如果您不是現有的品牌入口網站使用者，請AEM要求管理員在管理主控台中建立您的使用者，並將您的個人檔案新增至品牌入口網站使用者清單中的使用者設定檔案。

**客戶。用戶導入的CSV檔案格式是什麼？**

**Ans。** 其格式與大量使用者匯入Admin Console所支援的格式相同。電子郵件、名字和姓氏是必填的。



**客戶。「資產貢獻」使用者下拉式清單中填入使用者清單（品牌入口網站參與者）的內容？**

**Ans。** 下拉式清單中的使用者會從上傳的品牌入口網站使用者設定(.csv)檔案中填入AEM。



**客戶。我可以在何處查看導入和發佈作業的狀態？**

**Ans。** 在中AEM，您可以在非同步作業頁面中查看導入 **** 的狀態。在品牌入口網站中，您可以在&#x200B;**[!UICONTROL 工具>資產貢獻狀態]**&#x200B;中查看發佈工作的狀態。



**客戶。定期在中運行的導入作業的頻AEM率是多少？**

**Ans。** 投AEM票每5分鐘執行一次。



**客戶。資料夾可從Brand Portal發佈至AEM Assets的次數是否有任何原因？**

**Ans。** 否。  **** NEWfolder中的所有資產都會發佈至AEM Assets，不論這些資產是否在先前發佈。每當&#x200B;**Contribution**&#x200B;資料夾從品牌入口網站發佈至AEM Assets時，它會覆寫&#x200B;**NEW**&#x200B;資料夾的內容。



**客戶。如何上傳「貢獻」檔案夾中的新資產？**

**Ans。** 請參閱上傳資產至貢獻資 [料夾的詳細檔案](brand-portal-publish-contribution-folder-to-brand-portal.md)。



**客戶。品牌入口網站使用者上傳至NEW檔案夾的資產上沒有縮圖／預覽？**

**Ans。** 它如設計般，品牌入口網站端不會執行工作流程。



**客戶。如果資料夾從AEM Assets發佈至動態的品牌入口網站，會發生什麼情況？**

**Ans。** 在中AEM，每次將資料夾發佈至品牌入口網站時，都會保留記錄檔。在發佈時，所有未發佈至品牌入口網站的資產都會放入複製佇列。 觸發發佈工作後新增至資料夾的任何資產都不會發佈至品牌入口網站。 當使用AEM者再次發佈資料夾時，只有先前未發佈的資產（存在於複製佇列中）才會發佈至品牌入口網站。
從AEM Assets發佈至品牌入口網站的任何資料夾，以及貢獻資料夾中的SHARED資料夾，都適用此點。

**客戶。我要與誰聯繫，問題包括：**

**Ans。** 聯絡您的Adobe客戶經理或客戶支援。

>[!NOTE]
>
>發行時間表尚未確定，可能會有所變更。 請連絡您的Adobe客戶經理或客戶支援以取得更新的發行計畫。


## 產品存取與支援（受限制網站）{#product-access-and-support-restricted-sites}

這些網站僅提供給客戶使用。 如果您是客戶並需要存取權，請聯絡您的Adobe客戶經理。

* [](https://daycare.day.com) [產品存取](https://login.marketing.adobe.com)

* [Adobe客戶服務](https://helpx.adobe.com/contact.html)
