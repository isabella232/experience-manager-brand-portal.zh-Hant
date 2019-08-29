---
title: 使用中繼資料結構表單
seo-title: 使用中繼資料結構表單
description: 中繼資料結構描述了「屬性」頁面的版面配置，以及針對使用特定結構的資產所顯示的中繼資料屬性。您套用至資產的結構會決定顯示在其屬性頁面上的中繼資料欄位。
seo-description: 中繼資料結構描述了「屬性」頁面的版面配置，以及針對使用特定結構的資產所顯示的中繼資料屬性。您套用至資產的結構會決定顯示在其屬性頁面上的中繼資料欄位。
uuid: a944a3b-5152-425f-b1 ea-bfe3331 de928
content-type: 引用
products: SG_ PERIENCENCENAGER/Brand_ Portal
topic-tags: 管理
discoiquuid: 500b46da-ef67-46a0-a069-192f4 b1 a0 a0
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# 使用中繼資料結構表單 {#use-the-metadata-schema-form}

中繼資料結構描述了「屬性」頁面的版面配置，以及針對使用特定結構的資產所顯示的中繼資料屬性。您套用至資產的結構會決定顯示在其屬性頁面上的中繼資料欄位。

每個資產的 **「屬性** 」頁面包含預設中繼資料屬性，視資產的MIME類型而定。管理員可以使用中繼資料結構編輯器來修改現有的結構描述或新增自訂中繼資料結構。[!DNL AEM] 資產 [!DNL Brand Portal] 為各種MIME類型的資產提供預設表單。不過，您也可以為該資產新增自訂表單。

## 新增中繼資料結構表單 {#add-a-metadata-schema-form}

若要建立新的中繼資料結構表單，請執行下列動作：

1. 從上方的 [!DNL AEM] 工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

2. 從管理工具面板，按一下 **中繼資料結構。**

   ![](assets/navigation-panel.png)

3. 在 **「中繼資料結構表格** 」頁面上，按一下 **「建立**」。

   ![](assets/create-metadata-schema-form.png)

4. 在 **「建立結構表格」** 對話方塊中，指定結構表格的標題，然後按一下 **「建立」** 以完成表單建立程序。

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

您可以編輯新加入的或現有的中繼資料結構表格。中繼資料結構表單包含從其父項衍生的內容，包括標籤中的標籤和表單項目。您可以將這些表單項目對應至中繼資料節點內的欄位。

您可以新增標籤或表格項目至中繼資料結構表格。衍生標籤和表單項目(來自父項)處於鎖定狀態。您無法在子層級變更它們。

若要編輯中繼資料結構表單，請執行下列動作：

1. 從上方的 [!DNL AEM] 工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

2. 從管理工具面板，按一下 **中繼資料結構。**
3. 從 **「中繼資料結構表單** 」頁面中，選取結構表格以編輯其屬性，例如 **系列**。

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未編輯的範本會在他們之前顯示 **鎖定** 符號。如果您自訂任何範本，範本 **** 會在範本消失之前消失。

4. 從上方的工具列，按一下 **「編輯**」。

   **「中繼資料結構編輯器」** 頁面隨即開啓，左側會開啓「 **基本** 」標籤，右側的「 **建立表單** 」索引標籤隨即開啓。

5. 在 **「中繼資料結構編輯器** 」頁面中，將 **一或多** 個元件從「 **建置表單** 」標籤中的元件類型清單拖曳至「 **基本** 」標籤，自訂資產的「屬性」頁面。

   ![](assets/metadata-schemaeditor-page.png)

6. 若要設定元件，請在「 **設定** 」標籤中選取並修改其屬性。

### 「建置表單」索引標籤中的元件 {#components-in-the-build-form-tab}

**「建立表單** 」索引標籤會列出可用於結構表單的項目。**「設定** 」標籤提供您在 **「建置表單」** 索引標籤中選取的每個項目屬性。下表列出 **「建置表單** 」索引標籤中可用的表單項目：

