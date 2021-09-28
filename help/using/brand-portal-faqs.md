---
title: 常見問題
seo-title: null
description: 深入了解Adobe Experience Manager Assets Brand Portal中的常見問題。
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: d7dbf9ae2d27dda2edb60d8f861e618fb6332ec7
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# 常見問題 {#frequently-asked-questions}

Brand Portal常見問題集著重於使用最新AEM Assets Brand Portal 6.4.6版或更舊版本時，一般使用者可能會遇到的查詢和問題。


## Brand Portal 6.4.6常見問題集  {#faqs-bp646}

**是的。現有的舊版OAuth端點(`https://legacy-oauth.cloud.adobe.io/login`)無法運作。 可能的原因是什麼？**

**安。** 舊版OAuth設定已淘汰。您必須將AEM Assets製作執行個體升級至最新的Service Pack，並透過Adobe開發人員控制台進行設定。 如需詳細資訊，請參閱[使用Brand Portal設定AEM Assets](configure-aem-assets-with-brand-portal.md) 。 不過，若要讓舊版OAuth設定在升級前一直有效，請將舊版OAuth端點更新為`https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`。

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**是的。升級至「Adobe開發人員控制台」後，我無法將貢獻資料夾的資產從Brand Portal發佈至AEM Assets。 我的作者例項位於AEM 6.5.4。可能的原因為何？**

**安。** 是的，透過「Adobe開發人員控制台」，在AEM 6.5.4上將貢獻資料夾的資產發佈至AEM Assets時，有一個已知問題。

此問題已在AEM 6.5.5中修正。您可以將AEM Assets執行個體升級至最新的Service Pack AEM 6.5.5和[升級Adobe開發人員主控台上的設定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65)。

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**是的。我沒有看到從AEM Assets中的Brand Portal發佈的貢獻資料夾內容。 可能的原因是什麼？**

**安。** 請連絡您的AEM Assets管理員以驗證設定，並確認您的Brand Portal租用戶僅設定一個AEM Assets製作例項。

若您在多個Brand Portal製作執行個體上設定了AEM Assets租用戶，就可能會發生此問題。 例如，管理員會在測試和生產環境的AEM Assets製作例項上設定相同的Brand Portal租用戶。 在此情況下，Brand Portal會觸發資產發佈，但AEM Assets製作例項無法匯入資產coz，復寫代理程式不會收到要求的代號。


**是的。我無法將資產從AEM Assets發佈至Brand Portal。 復寫記錄會指出連線逾時。 有快速修復嗎？**

**安。** 如果復寫佇列中有多個待處理請求，發佈通常會因逾時錯誤而失敗。若要解決此問題，請確定復寫代理已設定為避免逾時。

執行下列步驟來配置復寫代理：

1. 登入您的AEM Assets製作例項。
1. 從&#x200B;**工具**&#x200B;面板，導覽至&#x200B;**[!UICONTROL 部署]** > **[!UICONTROL 復寫]**。
1. 在「復寫」頁面中，按一下「作者上的代理」**[!UICONTROL 。]**&#x200B;您可以看到Brand Portal租用戶的四個復寫代理。
1. 按一下復寫代理URL以開啟代理詳細資訊。
1. 按一下&#x200B;**[!UICONTROL 編輯]**&#x200B;以修改複製代理設定。
1. 在「代理設定」中，按一下&#x200B;**[!UICONTROL Extended]**&#x200B;頁簽。
1. 選中&#x200B;**[!UICONTROL 關閉連接]**&#x200B;複選框。
1. 重複步驟4到7以配置所有四個複製代理。
1. 重新啟動伺服器並驗證連接。


## Brand Portal 6.4.5常見問題集  {#faqs-bp645}

**是的。Brand Portal 6.4.5版有何重大變更？**

**安。** AEM Assets Brand Portal 6.4.5是功能版本，可讓Brand Portal使用者從Brand Portal執行個體內上傳內容，並將「貢獻」資料夾發佈回AEM Assets，而不需要管理員權限。如需詳細資訊，請參閱[Brand Portal中的Asset Sourcing](brand-portal-asset-sourcing.md)。



**是的。我是否會失去已建立之任何現有資產、功能或設定的存取權？**

**安。** 您現有的所有功能和設定都保持不變。您的使用者不受影響，您的內容會保持不變。



**是的。何時要改用新版Brand Portal?**

**安。** Brand Portal 6.4.5已於2019年10月正式發行。下一個Brand Portal版本預計於2020年第3季度發行。
若為更新和版本變更，建議您追蹤[發行說明](brand-portal-release-notes.md)和[Brand Portal的新增功能](whats-new.md)。



**是的。我的使用者是否會受到影響？**

**安。** Brand Portal 6.4.5版僅限Brand Portal內部使用，因此對您的使用者沒有影響。



**是的。身為Brand Portal使用者，我是否需要執行任何動作？**

**安。** Brand Portal 6.4.5版隨附名為Asset Sourcing的新功能。AEM管理員必須在AEM Assets中設定Asset Sourcing功能，才能為Brand Portal使用者啟用此功能。 如需詳細資訊，請參閱[啟用資產來源補充](brand-portal-asset-sourcing.md)。



**是的。誰可以建立貢獻資料夾？**

