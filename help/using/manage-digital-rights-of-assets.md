---
title: 管理資產數位版權
seo-title: 管理資產數位版權
description: 授權資產及設定資產和共用連結的有效期，可確保控制這些資產的使用情況並保護這些資產。
seo-description: 授權資產及設定資產和共用連結的有效期，可確保控制這些資產的使用情況並保護這些資產。
uuid: ce30e398-0109-41fb-a4 d2-2fcca476 f499
contentOwner: bdhar
topic-tags: 下載安裝
products: SG_ PERIENCENCENAGER/Brand_ Portal
content-type: 引用
discoiquuid: f77003ba-31Fe-4a9e-96c8-dbc4 c2 ea79 e
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 管理資產數位版權 {#manage-digital-rights-of-assets}

確保資產的安全發佈與使用，以及品牌材料的使用對於保護品牌的安全至關重要。這可在組織內外執行，並將核准資產與從AEM發佈到品牌入口網站的核准資產相關聯，或是授權這些資產以供條件使用。此外，品牌入口網站可讓您指定連結至從品牌入口網站共用之資產的連結。

瞭解如何在品牌入口網站上確保資產安全，並瞭解相關的使用權限。

## 資產過期 {#asset-expiration}

資產過期是控制在組織內部品牌入口網站上使用核准資產的有效方式。從AEM Assets發佈至品牌入口網站的所有資產都可以擁有到期日，限制不同使用者角色的使用這些資產。

### 過期資產相關的使用權限 {#usage-permissions-expired-assets}

在品牌入口網站中，管理員可以檢視、下載並新增過期資產至系列。此外，編輯和檢視者只能檢視並新增過期資產至系列。

管理員可以將過期資產從AEM Assets發佈至品牌入口網站。不過，過期的資產無法透過品牌入口網站透過油墨共用。如果您從包含過期和非過期資產的資料夾中選取任何過期資產，則無法使用 **[!UICONTROL 「共用連結]** 」動作。但是，如果您選取包含過期和非過期資產的資料夾，則可使用 [!UICONTROL 「共用] 」和 **[!UICONTROL 「共用連結]** 」動作。

>[!NOTE]
>
>資料夾仍然可以共用為連結，即使它包含過期的資產亦然。在此情況下，連結不會列出過期的資產，只會共用非過期的資產。

下表顯示過期資產的使用權限：

|  | **[!UICONTROL 連結共用]** | **[!UICONTROL 下載]** | **[!UICONTROL 屬性]** | **[!UICONTROL 新增至系列]** | **[!UICONTROL 刪除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理員]** | 無法使用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 編輯者]** | 無法使用 | 無法使用 | 可用 | 可用 | 無法使用 |
| **[!UICONTROL 檢視器]** | 無法使用 | 無法使用 | 可用 | 可用 | 無法使用 |
| **[!UICONTROL 來賓使用者]** | 無法使用 | 無法使用 | 可用 | 可用 | 無法使用 |

>[!NOTE]
>
>如果檢視器和編輯器下載包含過期和非過期資產的資料夾，則只會下載非過期的資產。如果資料夾僅包含過期的資產，則會下載空白資料夾。

### 資產的過期狀態 {#expiration-status-of-assets}

您可以在 [!UICONTROL 其「卡片檢視]」中檢視資產的過期狀態。卡片上的紅色標幟表示資產已過期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>清單和欄檢視不會顯示資產的過期狀態。

## 資產連結有效期 {#asset-link-expiration}

在透過連結共用資產時，管理員和編輯可以使用「連結共用」對話框中的 **[!UICONTROL 「過期」]** 欄位來設定到期日 **[!UICONTROL 和過期]** 時間。連結的預設有效期是從共用連結的日期開始七天。

![](assets/asset-link-sharing.png)

它可確保共用時共用的資產在Brand Portal管理員和編輯人員所設定的日期和時間到期，且無法再在到期日之外檢視和下載。由於共用透過連結共用的資產也可以由不屬於組織的外部使用者檢視，借由指定有效期，您可以確定已核准的資產受到保護，且不會在指定的時間暴露於未知實體。

如需連結共用的詳細資訊，請參閱 [共用資產作為連結](../using/brand-portal-link-share.md)。

## 授權資產 {#licensed-assets}

授權資產必須先接受授權合約才能從品牌入口網站下載。此授權資產的合約將於您直接從品牌入口網站或透過共用連結下載資產時取得。無論過期與否，都可以由所有使用者檢視受授權保護的資產。但是，已過期授權資產的下載和使用有限。若要瞭解已過期之授權資產的行為以及根據使用者角色的權限活動，請參閱過期資產 [的使用權限](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)。

受授權保護的資產具有 [附加的授權合約，可透過在AEM](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) Assets中設定資產 [中繼資料屬性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) 來完成。

如果您選擇下載受授權保護的資產，則會重新導向 [!UICONTROL 至「版權管理] 」頁面。

![](assets/asset-copyright-mgmt.png)

在這裡，您需要選取資產以下載並接受相關的授權合約。如果您不接受授權合約，則無法啓用 [!UICONTROL 「下載] 」按鈕。

![](assets/licensed-asset-download-2.png)

如果選取範圍包含多個受保護資產，請一次選取一個資產、接受授權合約，然後繼續下載資產。

## 產生過期資產的報告 {#generate-report-about-expired-assets}

管理員可以產生並下載報告，列出所有在特定時間範圍內過期的資產。此報表包含詳細資訊，例如大小、類型、指定資產階層中資產位置的路徑、資產過期時間，以及發佈資產的時機(關於過期的資產)。可自訂此報表欄，以根據使用者需求顯示更多資料。

![](assets/assets-expired.png)

如需報表功能的詳細資訊，請參閱 [「使用報表](../using/brand-portal-reports.md#work-with-reports)」。
