---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET 文档注释 API |注释 PDF Word Excel PPTX 图像文件"
head_description: "C# .NET 文档注释 API。查看、标记、评论和注释 PDF Word DOC DOCX、Excel XLS XLSX、PPT PPTX、OTP、CAD、EMF WMF 和图像文件."

############################# Header ############################
title: "注释文档中的文本或图像"
description: "使您的 .NET 应用程序能够从 50 多种文档格式中添加、编辑和删除所有流行的注释类型，以实现更轻松、更高效的协作."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "下载免费试用版"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for .NET"
        image: "/border/groupdocs-annotation-net.svg"
        product: "GroupDocs.Annotation"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "概述"

            # button loop
            - link: "#features"
              text: "特征"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation for .NET 是一套全面的 API，可帮助您使用 C#、ASP.NET 和其他相关 .NET 技术构建文档注释管理应用程序。您可以为 PDF、HTML、微软办公软件 Word、Excel 电子表格、PowerPoint 演示文稿创建和使用所有流行的注释类型，例如区域、点、文本、椭圆、链接、下划线、折线、箭头、距离、水印、图像等， Visio、图像、CAD 绘图和各种其他格式。文档注释器库允许您在添加注释、评论或突出显示的注释后将文档导出回其原始格式。它还为您提供了一组方便的数据对象，您可以通过这些对象根据您的要求自定义注释。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 .NET 的 GroupDocs.Annotation 的概述：

        right:
          enable: true
          icon: "fab fa-html5"
          title: "概述"
          content: |
            * 添加注释
            * 导出注释
            * 导入注释            
            * 基于回复的评论
            * 注释兼容性
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation for .NET 支持所有流行的[文档文件格式](https://docs.groupdocs.com/annotation/net/supported-document-formats/)，包括：微软办公软件、PDF、图像等。

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公格式"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF 
                * **Microsoft Excel**: XLS, XLSX, XLSM, XLSB, CSV
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Microsoft Visio**: VSD, VSS, VSDX, VST, VSDM, VSSX, VSTM

        right:
          enable: true
          table:
            # table loop
            - title: "其他格式"
              content: |
                * **便携式**：PDF（PDF/A-1a、PDF/A-1b、PDF/A-2a）
                * **OpenDocument**：ODT、ODS、ODP
                * **图像**：BMP、JPEG、PNG、TIFF
                * **AutoCAD**：DWG、DXF
                * **元文件**：EMF、WMF
                * **电子邮件**：EML、EMLX
                * **网络**：HTM、HTML

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for .NET 支持以下作品，Frameworks & 包管理器:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Windows Desktop (x86 & x64)
                * Windows Server (x86 & x64)
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * .NET 标准 2.0
                * .NET Framework 2.0 或更高版本
                * .NET Core 2.0 或更高版本
                * Mono 框架 1.2 或更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "包管理器"
              content: |
                * NuGet
            
            # table loop
            - icon: "fas fa-tools"
              title: "开发环境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# 特征 ############################
features:
    enable: true
    title: ".NET 功能的 GroupDocs.Annotation"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: "添加、编辑和删除注释和回复"

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: "导出注释 to Document"

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/net/evaluation-limitations-and-licensing-of-groupdocs-annotation/"
        content: "计量许可证 – 根据 API 使用情况付费控制计费"
      
      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/net/extract-annotations-from-document/"
        content: "单个函数调用以获取文档的所有注释"

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: "为点注释分配值或移动现有点值"

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/net/add-link-annotation/"
        content: "为 PDF、Word 和 PowerPoint 幻灯片添加链接注释"

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: "设置注释的背景颜色或从文档中删除所有注释"

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: "准确地注释 PDF 文件 - 获取 PDF 文档和缓存页面预览的图像表示"

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/import-annotations/"
        content: "获取文档图像表示中文本注释的文本坐标"

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: "将用户评论链接到区域注释并支持嵌套评论"

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/net/add-arrow-annotation/"
        content: "使用箭头注释指向特定内容"

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/net/add-distance-annotation/"
        content: "使用距离注释绘制表示对象之间距离的线"

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: "单击时弹出窗口以添加注释的基于点的注释"

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/net/add-polyline-annotation/"
        content: "创建作为折线注释创建的连接线段序列"

      # feature loop
      - icon: "fas fa-lock"
        link: "https://docs.groupdocs.com/annotation/net/add-ellipse-annotation/"
        content: "创建直线段、弧段或两者的组合"

      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: "标记建议编辑的文档区域"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        link: "https://docs.groupdocs.com/annotation/net/add-image-annotation/"
        content: "为 PDF、图表、Word、Excel、演示文稿和图像添加图像注释"

      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: "在文档中添加文本字段和基于文本的图章或水印"

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: "删除、下划线或替换文档中的特定文本"

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/net/update-annotations/"
        content: "通过分配新的高度和宽度参数来调整注释大小"

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: "获取文档页面的缩略图。管理各种带注释的图像和图表文档"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: "& 注释 & 处理多页 TIFF 文件"
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-watermark-annotation/"
        content: "调整水印注释的垂直和水平对齐方式"
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-text-field-annotation/"
        content: "为文本字段添加文本水平对齐"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/document-text-info/"  
        content: "获取有关文档文本行的信息（文本、宽度、高度、缩进）"

    more_feature:
      # more_feature_loop
      - title: "支持多种类型的注释"
        content: |
          GroupDocs.Annotation for .NET 使您能够使用各种类型的注释。这在与您的团队合作完成任务时提供了自由和轻松的沟通。您可以使用注释，例如区域注释（将区域标记为矩形并为其添加注释）、点注释（在文档中的任何位置粘贴注释）、文本注释（为选定文本添加注释）、删除线/下划线注释（应用于段落）、折线注释（绘制形状和手绘线）、箭头注释（带有附加注释的箭头指针）、椭圆注释（在椭圆内显示文本）、距离注释（绘制表示对象之间距离的线）、链接注释（添加支持的文档格式的 Web 链接）和水印注释（可以在文档中添加文本戳记或水印）。

          ```cs
          // 初始化 AnnotationInfo 列表
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          // 初始化文本注释
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          // 将注释添加到列表
          annotations.Add(textAnnotation);
          // 获取输入文件流
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          // 导出注释并保存输出文件
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for Java"
          image: "/border/groupdocs-annotation-java.svg"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
