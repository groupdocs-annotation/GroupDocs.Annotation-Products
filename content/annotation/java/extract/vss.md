---
############################# Static ############################
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:41+03:00
draft: false

############################# Head ############################
head_title: "Extract Annotation from VSS in Java - Annotation Extraction API"
head_description: "Java annotation extraction API to extract popular annotation types from VSS, images, drawings and document file formats."

############################# Header ############################
title: "Java Annotation Extraction API for VSS"
description: "Extract annotations from Microsoft Office documents, images, HTML, drawings and other file formats in any type of Java application."
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
        img_alt: "GroupDocs.Annotation for Java"
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
    title: "About GroupDocs.Annotation for Java API"
    content: |
        [GroupDocs.Annotation for Java](/annotation/java/) is an advanced annotation management solution, allowing developers to view, [add](/annotation/java/add/bmp/), update, [delete](/annotation/java/remove/bmp) and export annotations from images and document file formats. Users can easily extract comments, notes, remarks and various annotation types including text, graphics and watermarks from PDF, HTML, Microsoft Word documents, Excel spreadsheets, Visio diagrams, PowerPoint presentations, drawings, images, and many other file formats. The annotation-processing feature can accurately read the annotations from the imported documents and allows exporting back into the original or desired file format after implementing the annotations customization.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps for Extracting Annotations in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easy for Java developers to annotate documents and extract annotation information from VSS files within any Java-based application by implementing a few easy steps.

        *   Create Reply objects with comment and date.
        *   Instantiate LoadOptions object and call SetImportAnnotations with true argument.
        *   Define variable with type List.
        *   Call get method and return result to variable above.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environment: NetBeans, Intellij IDEA, Eclipse etc
        *   Java Runtime Environment: Java 7 (1.7) and above
        *   Get the latest version of GroupDocs.Annotation for Java from [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)
        
    code: |
        ```java
        // for using this example input file ("annotated.vss") must be with annotations
         
        LoadOptions loadOptions = new LoadOptions();
        loadOptions.setImportAnnotations(true);
        
        final Annotator annotator = new Annotator("annotated.vss", loadOptions);
        List annotations = annotator.get();
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Annotate Documents and Images"
    content: |
        Extract annotation information from VSS file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vss"
          title: "About VSS File Format"
          content: |
            VSS are stencil files created with Microsoft Visio 2007 and earlier. A relatively new file format is .VSSX that was introduced with Microsoft Visio 2013. Stencil files provide drawing objects that can be included in a .VSD Visio drawing. Microsoft Visio itself is known for creating drawing elements such as collection of shapes, connectors, flowcharts, network layout, UML diagrams, software diagrams, database models, objects mapping and other similar information. It also has rich conversion features of Visio documents to other file formats such as PNG, BMP, PDF and others. Visio is available for both Windows and Mac OS.

          link: "https://docs.fileformat.com/image/vss/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Extracting Annotations From Other Supported File Formats"
    content: |
        Java annotation extraction library for documents and image formats. Get annotation details of some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Extract Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/java/extract/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Extract Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/java/extract/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Extract Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/java/extract/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Extract Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/java/extract/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Extract Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/java/extract/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Extract Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/java/extract/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Extract Annotation from DOTM"
          link: "https://products.groupdocs.com/annotation/java/extract/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Extract Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/java/extract/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Extract Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/java/extract/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Extract Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/java/extract/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Extract Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/java/extract/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Extract Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/java/extract/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Extract Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/java/extract/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Extract Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/java/extract/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Extract Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/java/extract/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Extract Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/java/extract/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Extract Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/java/extract/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Extract Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/java/extract/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Extract Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/java/extract/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Extract Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/java/extract/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Extract Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/java/extract/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Extract Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/java/extract/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Extract Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/java/extract/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Extract Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/java/extract/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Extract Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/java/extract/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Extract Annotation from BMP"
          link: "https://products.groupdocs.com/annotation/java/extract/bmp/"
          description: "Bitmap File Format"

        # format loop
        - name: "Extract Annotation from EML"
          link: "https://products.groupdocs.com/annotation/java/extract/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Extract Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/java/extract/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Extract Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/java/extract/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Extract Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/java/extract/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Extract Annotation from VST"
          link: "https://products.groupdocs.com/annotation/java/extract/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Extract Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/java/extract/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Extract Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/java/extract/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Extract Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/java/extract/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Extract Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/java/extract/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Extract Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/java/extract/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
