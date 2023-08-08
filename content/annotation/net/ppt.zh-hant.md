---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "C# 中的 Net PPT 註釋 API 註釋"
head_description: "Net API 用於從 PPT、圖像、繪圖和文檔文件格式創建和註釋流行的註釋類型。"

############################# Header ############################
title: "從網絡註釋 PPT"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "下載免費試用版"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "關於 GroupDocs.Net API 註釋"
    content: |
        GroupDocs.Annotation for Net API 是一個庫，允許您在 Mac、Windows 或 Ubuntu 上向 PDF、Word 和其他文檔添加註釋。 [GroupDocs.Annotation for Net](/annotation/net) 是一個用於管理註釋的原生 Net API，全面支持從圖像和各種其他文檔中創建、添加、編輯、刪除、提取和導出註釋。您可以在此[頁面](https://docs.groupdocs.com/annotation/net/supported-document-formats/)上看到支持的文檔格式的完整列表。
        該庫不僅允許您處理 PPT 文檔，還可以處理許多其他類型的文檔，例如 Word、Excel、PowerPoint、Outlook 電子郵件、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad 等。
        GroupDocs.Annotation for Net API 允許您創建和添加新註釋、編輯註釋、提取註釋、註釋以及從文檔中刪除它們。該庫支持13 種不同的註釋類型，包括文本、折線、區域、下劃線、點、水印、箭頭、橢圓、文本替換、距離、文本字段、PDF、HTML、Microsoft Word 文檔、電子表格、圖表、演示文稿中的資源編輯，繪圖、圖像和許多其他文件格式。
        該示例（請參見下文）演示瞭如何使用 PPT 文檔，在此示例中您可以看到如何使用 GroupDocs 的主要步驟。註釋：設置許可證、打開要使用的文檔、創建註釋，根據需要添加數據對象設置註釋屬性，並將結果保存到需要的地方。您還可以在我們的 github [頁面](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) 或我們的產品 [文檔](https ://docs.groupdocs.com/ annotation/net/getting-started/）。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "在 Net 中向 PPT 添加註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) 通過實施幾個簡單的步驟，網絡開發人員可以輕鬆地將各種註釋類型添加到任何基於網絡的應用程序中的 PPT 文件。
        *   創建帶有評論和日期的 Reply 對象。
        *   創建 AreaAnnotation 對象，設置區域選項並添加回复。
        *   創建 Annotator 對象並添加區域註釋。
        *   保存輸出文件。
    title_right: "系統要求"
    content_right: |
        所有主要平台和操作系統均支持 GroupDocs.Annotation for Net API。在執行下面的代碼之前，請確保您的系統上安裝了以下先決條件。
        *   操作系統：Microsoft Windows、Linux、MacOS
        *   開發環境：Visual Studio、Xamarin、MonoDevelop
        *   框架：.NET Framework、.NET Standard、.NET Core、Mono
        *   從 [NuGet](https://www.nuget.org/packages/groupdocs.annotation) 下載最新版本的 GroupDocs.Annotation for .NET

############################# Preview ############################
preview_Add:
    enable: true
    title: 註釋預覽和代碼示例
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
        using (Annotator annotator = new Annotator("input.bmp"))
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "This is text field annotation",
                Opacity = 0.7,
                PageNumber = 0,
                PenStyle = PenStyle.Dot,
                PenWidth = 3,
                FontFamily = "Arial",
                TextHorizontalAlignment = HorizontalAlignment.Center,
                Replies = new List
                {
                    new Reply
                    {
                        Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "在 Net 中從 PPT 中刪除註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) 通過實施幾個簡單的步驟，網絡開發人員可以更輕鬆地從任何基於網絡的應用程序中的 PPT 文件中刪除註釋詳細信息。
        *   創建帶有評論和日期的 Reply 對象。
        *   實例化 SaveOptions 對象並設置 AnnotationTypes = AnnotationType.None。
        *   使用生成的文檔路徑或流以及 SaveOptions 對象調用 save 方法。

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "在 Net 中編輯 PPT 註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) 通過實施幾個簡單的步驟，網絡開發人員可以更輕鬆地從任何基於網絡的應用程序中的 PPT 文件更新各種註釋屬性。
        *   使用輸入文檔路徑或流實例化 Annotator 對象，並使用 ImportAnnotations = true 實例化 LoadOptions。
        *   創建一些 AnnotationBase 實現並設置現有註釋的 Id（如果未找到具有該 Id 的註釋，則不會更改任何內容）或註釋的路徑列表（所有現有註釋將被刪除）。
        *   使用傳遞的註釋調用 Annotator 對象的更新方法。
        *   使用生成的文檔路徑或流以及 SaveOptions 對象調用 save 方法。

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```cs
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Updated first comment",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Updated second comment",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "從 Net 中的 PPT 提取註釋的步驟"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) 通過實施幾個簡單的步驟，網絡開發人員可以輕鬆地對文檔進行註釋並從任何基於網絡的應用程序中的 PPT 文件中提取註釋信息。
        *   創建帶有評論和日期的 Reply 對象。
        *   實例化 LoadOptions 對象並使用 true 參數調用 SetImportAnnotations。
        *   定義類型為 List 的變量。
        *   調用 get 方法並將結果返回到上面的變量。

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```cs
        // for using this example input file ("annotated.bmp") must be with annotations
        using (Annotator annotator = new Annotator("annotated.bmp"))
        {
            List annotations = annotator.Get();
            XmlSerializer formatter = new XmlSerializer(typeof(List));
            using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
                fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "現場演示添加、刪除、編輯、提取文檔和圖像的註釋"
    content: |
        立即訪問 [GroupDocs.Annotation 現場演示](https://products.groupdocs.app/annotation/family) 網站，向 PPT 文件添加、刪除、編輯和提取註釋。 現場演示有以下好處

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppt"
          title: "關於 PPT 文件格式"
          content: |
            具有 PPT 擴展名的文件表示由一組用於顯示為幻燈片的幻燈片組成的 PowerPoint 文件。它指定 Microsoft PowerPoint 97-2003 使用的二進製文件格式。 PPT 文件可以包含多種不同類型的信息，例如文本、項目符號點、圖像、多媒體和其他嵌入的 OLE 對象。 Microsoft 從 2007 年開始為 PowerPoint 提供了更新的文件格式（稱為 PPTX），它基於 Office OpenXML，與這種二進製文件格式不同。其他幾個應用程序（例如 OpenOffice Impress 和 Apple Keynote）也可以創建 PPT 文件。

          link: "https://docs.fileformat.com/image/ppt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "使用其他流行的文檔格式"
    content: |
        更新一些流行文件格式的註釋屬性，如下所述。
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/net/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/net/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/net/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/net/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/net/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/net/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/net/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/net/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/net/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/net/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/net/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/net/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/net/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/net/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/net/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/net/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/net/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/net/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/net/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/net/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/net/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/net/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/net/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/net/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/net/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/net/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/net/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/net/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/net/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/net/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/net/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/net/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/net/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/net/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/net/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---