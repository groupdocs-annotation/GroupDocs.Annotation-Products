
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/pptx"/>

############################# Head ############################
head_title: "消除 注解 从 PPTX 在 Net 应用程序中"
head_description: "用于创建 Net API 和 消除 流行注释类型 从 PPTX、图像、绘图和文档文件格式。"

############################# Header ############################
title: "注释 PPTX 从 Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "Net 的 GroupDocs.Annotation"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "关于 Net API 的 GroupDocs.Annotation"
    content: |
        GroupDocs.Annotation for Net API 是一个库，允许您在 Mac、Windows 或 Ubuntu 上向 PDF、Word 和其他文档添加注释。 [GroupDocs.Annotation for Net](/annotation/net) 是用于管理注释的原生 Net API，全面支持创建、添加、编辑、删除、提取和导出注释图像和各种其他文档。您可以在此[页面](https://docs.groupdocs.com/annotation/net/supported-document-formats/)上看到支持的文档格式的完整列表。

        该库不仅允许您处理 PPTX 文档，还可以处理许多其他类型的文档，例如 Word、Excel、PowerPoint、Outlook 电子邮件、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad 等。

        Net API 的 GroupDocs.Annotation 允许您创建和添加新注释、编辑 注释、提炼 注释、注释，并从文档中 删除 它们。该库支持 13 种不同的注释类型，包括文本、折线、区域、下划线、点、水印、箭头、椭圆、文本替换、距离、文本字段、PDF、HTML、Microsoft Word 文档、电子表格、图表、演示文稿中的资源编辑，绘图、图像和许多其他文件格式。

        该示例（请参见下文）演示了如何使用 PPTX 文档，在此示例中您可以看到如何使用 GroupDocs 的主要步骤。注释: 设置许可证、打开要使用的文档、创建注释，根据需要添加数据对象设置注释属性，并将结果保存到需要的地方。此外，您还可以在我们的 github [页面](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net) 或我们的产品 上查看更详细的支持功能 [文档](https://docs.groupdocs.com/annotation/net/getting-started/)。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "在 Net 中添加注释 从 PPTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Net 开发人员可以轻松地将各种注释类型添加到任何基于 Net 的应用程序中的 PPTX 文件。
        * 创建带有评论和日期的回复对象。
        * 创建AreaAnnotation对象，设置区域选项并添加回复。
        * 创建Annotator对象并添加区域注释。
        * 保存输出文件。
    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 Net API 的 GroupDocs.Annotation。在执行下面的代码之前，请确保您的系统上安装了以下先决条件。
        * 操作系统: Microsoft Windows、Linux、MacOS
        * 开发环境: Visual Studio、Xamarin、MonoDevelop
        * 框架: .NET Framework、.NET Standard、.NET Core、Mono
        * 从 [NuGet](https://www.nuget.org/packages/groupdocs.annotation) 下载最新版本的 GroupDocs.Annotation for .NET

############################# Preview ############################
preview_Add:
    enable: true
    title: "注解预览和代码示例"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ````cs
        //从本地磁盘向文档添加文本字段注释
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
                Message = "这是文本字段注释",
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
                        Comment = "第一条评论",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "第二条评论",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ````

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "在 Net 中删除注释 从 PPTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Net 开发人员可以更轻松地从任何基于 Net 的应用程序中的 PPTX 文件中删除注释详细信息。
        * 创建带有评论和日期的回复对象。
        * 实例化 SaveOptions 对象并设置 AnnotationTypes = AnnotationType.None。
        * 使用生成的文档路径或流以及 SaveOptions 对象调用保存方法。

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ````cs
        // 1-如何使用注释索引从文档中删除注释
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2-如何使用注释对象从文档中删除注释
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3-如何使用 ID 列表从文档中删除一些注释
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4-如何使用注释列表从文档中删除一些注释
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ````

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "在 Net 中编辑注释 从 PPTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Net 开发人员可以更轻松地在任何基于 Net 的应用程序中更新来自 PPTX 文件的各种注释属性。
        * 使用输入文档路径或流实例化 Annotator 对象，并使用 ImportAnnotations = true 实例化 LoadOptions。
        * 创建一些AnnotationBase实现并设置现有注释的Id（如果未找到具有该Id的注释，则不会更改任何内容）或注释的路径列表（所有现有注释将被删除）。
        * 使用传递的注释调用 Annotator 对象的更新方法。
        * 使用生成的文档路径或流以及 SaveOptions 对象调用保存方法。

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ````cs
        // 打开带注释的文档
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
                            Message = "这是更新的注释",
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "更新了第一条评论",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "更新了第二条评论",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // 更新注解
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ````

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "在 Net 中提取注释 从 PPTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Net 开发人员可以轻松地在任何基于 Net 的应用程序中对文档进行注释并从 PPTX 文件中提取注释信息。
        * 创建带有评论和日期的回复对象。
        * 实例化 LoadOptions 对象并使用 true 参数调用 SetImportAnnotations。
        * 定义List类型的变量。
        * 调用get方法并将结果返回给上面的变量。

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ````cs
        // 要使用此示例，输入文件（“annotated.bmp”）必须带有注释
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
        ````

############################# Demos ############################
demos:
    enable: true
    title: "提取注释的现场演示"
    content: |
        立即访问 [GroupDocs.Annotation 实时演示](https://products.groupdocs.app/annotation/family) 网站，查看并删除 PPTX 文件中的注释。
        现场演示有以下好处

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pptx"
          title: "关于 PPTX 文件格式"
          content: |
            带有 PPTX 扩展名的文件是使用流行的 Microsoft PowerPoint 应用程序创建的演示文稿文件。与以前版本的二进制演示文稿文件格式 PPT 不同，PPTX 格式基于 Microsoft PowerPoint 开放 XML 演示文稿文件格式。演示文稿文件是幻灯片的集合，其中每张幻灯片可以包含文本、图像、格式、动画和其他媒体。这些幻灯片以具有自定义演示设置的幻灯片形式呈现给观众。
          link: "https://docs.fileformat.com/image/pptx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "使用其他流行的文档格式"
    content: |
        更新一些流行文件格式的注释属性，如下所述。
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