| 元件名稱 | 說明 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 區段標題 | 新增區段標題，以取得常用元件清單。 |
| 單行文字 | 新增單行文字屬性。它會儲存為字串。 |
| MultiValue Ext | 新增多值文字屬性。它會儲存為字串陣列。 |
| 數字 | 新增數字元件。 |
| 日期 | 新增日期元件。 |
| 下拉式 | 新增下拉式清單。 |
| 標準標記 | 新增標記. **注意：** 管理員可能需要變更路徑值， `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`例如，如果他們從路徑中發佈中繼資料 [!DNL AEM]結構表單，例如，路徑不包含租用者資訊 `/etc/tags/<custom_tag_namespace>`。 |
| 智慧標記 | 如果您已購買並設定 [!DNL AEM] 智慧標籤附加元件，則自動偵測到標記。 |
| 隱藏欄位 | 新增隱藏欄位。儲存資產時，會以POST參數傳送。 |
| 資產引用者 | 新增此元件以檢視資產參考資產的清單。 |
| 資產引用 | 新增以顯示參考資產的資產清單。 |
| 資產評等 | [!DNL AEM] 資產在發佈至 [!DNL Brand Portal]資產前的平均評分。 |
| 關聯式中繼資料 | 新增以控制資產頁面中其他中繼資料標籤的顯示。 |

>[!NOTE]
>
>請勿使用 **產品參考** ，因為它無法運作。

#### 編輯中繼資料元件 {#edit-the-metadata-component}

若要編輯表單上中繼資料元件的屬性，請按一下元件並在 **「設定** 」標籤中編輯其屬性。

* **欄位標籤**：資產屬性頁面上顯示的中繼資料屬性名稱。

* **映射至屬性**：此屬性的值提供資產節點在CRM儲存庫中儲存的資產節點的相對路徑/名稱。開頭&#x200B;**為「./**「因為指出路徑位於資產的節點下」。

下列是此屬性的有效值：

— `./jcr:content/metadata/dc:title`：將資產的中繼資料節點上的值儲存為屬性 `dc:title`。

— `./jcr:created`：顯示資產節點上的jcr屬性。如果您在檢視屬性上設定這些屬性，我們建議您將它們標示為「停用編輯」，因為它們受到保護。否則，當您儲存資產屬性時，會發生「資產無法修改」錯誤。

* **預留位置**：使用此屬性可提供使用者有關中繼資料屬性的任何相關資訊。
* **需要**：使用此屬性，將中繼資料屬性標示為「屬性」頁面上的必要項目。
* **停用編輯**：使用此屬性可讓中繼資料屬性無法在「屬性」頁面上編輯。
* **以唯讀方式顯示空白欄位**：標示此屬性，以便在「屬性」頁面上顯示中繼資料屬性，即使它沒有值。根據預設，中繼資料屬性沒有值，而不會列在「屬性」頁面上。
* **說明**：使用此屬性可新增中繼資料元件的簡短說明。
* **刪除圖示**：按一下此圖示可從結構表格中刪除元件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>所有中繼資料欄位都是唯讀的，而且是資產的中繼資料編輯器形式。因為資產的中繼資料必須在 [!DNL AEM] 資產發佈至 [!DNL Brand Portal]資產之前先編輯。

#### 新增或刪除結構表格中的標籤 {#add-or-delete-a-tab-in-the-schema-form}

預設結構表單包含 **「基本** 」和「 **進階」** 標籤。結構編輯器可讓您新增或刪除標籤。

![](assets/add_delete_tabs_metadataschemaform.png)

* 若要在結構表格上新增標籤，請按一下 **+**。依預設，新標籤的名稱為「未命名-1」。您可以從 **「設定** 」標籤修改名稱。

![](assets/add-tab-metadata-form.png)

* 若要刪除標籤，請按一下 **x**。按一下 **「儲存** 」以儲存變更。

## 套用中繼資料結構至資料夾 {#apply-a-metadata-schema-to-a-folder}

