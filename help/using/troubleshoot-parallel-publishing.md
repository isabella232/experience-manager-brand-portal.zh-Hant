---
title: 疑難排解並行發佈至品牌入口網站的問題
seo-title: 疑難排解並行發佈至品牌入口網站的問題
description: 疑難排解並行發佈。
seo-description: 疑難排解並行發佈。
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_ PERIENCENCENAGER/Brand_ Portal
content-type: 引用
topic-tags: 品牌入口網站
discoiquuid: a4801024-b509-4c51-afd8-e337417 e658 b
translation-type: tm+mt
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# 疑難排解並行發佈至品牌入口網站的問題 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

[!DNL Brand Portal] 支援與AEM [!DNL AEM Assets] Assets作者實例順暢吸收(或發佈)的核准品牌資產整合。[整合後](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)[!DNL AEM] ，Author會使用複製代理程式將選取的資產複製到 [!DNL Brand Portal] 雲端服務，供 [!DNL Brand Portal] 使用者核准。使用 [!DNL AEM 6.2 SP1-CFP5]多個複製代理程式 [!DNL AEM CFP 6.3.0.2]，以及允許高速並行發佈。

>[!NOTE]
>
>Adobe建議升級以確保成功整合AEM [!DNL AEM 6.4.1.0][!DNL AEM Assets Brand Portal] Assets。限制在 [!DNL AEM 6.4] 設定與品牌入口網站和複製的整合失敗時發生錯誤。

在 [!UICONTROL /etc/cloudservice]下為品牌入口網站設定雲端服務時，所有必要的使用者和Token都會自動產生並儲存在儲存庫中。雲端服務設定建立時，也會建立複製和複製代理程式所需的服務使用者，以複製內容。這會建立四個復本代理程式。因此，當您發佈許多資產時，這些資產會透過Roop [!DNL AEM][!DNL Brand Portal]Robin佇列在這些複製代理程式之間。

但是，由於大型投影片工作、提高作者執行個體的「網路和磁碟 [!UICONTROL I/O」] ，或是 [!DNL AEM][!DNL AEM] 「作者」實例的效能變慢，發佈作業偶爾會失敗。因此，建議在開始發佈之前測試與複製代理程式的連線。

![](assets/test-connection.png)

## 第一次發佈失敗時發生故障排除：驗證您的發佈設定 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

驗證您的發佈組態：

1. 檢查錯誤記錄檔
2. 檢查複製代理是否建立
3. 測試連線

**建立雲端服務時**

檢查尾記錄檔。檢查是否建立了複製代理程式。如果複製代理程式建立失敗，請在雲端服務中進行小幅變更以編輯雲端服務。驗證並再次檢查是否建立了複製代理程式。否則，請重新編輯服務。

如果重復編輯該雲端服務未正確設定，請報告日照護票證。

**測試與複製代理程式的連線**

檢視記錄(如果出現在複製記錄中)：

1. 聯絡Adobe支援。

2. 重新嘗試 [清除](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 並重新建立發佈設定。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### 清除現有品牌入口網站發佈設定 {#clean-up-existing-config}

大部分的時候發佈無法運作的使用者，其原因可能是發佈的使用者(mac-&lt; tenand&gt;-replication)沒有最新的私密金鑰，因此發佈失敗，「401未授權」，而不會報告任何其他錯誤，也就是複製代理記錄檔。您可能想要避免疑難排解並建立新設定。為讓新設定正常運作，您應清除AEM作者設定後的下列作業：

1. 前往 [!UICONTROL localhost：4502/crx/de] (假設您正在localhost上 [!UICONTROL 執行author實例：4502])：\
   i刪除 [!UICONTROL /etc/replication/agents.author/mp_replication與#42]；\
   ii刪除 [!UICONTROL /etc/cloudservices/mediaportal/&lt; config_ name&amp; gt]；

2. 前往 [!UICONTROL localhost：4502/usermin]：\
   i search user [!UICONTROL mac-&lt; tenand&gt;-replication]\
   ii刪除此使用者

現在系統全部清理完畢。現在您可以嘗試建立新的雲端服務組態，而且仍可使用現有 [!DNL JWT] 的 [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)。您無需建立新的應用程式，而只需要從新建立的雲端設定更新公開金鑰。

## Developer Connection JWT應用程式租用戶可見度問題 {#developer-connection-jwt-application-tenant-visibility-issue}

如果在 [!UICONTROL https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)上，則列出目前使用者擁有系統管理員的所有組織(租用戶)。如果您在此處找不到組織名稱，或者您無法在此處建立必要的租用戶，請檢查是否有足夠的權限(系統管理員)可執行此動作。

此使用者介面上有一個已知的問題，這個使用者介面只會顯示前10個應用程式。當您建立應用程式時，請留在該頁面並將URL書簽化。您不需要前往應用程式的清單頁面，並尋找您建立的應用程式。您可以直接點擊此書簽化URL，並視需要更新/刪除應用程式。

[!DNL JWT] 應用程式可能無法正確列出。因此，建議您在建立JWT應用程式時記下/建立URL。

## 執行設定停止運作 {#running-configuration-stops-working}

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

如果複製代理程式(這是發佈至品牌入口網站)停止處理發佈工作，請檢查複製記錄檔。[!DNL AEM] 自動重新嘗試內建，因此當特定資產發佈失敗時，會自動重試。如果發生網路錯誤等間歇性問題，在重新嘗試期間可能會成功。

但如果持續發佈失敗，佇列便會被封鎖。然後您應該檢查「測試連線」，並嘗試解決所回報的錯誤。

根據錯誤，建議您記錄支援票證， [!DNL Brand Portal] 讓工程團隊可協助您解決問題。
