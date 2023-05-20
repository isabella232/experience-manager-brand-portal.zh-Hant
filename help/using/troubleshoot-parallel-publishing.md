---
title: 疑難排解平行發佈至 Brand Portal 的問題
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: 排除並行發佈故障。
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: 72cd0ebbf05067287d94e1dc4e1b68f5fb6c2888
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 1%

---

# 疑難排解平行發佈至 Brand Portal 的問題 {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal配置Experience Manager Assets，以無縫接收（或發佈）Experience Manager Assets作者實例的經批准的品牌資產。 一次 [配置](../using/configure-aem-assets-with-brand-portal.md),Experience Manager作者使用複製代理將所選資產複製到Brand Portal雲服務，供Brand Portal用戶使用。 使用多個複製代理Experience Manager6.2 SP1-CFP5、Experience ManagerCFP 6.3.0.2和以後，以允許高速並行發佈。

>[!NOTE]
>
>Adobe建議升級為6.4.1.0Experience Manager，以確保Experience Manager AssetsBrand Portal成功配置Experience Manager Assets。 Experience Manager6.4的限制在配置Experience Manager Assets為Brand Portal時出錯，複製失敗。

Brand Portal雲服務配置 **[!UICONTROL /etc/cloudservice]**，所有必需的用戶和令牌都將自動生成並保存到儲存庫中。 建立雲服務配置，還建立複製代理和複製代理複製內容所需的服務用戶。 它建立四個複製代理。 因此，當您發佈從Experience Manager到Brand Portal的大量資產時，這些資產將通過Round Robin排隊並分發到複製代理中。

但是，發佈可能會因為大型吊帶作業、網路增加和 **[!UICONTROL 磁碟I/O]** Experience Manager作者實例，或減慢Experience Manager作者實例的效能。 因此，建議在開始發佈之前test與複製代理的連接。

![](assets/test-connection.png)

## 首次發佈中的故障排除：驗證發佈配置 {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

要驗證發佈配置：

1. 檢查錯誤日誌
1. 檢查是否建立了複製代理
1. Test連接

**建立尾日誌時的Cloud Service**

檢查尾部日誌。 檢查是否建立了複製代理。 如果複製代理建立失敗，請通過對雲服務進行微小更改來編輯雲服務。 驗證並再次檢查是否建立了複製代理。 否則，請重新編輯服務。

如果重複編輯雲服務時未正確配置，請報告日托票證。

**Test與複製代理的連接**

查看日誌，如果在複製日誌中發現錯誤：

1. 聯繫客戶支援。

1. 重試 [清理](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) 並再次建立發佈配置。

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## 清理現有Brand Portal發佈配置 {#clean-up-existing-config}

大多數發佈不起作用的時候，原因可能是發佈的用戶(例如： `mac-<tenantid>-replication` 沒有最新的私鑰，因此發佈失敗，出現「401 unauthed」錯誤，並且複製代理日誌中未報告其他錯誤。 您可能希望避免故障排除並改為建立配置。 要使新配置正常工作，請從Experience Manager作者設定中清除以下內容：

1. 轉到 `localhost:4502/crx/de/` (考慮到您正在localhost上運行作者實例:4502:\
   我。刪除 `/etc/replication/agents.author/mp_replication`
二。 刪除 
`/etc/cloudservices/mediaportal/<config_name>`

1. 轉到localhost:4502/useradmin:\
   我。搜索用戶 `mac-<tenantid>replication`
二。 刪除此用戶

現在系統已全部清理完畢。 現在，您可以嘗試建立雲服務配置，但仍使用現有的JWT應用程式。 無需建立應用程式，而是從新建立的雲配置中更新公鑰。

>[!NOTE]
>
>不要修改任何自動生成的設定。


## 開發人員連接JWT應用程式租戶可見性問題 {#developer-connection-jwt-application-tenant-visibility-issue}

如果開啟 `https://legacy-oauth.cloud.adobe.io/`，列出當前用戶擁有系統管理員的所有組織（租戶）。 如果在此處找不到組織名稱，或者無法在此處為所需租戶建立應用程式，請檢查您是否具有足夠的（系統管理員）權限。

此用戶介面上存在一個已知問題，即對於任何租戶，只有前十個應用程式可見。 建立應用程式時，請保留在該頁面上，並將URL加入書籤。 您無需轉到應用程式的清單頁並查找您建立的應用程式。 您可以直接點擊此書籤的URL，並在需要時更新/刪除應用程式。

JWT應用程式可能未正確列出。 因此，建議在建立JWT應用程式時記錄/書籤URL。

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

如果複製代理(正在向Brand Portal發佈)停止處理發佈作業，請檢查複製日誌。 Experience Manager具有自動重試內置功能，因此，如果特定資產發佈失敗，將自動重試。 如果出現網路錯誤等間歇性問題，則在重試期間可能會成功。

如果連續發佈失敗且隊列被阻止，則應檢查 **[!UICONTROL test連接]** 並嘗試解決所報告的錯誤。

根據錯誤，建議您記錄支援票證，以便Brand Portal工程團隊可以幫助您解決問題。

## Brand PortalIMS配置令牌已過期 {#token-expired}

如果您的Brand Portal環境突然停止，則IMS配置有可能無法正常工作。 系統顯示不正常的IMS配置，並反映出訪問令牌已過期的錯誤消息（類似於以下內容）。

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

要解決此問題，建議手動保存並關閉IMS配置，並再次檢查運行狀況。 如果配置不起作用，請刪除現有配置並建立新配置。


## 配置複製代理以避免連接超時錯誤 {#connection-timeout}

通常，如果複製隊列中存在多個掛起請求，則發佈作業將失敗並出現超時錯誤。 要解決此問題，請確保將複製代理配置為避免超時。

配置複製代理：

1. 登錄到您的AEM Assets作者實例。
1. 從 **工具** 面板，導航至 **[!UICONTROL 部署]** > **[!UICONTROL 複製]**。
1. 在「複製」頁中，按一下 **[!UICONTROL 作者代理]**。 您可以看到您的Brand Portal租戶的四個複製代理。
1. 按一下複製代理URL，然後按一下 **[!UICONTROL 編輯]**。
1. 在代理設定中，按一下 **[!UICONTROL 擴展]** 頁籤。
1. 選擇 **[!UICONTROL 關閉連接]** 的子菜單。
1. 重複步驟4至7以配置所有四個複製代理。
1. 重新啟動伺服器。
