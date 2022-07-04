---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java 文档注释 API |查看和注释 PDF Word Excel PPTX 图像"
head_description: "Java 文档注释 API。查看、标记、评论和注释 PDF Word DOCX、Excel XLSX、PPTX、EML EMLX、VSS VSD、OTP、CAD 和图像文件格式."

############################# Header ############################
title: "通过 Java API 进行文档注释"
description: "构建具有查看和注释 PDF、HTML、MS Office 和其他文档格式的 Java 应用程序，而无需安装任何外部软件."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "下载免费试用版"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "/border/groupdocs-annotation-java.svg"
        product: "GroupDocs.Annotation"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "价钱"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# 概述 ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation for Java API 提供了易于使用的文档、注释管理和操作功能，可在基于 Java 的业务应用程序中使用。我们的 Java 注释器库允许您使用多种类型的注释，包括文本、折线、区域、下划线、点、水印、箭头、椭圆、文本替换、距离、文本字段、资源编辑等。它还提供了一个全面的集合数据对象以根据您的要求在所有支持的文档格式中自定义注释属性，包括：PDF、HTML、微软办公软件 Word、Excel 电子表格、PowerPoint 演示文稿、Visio、Outlook 电子邮件、图像、元文件、CAD 绘图和各种其他格式。
        
      API 提供了获取文档页面缩略图的能力，并支持在 PDF 文件中导入和导出注释。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下是 GroupDocs.Annotation for Java 的概述：
      
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
          GroupDocs.Annotation for Java 支持所有流行的 [文档文件格式](https://docs.groupdocs.com/annotation/java/supported-document-formats/)，包括：微软办公软件、PDF、图像等。

        left:
          enable: true
          table:
            # table loop
            - title: "微软办公格式"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **Excel**: XLS, XLSX, XLSB, XLSM
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Outlook**: EML, EMLX
                * **Visio**: VSS, VST, VSD, VSDX

        right:
          enable: true
          table:
            # table loop
            - title: "其他格式"
              content: |
                * **便携式**：PDF（PDF/A-1a、PDF/A-1b、PDF/A-2a）
                * **OpenDocument**：ODT、ODS、ODP
                * **图片**：BMP、JPG、TIFF、TIF、PNG
                * **AutoCAD**：DWG、DXF
                * **其他**：HTML

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Java 支持以下操作系统、框架和包管理器：
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "操作系统"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "支持的框架"
              content: |
                * Java 7 (1.7) 及更高版本

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "开发环境"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "构建自动化工具"
              content: |
                * Maven

############################# 特征 ############################
features:
    enable: true
    title: "GroupDocs.Annotation for Java 功能"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/java/add-area-annotation/"
        content: "在文档中添加区域注释并链接简单和嵌套注释"

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/java/add-arrow-annotation/"
        content: "使用箭头注释指向特定内容"

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: "在倾斜位置将文本水印设置为 PDF、幻灯片、Excel 工作表、图像和图表"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "使用点注释将弹出式注释添加到文档中的任何位置"

      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/java/add-polyline-annotation/"
        content: "使用折线注释连接线段、弧段或两者的序列"

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/java/add-ellipse-annotation/"
        content: "为 PDF、Word 文档、电子表格、演示文稿、图表和图像添加椭圆注释"

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: "为 PDF、PowerPoint、Excel、图像和图表添加角度水印"

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/java/extract-annotations-from-document/"
        content: "获取文档图像表示中文本注释的坐标"

      # feature loop
      - icon: "fas fa-location-arrow"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "下划线、删除线或修改文档中的特定文本"

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "在文档中添加文本图章或水印和文本字段"

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/advanced-usage/"
        content: "导入和注释 Word 文档和 PowerPoint 演示文稿之间的注释"

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "使用文本、TextReplacement、水印和资源编辑注释类型注释 Excel 电子表格"

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "向 PowerPoint 演示文稿和幻灯片添加折线、删除线、下划线或文本注释"

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "使用 X、Y 坐标在演示文稿中标记点注释"

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "为图像添加删除线、文本、下划线或折线注释"

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: "获取 Visio 图表的文档信息和图像，例如 VSS 和 VSD"

      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/java/basic-usage/"
        content: "获取文档页面的缩略图并使用多页 TIFF 文件"
      
      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: "使用单个函数调用获取文档的所有注释"

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/java/add-link-annotation/"
        content: "为 PDF、Word 和 PowerPoint 演示文稿添加链接注释"

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "SVG 路径解析支持 PDF、Word、图表、幻灯片和其他主要文档格式"

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: "支持在 Word 文档中添加水印注释并清理文本替换"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: "图表中对文本注释的形状处理支持"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/advanced-usage/"
        content: "通过缓存文档的页面预览以加快处理速度，从而节省时间"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "即使使用旧格式也能轻松注释 Word、Excel 和 PowerPoint 文档"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-distance-annotation/"
        content: "为 Excel、PowerPoint 和图表显示距离注释标题"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation 为其他流行的开发环境提供文档查看 API"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for .NET"
          image: "/border/groupdocs-annotation-net.svg"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
