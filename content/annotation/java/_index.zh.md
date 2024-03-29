---
############################# Static ############################
layout: "product"
date: 2022-02-23T12:00:00+02:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 文档注释 API |查看和注释 PDF Word Excel PPTX 图像"
head_description: "Java 文档注释 API。查看、标记、评论和注释 PDF、Word DOCX、Excel XLSX、PPTX、EML EMLX、VSS VSD、OTP、CAD 和图像文件格式。"

############################# Header ##########################
title: "通过 Java API 进行文档注释"
description: "构建具有查看和注释 PDF、HTML、MS Office 和其他文档格式功能的 Java 应用程序，无需安装任何外部软件。"
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "下载免费试用版"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu #########################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "现场演示"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Java API 是一款产品，允许您在不同平台和操作系统（例如 Android、MacOS、Linux、Windows）上处理文档中的注释。 GroupDocs.Annotation 提供了一个具有简单 API 的库，具有许多优点：例如，如果您需要对数据保密或选择使用该库需要多少权限，或者部分更改使用注释的工作，该库非常适合轻便灵活。

      GroupDocs.Annotation for Java API 允许您使用不同类型的注释，其中包括：文本、折线、区域、下划线、点、水印、箭头、椭圆、文本替换、距离、文本字段、资源编辑等。并支持大多数流行的文档格式，例如：PDF、HTML、Microsoft Office Word、Excel 电子表格、PowerPoint 演示文稿、Visio、Outlook 电子邮件、图像、图元文件、CAD 绘图和各种其他格式。该 API 提供获取文档页面缩略图的功能，并支持在 PDF 文件中导入和导出注释。

      使用库，您可以[添加]（/annotation/java/bmp/），[编辑]（/annotation/java/bmp/），[提取]（/annotation/java/bmp/）和[删除]（/annotation/java/bmp/) 来自文档的注释、旋转文档、更改缩略图解决方案，这并不是所有可能性的完整列表。它还提供了一套全面的数据对象，可根据您的要求在所有受支持的文档格式中自定义注释属性。

      使用 GroupDocs.Annotation for Java API 非常简单，仅包含几个基本步骤。首先，您需要设置许可证，然后选择要使用的文件，然后使用文档注释进行某种操作（删除/编辑/提取/删除）并保存结果。有关更多信息，请参阅产品[文档](https://docs.groupdocs.com/annotation/java/getting-started/) 或我们的[示例](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) 设置。
      
      GroupDocs.Annotation 定期更新并为其客户提供支持，随时欢迎您向我们提问或发送您的想法或告诉我们您对新内容的需求，我们很乐意在新版本中实现它。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 GroupDocs.Annotation for Java 的概述：
      
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
          GroupDocs.Annotation for Java 支持所有流行的[文档文件格式](https://docs.groupdocs.com/annotation/java/supported-document-formats/)，包括：Microsoft Office、PDF、图像等。

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: [DOC](/annotation/java/doc/), [DOCX](/annotation/java/docx/), [DOCM](/annotation/java/docm/), [DOT](/annotation/java/dot/), [DOTX](/annotation/java/dotx/), [RTF](/annotation/java/rtf/)
                * **Excel**: [XLS](/annotation/java/xls/), [XLSX](/annotation/java/xlsx/), [XLSB](/annotation/java/xlsb/), [XLSM](/annotation/java/xlsm/)
                * **PowerPoint**: [PPT](/annotation/java/ppt/), [PPTX](/annotation/java/pptx/), [PPS](/annotation/java/pps/), [PPSX](/annotation/java/ppsx/), [POTM](/annotation/java/potm/), [POTX](/annotation/java/potx/), [PPSM](/annotation/java/ppsm/), [PPTM](/annotation/java/pptm/), [WMF](/annotation/java/wmf/), [EMF](/annotation/java/emf/)
                * **Outlook**: [EML](/annotation/java/eml/), [EMLX](/annotation/java/emlx/), [MSG](/annotation/java/msg/)
                * **Visio**: [VSS](/annotation/java/vss/), [VST](/annotation/java/vst/), [VSD](/annotation/java/vsd/), [VSDX](/annotation/java/vsdx/), [VSX](/annotation/java/vsx/)

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **Portable**: [PDF](/annotation/java/pdf/) (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: [ODT](/annotation/java/odt/), [ODS](/annotation/java/ods/), [ODP](/annotation/java/odp/)
                * **Images**: [BMP](/annotation/java/bmp/), [JPG](/annotation/java/jpg/), [JPEG](/annotation/java/jpeg/), [TIFF](/annotation/java/tiff/), [TIF](/annotation/java/tif/), [PNG](/annotation/java/png/), [GIF](/annotation/java/gif/), [DCM](/annotation/java/dcm/), [DICOM](/annotation/java/dicom/)
                * **AutoCAD**: [DWG](/annotation/java/dwg/), [DXF](/annotation/java/dxf/), [CAD](/annotation/java/cad/)
                * **Other**: [HTM](/annotation/java/htm/), [HTML](/annotation/java/html/), [CSV](/annotation/java/csv/), [DJVU](/annotation/java/djvu/), [OTP](/annotation/java/otp/), [OTT](/annotation/java/ott/)

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Java 支持以下操作系统、框架和包管理器：
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title:  操作系统
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title:  支持的框架
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title:  开发环境
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse

            # table loop
            - icon: "fas fa-tools"
              title:  构建自动化工具
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: Java 功能的 GroupDocs.Annotation

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/java/add-area-annotation/"
        content: 在文档中添加区域注释并链接简单和嵌套注释

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/java/add-arrow-annotation/"
        content: 使用箭头注释指向特定内容

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: 将文本水印设置为 PDF、幻灯片、Excel 工作表、图像和图表的倾斜位置
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: 使用点注释将弹出注释添加到文档中的任何位置

      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/java/add-polyline-annotation/"
        content: 使用折线注释连接线段、弧段或两者的序列

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/java/add-ellipse-annotation/"
        content: 将椭圆注释添加到 PDF、Word 文档、电子表格、演示文稿、图表和图像

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: 为 PDF、PowerPoint、Excel、图像和图表添加倾斜水印

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/java/add-underline-annotation/"
        content: 获取文档图像表示中文本注释的坐标

      # feature loop
      - icon: "fas fa-location-arrow"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: 在文档中添加下划线、删除线或修改特定文本

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: 在文档中添加文本图章或水印和文本字段

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: 在 Word 文档和 PowerPoint 演示文稿中导入和导出注释

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/java/add-strikeout-annotation/"
        content: 使用文本、文本替换、水印和资源编辑注释类型对 Excel 电子表格进行注释

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: 向 PowerPoint 演示文稿和幻灯片添加折线、删除线、下划线或文本注释

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/java/basic-usage/"
        content: 使用 X、Y 坐标在演示文稿中标记点注释

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/java/add-strikeout-annotation/"
        content: 向图像添加删除线、文本、下划线或多段线注释

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/java/add-link-annotation/"
        content: 获取 Visio 图表的文档信息和图像，例如 VSS 和 VSD
      
      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/java/basic-usage/"
        content: 获取文档页面的缩略图并使用多页 TIFF 文件

      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: 使用单个函数调用获取文档的所有注释

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/java/add-link-annotation/"
        content: 将链接注释添加到 PDF、Word 和 PowerPoint 演示文稿

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: SVG 路径解析支持 PDF、Word、图表、幻灯片和其他主要文档格式

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: 支持为Word文档添加水印注释和清理文本替换

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: 文本注释图表中的形状处理支持
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/advanced-usage/"
        content: 通过缓存文档页面预览以加快处理速度来节省时间
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: 即使使用旧格式，也可以轻松注释 Word、Excel 和 PowerPoint 文档

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-distance-annotation/"
        content: 显示 Excel、PowerPoint 和图表的距离注释标题

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: GroupDocs.Annotation 为其他流行的开发环境提供文档查看 API

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---