[!DNL Brand Portal] 可讓您自訂和控制中繼資料結構，讓資產的 **「屬性** 」頁面只顯示您選擇要顯示的特定資訊。若要控制顯示在 **「屬性** 」頁面中的中繼資料，請從中繼資料結構表單移除必要中繼資料，並將其套用至特定資料夾。

若要將中繼資料結構表格套用至資料夾，請執行下列動作：

1. 從上方的 [!DNL AEM] 工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

2. 從管理工具面板，按一下 **中繼資料結構。**

3. 從 **「中繼資料結構表單** 」頁面，選取您要套用至資產(例如 **服裝**)的結構表格。

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. 從上方的工具列，按一下 **「套用至資料夾**」。

5. 從 **「選取資料夾」** 頁面，導覽至您要套用 **服裝** 中繼資料結構的資料夾，例如 **Groves**。

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. 按一下 **「套用」** ，將中繼資料結構表格套用至資料夾。

   **服裝** 中繼資料結構表格中可用的中繼資料會套用至 **「群組」** 資料夾，並顯示在檔案夾的 **「屬性** 」頁面中。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果您將包含巢狀結構的結構套用至包含視訊檔案的檔案夾，視訊檔案的中繼資料屬性可能無法正確呈現。若要確保中繼資料屬性正確呈現，請移除巢狀結構描述，並僅套用上層架構至資料夾。

## Delete a metadata schema form {#delete-a-metadata-schema-form}

[!DNL Brand Portal] 可讓您僅刪除自訂結構表單。它不允許您刪除預設結構表單/範本。不過，您可以刪除這些表格中的任何自訂變更。

若要刪除表單，請選取表單，然後按一下 **「刪除** 」圖示。

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>刪除預設表單所做的自訂變更後， **「** 中繼資料結構」介面上的表單名稱會重新出現在「中繼資料結構」介面上，指出表單已回復為其預設狀態。

## MIME類型的結構表單 {#schema-forms-for-mime-types}

### 新增MIME類型的表格 {#adding-new-forms-for-mime-types}

除了預設表單外，您還可以為各種MIME類型新增自訂表單，或在適當表格類型下建立新表格。例如，若要新增 **影像/png** 子類型的範本，請在「影像」表單下建立表格。結構表格的標題為子類型名稱。在此情況下，標題為「png」。

#### 針對各種MIME類型使用現有的結構範本 {#using-an-existing-schema-template-for-various-mime-types}

您可以針對不同的MIME類型使用現有範本。例如，針對MIME類型image/png的資產使用 **image/jpeg****表格**。

在此情況下，請在CREX儲存庫 `/etc/dam/metadataeditor/mimetypemappings` 中建立新節點。指定節點的名稱並定義下列屬性：

| **名稱** | **類型** | **值** |
|---|---|---|
| presentedmametype | 字串 | image/jpeg |
| mimetype | String[] | image/png |

* **representedmametype**：要對應的現有表格名稱
* **mimetype**：使用 **公開mamemedype** 屬性中定義之表單的MIME類型清單

[!DNL Brand Portal] 對應下列MIME類型和結構表格：

| **結構表單** | **MIME類型** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-imageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSett | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi，video/msvideo，video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

以下是預設中繼資料屬性清單：

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr：content/metadata/videoCodec
* jcr：content/metadata/AudioCodec
* jcr：content/metadata/dc：title
* jcr：content/metadata/dc：description
* jcr：content/metadata/xMPmm：socialeID
* jcr：content/metadata/xMPmm：DocumentID
* jcr：content/metadata/dam：sha1
* jcr：content/metadata/dam：解決方案內容
* jcr：content/metadata/VideoItrate
* jcr：content/metadata/AudioItate
* jcr：content/users/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr：content/onTime
* jcr：content/offTime
* jcr:content/metadata/dam:size
* jcr：content/metadata/tiff：imageWidth
* jcr：content/metadata/tiff：imageLength
