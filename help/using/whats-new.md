---
title: AEM Assets品牌入口網站的新增功能
seo-title: AEM Assets品牌入口網站的新增功能
description: 檢視6.4.4的新功能和增強功能。
seo-description: 檢視6.4.4的新功能和增強功能。
uuid: 2c59d738-9b53-4f25-a205-13bb75 c80 b77
contentOwner: bdhar
products: SG_ PERIENCENCENAGER/Brand_ Portal
content-type: 引用
topic-tags: 簡介
discoiquuid: fec32ca3-214b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: cbb64eb8a79480a1ccedbe5131a38ddf6eaec88d

---


# AEM Assets品牌入口網站的新增功能 {#what-s-new-in-aem-assets-brand-portal}

Adobe Experience Manager(AEM) Assets Brand Portal可協助您輕鬆地取得、控制並安全地將已核准的創意資產發佈給外部廠商和內部業務使用者。它有助於提高資產共用的效率、加快資產的上市時間，並降低不符合規定和未經授權存取的風險。Adobe正在努力改善整體品牌入口網站體驗。搶先一窺新功能和增強功能。

## 6.4.4版變更內容 {#what-is-changing-in}

Brand Portal6.4.4版本著重於文字搜尋和主要客戶要求的增強功能。請參閱最新 [品牌入口網站發行說明](brand-portal-release-notes.md)。

### 搜尋增強功能 {#search-enhancements}

品牌入口網站6.4.4在篩選窗格中支援部分文字搜尋在屬性預覽中。若要允許部分文字搜尋，您必須在 **搜尋表單中啓用「屬性Predicate** 」中的「部分搜尋」。

閱讀更多有關部分文字搜尋和萬用字元搜尋的資訊。

#### 部分片語搜尋 {#partial-phrase-search}

您現在可以在篩選窗格中只指定一部分(或兩個)的部分，以搜尋資產。

**使用案例**&#x200B;當您不確定在搜尋的片語中出現的單字確切組合時，部分片語搜尋很有用。

例如，如果您在品牌入口網站中的搜尋表格使用屬性Predicate來部分搜尋資產標題，則指定詞語 **營會** 將所有資產連同字詞片語填入其標題片語中。

![](assets/partialphrasesearch.png)

#### 萬用字元搜尋 {#wildcard-search}

品牌入口網站允許在搜尋查詢中使用星號(*)以及搜尋片語中的部分字詞。

**使用案例**：如果您無法確定搜尋到的片語中所出現的確切字詞，您可以使用萬用字元搜尋來填補搜尋查詢中的空隙。

例如，指定 **爬升*會** 在品牌入口網站中的搜尋表格使用屬性Predicate做為部分搜尋資產標題的屬性Predicate時，傳回字元開頭 **的** 所有資產。

![](assets/wildcard-prop.png)

同樣地，指定：

* ***爬升** 會傳回所有具有字元結尾字詞 **的** 資產。

* ***爬升*** 會傳回所有包含字元的字詞，這些字詞包含 **** 其標題片語中的字元。

>[!NOTE]
>
>選取 **部分搜尋** 核取方塊時，預設會選取 **忽略大小寫** 。

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## 6.4.3中的變更 {#what-changed-in}

Brand Portal6.4.3版本著重於—為組織提供替代別名，除了品牌入口網站存取URL中的租用用戶ID、新資料夾階層設定、視訊支援增強功能、排程發佈從AEM作者實例到品牌入口網站、作業增強功能—並滿足客戶要求。

### 非管理員的資料夾階層導覽

管理員現在可以設定如何在登入時向非管理員使用者(編輯、檢視者和來賓使用者)顯示資料夾。[「啓用資料夾階層](../using/brand-portal-general-configuration.md) 」設定會新增至管理工具面板中的 **一般設定**&#x200B;中。如果設定為：

