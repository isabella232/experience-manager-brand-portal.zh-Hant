---
title: Apply image presets or dynamic renditions
seo-title: 套用影像預設集或動態轉譯
description: 'Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable AEM Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties. '
seo-description: 'Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable AEM Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: 引用
topic-tags: 管理
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
translation-type: tm+mt
source-git-commit: c0169450c5cf1d8c99f8604df3bd2667445ff1ed

---


# Apply image presets or dynamic renditions {#apply-image-presets-or-dynamic-renditions}

Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable AEM Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties.

影像預設集用來產生可預覽及下載之影像的動態轉譯。 When previewing images and their renditions, you can choose a preset to reformat images to the specifications set by your Administrator.

To view dynamic renditions of an asset in Brand Portal, ensure that its Pyramid tiff rendition exists at the AEM author instance from where you publish to Brand Portal. When you publish the asset, its PTIFF rendition is also published to Brand Portal. There is no way of generating the PTIFF rendition from Brand Portal.

>[!NOTE]
>
>當下載影像及其轉譯時，您無法從現有的預設集中選擇。 您可以改為指定自訂影像預設集的屬性。 如需詳細資訊，請參 [閱下載影像時套用影像預設集](../using/brand-portal-image-presets.md#main-pars-text-1403412644)。

如需建立影像預設集時所需參數的詳細資訊，請參閱「管理 [影像預設集」](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)。

## 建立影像預設集 {#create-an-image-preset}

管理員可以建立影像預設集，這些預設集會在資產詳細資料頁面上顯示為動態轉譯。 您可以從頭開始建立影像預設集，或以新名稱儲存現有的影像預設集。 建立影像預設集時，請選擇影像傳送的大小和格式命令。 當影像被傳送以供觀看時，其外觀根據所選擇的命令被優化。
請注意，只有管理員才能在品牌入口網站中建立影像預設集。

請注意，只有管理員才能在品牌入口網站中建立影像預設集。

>[!NOTE]
>
>動態轉譯會針對可使用PTIFF的資產建立。 因此，如果資產沒有在AEM上建立Pyramid TIFF轉譯並發佈至品牌入口網站，則只能匯出其系統轉譯，但動態轉譯會以選項呈現。
必須在AEM（作者）上啟用動態媒體混合模式，才能建立資產的金字塔圖文框(ptiff)。 當此類資產發佈至品牌入口網站時，會套用影像預設集並顯示動態轉譯。

1. 從頂端的AEM工具列，按一下Adobe標誌以存取管理工具。

2. 在管理工具面板中，按一下「影像預 **[!UICONTROL 設集」]**。

   ![](assets/admin-tools-panel-4.png)

3. 在影像預設集頁面中，按一下「 **[!UICONTROL 建立]**」。

   ![](assets/image_preset_homepage.png)

4. 在「編 **[!UICONTROL 輯影像預設集]********** 」頁面中，視需要在「基本」和「進階」標籤中輸入值，包括名稱。 這些選項在「影像預設集」 [選項中概述](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)。 預設集會出現在左窗格中，並可與其他資產一起即時使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您也可以使用「編 **[!UICONTROL 輯影像預設集]** 」頁面來編輯現有影像預設集的屬性。 若要編輯影像預設集，請從影像預設集頁面選取它，然後按一下「編 **[!UICONTROL 輯」]**。

5. Click **[!UICONTROL Save]**. 影像預設集會建立並顯示在影像預設集頁面上。
6. 若要刪除影像預設集，請從影像預設集頁面選取它，然後按一下「刪 **[!UICONTROL 除」]**。 在確認頁面中，按一下 **[!UICONTROL 刪除]** ，確認刪除。 影像預設集會從影像預設集頁面中移除。

## 在預覽影像時套用影像預設集 {#apply-image-presets-when-previewing-images}

在預覽影像及其轉譯時，從現有的預設集中選擇，以依照管理員設定的規格重新格式化影像。

1. From the Brand Portal interface, click an image to open it.
2. Click the overlay icon on the left, and choose Renditions.****

   ![](assets/image-preset-previewrenditions.png)

3. From the Renditions list, select the appropriate dynamic rendition, for example, Thumbnail. ******** The preview image is rendered based on your choice of the rendition.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Apply image presets when downloading images {#apply-image-presets-when-downloading-images}

When downloading images and their renditions from Brand Portal, you cannot choose from the existing image presets. However, you can customize image preset properties based on which you want to reformat images.

1. From the Brand Portal interface, do one of the following:

   * Hover the pointer over the image you want to download. 從可用的快速動作縮圖中，按一下「下 **[!UICONTROL 載]** 」圖示。
   ![](assets/downloadsingleasset.png)

   * 選取您要下載的影像。 From the toolbar at the top, click the Download icon.****
   ![](assets/downloadassets.png)

2. 從「下 **[!UICONTROL 載]** 」對話方塊中，根據您要下載資產時是否包含其轉譯，選取所需的選項。

   ![](assets/donload-assets-dialog.png)

3. 若要下載資產的動態轉譯，請選取「 **[!UICONTROL 動態轉譯」選項]** 。
4. 自訂影像預設集屬性，讓您在下載期間根據要動態重新格式化影像及其轉譯的影像。 指定大小、格式、色域、解析度和影像修飾元。

   ![](assets/dynamicrenditions.png)

5. 按一 **[!UICONTROL 下下載]**。 自訂動態轉譯會與您選擇下載的影像和轉譯一起下載在ZIP檔案中。 不過，如果下載單一資產，則不會建立任何zip檔案，如此可確保快速下載。
