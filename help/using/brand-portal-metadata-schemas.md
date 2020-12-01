---
title: 使用中繼資料結構表單
seo-title: 使用中繼資料結構表單
description: 中繼資料結構描述「屬性」頁面的版面配置，以及使用特定結構的資產所顯示的中繼資料屬性。 您套用至資產的架構會決定顯示在其「屬性」頁面上的中繼資料欄位。
seo-description: 中繼資料結構描述「屬性」頁面的版面配置，以及使用特定結構的資產所顯示的中繼資料屬性。 您套用至資產的架構會決定顯示在其「屬性」頁面上的中繼資料欄位。
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1756'
ht-degree: 11%

---


# 使用中繼資料結構表單 {#use-the-metadata-schema-form}

中繼資料結構描述「屬性」頁面的版面配置，以及使用特定結構的資產所顯示的中繼資料屬性。 您套用至資產的架構會決定顯示在其「屬性」頁面上的中繼資料欄位。

每個資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁面包含預設中繼資料屬性，視資產的MIME類型而定。 管理員可以使用中繼資料結構編輯器來修改現有結構或新增自訂的中繼資料結構。 AEM Assets品牌入口網站提供各種MIME類型資產的預設表單。 不過，您也可以為此類資產新增自訂表格。

## 添加元資料架構表單{#add-a-metadata-schema-form}

要建立新的元資料架構表單，請執行以下操作：

1. 從頂端的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下&#x200B;**[!UICONTROL 元資料結構]**。

   ![](assets/navigation-panel.png)

1. 在&#x200B;**[!UICONTROL 中繼資料結構表單]**&#x200B;頁面上，按一下&#x200B;**[!UICONTROL 建立]**。

   ![](assets/create-metadata-schema-form.png)

1. 在&#x200B;**[!UICONTROL 建立架構表單]**&#x200B;對話框中，指定架構表單的標題，然後按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以完成表單建立過程。

   ![](assets/create-schema-form.png)

## 編輯{#edit-a-metadata-schema-form}表單的元資料架構

您可以編輯新增或現有的中繼資料結構表單。 中繼資料結構表單包含衍生自其父項的內容，包括標籤和標籤內的表單項目。 您可以將這些表單項目映射或設定至中繼資料節點內的欄位。

您可以將新標籤或表單項目新增至中繼資料結構表單。 衍生標籤和表單項（來自父項）處於鎖定狀態。 您無法在子級更改它們。

要編輯元資料結構表單，請執行以下操作：

1. 從頂端的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下&#x200B;**[!UICONTROL 元資料結構]**。
1. 從&#x200B;**[!UICONTROL 中繼資料結構表單]**&#x200B;頁面中，選擇結構表單以編輯其屬性，例如&#x200B;**[!UICONTROL collection]**。

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未編輯的範本會在其前顯示鎖定符號。 如果自定義任何模板，則模板前的「鎖定」符號將消失。

1. 在頂部的工具欄中，按一下&#x200B;**[!UICONTROL 編輯]**。

   「**[!UICONTROL 元資料結構編輯器]**」頁開啟，左側開啟&#x200B;**[!UICONTROL 基本]**&#x200B;頁籤，右側開啟&#x200B;**[!UICONTROL 構建表單]**&#x200B;頁籤。

1. 在&#x200B;**[!UICONTROL 元資料結構編輯器]**&#x200B;頁中，通過將一個或多個元件從&#x200B;**[!UICONTROL 構建表單]**&#x200B;頁籤的元件類型清單中拖動到&#x200B;**[!UICONTROL 基本]**&#x200B;頁籤，定制資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁。

   ![](assets/metadata-schemaeditor-page.png)

1. 要配置元件，請選擇該元件並在&#x200B;**[!UICONTROL Settings]**&#x200B;頁籤中修改其屬性。

### 「生成表單」頁籤中的元件{#components-in-the-build-form-tab}

**[!UICONTROL 建置表單]**&#x200B;標籤列出可在架構表單中使用的項目。 **[!UICONTROL Settings]**&#x200B;標籤提供您在&#x200B;**[!UICONTROL Build Form]**&#x200B;標籤中選擇的每個項目的屬性。 下表列出了&#x200B;**[!UICONTROL Build Form]**&#x200B;頁籤中可用的表單項：

