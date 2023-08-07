---
############################# Static ############################
layout: "product"
date: 2022-02-23T12:00:00+02:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: "网络文档注释API |查看和注释 PDF Word Excel PPTX 图像"
head_description: "网络文档注释 API。查看、标记、评论和注释 PDF、Word DOCX、Excel XLSX、PPTX、EML EMLX、VSS VSD、OTP、CAD 和图像文件格式。"

############################# Header ##########################
title: "通过 Net API 进行文档注释"
description: "构建具有查看和注释 PDF、HTML、MS Office 和其他文档格式功能的网络应用程序，无需安装任何外部软件。"
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "下载免费试用版"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu #########################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Net"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "现场演示"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Net API 是一款产品，允许您在不同平台和操作系统（例如 Android、MacOS、Linux、Windows）上处理文档中的注释。 GroupDocs.Annotation 提供了一个具有简单 API 的库，具有许多优点：例如，如果您需要对数据保密或选择使用该库需要多少权限，或者部分更改使用注释的工作，该库非常适合轻便灵活。

      GroupDocs.Annotation for Net API 允许您使用不同类型的注释，其中包括：文本、折线、区域、下划线、点、水印、箭头、椭圆、文本替换、距离、文本字段、资源编辑等。并支持大多数流行的文档格式，例如：PDF、HTML、Microsoft Office Word、Excel 电子表格、PowerPoint 演示文稿、Visio、Outlook 电子邮件、图像、图元文件、CAD 绘图和各种其他格式。该 API 提供获取文档页面缩略图的功能，并支持在 PDF 文件中导入和导出注释。

      使用库，您可以添加、编辑、提取和删除文档中的注释、旋转文档、更改缩略图解决方案，这并不是所有可能性的完整列表。它还提供了一套全面的数据对象，可根据您的要求在所有受支持的文档格式中自定义注释属性。

      使用 GroupDocs.Annotation for Net API 非常简单，仅包含几个基本步骤。首先，您需要设置许可证，然后选择要使用的文件，然后使用文档注释进行某种操作（删除/编辑/提取/删除）并保存结果。有关更多信息，请参阅产品文档或我们的示例集。
      
      GroupDocs.Annotation 定期更新并为其客户提供支持，随时欢迎您向我们提问或发送您的想法或告诉我们您对新内容的需求，我们很乐意在新版本中实现它。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 GroupDocs.Annotation for Net 的概述：
      
        right:
          enable: true
          icon: "fab fa-html5"
          title:  概述
          content: |
            * 添加注释
            * 导出注释 
            * 导入注释
            * 基于回复的评论
            * 注释兼容性
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation for Net 支持所有流行的[文档文件格式](https://docs.groupdocs.com/annotation/Net/supported-document-formats/)，包括：Microsoft Office、PDF、图像等。

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: [DOC](/annotation/net/doc/), [DOCX](/annotation/net/docx/), [DOCM](/annotation/net/docm/), [DOT](/annotation/net/dot/), [DOTX](/annotation/net/dotx/), [RTF](/annotation/net/rtf/)
                * **Excel**: [XLS](/annotation/net/xls/), [XLSX](/annotation/net/xlsx/), [XLSB](/annotation/net/xlsb/), [XLSM](/annotation/net/xlsm/)
                * **PowerPoint**: [PPT](/annotation/net/ppt/), [PPTX](/annotation/net/pptx/), [PPS](/annotation/net/pps/), [PPSX](/annotation/net/ppsx/), [POTM](/annotation/net/potm/), [POTX](/annotation/net/potx/), [PPSM](/annotation/net/ppsm/), [PPTM](/annotation/net/pptm/), [WMF](/annotation/net/wmf/), [EMF](/annotation/net/emf/)
                * **Outlook**: [EML](/annotation/net/eml/), [EMLX](/annotation/net/emlx/), [MSG](/annotation/net/msg/)
                * **Visio**: [VSS](/annotation/net/vss/), [VST](/annotation/net/vst/), [VSD](/annotation/net/vsd/), [VSDX](/annotation/net/vsdx/), [VSX](/annotation/net/vsx/)

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **Portable**: [PDF](/annotation/net/pdf/) (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: [ODT](/annotation/net/odt/), [ODS](/annotation/net/ods/), [ODP](/annotation/net/odp/)
                * **Images**: [BMP](/annotation/net/bmp/), [JPG](/annotation/net/jpg/), [JPEG](/annotation/net/jpeg/), [TIFF](/annotation/net/tiff/), [TIF](/annotation/net/tif/), [PNG](/annotation/net/png/), [GIF](/annotation/net/gif/), [DCM](/annotation/net/dcm/), [DICOM](/annotation/net/dicom/)
                * **AutoCAD**: [DWG](/annotation/net/dwg/), [DXF](/annotation/net/dxf/), [CAD](/annotation/net/cad/)
                * **Other**: [HTM](/annotation/net/htm/), [HTML](/annotation/net/html/), [CSV](/annotation/net/csv/), [DJVU](/annotation/net/djvu/), [OTP](/annotation/net/otp/), [OTT](/annotation/net/ott/)

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Net 支持以下操作系统、框架和包管理器：
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title:  操作系统
              content: |
                * Windows Desktop (x86 & x64)
                * Windows Server (x86 & x64)
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title:  支持的框架
              content: |
                * .NET Standard 2.0
                * .NET Framework 2.0 or higher
                * .NET Core 2.0 or higher
                * Mono Framework 1.2 or higher

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title:  包管理器
              content: |
                * NuGet
            
            # table loop
            - icon: "fas fa-tools"
              title:  开发环境
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: GroupDocs.网络特征注释

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: 添加、编辑和删除注释和回复

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: 将注释导出到文档

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/net/evaluation-limitations-and-licensing-of-groupdocs-annotation/"
        content: 计量许可证 – 通过根据 API 使用情况付费来控制计费
      
      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/net/extract-annotations-from-document/"
        content: 单个函数调用以获取文档的所有注释

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: 将值分配给点注释或移动现有点值

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/net/add-link-annotation/"
        content: 将链接注释添加到 PDF、Word 和 PowerPoint 幻灯片

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: 设置注释的背景颜色或从文档中删除所有注释

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: 准确注释 PDF 文件 – 获取 PDF 文档的图像表示和缓存页面预览

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/import-annotations/"
        content: 获取文档图像表示中文本注释的文本坐标

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: 将用户评论链接到区域注释并支持嵌套评论

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/net/add-arrow-annotation/"
        content: 使用箭头注释指向特定内容

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/net/add-distance-annotation/"
        content: 使用距离注释绘制代表对象之间距离的线

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: 基于点的注释，单击时会弹出窗口以添加注释

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/net/add-polyline-annotation/"
        content: 创建作为折线注释创建的线段的连接序列

      # feature loop
      - icon: "fas fa-lock"
        link: "https://docs.groupdocs.com/annotation/net/add-ellipse-annotation/"
        content: 创建直线段、圆弧段或两者的组合

      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: 标记建议密文的文档区域
      
      # feature loop
      - icon: "fas fa-fill-drip"
        link: "https://docs.groupdocs.com/annotation/net/add-image-annotation/"
        content: 将图像注释添加到 PDF、图表、Word、Excel、演示文稿和图像

      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: 在文档中添加文本字段和基于文本的图章或水印

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: 在文档中删除特定文本、添加下划线或替换特定文本

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/net/update-annotations/"
        content: 通过分配新的高度和宽度参数来调整注释大小

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: 获取文档页面的缩略图。管理各种图像和图表的注释文档

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: 将注释导出到多页 TIFF 文件并使用它
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-watermark-annotation/"
        content: 调整水印注释的垂直和水平对齐方式
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-text-field-annotation/"
        content: 为文本字段添加文本水平对齐方式

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/document-text-info/"
        content: 获取有关文档文本行的信息（文本、宽度、高度、缩进）

    more_feature:
      # more_feature_loop
      - title: 支持多种类型的注释
        content: |
          GroupDocs.Annotation for .NET 使您能够使用各种类型的注释。这在与您的团队协作完成任务时提供了自由和轻松的沟通。您可以使用注释，例如区域注释（将区域标记为矩形并为其添加注释）、点注释（在文档中的任意点粘贴注释）、文本注释（为选定的文本添加注释）、删除线/下划线注释（应用于段落）、折线注释（绘制形状和手绘线）、箭头注释（带有附加注释的箭头指针）、椭圆注释（在椭圆内显示文本）、距离注释（绘制表示对象之间距离的线）、链接注释（将网页链接添加到支持的文档格式）和水印注释（可以在文档中添加文本印记或水印）。

          ```cs
          // Initialize list of AnnotationInfo
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          // Initialize text annotation
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          // Add annotation to list
          annotations.Add(textAnnotation);
          // Get input file stream
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          // Export annotation and save output file
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: GroupDocs.Annotation 为其他流行的开发环境提供文档查看 API

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---