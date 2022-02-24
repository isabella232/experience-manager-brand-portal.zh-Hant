---
title: 管理資產的數位版權
seo-title: Manage digital rights of assets
description: 授權資產和設定資產和共用連結的到期可確保對這些資產的受控使用並保護它們。
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# 管理資產的數位版權 {#manage-digital-rights-of-assets}

確保創意資產和品牌材料的安全分發和使用對保護您的品牌至關重要。 通過將到期日（和時間）與從Brand Portal發佈到的已批准資產相關聯，或通過授權這些資產以便有條件地使用，可以在整個組織和外部AEM強制執行此操作。 此外，Brand Portal還允許您指定從Brand Portal共用的資產連結的到期日期。

閱讀以瞭解如何在Brand Portal保護資產並瞭解相關的使用權限。

## 資產到期 {#asset-expiration}

資產到期是控制整個組織在Brand Portal使用批准資產的有效方法。 從AEM Assets發佈到Brand Portal的所有資產都可以具有到期日期，這將限制不同用戶角色對這些資產的使用。

### 與過期資產相關的使用權限 {#usage-permissions-expired-assets}

在Brand Portal，管理員可以查看、下載過期資產並將其添加到集合中。 但是，編輯和查看者只能查看過期資產並將其添加到收藏。

管理員可以將過期資產從AEM Assets發佈到Brand Portal。 但是，過期資產不能通過Brand Portal的墨水共用。 如果從包含過期資產和非過期資產的資料夾中選擇任何過期資產， **[!UICONTROL 共用連結]** 操作不可用。 但是，如果您選擇包含過期和未過期資產的資料夾， [!UICONTROL 共用] 和 **[!UICONTROL 共用連結]** 操作可用。

>[!NOTE]
>
>即使資料夾包含過期資產，仍可以將其作為連結共用。 在這種情況下，連結不列出過期資產，並且僅共用未過期資產。

下表顯示過期資產的使用權限：

|  | **[!UICONTROL 連結共用]** | **[!UICONTROL 下載]** | **[!UICONTROL 屬性]** | **[!UICONTROL 添加到集合]** | **[!UICONTROL 刪除]** |
|---|---|---|---|---|---|
| **[!UICONTROL 管理員]** | 不可用 | 可用 | 可用 | 可用 | 可用 |
| **[!UICONTROL 編輯者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 檢視者]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |
| **[!UICONTROL 來賓用戶]** | 不可用 | 不可用 | 可用 | 可用 | 不可用 |

>[!NOTE]
>
>如果查看者和編輯下載包含過期和未過期資產的資料夾，則只下載未過期資產。 如果資料夾僅包含過期資產，則會下載空資料夾。

### 資產的到期狀態 {#expiration-status-of-assets}

您可以查看其中資產的到期狀態 **[!UICONTROL 卡視圖]**。 卡上的紅色標誌表示資產已過期。

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>「清單」和「列」視圖不顯示資產的到期狀態。

## 資產連結到期 {#asset-link-expiration}

通過連結共用資產時，管理員和編輯可以使用 **[!UICONTROL 到期]** 的 **[!UICONTROL 連結共用]** 對話框。 連結的預設到期時間為共用連結之日起七天。

![](assets/asset-link-sharing.png)

它確保作為連結共用的資產在Brand Portal管理員和編輯設定的日期和時間過期，並且在過期日期之後無法再查看和下載。 由於通過連結共用的資產也可以由不屬於組織的外部用戶查看，因此，通過指定過期時間，您可以確保已批准的資產受到保護，並且在指定時間後不會暴露給未知實體。

有關連結共用的詳細資訊，請參閱 [將資產作為連結共用](../using/brand-portal-link-share.md)。

## 授權資產 {#licensed-assets}

授權資產在從Brand Portal下載前必須接受許可協定。 此授權資產協定將在您直接從Brand Portal下載資產或通過共用連結下載時提供。 無論是否過期，所有用戶都可以查看受許可證保護的資產。 但是，已到期的許可資產的下載和使用受到限制。 要瞭解過期的授權資產行為以及基於用戶角色的允許活動，請參閱 [過期資產的使用權限](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)。

受許可證保護的資產 [附加的許可協定](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) 通過在 [!DNL Experience Manager Assets]。

如果資產包含以下（或兩者）元資料屬性之一，則該資產被視為受保護：

* `xmpRights:WebStatement`:此屬性引用包含資產許可協定的頁的路徑。 `xmpRights:WebStatement` 應是儲存庫中的有效路徑。
* `adobe_dam:restrictions`:此屬性的值是指定許可協定的原始HTML。


如果您選擇下載受許可證保護的資產，則系統會將您重定向到 **[!UICONTROL 版權管理]** 頁，具體取決於元資料屬性。

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | 版權管理 |
| --- | --- | --- |
| 是 | - | 介面同時出現在Assets和Brand Portal |
| - | 是（無效路徑） | 無介面 |
| 是 | 是（無效路徑） | 無介面 |
| 是 | 是（有效路徑） | 該介面出現在Assets或Brand Portal </br> 取決於路徑是否對Assets或Brand Portal（或兩者）有效。 |

![](assets/asset-copyright-mgmt.png)

在此，您需要選擇要下載的資產並接受關聯的許可協定。 如果您不接受許可協定， **[!UICONTROL 下載]** 按鈕。

![](assets/licensed-asset-download-2.png)

如果所選內容包含多個受保護資產，則一次選擇一個資產，接受許可協定，然後繼續下載該資產。

## 生成有關過期資產的報告 {#generate-report-about-expired-assets}

管理員可以生成並下載一份報告，其中列出在特定時間範圍內到期的所有資產。 此報表包括有關已到期資產的詳細資訊，如大小、類型、在資產層次結構中指定資產位置的路徑、資產到期的時間以及資產發佈的時間。 可以根據用戶要求自定義此報表的列以顯示更多資料。

![](assets/assets-expired.png)

有關報告功能的詳細資訊，請參閱 [使用報告](../using/brand-portal-reports.md#work-with-reports)。
