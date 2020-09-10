---
title: 疑難排解平行發佈至 Brand Portal 的問題
seo-title: 疑難排解平行發佈至 Brand Portal 的問題
description: 疑難排解並行發佈。
seo-description: 疑難排解並行發佈。
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
translation-type: tm+mt
source-git-commit: 77555866aaf5185a99b83d94f265ad08ec2b337e
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 2%

---


# 疑難排解平行發佈至 Brand Portal 的問題 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

品牌入口網站已設定AEM Assets，讓核准的品牌資產順暢地從AEM Assets作者例項接收（或發佈）。 設 [定後](../using/configure-aem-assets-with-brand-portal.md),AEM Author會使用複製代理將選取的資產複製至Brand Portal雲端服務，以供Brand Portal使用者核准使用。 AEM 6.2 SP1-CFP5、AEM CFP 6.3.0.2和更新版本都使用多個複製代理，以允許高速並行發佈。

>[!NOTE]
>
>Adobe建議升級至AEM 6.4.1.0，以確保AEM Assets品牌入口網站已成功設定為AEM Assets。 AEM 6.4的限制會在使用品牌入口網站設定AEM資產時顯示錯誤，複製會失敗。

在設定品牌入口網站的雲端服務 **[!UICONTROL /etc/cloudservice下]**，系統會自動產生所有必要的使用者和Token並儲存在儲存庫中。 建立雲服務配置，並建立複製和複製代理複製內容所需的服務用戶。 這將建立四個複製代理。 因此，當您從AEM發佈許多資產至品牌入口網站時，這些資產會排入佇列，並透過「輪流作業」在這些複製代理之間分發。

不過，發佈可能會因為大型sling工作、AEM Author執行個體的Network and **[!UICONTROL Disk I/O]** （網路和磁碟I/O）增加或AEM Author執行個體的效能降低而間歇性失敗。 因此，建議在開始發佈之前測試與複製代理的連接。

![](assets/test-connection.png)

## 疑難排解首次發佈失敗：驗證發佈配置 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

若要驗證您的發佈設定：

1. 檢查錯誤日誌
1. 檢查是否建立了複製代理
1. 測試連線

**建立雲端服務時的尾隨記錄檔**

檢查尾部記錄。 檢查是否建立了複製代理。 如果複製代理建立失敗，請通過對雲服務進行小幅更改來編輯雲服務。 驗證並再次檢查是否建立了複製代理。 否則，請重新編輯服務。

如果重複編輯雲端服務時未正確設定，請報告日托服務票證。

**測試與複製代理的連接**

查看日誌，如果在複製日誌中發現錯誤：

1. 聯絡Adobe支援。

1. 請重 [試清除](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) ，並重新建立發佈設定。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### 清除現有品牌入口網站發佈設定 {#clean-up-existing-config}

發佈時的大部分時間都無法運作，原因可能是發佈使用者(例如： `mac-<tenantid>-replication` 沒有最新的私鑰，因此發佈失敗，出現「401 unauthorized」錯誤，複製代理日誌中未報告其他錯誤。 您可能希望避免疑難排解，並改為建立新的設定。 若要讓新設定正常運作，請從AEM作者設定中清除下列項目：

1. 前往(考 `localhost:4502/crx/de/` 慮您正在localhost:4502上執行作者例項：\
   i.刪除 `/etc/replication/agents.author/mp_replication`ii。 刪除 
`/etc/cloudservices/mediaportal/<config_name>`

1. 前往localhost:4502/useradmin:\
   i.搜索用戶 `mac-<tenantid>replication`ii。 刪除此用戶

現在系統都清理乾淨了。 現在，您可以嘗試建立新的cloudservice組態，並仍然使用https://legacy-oauth.cloud.adobe.io/中現有的JWT應用 [程式](https://legacy-oauth.cloud.adobe.io/)。 您不需要建立新的應用程式，只需從新建立的雲端組態更新公開金鑰。

## 開發人員連線JWT應用程式租用戶可見度問題 {#developer-connection-jwt-application-tenant-visibility-issue}

如果位 [於https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)，則會列出目前使用者持有系統管理員的所有組織（租戶）。 如果您在這裡找不到組織名稱，或者您無法在這裡為必要的租用戶建立應用程式，請檢查您是否擁有足夠的（系統管理員）權限。

此使用者介面有一個已知問題：任何租用戶只能看到前10個應用程式。 當您建立應用程式時，請停留在該頁面上並為URL建立書籤。 您不需要前往應用程式的清單頁面，並尋找您建立的應用程式。 您可以直接點按此書籤化URL，並視需要更新／刪除應用程式。

JWT應用程式可能未正確列出。 因此，建議在建立JWT應用程式時記下URL/為其添加書籤。

## 運行配置停止工作 {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

如果複製代理（發佈到品牌門戶時情況正常）停止處理發佈作業，請檢查複製日誌。 AEM已內建自動重試，因此，如果特定資產發佈失敗，則會自動重試。 如果出現網路錯誤等間歇性問題，則可能會在重試期間成功。

如果連續發佈失敗且佇列遭到封鎖，則應檢查 **[!UICONTROL 測試連線]** ，並嘗試解決所報告的錯誤。

根據錯誤，建議您記錄支援票證，以便品牌入口網站工程團隊協助您解決問題。


## 配置複製代理以避免連接超時錯誤 {#connection-timeout}

如果複製佇列中有多個待審請求，發佈作業通常會失敗並出現逾時錯誤。 要解決此問題，請確保將複製代理配置為避免超時。

執行以下步驟以配置複製代理：
1. 登入您的AEM Assets作者實例。
1. 從「工 **具** 」面板，導覽至「部 **[!UICONTROL 署]** >復 **[!UICONTROL 制」]**。
1. 在「複製」頁中，按一下「作 **[!UICONTROL 者上的代理」]**。 您可以看到您的品牌門戶租用戶的四個複製代理。
1. 按一下複製代理URL以開啟代理詳細資訊。
1. 按一下 **[!UICONTROL 編輯]** ，修改複製代理設定。
1. 在「代理設定」中，按一下「 **[!UICONTROL Extended]** 」頁籤。
1. 選中「關 **[!UICONTROL 閉連接]** 」複選框。
1. 重複步驟4到7 ，以配置所有四個複製代理。
1. 重新啟動伺服器。