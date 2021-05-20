---
title: 管理資產的數位版權
seo-title: 管理資產的數位版權
description: 為資產授權並為資產和共用連結設定到期日，可確保對這些資產的使用受到控制並予以保護。
seo-description: 為資產授權並為資產和共用連結設定到期日，可確保對這些資產的使用受到控制並予以保護。
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Administrator
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 2%

---

# 管理資產的數位版權 {#manage-digital-rights-of-assets}

確保創意資產和品牌資料的安全分發和使用對保護您的品牌至關重要。 您可以將到期日（和時間）與從AEM發佈至Brand Portal的已核准資產建立關聯，或將這些資產授權以供條件性使用，借此在組織內外強制執行此作業。 此外，Brand Portal也可讓您指定從Brand Portal共用之資產的連結到期日。

請閱讀下文，了解資產在Brand Portal上的安全性，並了解相關的使用權限。

## 資產到期日{#asset-expiration}

資產過期是控制整個組織在Brand Portal上使用已核准資產的有效方式。 從AEM Assets發佈至Brand Portal的所有資產都可能有到期日，這會限制不同使用者角色使用這些資產。

### 與過期資產相關的使用權限{#usage-permissions-expired-assets}

在Brand Portal中，管理員可以檢視、下載過期的資產，以及將其新增至集合。 但是，編輯器和檢視器只能檢視過期的資產，並將其新增至集合。

管理員可將過期的資產從AEM Assets發佈至Brand Portal。 不過，過期的資產無法透過Brand Portal的連結來共用。 如果您從同時包含過期和未過期資產的資料夾中選取任何過期資產，將無法使用&#x200B;**[!UICONTROL 共用連結]**&#x200B;動作。 但是，如果您選取包含過期和未過期資產的資料夾，則可使用[!UICONTROL 共用]和&#x200B;**[!UICONTROL 共用連結]**&#x200B;動作。

>[!NOTE]
>
>即使資料夾包含過期的資產，該資料夾仍可以作為連結共用。 在此情況下，連結不會列出過期的資產，而只會共用未過期的資產。

下表顯示過期資產的使用權限：

|  | **[!UICONTROL 連結共用]** | **[!UICONTROL 下載]** | **[!UICONTROL 屬性]** | **[!UICONTROL 新增至集合]** | **[!UICONTROL 刪除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理員]** | 不可用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 編輯者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 檢視者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 來賓用戶]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |

>[!NOTE]
>
>如果檢視器與編輯器下載包含過期和未過期資產的資料夾，則只會下載未過期的資產。 如果資料夾只包含過期的資產，則會下載空白資料夾。

### 資產的到期狀態{#expiration-status-of-assets}

您可以在資產的&#x200B;**[!UICONTROL 卡片檢視]**&#x200B;中檢視資產的到期狀態。 卡片上的紅色標幟表示資產已過期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>清單和欄檢視不會顯示資產的到期狀態。

## 資產連結過期{#asset-link-expiration}

透過連結共用資產時，管理員和編輯人員可以使用&#x200B;**[!UICONTROL 連結共用]**&#x200B;對話方塊中的&#x200B;**[!UICONTROL 過期]**&#x200B;欄位，設定到期的日期和時間。 連結的預設過期時間為從共用連結的日期起七天。

![](assets/asset-link-sharing.png)

它可確保以連結形式共用的資產在Brand Portal管理員和編輯人員設定的日期和時間過期，且在過期後無法再檢視和下載。 由於非組織成員的外部使用者也可以檢視透過連結共用的資產，因此指定到期日後，您就可以確定已核准的資產受到保護，且不會在指定時間後暴露給未知的實體。

如需連結共用的詳細資訊，請參閱[以連結形式共用資產](../using/brand-portal-link-share.md)。

## 授權資產{#licensed-assets}

授權資產須先接受授權合約，再從Brand Portal下載。 授權資產的此合約會在您直接從Brand Portal或透過共用連結下載資產時提供。 無論過期與否，所有使用者都可檢視受授權保護的資產。 不過，過期授權資產的下載和使用有限。 若要根據使用者角色了解過期授權資產的行為以及允許的活動，請參閱過期資產的使用權限[。](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)

受授權規範的資產會附加[授權合約](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)，您可在AEM Assets中設定資產的[中繼資料屬性](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets)，完成此作業。

如果您選擇下載受授權保護的資產，系統會將您重新導向至&#x200B;**[!UICONTROL 版權管理]**&#x200B;頁面。

![](assets/asset-copyright-mgmt.png)

您需要在此選取要下載的資產，並接受相關的授權合約。 如果您不接受許可協定，則&#x200B;**[!UICONTROL Download]**&#x200B;按鈕將不啟用。

![](assets/licensed-asset-download-2.png)

如果選取項目包含多個受保護的資產，請一次選取一個資產、接受授權合約，然後繼續下載資產。

## 產生關於過期資產的報表{#generate-report-about-expired-assets}

管理員可產生並下載報表，列出特定時間範圍內到期的所有資產。 此報表包含有關過期資產的詳細資訊，例如大小、類型、在資產階層中指定資產位置的路徑、資產過期的時間，以及資產發佈的時間。 此報表的欄可自訂，以根據使用者需求顯示更多資料。

![](assets/assets-expired.png)

如需報表功能的詳細資訊，請參閱[使用報表](../using/brand-portal-reports.md#work-with-reports)。
