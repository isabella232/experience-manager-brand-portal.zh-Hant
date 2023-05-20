---
title: 使用中繼資料結構表單
seo-title: Use the metadata schema form
description: 元資料架構描述「屬性」頁的佈局以及為使用特定架構的資產顯示的元資料屬性。 您應用於資產的架構決定了在其「屬性」頁上顯示的元資料欄位。
seo-description: A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Admin
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 11%

---

# 使用中繼資料結構表單 {#use-the-metadata-schema-form}

元資料架構描述「屬性」頁的佈局以及為使用特定架構的資產顯示的元資料屬性。 您應用於資產的架構決定了在其「屬性」頁上顯示的元資料欄位。

的 **[!UICONTROL 屬性]** 每個資產的頁面包括預設元資料屬性，具體取決於資產的MIME類型。 管理員可以使用元資料架構編輯器修改現有架構或添加自定義元資料架構。 Experience Manager AssetsBrand Portal為各種MIME類型的資產提供預設表單。 但是，您也可以為此類資產添加自定義表單。

## 添加元資料架構窗體 {#add-a-metadata-schema-form}

要建立新的元資料架構表單，請執行以下操作：

1. 在頂部的工具欄中，按一下Experience Manager徽標以訪問管理工具。

   ![](assets/aemlogo.png)

1. 在「管理工具」面板中，按一下 **[!UICONTROL 中繼資料]** 結構。

   ![](assets/navigation-panel.png)

1. **[!UICONTROL 在「元資料結構 Forms]** 頁面上，按一下 **[!UICONTROL 建立]** 。

   ![](assets/create-metadata-schema-form.png)

1. 在 **[!UICONTROL 建立架構窗體]** 對話框，指定「架構」窗體的標題，然後按一下 **[!UICONTROL 建立]** 的子菜單。

   ![](assets/create-schema-form.png)

## 編輯元資料架構窗體 {#edit-a-metadata-schema-form}

可以編輯新添加的或現有的元資料架構表單。 元資料架構表單包含從其父級派生的內容，包括制表符內的制表符和表單項。 您可以將這些表單專案對應至中繼資料節點中的欄位。

您可以新增標籤或表單專案至中繼資料綱要表單。 派生的標籤和表單專案（來自父級）處於鎖定狀態。 您無法在子層級變更。

若要編輯中繼資料綱要表單，請執行下列操作：

1. 從頂部的工具列中，按一下 Experience Manager 標誌以存取「管理工具」。

   ![](assets/aemlogo.png)

1. 在「管理工具」面板中，按一下 **[!UICONTROL 中繼資料]** 結構。
1. 從 **[!UICONTROL 元資料架構Forms]** 頁，選擇要編輯其屬性的架構表單，例如， **[!UICONTROL 集合]**。

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >未編輯的模板前面顯示鎖定符號。 如果自定義任何模板，則模板消失之前的「鎖定」符號。

1. 在頂部的工具欄中，按一下 **[!UICONTROL 編輯]**。

   的 **[!UICONTROL 元資料架構編輯器]** 頁面 **[!UICONTROL 基本]** 頁籤 **[!UICONTROL 生成窗體]** 的上界。

1. 在 **[!UICONTROL 元資料架構編輯器]** 的子菜單。 **[!UICONTROL 屬性]** 從中的元件類型清單中拖動一個或多個元件， **[!UICONTROL 生成窗體]** 頁籤 **[!UICONTROL 基本]** 頁籤。

   ![](assets/metadata-schemaeditor-page.png)

1. 要配置元件，請選擇它並在 **[!UICONTROL 設定]** 頁籤。

### 「生成表單」頁籤中的元件 {#components-in-the-build-form-tab}

的 **[!UICONTROL 生成窗體]** 頁籤列出可在架構窗體中使用的項目。 的 **[!UICONTROL 設定]** 頁籤提供您在 **[!UICONTROL 生成窗體]** 頁籤。 下表列出了 **[!UICONTROL 生成窗體]** 頁籤：

