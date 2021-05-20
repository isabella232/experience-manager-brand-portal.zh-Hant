---
title: 使用中繼資料結構表單
seo-title: 使用中繼資料結構表單
description: 中繼資料結構描述「屬性」頁面的版面配置，以及針對使用特定結構的資產所顯示的中繼資料屬性。 您套用至資產的結構會決定其「屬性」頁面上顯示的中繼資料欄位。
seo-description: 中繼資料結構描述「屬性」頁面的版面配置，以及針對使用特定結構的資產所顯示的中繼資料屬性。 您套用至資產的結構會決定其「屬性」頁面上顯示的中繼資料欄位。
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Administrator
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: d2bfd06f8cd8a9e78efbc8dd92880e0faae39176
workflow-type: tm+mt
source-wordcount: '1756'
ht-degree: 11%

---

# 使用中繼資料結構表單 {#use-the-metadata-schema-form}

中繼資料結構描述「屬性」頁面的版面配置，以及針對使用特定結構的資產所顯示的中繼資料屬性。 您套用至資產的結構會決定其「屬性」頁面上顯示的中繼資料欄位。

每個資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁面包含預設中繼資料屬性，視資產的MIME類型而定。 管理員可以使用中繼資料結構編輯器來修改現有結構或新增自訂中繼資料結構。 AEM Assets Brand Portal提供各種MIME類型資產的預設表單。 不過，您也可以為這類資產新增自訂表單。

## 添加元資料架構表單{#add-a-metadata-schema-form}

要建立新的元資料結構表單，請執行以下操作：

1. 在頂端的AEM工具列中，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下&#x200B;**[!UICONTROL 元資料結構]**。

   ![](assets/navigation-panel.png)

1. 在&#x200B;**[!UICONTROL 中繼資料結構Forms]**&#x200B;頁面上，按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/create-metadata-schema-form.png)

1. 在&#x200B;**[!UICONTROL 建立架構表單]**&#x200B;對話框中，指定架構表單的標題，然後按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以完成表單建立過程。

   ![](assets/create-schema-form.png)

## 編輯元資料架構表單{#edit-a-metadata-schema-form}

您可以編輯新增或現有的中繼資料結構表單。 中繼資料結構表單包含衍生自其上層的內容，包括索引標籤和索引標籤內的表單項目。 您可以將這些表單項目對應或設定至中繼資料節點內的欄位。

您可以將新索引標籤或表單項目新增至中繼資料結構表單。 衍生索引標籤和表單項目（來自父項）處於鎖定狀態。 不能在子級更改它們。

要編輯元資料結構表單，請執行以下操作：

1. 在頂端的AEM工具列中，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下&#x200B;**[!UICONTROL 元資料結構]**。
1. 從&#x200B;**[!UICONTROL 中繼資料結構Forms]**&#x200B;頁面中，選取要編輯其屬性的結構表單，例如&#x200B;**[!UICONTROL collection]**。

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未編輯的範本會先顯示鎖定符號。 如果自定義任何模板，則模板前的「鎖定」符號將消失。

1. 在頂部工具欄中，按一下「**[!UICONTROL 編輯]**」。

   此時將開啟「**[!UICONTROL 元資料結構編輯器]**」頁，左側開啟「**[!UICONTROL 基本]**」頁簽，右側開啟「**[!UICONTROL 構建表單]**」頁簽。

1. 在&#x200B;**[!UICONTROL 元資料結構編輯器]**&#x200B;頁中，通過將一個或多個元件從&#x200B;**[!UICONTROL 構建表單]**&#x200B;頁簽中的元件類型清單拖到&#x200B;**[!UICONTROL 基本]**&#x200B;頁簽，自定義資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁。

   ![](assets/metadata-schemaeditor-page.png)

1. 要配置元件，請選擇該元件並在&#x200B;**[!UICONTROL Settings]**&#x200B;頁簽中修改其屬性。

### 「生成表單」頁簽{#components-in-the-build-form-tab}中的元件

**[!UICONTROL 建置表單]**&#x200B;索引標籤會列出您可在架構表單中使用的項目。 **[!UICONTROL 設定]**&#x200B;標籤提供您在&#x200B;**[!UICONTROL 建置表單]**&#x200B;標籤中選擇的每個項的屬性。 下表列出&#x200B;**[!UICONTROL Build Form]**&#x200B;索引標籤中可用的表單項目：

