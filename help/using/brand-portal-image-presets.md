---
title: 套用影像預設集或動態轉譯
seo-title: 套用影像預設集或動態轉譯
description: '像宏一樣，影像預設集是以名稱保存的一組預定義大小和格式命令。 影像預設集可讓AEM Assets品牌入口網站動態傳送不同大小、格式和屬性的影像。 '
seo-description: '像宏一樣，影像預設集是以名稱保存的一組預定義大小和格式命令。 影像預設集可讓AEM Assets品牌入口網站動態傳送不同大小、格式和屬性的影像。 '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: 引用
topic-tags: 管理
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# 套用影像預設集或動態轉譯 {#apply-image-presets-or-dynamic-renditions}

像宏一樣，影像預設集是以名稱保存的一組預定義大小和格式命令。 影像預設集可讓AEM Assets品牌入口網站動態傳送不同大小、格式和屬性的影像。

影像預設集用來產生可預覽及下載之影像的動態轉譯。 在預覽影像及其轉譯時，您可以選擇預設集，以依照管理員設定的規格重新格式化影像。

若要在品牌入口網站中檢視資產的動態轉譯，請確定其Pyramid tiff轉譯存在於您發佈至品牌入口網站的AEM作者例項中。 當您發佈資產時，其PTIFF轉譯也會發佈至品牌入口網站。 無法從Brand Portal產生PTIFF轉譯。

>[!NOTE]
>
>當下載影像及其轉譯時，您無法從現有的預設集中選擇。 您可以改為指定自訂影像預設集的屬性。 如需詳細資訊，請參 [閱下載影像時套用影像預設集](../using/brand-portal-image-presets.md#main-pars-text-1403412644)。

如需建立影像預設集時所需參數的詳細資訊，請參閱「管理 [影像預設集」](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)。

## Create an image preset {#create-an-image-preset}

Administrators can create image presets that appear as dynamic renditions on the asset detail page. You can create an image preset from scratch or save an existing one with a new name. When creating an image preset, choose a size for image delivery and the formatting commands. When an image is delivered for viewing, its appearance is optimized according to the chosen commands.
Note that only Administrators can create image presets in Brand Portal.

請注意，只有管理員才能在品牌入口網站中建立影像預設集。

>[!NOTE]
>
>Dynamic renditions of an image are created using its Pyramid TIFF. 如果金字塔TIFF不適用於任何資產，則無法在品牌入口網站中擷取該資產的動態轉譯。
If AEM (Author) instance is running on Dynamic Media Hybrid mode, then Pyramid TIFF renditions of image assets are created and saved in AEM repository. ****Whereas, if AEM (Author) instance is running on Dynamic Media Scene 7 mode, then Pyramid TIFF renditions of image assets exist on Scene 7 server.
**** When such assets are published to brand portal, image presets are applied and dynamic renditions are displayed.

1. From the AEM toolbar at the top, click the Adobe logo to access administrative tools.

1. 在管理工具面板中，按一下「影像預 **[!UICONTROL 設集」]**。

   ![](assets/admin-tools-panel-4.png)

1. In the image presets page, click Create.****

   ![](assets/image_preset_homepage.png)

1. 在「編 **[!UICONTROL 輯影像預設集]********** 」頁面中，視需要在「基本」和「進階」標籤中輸入值，包括名稱。 這些選項在「影像預設集」 [選項中概述](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)。 預設集會出現在左窗格中，並可與其他資產一起即時使用。

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >您也可以使用「編 **[!UICONTROL 輯影像預設集]** 」頁面來編輯現有影像預設集的屬性。 若要編輯影像預設集，請從影像預設集頁面選取它，然後按一下「編 **[!UICONTROL 輯」]**。

1. Click **[!UICONTROL Save]**. 影像預設集會建立並顯示在影像預設集頁面上。
1. 若要刪除影像預設集，請從影像預設集頁面選取它，然後按一下「刪 **[!UICONTROL 除」]**。 在確認頁面中，按一下 **[!UICONTROL 刪除]** ，確認刪除。 影像預設集會從影像預設集頁面中移除。

## 在預覽影像時套用影像預設集 {#apply-image-presets-when-previewing-images}

在預覽影像及其轉譯時，從現有的預設集中選擇，以依照管理員設定的規格重新格式化影像。

1. 在品牌入口網站介面中，按一下影像以開啟它。
1. 按一下左側的覆蓋圖示，然後選擇「轉 **[!UICONTROL 譯」]**。

   ![](assets/image-preset-previewrenditions.png)

1. 從「轉 **[!UICONTROL 譯]** 」清單中，選取適當的動態轉譯，例如「縮 **[!UICONTROL 圖」]**。 預覽影像會根據您選擇的轉譯來轉譯。

   ![](assets/image-preset-previewrenditionthumbnail.png)

## 下載影像時套用影像預設集 {#apply-image-presets-when-downloading-images}

When downloading images and their renditions from Brand Portal, you cannot choose from the existing image presets. However, you can customize image preset properties based on which you want to reformat images.

1. From the Brand Portal interface, do one of the following:

   * 將指標暫留在您要下載的影像上。 從可用的快速動作縮圖中，按一下「下 **[!UICONTROL 載]** 」圖示。
   ![](assets/downloadsingleasset.png)

   * 選取您要下載的影像。 從頂端的工具列，按一下「下 **[!UICONTROL 載]** 」圖示。
   ![](assets/downloadassets.png)

1. 從「下 **[!UICONTROL 載]** 」對話方塊中，根據您要下載資產時是否包含其轉譯，選取所需的選項。

   ![](assets/donload-assets-dialog.png)

1. 若要下載資產的動態轉譯，請選取「 **[!UICONTROL 動態轉譯」選項]** 。
1. 自訂影像預設集屬性，讓您在下載期間根據要動態重新格式化影像及其轉譯的影像。 指定大小、格式、色域、解析度和影像修飾元。

   ![](assets/dynamicrenditions.png)

1. 按一 **[!UICONTROL 下下載]**。 自訂動態轉譯會與您選擇下載的影像和轉譯一起下載在ZIP檔案中。 不過，如果下載單一資產，則不會建立任何zip檔案，如此可確保快速下載。