* **已啓用**，從根資料夾開始的資料夾樹狀結構會顯示給非管理員使用者。因此，授予他們類似於管理員的導覽體驗。
* **停用**，則只有共用資料夾會顯示在登陸頁面上。

![](assets/enable-folder-hierarchy.png)**使用案例**

[「啓用資料夾階層](../using/brand-portal-general-configuration.md) 」功能(啓用時)可協助您區分與不同階層共用的相同名稱。登入時，非管理員使用者現在會看到共用資料夾的虛擬父資料(和系列)資料夾。![](assets/disabled-folder-hierarchy1-2.png)![](assets/enabled-hierarchy1-2.png)


共用資料夾會組織在虛擬檔案夾中的個別目錄內。您可以使用鎖定圖示辨識這些虛擬資料夾。

請注意，虛擬檔案夾的預設縮圖是第一個共用資料夾的縮圖影象。

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### 在特定資料夾階層或路徑中搜尋

**路徑瀏覽器** 首碼會引入搜尋表單中，以允許搜尋特定目錄中的資產。路徑瀏覽器的搜尋預覽路徑預設搜尋路徑為 */content/dam/mac/&lt; tenant-id&gt;/*，可透過編輯預設搜尋表單來設定。

* 管理員使用者可使用路徑瀏覽器瀏覽至品牌入口網站上的任何資料夾目錄。
* 非管理員使用者可以使用路徑瀏覽器，只導覽至與其共用的資料夾(並導覽至上層資料夾)。
例如， */content/dam/mac/&lt; tenant-id&gt;/FolderA/FolderB/FolderC* 會與非管理員使用者共用。使用者可使用路徑瀏覽器在FolderC中搜尋資產。此使用者也可以導覽至FolderB和FolderA(因為它們是共用給使用者的FolderC擁有權)。

![](assets/edit-search-form.png)

**使用案例**

您現在可以限制您瀏覽的特定資料夾內的資產搜尋，而不是從根資料夾開始。

請注意，在這些資料夾下搜尋只會傳回已與使用者共用的資產結果。

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### 動態媒體視訊轉譯支援

AEM作者實例採用Dynamic Media混合模式的使用者，除了原始的視訊檔案外，還可以預覽並下載動態媒體轉譯。

為允許在特定租用戶帳戶上預覽和下載動態媒體轉譯，管理員必須在管理工具面板中指定 **動態媒體設定** (視訊服務URL)和註冊ID，以便在 **視訊** 設定中擷取動態視訊)。

**您可以在下列位置預覽**&#x200B;動態媒體影片：

* 資產詳細資料頁面
* 資產卡片檢視
* 連結共用預覽頁面

動態媒體視訊編碼可從下列位置下載：

* 品牌入口網站
* 共用連結

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 已排程發佈至品牌入口網站