| 元件名稱 | 說明 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL 區段標題]** | 新增區段標題，以取得通用元件清單。 |
| **[!UICONTROL 單行文字]** | 新增單行文字屬性。 會儲存為字串。 |
| **[!UICONTROL 多值文本]** | 新增多值文字屬性。 會儲存為字串陣列。 |
| **[!UICONTROL 數量]** | 新增數字元件。 |
| **[!UICONTROL 日期]** | 新增日期元件。 |
| **[!UICONTROL 下拉式]** | 新增下拉式清單。 |
| **[!UICONTROL 標準標記]** | 新增標記. **注意：** 如果管理員從AEM發佈中繼資料結構表單，而路徑不包含租用戶資訊(例如 `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`)，則可能需要變更路徑值(例如 `/etc/tags/<custom_tag_namespace>`)。 |
| **[!UICONTROL 智慧標記]** | 如果您已購買並設定AEM智慧標籤附加元件，則會自動偵測標籤。 |
| **[!UICONTROL 隱藏欄位]** | 新增隱藏欄位。 資產儲存時會以POST參數的形式傳送。 |
| **[!UICONTROL 資產引用者]** | 新增此元件以檢視資產參考的資產清單。 |
| **[!UICONTROL 資產引用]** | 新增以顯示參考資產的資產清單。 |
| **[!UICONTROL 資產評等]** | 從AEM Assets新增至Brand Portal的資產在發佈前的平均評等。 |
| **[!UICONTROL 關聯式中繼資料]** | 在資產的「屬性」頁面中，「新增」可控制其他中繼資料索引標籤的顯示。 |

>[!NOTE]
>
>請勿使用&#x200B;**[!UICONTROL 產品參考]**，因為它無法運作。

#### 編輯元資料元件{#edit-the-metadata-component}

要編輯表單上元資料元件的屬性，請按一下該元件並在&#x200B;**[!UICONTROL Settings]**&#x200B;頁簽中編輯其屬性。

* **[!UICONTROL 欄位標籤]**:資產「屬性」頁面上顯示的中繼資料屬性名稱。

