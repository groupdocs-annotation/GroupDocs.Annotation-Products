
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/remove/bmp"/>

############################# Head ############################
head_title: "Remove Annotations from BMP in Java Application"
head_description: "Java API to create and Remove popular annotation types from BMP, images, drawings and document file formats."

############################# Header ############################
title: "Remove BMP Files from Java"
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
        GroupDocs.Annotation for Java API is a library that allows you to add annotations to PDF, Word and other documents on Mac, Windows or Ubuntu. [GroupDocs.Annotation for Java](/annotation/java]) is a native Java API for managing annotations with comprehensive support for creating, adding, editing, deleting, extracting and exporting annotations from images and various other documents. The full list of supported document formats you could see on this [page](https://docs.groupdocs.com/annotation/java/supported-document-formats/).

        This library allows you to work not only with BMP document but also with many other types documents such as Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad and many others.

        The GroupDocs.Annotation for Java API allows you to create and [add](/annotation/java/add/bmp/) new notes, [edit](/annotation/java/edit/bmp/) annotations, [extract](/annotation/[PLATFORM_URL]/extract/bmp/) comments, annotations, and remove them from documents. The library supports 13 different annotation types, including Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction in PDF, HTML, Microsoft Word documents, spreadsheets, diagrams, presentations, drawings, images and many other file formats.

        The example (please see below) demonstrates working with BMP document, in this example you could see the main steps of how to work with GroupDocs.Annotation: Setup a license, open a document you want to work with, creating an annotation, adding data objects to set annotation properties according to your requirements and saving the result to the needed place. Also you could have a look more detailed on the supported features on our github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), or in our product [documentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps to Remove Annotations from BMP in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easier for Java developers to remove annotation details from BMP files within any Java-based application by implementing a few easy steps.
        
        *   Create Reply objects with comment and date.
        *   Instantiate SaveOptions object and set AnnotationTypes = AnnotationType.None.
        *   Call save method with resultant document path or stream and SaveOptions object.
    
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.
        
        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environment: NetBeans, Intellij IDEA, Eclipse etc
        *   Java Runtime Environment: Java 7 (1.7) and above
        *   Get the latest version of GroupDocs.Annotation for Java from [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)
    

############################# Preview ############################
preview:
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

############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Extract Annotations"
    content: |
        View and remove annotations from BMP file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.
        The live demo has the following benefits

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-bmp"
          title: "About BMP File Format"
          content: |
            Files having extension .BMP represent Bitmap Image files that are used to store bitmap digital images. These images are independent of graphics adapter and are also called device independent bitmap (DIB) file format. This independence serves the purpose of opening the file on multiple platforms such as Microsoft Windows and Mac. The BMP file format can store data as two-dimensional digital images in both monochrome as well as color format with various colour depths.
          link: "https://docs.fileformat.com/image/bmp/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Annotating From Other Popular File Formats"
    content: |
        Java annotations editor API for documents and image formats. Update annotation properties from some of the popular file formats as stated below.
    format:
        # format loop
        - name: "Remove Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/java/remove/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Remove Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/java/remove/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Remove Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/java/remove/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Remove Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/java/remove/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Remove Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/java/remove/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Remove Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/java/remove/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Remove Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/java/remove/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Remove Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/java/remove/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Remove Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/java/remove/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Remove Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Remove Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/java/remove/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Remove Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/java/remove/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/java/remove/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Remove Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/java/remove/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Remove Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/java/remove/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Remove Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/java/remove/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/java/remove/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Remove Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/java/remove/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Remove Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/java/remove/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Remove Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/java/remove/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Remove Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/java/remove/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Remove Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/java/remove/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Remove Annotation from EML"
          link: "https://products.groupdocs.com/annotation/java/remove/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Remove Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/java/remove/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Remove Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/java/remove/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Remove Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/java/remove/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Remove Annotation from VSS"
          link: "https://products.groupdocs.com/annotation/java/remove/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Remove Annotation from VST"
          link: "https://products.groupdocs.com/annotation/java/remove/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Remove Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/java/remove/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Remove Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/java/remove/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Remove Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/java/remove/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Remove Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/java/remove/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Remove Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/java/remove/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---