| 元件名稱 | 說明 |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL 區段標題]** | 為公用元件清單添加節標題。 |
| **[!UICONTROL 單行文字]** | 添加單行文本屬性。 它儲存為字串。 |
| **[!UICONTROL 多值文本]** | 添加多值文本屬性。 它儲存為字串陣列。 |
| **[!UICONTROL 數字]** | 添加數字元件。 |
| **[!UICONTROL 日期]** | 添加日期元件。 |
| **[!UICONTROL 下拉式]** | 添加下拉清單。 |
| **[!UICONTROL 標準標記]** | 新增標記. **注：** 管理員可能需要更改路徑值，例如， `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`，如果它們從Experience Manager Assets發佈元資料架構表單，其中路徑不包括租戶資訊，例如， `/etc/tags/<custom_tag_namespace>`。 |
| **[!UICONTROL 智慧標記]** | 如果已購買並配置了Experience Manager Assets智慧標籤附加模組，則自動檢測標籤。 |
| **[!UICONTROL 隱藏欄位]** | 添加隱藏欄位。 保存資產時，它將作為POST參數發送。 |
| **[!UICONTROL 資產引用者]** | 添加此元件以查看資產引用的資產清單。 |
| **[!UICONTROL 資產引用]** | 添加以顯示引用資產的資產清單。 |
| **[!UICONTROL 資產評等]** | 在Experience Manager Assets發佈到Brand Portal之前，從添加的資產的平均評級。 |
| **[!UICONTROL 關聯式中繼資料]** | 添加以控制資產「屬性」頁中其他元資料頁籤的顯示。 |

>[!NOTE]
>
>不使用 **[!UICONTROL 產品參考]**，因為它不起作用。

#### 編輯元資料元件 {#edit-the-metadata-component}

要編輯表單上元資料元件的屬性，請按一下該元件並在 **[!UICONTROL 設定]** 頁籤。

* **[!UICONTROL 欄位標籤]**:顯示在資產的「屬性」頁上的元資料屬性的名稱。

* **[!UICONTROL 映射到屬性]**:此屬性的值提供了保存在CRX儲存庫中的資產節點的相對路徑/名稱。 它以&quot;開頭&#x200B;**。/**&#x200B;因為表示路徑位於資產的節點下。

以下是此屬性的有效值：

— `./jcr:content/metadata/dc:title`:將資產的元資料節點上的值儲存為屬性 [!UICONTROL `dc:title`]。

— `./jcr:created`:在資產的節點顯示jcr屬性。 如果您在檢視屬性上設定這些屬性，建議您將它們標示為「停用編輯」，因為這些屬性受到保護。否則，當您儲存資產的屬性時，會出現「資產無法修改」錯誤。

* **[!UICONTROL Placeholder]** ：使用此屬性提供有關中繼資料屬性的用戶相關資訊。
* **[!UICONTROL 必要]** ：使用此屬性，在屬性頁面上將中繼資料屬性標記為強制性。
* **[!UICONTROL 禁用編輯]**:使用此屬性可使元資料屬性在「屬性」頁上不可編輯。
* **[!UICONTROL 以只讀方式顯示空欄位]**:將此屬性標籤為在「屬性」頁上顯示元資料屬性，即使它沒有值。 預設情況下，當元資料屬性沒有值時，該屬性不會列在「屬性」頁上。
* **[!UICONTROL 說明]**:使用此屬性可為元資料元件添加簡短說明。
* **[!UICONTROL 刪除圖示]** ：按一下此圖示可從「綱要」表單中刪除元件。

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>所有中繼資料欄位在資產的中繼資料編輯者表單中均為唯讀。 因為資產的中繼資料必須先在 Experience Manager Assets 中進行編輯，才會將資產發佈到品牌入口網站。

#### 在綱要表單中新增或刪除標籤 {#add-or-delete-a-tab-in-the-schema-form}

預設綱要表單包含 **[!UICONTROL 基本]** 和 **[!UICONTROL 進階]** 標籤。 架構編輯器可讓您新增或刪除標籤。

![](assets/add_delete_tabs_metadataschemaform.png)

* 要在架構表單上添加新頁籤，請按一下 **[!UICONTROL +]**。 預設情況下，新頁籤的名稱為「未命名–1」。 可以從 **[!UICONTROL 設定]** 頁籤。

![](assets/add-tab-metadata-form.png)

* 要刪除頁籤，請按一下 **[!UICONTROL x]**。 按一下 **[!UICONTROL 保存]** 的子菜單。

## 將元資料架構應用於資料夾 {#apply-a-metadata-schema-to-a-folder}

