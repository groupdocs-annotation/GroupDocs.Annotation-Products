
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/potx"/>

############################# Head ############################
head_title: "消除 注解 从 POTX 在 Java 应用程序中"
head_description: "用于创建 Java API 和 消除 流行注释类型 从 POTX、图像、绘图和文档文件格式。"

############################# Header ############################
title: "注释 POTX 从 Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "Java 的 GroupDocs.Annotation"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "关于 Java API 的 GroupDocs.Annotation"
    content: |
        GroupDocs.Annotation for Java API 是一个库，允许您在 Mac、Windows 或 Ubuntu 上向 PDF、Word 和其他文档添加注释。 [GroupDocs.Annotation for Java](/annotation/java) 是用于管理注释的原生 Java API，全面支持创建、添加、编辑、删除、提取和导出注释图像和各种其他文档。您可以在此[页面](https://docs.groupdocs.com/annotation/java/supported-document-formats/)上看到支持的文档格式的完整列表。

        该库不仅允许您处理 POTX 文档，还可以处理许多其他类型的文档，例如 Word、Excel、PowerPoint、Outlook 电子邮件、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad 等。

        Java API 的 GroupDocs.Annotation 允许您创建和添加新注释、编辑 注释、提炼 注释、注释，并从文档中 删除 它们。该库支持 13 种不同的注释类型，包括文本、折线、区域、下划线、点、水印、箭头、椭圆、文本替换、距离、文本字段、PDF、HTML、Microsoft Word 文档、电子表格、图表、演示文稿中的资源编辑，绘图、图像和许多其他文件格式。

        该示例（请参见下文）演示了如何使用 POTX 文档，在此示例中您可以看到如何使用 GroupDocs 的主要步骤。注释: 设置许可证、打开要使用的文档、创建注释，根据需要添加数据对象设置注释属性，并将结果保存到需要的地方。此外，您还可以在我们的 github [页面](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) 或我们的产品 上查看更详细的支持功能 [文档](https://docs.groupdocs.com/annotation/java/getting-started/)。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "在 Java 中添加注释 从 POTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Java 开发人员可以轻松地将各种注释类型添加到任何基于 Java 的应用程序中的 POTX 文件。
        * 创建带有评论和日期的回复对象。
        * 创建AreaAnnotation对象，设置区域选项并添加回复。
        * 创建Annotator对象并添加区域注释。
        * 保存输出文件。
    title_right: "系统要求"
    content_right: |
        所有主要平台和操作系统都支持 Java API 的 GroupDocs.Annotation。在执行下面的代码之前，请确保您的系统上安装了以下先决条件。
        * 操作系统: Microsoft Windows、Linux、MacOS
        * 开发环境: NetBeans、Intellij IDEA、Eclipse等
        * Java运行时环境: Java 7 (1.7)及以上
        * 从 [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) 获取最新版本的 GroupDocs.Annotation for Java

############################# Preview ############################
preview_Add:
    enable: true
    title: "注解预览和代码示例"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ``java
        // 创建Reply类的实例并添加注释
        Reply firstReply = new Reply();
        firstReply.setComment("第一条评论");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondaryreply.setComment("第二条评论");
        SecondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // 创建 AreaAnnotation 类的实例并设置选项
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("这是区域注释");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte)3);
        area.setReplies(replies);
        
        // 创建 Annotator 类的实例
        Annotator annotator = new Annotator("input.bmp");
        
        // 添加注释
        annotator.add(area);
        
        // 保存到文件
        annotator.save("output.bmp");
        annotator.dispose();
        ````

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "在 Java 中删除注释 从 POTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Java 开发人员可以更轻松地从任何基于 Java 的应用程序中的 POTX 文件中删除注释详细信息。
        * 创建带有评论和日期的回复对象。
        * 实例化 SaveOptions 对象并设置 AnnotationTypes = AnnotationType.None。
        * 使用生成的文档路径或流以及 SaveOptions 对象调用保存方法。

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ``java
        // 创建 Annotator 类的实例
        Annotator annotator = new Annotator("C://input.bmp");

        // 通过设置类型 None 移除注解
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // 将注释保存到输出文件
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ````

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "在 Java 中编辑注释 从 POTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Java 开发人员可以更轻松地在任何基于 Java 的应用程序中更新来自 POTX 文件的各种注释属性。
        * 使用输入文档路径或流实例化 Annotator 对象，并使用 ImportAnnotations = true 实例化 LoadOptions。
        * 创建一些AnnotationBase实现并设置现有注释的Id（如果未找到具有该Id的注释，则不会更改任何内容）或注释的路径列表（所有现有注释将被删除）。
        * 使用传递的注释调用 Annotator 对象的更新方法。
        * 使用生成的文档路径或流以及 SaveOptions 对象调用保存方法。

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ``java
        String outputPath = "UpdateAnnotation.bmp";

        // 创建 Annotator 类的实例
        Annotator annotator = new Annotator("input.bmp");
        
        // 为第一个示例创建 Reply 类的实例并添加注释
        Reply reply1 = new Reply();
        reply1.setComment("原第一条评论");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("原第二条评论");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // 创建 AreaAnnotation 类的实例并设置选项
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        Original.setCreatedOn(Calendar.getInstance().getTime());
        Original.setMessage("这是原始注释");
        original.setReplies(replies);
        
        // 添加原始注释
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // 打开带注释的文档
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // 创建 Reply 类的实例以用于更新第一个示例
        Reply reply3 = new Reply();
        reply3.setComment("更新第一条评论");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("更新第二条评论");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // 建议我们要更改现有注释的一些属性
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        Updated.setMessage(“这是更新的注释”);
        updated.setReplies(replies1);
        
        // 更新并保存注释
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ````

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "在 Java 中提取注释 从 POTX 的步骤"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) 通过实施几个简单的步骤，Java 开发人员可以轻松地在任何基于 Java 的应用程序中对文档进行注释并从 POTX 文件中提取注释信息。
        * 创建带有评论和日期的回复对象。
        * 实例化 LoadOptions 对象并使用 true 参数调用 SetImportAnnotations。
        * 定义List类型的变量。
        * 调用get方法并将结果返回给上面的变量。

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ``java
        // 要使用此示例，输入文件（“annotated.bmp”）必须带有注释
        LoadOptions loadOptions = new LoadOptions();
        
        // 创建Annotator类的实例并获取注释
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ````

############################# Demos ############################
demos:
    enable: true
    title: "提取注释的现场演示"
    content: |
        立即访问 [GroupDocs.Annotation 实时演示](https://products.groupdocs.app/annotation/family) 网站，查看并删除 POTX 文件中的注释。
        现场演示有以下好处

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-potx"
          title: "关于 POTX 文件格式"
          content: |
            扩展名为 .POTX 的文件代表使用 Microsoft PowerPoint 2007 及更高版本创建的 Microsoft PowerPoint 模板演示文稿。创建此格式是为了替换基于二进制文件格式并受 PowerPoint 97-2003 支持的 POT 文件格式。生成的文件可用于创建具有相同布局和需要应用于新文件的其他设置的演示文稿。这些设置可以包括样式、背景、调色板、字体和默认值。生成此类文件是为了创建可供正式使用的现成模板文件。
          link: "https://docs.fileformat.com/image/potx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "使用其他流行的文档格式"
    content: |
        更新一些流行文件格式的注释属性，如下所述。
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