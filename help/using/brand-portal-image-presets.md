---
title: 套用影像預設集或動態轉譯
seo-title: 套用影像預設集或動態轉譯
description: '如同巨集，影像預設集是儲存在名稱下的預先定義大小和格式指令集。影像預設集可讓AEM Assets Brand Portal動態傳送不同大小、格式和屬性的影像。 '
seo-description: '如同巨集，影像預設集是儲存在名稱下的預先定義大小和格式指令集。影像預設集可讓AEM Assets Brand Portal動態傳送不同大小、格式和屬性的影像。 '
uuid: a3c8705c-5fbd-472c-8b61-f65 b3 e552 c1 b
content-type: 引用
topic-tags: 管理
products: SG_ PERIENCENCENAGER/Brand_ Portal
discoiquuid: a512dfa0-fef3-4c3 f-a389-a0 a3 a7415 bac
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 套用影像預設集或動態轉譯 {#apply-image-presets-or-dynamic-renditions}

如同巨集，影像預設集是儲存在名稱下的預先定義 [!UICONTROL 大小和格式指令集] 。影像預設集可讓 [!DNL AEM] 資產 [!DNL Brand Portal] 動態傳送不同大小、格式和屬性的影像。

影像預設集可用來產生可預覽和下載的影像動態轉譯。預覽影像及其轉譯時，您可以選擇預設集，將影像重新格式化為您管理員設定的規格。

若要檢視資產的動態轉譯， [!DNL Brand Portal]請確定其PIFF轉譯存在 [!DNL AEM] 於您發佈到 [!DNL Brand Portal]的作者實例上。當您發佈資產時，其PIFF轉譯也會發佈 [!DNL Brand Portal]至。無法產生PIFF轉譯 [!DNL Brand Portal]。

>[!NOTE]
>
>下載影像及其轉譯時，無法選擇從現有預設集選擇。您可以指定自訂影像預設集的屬性。如需詳細資訊，請參閱 [「在下載影像](../using/brand-portal-image-presets.md#main-pars-text-1403412644)時套用影像預設集」。

如需建立影像預設集時所需參數的詳細資訊，請參閱 [管理影像預設集](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html)[!DNL AEM]。

## 建立影像預設集 {#create-an-image-preset}

管理員可以建立在資產詳細資料頁面上顯示為動態轉譯的影像預設集。您可以從頭開始建立影像預設集，或使用新名稱儲存現有的預設集。建立影像預設集時，請選擇影像傳送的大小和格式化命令。當影像傳送為檢視時，會根據選取的指令最佳化其外觀。
請注意，只有管理員可以建立影像預設集 [!DNL Brand Portal]。

請注意，只有管理員可以建立影像預設集 [!DNL Brand Portal]。

>[!NOTE]
>
>針對可供PIFF使用的資產，建立動態轉譯。因此，如果資產沒有建立上的Mercurid TIFF轉譯 [!DNL AEM] 和發佈至 [!DNL Brand Portal]，則只能匯出其系統轉譯，但動態轉譯會顯示為選項。
必須啓用Dynamic Media Mix模式( [!DNL AEM] 作者)才能建立資產的金字塔(ptf)。當發佈該資產時 [!DNL Brand Portal]，會套用影像預設集，並顯示動態轉譯。

1. 從上方的 [!DNL AEM] 工具列，按一下Adobe標誌以存取管理工具。

   !![](assets/[!DNL AEM]logo. png)

2. 在管理工具面板中，按一下 **「影像預設集**」。

   ![](assets/admin-tools-panel-4.png)

3. 在影像預設集頁面中，按一下 **「建立**」。

   ![](assets/image_preset_homepage.png)

4. 在 **「編輯影像預設集** 」頁面中，視需要在 **「基本** 」和 **「進階** 」標籤中輸入值，包括名稱。[「影像預設集」選項](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)[!DNL AEM]中會列出選項。預設集會出現在左側窗格中，並可與其他資產即時使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您也可以使用 **「編輯影像預設集** 」頁面來編輯現有影像預設集的屬性。若要編輯影像預設集，請從影像預設集頁面中選取，然後按一下 **「編輯**」。

5. 按一下&#x200B;**「儲存」**。影像預設集會在影像預設集頁面上建立並顯示。
6. 若要刪除影像預設集，請從影像預設集頁面中選取它，然後按一下 **「刪除**」。在確認頁面中，按一下 **「刪除** 」以確認刪除。影像預設集會從影像預設集頁面中移除。

## 預覽影像時套用影像預設集 {#apply-image-presets-when-previewing-images}

在預覽影像及其轉譯時，請從現有預設集選擇，將影像重新格式化為您管理員設定的規格。

1. 在 [!DNL Brand Portal] 介面中，按一下影像以開啓它。
2. 按一下左側的覆蓋圖示，然後選擇 **轉譯**。

   ![](assets/image-preset-previewrenditions.png)

3. 從 **「轉譯** 」清單中，選取適當的動態轉譯，例如 **縮圖**。預覽影像會根據您的轉譯選擇而產生。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 在下載影像時套用影像預設集 {#apply-image-presets-when-downloading-images}

在下載影像及其轉譯時，無法從 [!DNL Brand Portal]現有的影像預設集中進行選擇。不過，您可以根據想要重新格式化影像的影像預設集屬性進行自訂。

1. 在 [!DNL Brand Portal] 介面中執行下列任一項作業：

   * 將指標暫留在您要下載的影像上。從可用的快速動作縮圖中，按一下 **「下載** 」圖示。
   ![](assets/downloadsingleasset.png)

   * 選取您要下載的影像。從頂端的工具列，按一下 **「下載** 」圖示。
   ![](assets/downloadassets.png)

2. 從 **「下載** 」對話方塊中，視您是否要下載或不含轉譯而下載資產。

   ![](assets/donload-assets-dialog.png)

3. 若要下載資產的動態轉譯，請選取 **「動態轉譯」** 選項。
4. 自訂影像預設集屬性，以在下載期間動態重新格式化影像及其轉譯。指定大小、格式、顏色空間、解析度和影像修飾元。

   ![](assets/dynamicrenditions.png)

5. 按一下 **「下載**」。自訂動態轉譯會下載在ZIP檔案中，以及您選擇下載的影像和轉譯。不過，如果下載單一資產，則不會建立郵遞區號，以確保快速下載。