**安。** 任何AEM使用者只要有權在AEM Assets中建立新資料夾，都可以建立「貢獻」 **** 資料夾。若要建立&#x200B;**貢獻**&#x200B;資料夾，請建立類型&#x200B;**資產貢獻**的新資料夾。
此資料夾會與作用中的Brand Portal使用者共用以供貢獻。



**是的。貢獻資料夾包含什麼？**

**安。** **** 貢獻資料夾包含兩個子資料 **** 夾NEW **和SHARED**。NEW資料夾一開始為空白，而SHARED資料夾包含Brand Portal使用者的參考內容（可重複使用的資產）。
Brand Portal使用者會存取**Contribution**&#x200B;資料夾，並上傳&#x200B;**NEW**&#x200B;資料夾中的內容。



**是的。我可以修改現有「貢獻」資料夾的名稱嗎？**

**安。** **否**，您無法修改現有Contribution資料夾的 **** 名稱。



**是的。w.r.t貢獻的資產需求為何？**

**安。** 附加 **** 至貢獻資料夾的簡 **** 要檔案以及上傳至SHARED資料夾的參考內容(可重複使用的資 **** 產)，可協助Brand Portal使用者了解貢獻與期望作為貢獻者的需求，並統稱為資產需求。



**是的。我可以將資產上傳至任何允許的資料夾嗎？**

**安。** 並非所有允許的資料夾。Brand Portal使用者只能將內容上傳至AEM或Brand Portal管理員共用的&#x200B;**貢獻**&#x200B;資料夾。



**是的。如何存取貢獻資料夾？**

**安。** 只有在已與 **** 您共用貢獻資料夾時，才可以存取該資料夾。每當貢獻資料夾與您共用時，您會收到電子郵件/脈衝通知。 您可以透過電子郵件中共用的連結存取「貢獻」資料夾，或登入您的Brand Portal例項，並導覽至鈴聲圖示，以取得存取「貢獻」資料夾的通知。

>[!NOTE]
>
>如果您不是現有的Brand Portal使用者，請要求AEM管理員在AEM Admin Console中建立您的使用者，並將您的設定檔新增至Brand Portal使用者清單中的使用者設定檔。

**是的。用戶導入的CSV檔案格式是什麼？**

**安。** 格式與大量使用者匯入Admin Console支援的格式相同。電子郵件、名字和姓氏是必填欄位。



**是的。什麼會填入「資產貢獻者」使用者下拉式清單中的使用者清單(Brand Portal貢獻者)?**

**安。** 下拉式清單中的使用者會從AEM中上傳的Brand Portal使用者設定(.csv)檔案填入。



**是的。在哪裡可以看到導入和發佈作業的狀態？**

**安。** 在AEM中，您可以在非同步作業頁面中查看匯 **** 入的狀態。在Brand Portal中，您可以在&#x200B;**[!UICONTROL 工具>資產貢獻狀態]**&#x200B;中查看發佈工作的狀態。



**是的。在AEM中定期運行的導入作業的頻率是多少？**

**安。** 在AEM中，輪詢每5分鐘執行一次。



**是的。資料夾可從Brand Portal發佈到AEM Assets的次數是否有任何保留？**

**安。** 否，無論先前發佈的 **** 事實為何，NEW資料夾中的所有資產都會發佈至AEM Assets。每次從Brand Portal發佈&#x200B;**貢獻**&#x200B;資料夾至AEM Assets時，它都會覆寫&#x200B;**NEW**&#x200B;資料夾的內容。



**是的。如何上傳「貢獻」資料夾中的新資產？**

**安。** 請參閱上傳資產至貢獻 [資料夾的詳細檔案](brand-portal-publish-contribution-folder-to-brand-portal.md)。



**是的。我在Brand Portal使用者上傳至NEW資料夾的資產上沒有看到縮圖/預覽？**

**安。** 如此一來，Brand Portal端就不會執行任何工作流程。



**是的。如果從AEM Assets發佈資料夾至流量中的Brand Portal，會發生什麼事？**

**安。** 在AEM中，每次將資料夾發佈至Brand Portal時，都會維護記錄。發佈時，所有未發佈至Brand Portal的資產都會放入復寫佇列。 觸發發佈工作後新增至資料夾的任何資產都不會發佈至Brand Portal。 當AEM使用者再次發佈資料夾時，只有先前未發佈的資產（存在於復寫佇列中）才會發佈至Brand Portal。
從AEM Assets發佈至Brand Portal的任何資料夾，以及「貢獻」資料夾內的「共用」資料夾，都會符合此條件。

**是的。我該聯繫誰以回答問題？**

**安。** 請連絡您的Adobe客戶經理或客戶支援。

>[!NOTE]
>
>發行時間表是暫時性的，可能會有所變更。 請連絡您的Adobe客戶經理或客戶支援，以取得更新的發行排程。


## 產品存取與支援（受限網站） {#product-access-and-support-restricted-sites}

這些網站僅供客戶使用。 如果您是Adobe，需要存取權，請聯絡您的客戶經理。

* [](https://daycare.day.com) [產品存取](https://login.marketing.adobe.com)

* [Adobe客戶服務](https://helpx.adobe.com/contact.html)