| 元件名稱 | 說明 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL 區段標題]** | 新增共用元件清單的區段標題。 |
| **[!UICONTROL 單行文字]** | 新增單行文字屬性。 它儲存為字串。 |
| **[!UICONTROL 多值文字]** | 新增多值文字屬性。 它儲存為字串陣列。 |
| **[!UICONTROL 數量]** | 添加數字元件。 |
| **[!UICONTROL 日期]** | 新增日期元件。 |
| **[!UICONTROL 下拉式]** | 新增下拉式清單。 |
| **[!UICONTROL 標準標記]** | 新增標記. **注意：** 管理員可能需要變更路徑值，例如 `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`，如果他們從AEM發佈中繼資料結構表單，其中路徑不包含租用戶資訊，例如 `/etc/tags/<custom_tag_namespace>`。 |
| **[!UICONTROL 智慧標記]** | 如果您已購買並設定AEM智慧型標籤附加元件，則自動偵測標籤。 |
| **[!UICONTROL 隱藏欄位]** | 新增隱藏欄位。 儲存資產時，會以POST參數傳送。 |
| **[!UICONTROL 資產引用者]** | 新增此元件以檢視資產參考的資產清單。 |
| **[!UICONTROL 資產引用]** | 新增以顯示參考資產的資產清單。 |
| **[!UICONTROL 資產評等]** | 從AEM Assets新增資產在發佈至品牌入口網站之前的平均評分。 |
| **[!UICONTROL 關聯式中繼資料]** | 新增以控制資產「屬性」頁面中其他中繼資料標籤的顯示。 |

>[!NOTE]
>
>請勿使用&#x200B;**[!UICONTROL 產品參考]**，因為它無法正常運作。

#### 編輯元資料元件{#edit-the-metadata-component}

要編輯表單上元資料元件的屬性，請按一下該元件，然後在&#x200B;**[!UICONTROL Settings]**&#x200B;頁籤中編輯其屬性。

* **[!UICONTROL 欄位標籤]**:顯示在資產「屬性」頁面上的中繼資料屬性名稱。