將工作流程從 [AEM(6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) 發佈到品牌入口網站的資產(和資料夾)發佈工作流程可排定稍後的日期。

同樣地，在稍後的日期(時間)中，您可以排程「取消發佈品牌入口網站」工作流程，從入口網站移除已發佈資產。

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### URL中可設定的租用戶別名

組織可以在URL中使用替代首碼，自訂其入口網站URL。若要在現有入口網站URL中取得用戶名稱別名，組織必須聯絡Adobe支援。

請注意，只能自訂品牌入口URL的前置詞，而不是整個URL。\
例如，具有現有網域 **geomettrix.brand-portal.adobe.com** 的組織可以取得 **在請求上建立的geomettrixinc.brand-portal.adobe.com** 。

不過，AEM作者實例只能 [透過](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) 租用戶id URL設定，而不能使用租用戶別名(替代) URL設定。

**使用案例**&#x200B;組織可自訂入口網站URL，而不需堅守Adobe提供的URL，以符合其品牌需求。

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### 下載體驗增強功能

此版本提供簡化的下載體驗，並可減少點按次數和警告次數，並提供下列功能：

* 選擇僅下載轉譯(而非原始資產)。
* 在存取原始轉譯時下載資產。

## 6.4.2版變更內容 {#what-changed-in-1}

Brand Portal6.4.2發行提供多種功能，以滿足組織的資產發送需求，並協助透過客戶存取及使用加速下載的最佳化體驗觸及全球大量使用者。品牌入口網站也透過管理員新設定、新加入的報告以及滿足客戶要求，為組織提供更佳的控制權。

### 訪客存取

![](assets/bp-login-screen-1.png)

AEM品牌入口網站可讓來賓存取入口網站。來賓使用者不需要認證才能進入入口網站，並且可以存取並下載所有公用資料夾和系列。來賓使用者可以將資產新增至其燈箱(私人系列)並下載相同的內容。他們也可以檢視由管理員設定的智慧標籤搜尋和搜尋預測。來賓作業不允許使用者建立系列和儲存的搜尋、進一步存取資料夾和系列設定，以及將資產共用為連結。

在組織中，允許多個並行訪客作業，其限定僅限每組織使用者配額的10%。

訪客工作階段會持續運作兩小時。因此，燈箱的狀態也會保留，直到從工作階段開始時間開始為止。在兩小時後，來賓作業必須重新啓動，因此燈箱狀態會遺失。

### 加速下載

Brand Portal使用者可運用以IBM Assera Connect為主的快速下載功能，快速下載速度加快25倍，並體驗順暢下載體驗，不論其位置為何。若要從品牌入口網站或共用連結更快下載資產，使用者必須在下載對話方塊中選取 **「啓用下載加速」** 選項，如此就可在其組織中啓用下載加速。

![](assets/donload-assets-dialog-2.png)

若要啓用組織的IBM Assera加速下載，管理員 **可從管理工具面板中的一般設定啓用「啓用下載加速**[](brand-portal-general-configuration.md#allow-download-acceleration) 」選項(預設停用)。若要更深入瞭解從品牌入口網站和共用連結下載資產檔案的必要條件和疑難排解步驟，請參閱 [指南以加速從品牌入口網站下載](../using/accelerated-download.md#main-pars-header)。

### 使用者登入報告

已推出追蹤使用者登入的新報表。**「使用者登入** 」報告可協助組織檢查並檢查委派管理員及品牌入口網站的其他使用者。

報表會記錄來自品牌入口網站6.4.2部署的每位使用者的名稱、電子郵件ID、個人化(管理員、檢視器、編輯者、訪客)、群組、上次登入、活動狀態和登入計數，直到產生報告為止。管理員可以將報表匯出為. csv。使用者登入報告可讓組織更密切地監控使用者與已核准品牌資源的互動情況，進而確保公司遵循辦公室的一致性。

![](assets/user-logins-1.png)

### 存取原始轉譯

管理員可以限制使用者存取原始影像檔案(.jpeg、. tiff、. png、. bmp、. gif、. pjpg、x-able-any map、x-portable-bitmap、x-portable-any map、x-portable-any map、x-domable-pitmap、x-domable-premap、x-clip-premap、x-publish-pimap、x-clip、image/photoshop、image/vnd. adobe. photoshop)，可存取從品牌入口網站或共用連結下載的低解析度轉譯。這項存取可在管理工具面板的使用者角色頁面的使用者群組層級控制。

![](assets/access-original-rend-1.png)

* 依預設，所有使用者都可以下載原始轉譯，因為對所有使用者都啓用了原始轉譯。
* 管理員需要取消選取個別核取方塊，以避免使用者群組存取原始轉譯。
* 如果使用者是多個群組的成員，但只有其中一個群組有限制，則限制適用於該使用者。
* 這些限制不適用於管理員，即使是受限制群組成員亦然。
* 使用者共用資產的權限會套用至使用共用連結下載資產的使用者。

### 卡片和清單檢視上的資料夾階層路徑

資料夾卡片在「卡片檢視」中，現在會顯示資料夾階層資訊給非管理員使用者(編輯者、檢視者和訪客使用者)。這項功能可讓使用者知道資料夾的位置，以及存取父階層的位置。

資料夾階層資訊對於區分資料夾的區別特別有用，此資料夾類似於其他資料夾階層共用的資料夾。如果非管理員使用者不知道與其共用資產的資料夾結構，具有類似名稱的資產/folders會造成混淆。

* 顯示在個別卡片上的路徑會被截斷，以符合卡片大小。不過，使用者可以將完整路徑視為停留在截斷路徑上的工具提示。

![](assets/folder-hierarchy1-1.png)

清單檢視顯示欄中的資產路徑給品牌入口網站的所有使用者。

![](assets/list-view-1.png)

### 檢視資產屬性的概述選項

品牌入口網站提供「概述」選項給非管理員使用者(編輯、檢視者、訪客使用者)，以檢視所選資產/檔案夾的資產屬性。「概述」選項可顯示：

1. 位於上方的工具列中，選取資產/檔案夾。
2. 在下拉式清單中，選取「邊欄選擇器」。

在選取資產/資料夾時選取「概述」選項時，使用者可以查看資產建立的標題、路徑和時間。而在資產詳細資料頁面選取「概述」選項時，使用者可查看資產的中繼資料。

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## 新組態

系統會新增個新設定，讓管理員啓用/停用特定租用戶的下列功能：

* 允許訪客存取
* 允許使用者要求存取品牌入口網站
* 允許管理員從品牌入口網站刪除資產
* 允許建立公用系列
* 允許建立公開智慧型系列
* 允許下載加速

上述設定可在管理工具面板的「存取」和「一般」設定下使用。

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe. io主機UI可設定OAuth整合

品牌入口網站6.4.2Onward使用Adobe. io [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) 介面建立JWT應用程式，此應用程式可讓您設定OAuth整合，以便與品牌入口網站整合AEM Assets。以前，設定OAuth整合的UI是以 [https://marketing.adobe.com/developer/代管](https://marketing.adobe.com/developer/)。若要深入瞭解將AEM資產與品牌入口網站整合，以便發佈資產和系列至品牌入口網站，請參閱 [「設定AEM資產與品牌入口網站](https://helpx.adobe.com/in/experience-manager/6-4/assets/using/brand-portal-configuring-integration.html)」。

## 搜尋增強功能

管理員可以使用更新的屬性Predicate(檢查忽略大小寫)，讓屬性預覽不區分大小寫。此選項適用於屬性predicate和多值屬性預設值。\
但是，非區分大小寫搜尋比預設搜尋屬性預設速度慢。如果搜尋篩選器中有太多不區分大小寫的Predicates，搜尋可能會減慢速度。因此，建議您謹慎使用非區分大小寫搜尋。

## 6.4.1版變更 {#what-changed-in-2}

Brand Portal6.4.1是平台升級版本，提供多種新功能和重要增強功能，例如瀏覽、搜尋和效能增強功能，以滿足客戶的體驗。

### 瀏覽增強功能

* 新的「內容樹狀結構」邊欄可快速導覽資產階層。

![](assets/contenttree-2.png)

* 推出新的鍵盤快速鍵，例如 _(p)_ 用於屬性頁面導覽、 _(e)_ 用於編輯，以及 _(ctrl+ c)_ 複製作業。
* 改善卡片和清單檢視中的捲動體驗，以瀏覽大量資產。
* 增強的卡片檢視，可支援根據檢視設定支援不同大小的卡片。

![](assets/cardviewsettings-1.png)

* 卡片檢視現在會在日期標籤上方的停留上顯示日期/時間戳記。

* 增強「欄」檢視，在資產快照下具有 **更多詳細資料** ，可讓您導覽至資產的詳細資料頁面。

![](assets/columnmoredetail.png)

* 清單檢視現在預設會在第一欄顯示資產名稱，除了地區設定、資產類型、維度、大小、分級和出版物資訊之外。「新 **的檢視設定** 」可用來設定在清單檢視中顯示的詳細程度。

* 改進資產詳細資料體驗，能夠使用新的導覽按鈕來回瀏覽資產，並檢視資產計數。

![](assets/navbtn.png)

* 在資產詳細資料頁面上預覽音訊檔案，從AEM上傳的新功能。
* 資產屬性中提供的新「相關資產」功能。與其他來源/衍生資產相關的資產(AEM上的其他來源/衍生資產)現在已在品牌入口網站中保持不變，並連結至屬性頁面上的相關資產。
* 已引進新設定以限制非管理員使用者建立公用系列。組織可與Adobe支援團隊合作，在特定帳戶上設定此功能。

### 搜尋增強功能

* 在導覽至搜尋項目後，會引入到搜尋結果中相同位置的功能，而不需再次執行搜尋查詢。
* 新增搜尋結果計數以顯示搜尋結果的數目。
* 改進檔案類型搜尋篩選器，能夠根據較精細的MIME類型(例如.jpg、. png和. psd)篩選搜尋結果，並與舊版影像、文件、多媒體選項進行比較。
* 增強的系列搜尋篩選器，具有精確的時間戳記，而非先前的時間滑桿功能。
* 已推出新的存取類型篩選，可搜尋為公用或非公開的系列。

![](assets/accesstypefilter.png)

### 下載最佳化

* 直接下載單一大型檔案，毋需建立zip檔案，進而提高速度和總處理能力。
* 連結共用功能的郵遞區號下載限制已從GB增加至GB。

* 使用者現在可以選擇僅下載自訂和原始檔案，並防止立即可用的轉譯，同時從品牌入口網站或透過共用連結功能下載資產。

![](assets/excludeautorendition.png)

### 效能增強

* 提升資產下載速度高達100%。
* 資產搜尋回應的改進高達40%。
* 瀏覽效能提升40%。

**注意**：指名的改進取決於實驗室中進行的測試。

### 增強的報告功能

**引入的連結共用報表**&#x200B;我們推出了一個新報表，提供共用連結的相關資訊。「連結共用」報表會將所有URL與指定時間範圍內的內部和外部使用者共用。它也會在共用連結、由誰和何時過期時通知。

![](assets/navigatereport.png)

**已修改進入點以存取「使用狀況」報表**「使用狀況」報表現在已與其他報表合併，現在可以從「資產報表」控制台檢視。若要觸及「資產報表」主控台，請導覽至 **「從管理工具面板建立/管理報表** 」。

![](assets/accessassetreport.png)

**在品牌入口網站上報告**&#x200B;報告介面的使用者體驗已變得更具直覺性，並為組織提供更大的控制權。除了建立各種報表外，管理員現在還可以重新造訪產生的報告，並下載或刪除這些報表，因為這些報表會儲存在品牌入口網站中。

每個建立的報表都可以借由新增或移除預設欄加以自訂。此外，可新增自訂欄至「下載」、「到期」和「發佈」報表，以控制其詳細程度。

### 改良的管理工具

改進中繼資料、搜尋和報表的管理工具中的屬性選擇器，具有前置及瀏覽功能以簡化管理體驗。

### 其他增強功能

* 從AEM6.3.2.1和6.4發佈至品牌入口網站的資產現在可以透過標示AEM Assets品牌「入口網站複製」對話方塊上的「公開資料夾發佈」核取方塊，向品牌入口網站的一般使用者提供。

![](assets/public-folder-publish.png)

* 如果有人要求存取品牌入口網站，則系統會透過存取要求電子郵件通知管理員，而非品牌入口網站通知區域中的通知。

## 6.3.2版變更內容 {#what-changed-in-3}

Brand Portal6.3.2包含針對主要客戶要求和一般效能增強功能的全新和增強功能。

### 要求存取品牌入口網站 {#request-access-to-brand-portal}

使用者現在可以要求使用新****存取品牌入口網站存取品牌入口網站的登入畫面。

![](assets/bplogin_request_access.png)

根據使用者是否擁有Adobe ID或需要建立Adobe ID，使用者可以依照適當的工作流程提交請求。品牌入口網站產品管理員會在其通知區域收到此類要求，並透過Adobe Admin Console授予存取權。

如需詳細資訊，請參閱 [「要求品牌入口網站存取](../using/brand-portal.md#requestaccesstobrandportal)」。

### 資產下載報告中的增強功能 {#enhancement-in-the-assets-downloaded-report}

資產下載的報告現在會在指定的日期和時間範圍內，納入每位使用者的資產下載計數。使用者可以下載此報告，以. csv格式下載，並編譯授權資產的總下載計數等資料。

![](assets/reports_download_downloaded_by.png)

如需詳細資訊，請參閱 [建立和管理其他報表中的步驟和6](../using/brand-portal-reports.md#createandmanageadditionalreports)。

### 品牌入口網站維護通知 {#brand-portal-maintenance-notification}

品牌入口網站現在會在即將到來的維護活動前幾天顯示通知橫幅。範例通知：

![](assets/bp_maintenance_notification-1.png)

如需詳細資訊，請參閱 [品牌入口網站維護通知](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)。

### 使用連結共用功能來增強共用資產的增強功能 {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

在使用連結共用功能下載授權資產時，現在會提示您同意這些資產的授權合約。

![](assets/copyright_management.png)

如需詳細資訊，請參閱「共用資產中 [的步驟12」做為連結](../using/brand-portal-link-share.md#shareassetsasalink)。

### 使用者選擇器增強功能 {#user-picker-enhancement}

使用者選擇器效能現在已增強為迎合擁有龐大使用者群之客戶的需求。

### Experience Cloud品牌變更 {#experience-cloud-branding-changes}

品牌入口網站現在符合新的Adobe Experience Cloud品牌。

![](assets/bp_solution_switcher.png)

## 6.3.1版變更內容 {#what-changed-in-4}

Brand Portal6.3.1包含與AEM對齊品牌入口網站的新功能和增強功能。

### 升級的使用者介面 {#upgraded-user-interface}

為了與AEM對齊品牌入口網站使用者體驗，Adobe正在轉換至Coral使用者介面。此項變更可增強整體可用性，包括導覽和外觀。

#### 增強導覽體驗 {#enhanced-navigational-experience}

* 透過全新的Adobe標誌快速存取管理工具：

![](assets/aemlogo-3.png)

* 透過覆蓋導覽產品：

![](assets/overlay_navigation.png)

* 快速導覽至父資料夾：

![](assets/navigationparentfolders.png)

* 快速搜尋並導覽至必要的內容和工具：

![](assets/omnisearchicon.png)

### 增強瀏覽體驗 {#enhanced-browsing-experience}

* 新欄檢視可瀏覽巢狀資料夾：

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* 在資料夾中的資產清單中，上傳的最新資產會顯示在頂端。

### 增強搜尋體驗 {#enhanced-search-experience}

* 全新的Omni搜尋功能可讓您在輸入搜尋關鍵字時，透過自動建議快速存取相關內容、功能或標籤。Omni搜尋適用於所有搜尋功能。

![](assets/omnisearch_whatsnew.png)

* 您也可以將搜尋篩選器新增至Omni搜尋，進一步縮小搜尋範圍並加快搜尋速度。

![](assets/omnisearch_withfilters.png)

* 新的資產分級搜尋功能可讓您在AEM Assets中搜尋具有評分的資產。
* 新的多值搜尋功能可使用AND運算子接受多個關鍵字，以更快地發現資產。
* 全新的搜尋增強功能可讓您改善搜尋相關性，讓特定資產出現在搜尋結果頂端。
* 新的路徑型搜尋功能可讓您提供巢狀資料夾的路徑，以便在該資料夾中搜尋資產。

#### 全新智慧標籤型搜尋 {#new-smart-tags-based-search}

如果使用智慧標記的影像從AEM Assets發佈至品牌入口網站，您可以使用智慧標籤名稱作為搜尋關鍵字，在品牌入口網站中搜尋這些影像。此功能僅適用於檔案。

### 增強下載體驗 {#enhanced-downloading-experience}

下載巢狀資料夾後，您可以保留原始資料夾階層。巢狀資料夾內的資產可在單一資料夾中下載，而非個別資料夾。

### 效能提升 {#improved-performance}

瀏覽、搜尋和下載功能中的增強功能可大幅改善品牌入口網站效能。

### 新的資產數位版權管理 {#new-digital-rights-management-for-assets}

管理員可以在共用資產之前，先設定資產的過期日期和時間。資產到期後，檢視器和編輯器便會顯現，但無法下載。當資產過期時，管理員會收到通知。

### 增強資產排序 {#enhanced-asset-sorting}

清單檢視資料夾中的資產排序不再局限於第一頁顯示的資產數。資料夾中的所有資產都會排序，不論第一頁是否列出所有資產。

### 增強報告功能 {#reporting-capabilities}

管理員可以建立並管理三種報表類型-下載、過期和發佈的資產。也可以將報表設定為報表中的欄，並將報表匯出為CSV格式。

![](assets/newreport.png)

### 其他 Metadata {#additional-metadata}

Brand Portal6.3.1引入其他中繼資料，與AEM Assets6.3相同。您可以使用結構編輯器表單來控制資產屬性頁面上應該顯示的中繼資料。外部連結共用使用者看不到資產中繼資料，使用者只能使用連結共用URL預覽和下載資產。

![](assets/additionsinmetadata.png)

### 管理員的額外功能 {#additional-capabilities-for-administrators}

* 在將自訂設定為登入畫面布紙之前，管理員可以預覽變更。

![](assets/wallpaperpreview.png)

* 管理員新增使用者後，不需要接受邀請加入品牌入口網站，就會自動新增邀請。

### AEM Assets6.3中的新發佈功能 {#new-publishing-capabilities-in-aem-assets}

* AEM管理員可使用AEM6.3SP1-CFP1(6.3.1.1)將中繼資料結構發佈至品牌入口網站，此功能將於2017年第季推出。

![](assets/publish_metadataschemaaemassets.png)

* AEM管理員可以使用AEM6.2SP1-CFP和AEM6.3 SP1-CFP1(6.3.1.1)，將所有標籤從AEM Assets發佈至品牌入口網站。

![](assets/publish_tags_aemassets.png)

* 從AEM Assets，您可以發佈具有標記(包括智慧標籤)的資產和系列。然後，您可以在品牌入口網站中使用這些標記搜尋這些資產或系列，作為搜尋關鍵字。

## Frequently asked questions {#frequently-asked-questions}

**隨堂測驗。我會失去我建立的任何現有資產、功能或組態的存取權嗎？****ans。** 您所有現有的功能和組態都將完整保留。您的使用者不受影響，您的內容將不受影響。

**Ks.我何時會移至新版品牌入口網站？****ans。** 品牌入口網站6.4.4於2019年月發行。下一個品牌入口網站版本預計於19日發行。

>[!NOTE]
>
>發行排程為暫定，可能會變更。請聯絡您的Adobe客戶經理或客戶支援，以取得更新的發行排程。

**Ks.我的使用者會受到影響嗎？****ans。** 此項變更僅限於品牌入口網站，因此對使用者沒有影響。

**Ks.我是否需要任何動作？****ans。** 管理員無需採取任何動作。一旦您存取新的品牌入口網站後，請參閱說明文件以檢視所有的黑白郵件。

**Ks.我要與誰聯絡？****ans。** 請聯絡您的Adobe客戶經理或客戶支援。
