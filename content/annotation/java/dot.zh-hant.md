---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DOT Annotation API C# 中的註釋"
head_description: "Java API 用於從 DOT、圖像、繪圖和文檔文件格式創建和註釋流行的註釋類型。"

############################# Header ############################
title: "從 Java 註釋 DOT"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "下載免費試用版"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "關於 Java API 的 GroupDocs.Annotation"
    content: |
        GroupDocs.Annotation for Java API 是一個庫，允許您在 Mac、Windows 或 Ubuntu 上向 PDF、Word 和其他文檔添加註釋。 [GroupDocs.Annotation for Java](/annotation/java) 是一個用於管理註釋的原生 Java API，全面支持從圖像和各種其他文檔中創建、添加、編輯、刪除、提取和導出註釋。您可以在此[頁面](https://docs.groupdocs.com/annotation/java/supported-document-formats/)上看到支持的文檔格式的完整列表。
        該庫不僅允許您處理 DOT 文檔，還可以處理許多其他類型的文檔，例如 Word、Excel、PowerPoint、Outlook 電子郵件、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad 等。
        GroupDocs.Annotation for Java API 允許您創建和添加新註釋、編輯註釋、提取註釋、註釋以及從文檔中刪除它們。該庫支持13 種不同的註釋類型，包括文本、折線、區域、下劃線、點、水印、箭頭、橢圓、文本替換、距離、文本字段、PDF、HTML、Microsoft Word 文檔、電子表格、圖表、演示文稿中的資源編輯，繪圖、圖像和許多其他文件格式。
        該示例（請參見下文）演示瞭如何使用 DOT 文檔，在此示例中您可以看到如何使用 GroupDocs 的主要步驟。註釋：設置許可證、打開要使用的文檔、創建註釋，根據需要添加數據對象設置註釋屬性，並將結果保存到需要的地方。您還可以在我們的 github [頁面](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) 或我們的產品 [文檔](https://docs.groupdocs.com/annotation/java/getting-started/)。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "在 Java 中向 DOT 添加註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通過實施幾個簡單的步驟，Java 開發人員可以輕鬆地將各種註釋類型添加到任何基於 Java 的應用程序中的 DOT 文件。
        *   創建帶有評論和日期的 Reply 對象。
        *   創建 AreaAnnotation 對象，設置區域選項並添加回复。
        *   創建 Annotator 對象並添加區域註釋。
        *   保存輸出文件。
    title_right: "系統要求"
    content_right: |
        所有主要平台和操作系統都支持 Java API 的 GroupDocs.Annotation。在執行下面的代碼之前，請確保您的系統上安裝了以下先決條件。
        *   操作系統：Microsoft Windows、Linux、MacOS
        *   開發環境：NetBeans、Intellij IDEA、Eclipse等
        *   Java 運行時環境：Java 7 (1.7) 及更高版本
        *   從 [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) 獲取最新版本的 GroupDocs.Annotation for Java

############################# Preview ############################
preview_Add:
    enable: true
    title: 註釋預覽和代碼示例
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Create an instance of Reply class and add comments
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("This is area annotation");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Add annotation
        annotator.add(area);
        
        // Save to file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "在 Java 中從 DOT 中刪除註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通過實施幾個簡單的步驟，Java 開發人員可以更輕鬆地從任何基於 Java 的應用程序中的 DOT 文件中刪除註釋詳細信息。
        *   創建帶有評論和日期的 Reply 對象。
        *   實例化 SaveOptions 對象並設置 AnnotationTypes = AnnotationType.None。
        *   使用生成的文檔路徑或流以及 SaveOptions 對象調用 save 方法。

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```java
        // Create an instance of Annotator class 
        Annotator annotator = new Annotator("C://input.bmp");

        // Remove annotation by set type None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Save annotation to output file
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "在 Java 中編輯 DOT 註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通過實施幾個簡單的步驟，Java 開發人員可以更輕鬆地從任何基於 Java 的應用程序中的 DOT 文件更新各種註釋屬性。
        *   使用輸入文檔路徑或流實例化 Annotator 對象，並使用 ImportAnnotations = true 實例化 LoadOptions。
        *   創建一些 AnnotationBase 實現並設置現有註釋的 Id（如果未找到具有該 Id 的註釋，則不會更改任何內容）或註釋的路徑列表（所有現有註釋將被刪除）。
        *   使用傳遞的註釋調用 Annotator 對象的更新方法。
        *   使用生成的文檔路徑或流以及 SaveOptions 對象調用 save 方法。

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Create an instance of Reply class for first example and add comments
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Create an instance of Reply class for update first example
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Update and save annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "在 Java 中從 DOT 提取註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通過實施幾個簡單的步驟，Java 開發人員可以輕鬆地對文檔進行註釋並從任何基於 Java 的應用程序中的 DOT 文件中提取註釋信息。
        *   創建帶有評論和日期的 Reply 對象。
        *   實例化 LoadOptions 對象並使用 true 參數調用 SetImportAnnotations。
        *   定義類型為 List 的變量。
        *   調用 get 方法並將結果返回到上面的變量。

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```java
        // For using this example input file ("annotated.bmp") must be with annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Create an instance of Annotator class and get annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "現場演示添加、刪除、編輯、提取文檔和圖像的註釋"
    content: |
        立即訪問 [GroupDocs.Annotation 現場演示](https://products.groupdocs.app/annotation/family) 網站，向 DOT 文件添加、刪除、編輯和提取註釋。 現場演示有以下好處

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dot"
          title: "關於 DOT 文件格式"
          content: |
            擴展名為 .DOT 的文件是由 Microsoft Word 創建的模板文件，具有用於生成更多 DOC 或 DOCX 文件的預格式化設置。創建模板文件是為了具有應應用於從這些文件創建的後續文件的特定用戶設置。這些設置包括頁邊距、邊框、頁眉、頁腳和其他頁面設置。此類模板用於官方文件，例如公司信頭和標準化表格。 DOT 文件格式特定於 Microsoft Word 2003 及更早版本，但更高版本也支持。默認情況下，Microsoft Word 基於 normal.dot 文件打開每個新文檔。如果進行修改，創建的所有新文件將產生與模板文件相同的設置。在 Microsoft Word 2007 中，DOT 文件格式已替換為基於 Office OpenXML 的 DOTX 文件格式。

          link: "https://docs.fileformat.com/image/dot/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "使用其他流行的文檔格式"
    content: |
        更新一些流行文件格式的註釋屬性，如下所述。
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/java/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/java/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/java/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/java/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/java/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/java/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/java/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/java/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/java/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/java/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/java/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/java/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/java/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/java/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/java/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/java/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/java/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/java/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/java/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/java/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/java/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/java/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/java/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/java/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/java/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/java/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/java/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/java/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/java/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/java/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/java/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/java/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/java/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/java/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/java/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---