* **[!UICONTROL 對應至屬性]**:此屬性的值為保存在CRX儲存庫中的資產節點提供相對路徑／名稱。開頭為&quot;**。/**」，因為這表示路徑位於資產的節點下。

以下是此屬性的有效值：

— `./jcr:content/metadata/dc:title`:將值儲存在資產的中繼資料節點，作為屬性[!UICONTROL `dc:title`]。

— `./jcr:created`:在資產節點顯示jcr屬性。 如果您在檢視屬性上設定這些屬性，建議您將它們標示為「停用編輯」，因為這些屬性受到保護。否則，當您儲存資產的屬性時，會出現「資產無法修改」錯誤。

* **[!UICONTROL 預留位置]**:使用此屬性可向使用者提供與中繼資料屬性相關的任何資訊。
* **[!UICONTROL 必要]**:使用此屬性可將中繼資料屬性標示為「屬性」頁面上的必要屬性。
* **[!UICONTROL 停用編輯]**:使用此屬性可讓中繼資料屬性在「屬性」頁面上無法編輯。
* **[!UICONTROL 在唯讀中顯示空白欄位]**:標籤此屬性可在「屬性」頁面上顯示中繼資料屬性，即使它沒有值亦然。預設情況下，當中繼資料屬性沒有值時，它不會列在「屬性」頁面上。
* **[!UICONTROL 說明]**:使用此屬性可為中繼資料元件新增簡短說明。
* **[!UICONTROL 刪除圖示]**:按一下此表徵圖可從架構表單中刪除元件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>所有中繼資料欄位都是資產的中繼資料編輯器形式中的唯讀欄位。 由於資產的中繼資料必須在AEM Assets中編輯，才能將資產發佈至品牌入口網站。

#### 在架構表單{#add-or-delete-a-tab-in-the-schema-form}中添加或刪除頁籤

預設模式表單包括&#x200B;**[!UICONTROL Basic]**&#x200B;和&#x200B;**[!UICONTROL Advanced]**&#x200B;頁籤。 架構編輯器可讓您新增或刪除標籤。

![](assets/add_delete_tabs_metadataschemaform.png)

* 要在模式表單上添加新頁籤，請按一下&#x200B;**[!UICONTROL +]**。 依預設，新標籤的名稱為「未命名-1」。 您可以從&#x200B;**[!UICONTROL Settings]**&#x200B;標籤中修改名稱。

![](assets/add-tab-metadata-form.png)

* 要刪除頁籤，請按一下&#x200B;**[!UICONTROL x]**。 按一下&#x200B;**[!UICONTROL 保存]**&#x200B;保存更改。

## 將元資料模式應用於{#apply-a-metadata-schema-to-a-folder}資料夾

品牌入口網站可讓您自訂和控制中繼資料結構，讓資產的&#x200B;**[!UICONTROL 屬性]**&#x200B;頁面僅顯示您選擇要顯示的特定資訊。 要控制顯示在&#x200B;**[!UICONTROL 屬性]**&#x200B;頁中的元資料，請從元資料模式表單中刪除所需的元資料，並將其應用到特定資料夾。

要將元資料結構表單應用於資料夾，請執行以下操作：

1. 從頂端的AEM工具列，按一下Adobe標誌以存取管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下&#x200B;**[!UICONTROL 元資料結構]**。

1. 從&#x200B;**[!UICONTROL 中繼資料結構表單]**&#x200B;頁面中，選取您要套用至資產的結構表單，例如&#x200B;**[!UICONTROL clothing]**。

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 在頂部的工具欄中，按一下&#x200B;**[!UICONTROL 應用到資料夾]**。

1. 從&#x200B;**[!UICONTROL 選擇資料夾]**&#x200B;頁面，導航到要應用&#x200B;**[!UICONTROL clothing]**&#x200B;元資料架構的資料夾，例如&#x200B;**[!UICONTROL Gloves]**。

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 按一下&#x200B;**[!UICONTROL Apply]**&#x200B;將元資料模式表單應用到資料夾。

   **[!UICONTROL clothing]**&#x200B;中繼資料架構表單中可用的中繼資料會套用至&#x200B;**[!UICONTROL Gloves]**&#x200B;檔案夾，並可在檔案夾的&#x200B;**[!UICONTROL Properties]**&#x200B;頁面中看到。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果您將包含巢狀結構描述的結構描述套用至包含視訊檔案的資料夾，則視訊檔案的中繼資料屬性可能無法正確呈現。 為確保元資料屬性正確顯示，請刪除嵌套的方案，並僅將父方案應用到資料夾。

## 刪除{#delete-a-metadata-schema-form}表單的元資料架構

品牌入口網站可讓您僅刪除自訂結構描述表單。 它不允許您刪除預設模式表單／模板。 不過，您可以刪除這些表單中的任何自訂變更。

要刪除表單，請選擇一個表單，然後按一下&#x200B;**[!UICONTROL Delete]**&#x200B;表徵圖。

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>刪除對預設表單所做的自定義更改後，**[!UICONTROL Lock]**&#x200B;符號將重新顯示在元資料架構介面上的表單名稱之前，以指示表單恢復為預設狀態。

## MIME類型{#schema-forms-for-mime-types}的架構表單

### 為MIME類型{#adding-new-forms-for-mime-types}添加新表單

除了預設表單外，您還可以為各種MIME類型的資產新增自訂表單，或在適當的表單類型下建立新表單。 例如，若要新增影像/png子類型 **[!UICONTROL 的新範本]** ，請在「影像」表單下建立表單。方案表單的標題是子類型名稱。在本例中，標題為&quot;png&quot;.

#### 對各種MIME類型{#using-an-existing-schema-template-for-various-mime-types}使用現有模式模板

您可以針對不同的MIME類型使用現有範本。 例如，對於MIME類型&#x200B;**image/png**&#x200B;的資產，請使用&#x200B;**image/jpeg**&#x200B;表單。

在這種情況下，請在CRX儲存庫的[!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`]處建立新節點。 指定節點的名稱並定義以下屬性：

| **名稱** | **類型** | **值** |
|---|---|---|
| 外露型 | 字串 | image/jpeg |
| mimetypes | String[] | image/png |

* **exposedmimetype**:要映射的現有表單的名稱
* **mimetypes**:使用exposedmimetypeattribute中定義的表單的MIME類 **** 型

品牌入口網站會對應下列MIME類型和架構表單：

| **架構表單** | **MIME類型** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | 視訊/avi，視訊/msvideo，視訊/x-msvideo |
| video/wmv | video/x-ms-wmv |
| 視訊/flv | video/x-flv |

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