* **[!UICONTROL 對應至屬性]**:此屬性的值會提供資產節點的相對路徑/名稱，資產節點會儲存在CRX存放庫中。開頭為&quot;**。/**」，因為表示路徑位於資產的節點下。

以下是此屬性的有效值：

— `./jcr:content/metadata/dc:title`將值儲存在資產的中繼資料節點，作為屬性[!UICONTROL `dc:title`]。

— `./jcr:created`在資產節點顯示jcr屬性。 如果您在檢視屬性上設定這些屬性，建議您將它們標示為「停用編輯」，因為這些屬性受到保護。否則，當您儲存資產的屬性時，會出現「資產無法修改」錯誤。

* **[!UICONTROL 佔位符]**:使用此屬性可向使用者提供與中繼資料屬性相關的任何資訊。
* **[!UICONTROL 必要]**:使用此屬性可在「屬性」頁面上將中繼資料屬性標示為必要屬性。
* **[!UICONTROL 停用編輯]**:使用此屬性可使元資料屬性在「屬性」頁上不可編輯。
* **[!UICONTROL 以唯讀方式顯示空白欄位]**:將此屬性標籤為在「屬性」頁上顯示元資料屬性，即使它沒有值也是如此。預設情況下，當元資料屬性沒有值時，該屬性不會列在「屬性」頁面上。
* **[!UICONTROL 說明]**:使用此屬性可為中繼資料元件新增簡短說明。
* **[!UICONTROL 刪除圖示]**:按一下此表徵圖可從架構表單中刪除元件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>所有中繼資料欄位在資產的中繼資料編輯器表單中為唯讀。 由於資產的中繼資料必須在AEM Assets中編輯，才能將資產發佈至Brand Portal。

#### 在架構表單{#add-or-delete-a-tab-in-the-schema-form}中添加或刪除頁簽

預設架構表單包含&#x200B;**[!UICONTROL Basic]**&#x200B;和&#x200B;**[!UICONTROL Advanced]**&#x200B;標籤。 架構編輯器可讓您新增或刪除標籤。

![](assets/add_delete_tabs_metadataschemaform.png)

* 要在架構表單上添加新頁簽，請按一下&#x200B;**[!UICONTROL +]**。 依預設，新索引標籤的名稱為「未命名–1」。 您可以從&#x200B;**[!UICONTROL Settings]**&#x200B;標籤修改名稱。

![](assets/add-tab-metadata-form.png)

* 若要刪除標籤，請按一下&#x200B;**[!UICONTROL x]**。 按一下&#x200B;**[!UICONTROL 儲存]**&#x200B;以儲存變更。

## 將元資料架構應用於資料夾{#apply-a-metadata-schema-to-a-folder}

Brand Portal可讓您自訂和控制中繼資料結構，讓資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁面只顯示您選擇顯示的特定資訊。 要控制&#x200B;**[!UICONTROL 屬性]**&#x200B;頁中顯示的元資料，請從元資料架構表單中刪除所需的元資料，並將其應用到特定資料夾。

要將元資料結構表單應用到資料夾，請執行以下操作：

1. 在頂端的AEM工具列中，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下&#x200B;**[!UICONTROL 元資料結構]**。

1. 從&#x200B;**[!UICONTROL 中繼資料結構Forms]**&#x200B;頁面中，選取您要套用至資產的結構表單，例如&#x200B;**[!UICONTROL clothing]**。

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 在頂部工具欄中，按一下&#x200B;**[!UICONTROL 應用到資料夾]**。

1. 從&#x200B;**[!UICONTROL 選擇資料夾]**&#x200B;頁，導航至要應用&#x200B;**[!UICONTROL clothing]**&#x200B;元資料架構的資料夾，例如&#x200B;**[!UICONTROL Gloves]**。

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 按一下&#x200B;**[!UICONTROL Apply]**&#x200B;將元資料架構表單應用到資料夾。

   **[!UICONTROL clothing]**&#x200B;元資料架構表單中可用的元資料應用於&#x200B;**[!UICONTROL Gloves]**&#x200B;資料夾，並可在資料夾的&#x200B;**[!UICONTROL Properties]**&#x200B;頁面中看到。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果將包含巢狀結構的結構套用至包含視訊檔案的資料夾，視訊檔案的中繼資料屬性可能無法正確轉譯。 若要確保中繼資料屬性正確呈現，請移除巢狀結構，並僅將上層結構套用至資料夾。

## 刪除元資料架構表單{#delete-a-metadata-schema-form}

Brand Portal可讓您僅刪除自訂結構描述表單。 它不會讓您刪除預設的結構描述表單/範本。 不過，您可以刪除這些表單中的任何自訂變更。

若要刪除表單，請選取表單並按一下&#x200B;**[!UICONTROL Delete]**&#x200B;圖示。

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>刪除對預設表單所做的自定義更改後，**[!UICONTROL Lock]**&#x200B;符號將重新出現在元資料架構介面上的表單名稱前面，以指示表單已恢復到其預設狀態。

## MIME類型{#schema-forms-for-mime-types}的架構表單

### 為MIME類型{#adding-new-forms-for-mime-types}添加新表單

除了預設表單外，您還可以為各種MIME類型的資產新增自訂表單，或在適當的表單類型下建立新表單。 例如，若要新增影像/png子類型 **[!UICONTROL 的新範本]** ，請在「影像」表單下建立表單。方案表單的標題是子類型名稱。在本例中，標題為&quot;png&quot;.

#### 對各種MIME類型{#using-an-existing-schema-template-for-various-mime-types}使用現有架構模板

您可以將現有範本用於不同的MIME類型。 例如，對於MIME類型&#x200B;**image/png**&#x200B;的資產，請使用&#x200B;**image/jpeg**&#x200B;表單。

在此情況下，請在CRX存放庫的[!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`]處建立新節點。 指定節點的名稱並定義下列屬性：

| **名稱** | **類型** | **值** |
|---|---|---|
| 出口型 | 字串 | image/jpeg |
| mimetypes | String[] | image/png |

* **exposedmitype**:要映射的現有表單的名稱
* **mimetypes**:使用exposedmimetypeattribute中定義的表單的MIME類型 **** 清單

Brand Portal會對應下列MIME類型和結構表單：

| **結構表單** | **MIME類型** |
|---|---|
| 影像/jpeg | image/pjpeg |
| image/tiff | 影像/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| 視頻/mpeg4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

以下是預設中繼資料屬性的清單：

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:ImageWidth
* jcr:content/metadata/tiff:ImageLength