Brand Portal允許您自定義和控制元資料架構，以便 **[!UICONTROL 屬性]** 資產的頁面僅顯示您選擇顯示的特定資訊。 控制在中顯示的元資料 **[!UICONTROL 屬性]** 頁，從元資料架構表單中刪除所需的元資料並將其應用於特定資料夾。

要將元資料架構表單應用於資料夾，請執行以下操作：

1. 在頂部的工具欄中，按一下Experience Manager徽標以訪問管理工具。

   ![](assets/aemlogo.png)

1. 在管理工具面板中，按一下 **[!UICONTROL 元資料架構]**。

1. 從 **[!UICONTROL 元資料架構Forms]** 頁，選擇要應用於資產的架構表單，例如， **[!UICONTROL 衣服]**。

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. 在頂部的工具欄中，按一下 **[!UICONTROL 應用於資料夾]**。

1. 從 **[!UICONTROL 選擇資料夾]** 頁，導航到要應用的資料夾 **[!UICONTROL 衣服]** 例如，元資料架構 **[!UICONTROL 手套]**。

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. 按一下 **[!UICONTROL 應用]** 將元資料架構窗體應用於資料夾。

   中的可用元資料 **[!UICONTROL 衣服]** 元資料架構窗體應用於 **[!UICONTROL 手套]** 資料夾中顯示 **[!UICONTROL 屬性]** 的子菜單。

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>如果將包含嵌套架構的架構應用到包含視頻檔案的資料夾，則視頻檔案的元資料屬性可能無法正確呈現。 要確保元資料屬性正確呈現，請刪除嵌套架構，並僅將父架構應用於資料夾。

## 刪除元資料架構窗體 {#delete-a-metadata-schema-form}

Brand Portal允許您僅刪除自定義架構表單。 它不允許您刪除預設架構表單/模板。 但是，您可以刪除這些表單中的任何自定義更改。

要刪除表單，請選擇一個表單，然後按一下 **[!UICONTROL 刪除]** 表徵圖

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>刪除對預設表單所做的自定義更改後， **[!UICONTROL 鎖]** 符號在元資料架構介面上的表單名稱前重新顯示，以指示表單已恢復為預設狀態。

## MIME類型的架構表單 {#schema-forms-for-mime-types}

### 為MIME類型添加新表單 {#adding-new-forms-for-mime-types}

除了預設表單外，您還可以為各種MIME類型的資產添加自定義表單，或在適當的表單類型下建立新表單。 例如，若要新增影像/png子類型 **[!UICONTROL 的新範本]** ，請在「影像」表單下建立表單。方案表單的標題是子類型名稱。在本例中，標題為&quot;png&quot;.

#### 將現有架構模板用於各種MIME類型 {#using-an-existing-schema-template-for-various-mime-types}

您可以將現有模板用於其他MIME類型。 例如，使用 **影像/jpeg** MIME類型資產的窗體 **影像/png**。

在這種情況下，在 [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] 的下界。 指定節點的名稱並定義以下屬性：

| **名稱** | **類型** | **值** |
|---|---|---|
| 暴露型 | 字串 | image/jpeg |
| mimetype | 字串[] | image/png |

* **暴露型**:要映射的現有窗體的名稱
* **mimetype**:使用中定義的表單的MIME類型清單 **暴露型** 屬性

Brand Portal映射以下MIME類型和架構表單：

| **架構窗體** | **MIME類型** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | 影像/x-tiff |
| application/pdf | application/postscript |
| 應用程式/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| 應用程式/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi、video/msvideo、video/x-msvideo |
| 視頻/wmv | video/x-ms-wmv |
| 視頻/flv | video/x-flv |

以下是預設元資料屬性的清單：

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr：內容/元資料/視頻編解碼器
* jcr：內容/元資料/音頻編解碼器
* jcr：內容/元資料/dc:title
* jcr：內容/元資料/dc：說明
* jcr：內容/中繼資料/xmpMM： InstanceID
* jcr：內容/中繼資料/xmpMM： DocumentID
* jcr：內容/中繼資料/dam： sha1
* jcr：內容/中繼資料/dam： solutionCoNtext
* jcr：內容/中繼資料/videoBitrate
* jcr：內容/元資料/音頻比特率
* jcr：內容/使用實例/使用者
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr：內容/開始時間
* jcr：內容/關機時間
* jcr:content/metadata/dam:size
* jcr：內容/元資料/tiff:ImageWidth
* jcr：內容/元資料/tiff:ImageLength
