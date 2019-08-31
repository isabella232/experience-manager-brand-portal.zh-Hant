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
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# 套用影像預設集或動態轉譯 {#apply-image-presets-or-dynamic-renditions}

如同巨集，影像預設集是儲存在名稱下的預先定義大小和格式指令集。影像預設集可讓AEM Assets Brand Portal動態傳送不同大小、格式和屬性的影像。

影像預設集可用來產生可預覽和下載的影像動態轉譯。預覽影像及其轉譯時，您可以選擇預設集，將影像重新格式化為您管理員設定的規格。

若要檢視「品牌入口網站」中資產的動態轉譯，請確定其「發行者」tiff轉譯存在於AEM作者實例，從您發佈至品牌入口網站的位置。當您發佈資產時，其PIFF轉譯也會發佈至品牌入口網站。無法從品牌入口網站產生PIFF轉譯。

>[!NOTE]
>
>下載影像及其轉譯時，無法選擇從現有預設集選擇。您可以指定自訂影像預設集的屬性。如需詳細資訊，請參閱 [「在下載影像](../using/brand-portal-image-presets.md#main-pars-text-1403412644)時套用影像預設集」。

如需建立影像預設集時所需參數的詳細資訊，請參閱 [管理影像預設集](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)。

## 建立影像預設集 {#create-an-image-preset}

管理員可以建立在資產詳細資料頁面上顯示為動態轉譯的影像預設集。您可以從頭開始建立影像預設集，或使用新名稱儲存現有的預設集。建立影像預設集時，請選擇影像傳送的大小和格式化命令。當影像傳送為檢視時，會根據選取的指令最佳化其外觀。
請注意，只有管理員可以在品牌入口網站中建立影像預設集。

請注意，只有管理員可以在品牌入口網站中建立影像預設集。

>[!NOTE]
>
>針對可供PIFF使用的資產，建立動態轉譯。因此，如果資產沒有AEM上建立的Missimid TIFF轉譯，並發佈至品牌入口網站，則只能匯出其系統轉譯，但動態轉譯會顯示為一個選項。
必須在AEM(作者)上啓用動態媒體混合模式，才能建立資產的金字塔(ptf)。當該資產發佈至品牌入口網站時，會套用影像預設集並顯示動態轉譯。

1. 從上方的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/AEMlogo.png)

2. 在管理工具面板中，按一下 **[!UICONTROL 「影像預設集]**」。

   ![](assets/admin-tools-panel-4.png)

3. 在影像預設集頁面中，按一下 **[!UICONTROL 「建立]**」。

   ![](assets/image_preset_homepage.png)

4. 在 **[!UICONTROL 「編輯影像預設集]** 」頁面中，視需要在 **[!UICONTROL 「基本]** 」和 **[!UICONTROL 「進階]** 」標籤中輸入值，包括名稱。[「影像預設集」選項](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)中會列出選項。預設集會出現在左側窗格中，並可與其他資產即時使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您也可以使用 **[!UICONTROL 「編輯影像預設集]** 」頁面來編輯現有影像預設集的屬性。若要編輯影像預設集，請從影像預設集頁面中選取，然後按一下 **[!UICONTROL 「編輯]**」。

5. Click **[!UICONTROL Save]**. 影像預設集會在影像預設集頁面上建立並顯示。
6. 若要刪除影像預設集，請從影像預設集頁面中選取它，然後按一下 **[!UICONTROL 「刪除]**」。在確認頁面中，按一下 **[!UICONTROL 「刪除]** 」以確認刪除。影像預設集會從影像預設集頁面中移除。

## 預覽影像時套用影像預設集 {#apply-image-presets-when-previewing-images}

在預覽影像及其轉譯時，請從現有預設集選擇，將影像重新格式化為您管理員設定的規格。

1. 從品牌入口網站介面，按一下影像以開啓它。
2. 按一下左側的覆蓋圖示，然後選擇 **[!UICONTROL 轉譯]**。

   ![](assets/image-preset-previewrenditions.png)

3. 從 **[!UICONTROL 「轉譯]** 」清單中，選取適當的動態轉譯，例如 **[!UICONTROL 縮圖]**。預覽影像會根據您的轉譯選擇而產生。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 在下載影像時套用影像預設集 {#apply-image-presets-when-downloading-images}

從品牌入口網站下載影像及其轉譯時，您無法從現有的影像預設集中進行選擇。不過，您可以根據想要重新格式化影像的影像預設集屬性進行自訂。

1. 從品牌入口網站介面，執行下列其中一項作業：

   * 將指標暫留在您要下載的影像上。從可用的快速動作縮圖中，按一下 **[!UICONTROL 「下載]** 」圖示。
   ![](assets/downloadsingleasset.png)

   * 選取您要下載的影像。從頂端的工具列，按一下 **[!UICONTROL 「下載]** 」圖示。
   ![](assets/downloadassets.png)

2. 從 **[!UICONTROL 「下載]** 」對話方塊中，視您是否要下載或不含轉譯而下載資產。

   ![](assets/donload-assets-dialog.png)

3. 若要下載資產的動態轉譯，請選取 **[!UICONTROL 「動態轉譯」]** 選項。
4. 自訂影像預設集屬性，以在下載期間動態重新格式化影像及其轉譯。指定大小、格式、顏色空間、解析度和影像修飾元。

   ![](assets/dynamicrenditions.png)

5. 按一下 **[!UICONTROL 「下載]**」。自訂動態轉譯會下載在ZIP檔案中，以及您選擇下載的影像和轉譯。不過，如果下載單一資產，則不會建立郵遞區號，以確保快速下載。
