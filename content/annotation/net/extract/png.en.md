
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/extract/png"/>

############################# Head ############################
head_title: "Extract Annotations from PNG in Net Application"
head_description: "Net API to create and Extract popular annotation types from PNG, images, drawings and document file formats."

############################# Header ############################
title: "Extract PNG Files from Net"
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
        img_alt: "GroupDocs.Annotation for Net"
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
    title: "About GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API is a library that allows you to add annotations to PDF, Word and other documents on Mac, Windows or Ubuntu. [GroupDocs.Annotation for Net](/annotation/net]) is a native Net API for managing annotations with comprehensive support for creating, adding, editing, deleting, extracting and exporting annotations from images and various other documents. The full list of supported document formats you could see on this [page](https://docs.groupdocs.com/annotation/net/supported-document-formats/).

        This library allows you to work not only with PNG document but also with many other types documents such as Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad and many others.

        The GroupDocs.Annotation for Net API allows you to create and [add](/annotation/net/add/png/) new notes, [edit](/annotation/net/edit/png/) annotations, extract comments, annotations, and [remove](/annotation/net/remove/png/) them from documents. The library supports 13 different annotation types, including Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction in PDF, HTML, Microsoft Word documents, spreadsheets, diagrams, presentations, drawings, images and many other file formats.

        The example (please see below) demonstrates working with PNG document, in this example you could see the main steps of how to work with GroupDocs.Annotation: Setup a license, open a document you want to work with, creating an annotation, adding data objects to set annotation properties according to your requirements and saving the result to the needed place. Also you could have a look more detailed on the supported features on our github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), or in our product [documentation](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps to Extract Annotations from PNG in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easy for Net developers to annotate documents and extract annotation information from PNG files within any Net-based application by implementing a few easy steps.
        
        *   Create Reply objects with comment and date.
        *   Instantiate LoadOptions object and call SetImportAnnotations with true argument.
        *   Define variable with type List.
        *   Call get method and return result to variable above.
    
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for Net APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.
        
        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Annotation for .NET from [NuGet](https://www.nuget.org/packages/groupdocs.annotation)
    

############################# Preview ############################
preview:
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
    title: "Live Demos to Delete Annotations from Documents and Images"
    content: |
        Extract annotation information from PNG file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.
        The live demo has the following benefits

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-png"
          title: "About PNG File Format"
          content: |
            PNG, Portable Network Graphics, refers to a type of raster image file format that use loseless compression. This file format was created as a replacement of Graphics Interchange Format (GIF) and has no copyright limitations. However, PNG file format does not support animations. PNG file format supports loseless image compression that makes it popular among its users. With the passage of time, PNG has evolved as one of the mostly used image file format. Almost all Operating Systems have support for opening PNG files. For example, Microsoft Windows viewer has the capability to open PNG files as the OS has by default the support available as part of installation.
          link: "https://docs.fileformat.com/image/png/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Extracting Annotations From Other Supported File Formats"
    content: |
        Java annotations editor API for documents and image formats. Update annotation properties from some of the popular file formats as stated below.
    format:
        # format loop
        - name: "Extract Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/net/extract/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Extract Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/net/extract/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Extract Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/net/extract/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Extract Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/net/extract/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Extract Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/net/extract/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Extract Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/net/extract/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Extract Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/net/extract/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Extract Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/net/extract/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Extract Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/net/extract/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Extract Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Extract Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Extract Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Extract Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/net/extract/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Extract Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/net/extract/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Extract Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/net/extract/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Extract Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/net/extract/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Extract Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/net/extract/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Extract Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/net/extract/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Extract Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/net/extract/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Extract Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/net/extract/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Extract Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/net/extract/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Extract Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/net/extract/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Extract Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/net/extract/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Extract Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/net/extract/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Extract Annotation from EML"
          link: "https://products.groupdocs.com/annotation/net/extract/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Extract Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/net/extract/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Extract Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/net/extract/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Extract Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/net/extract/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Extract Annotation from VSS"
          link: "https://products.groupdocs.com/annotation/net/extract/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Extract Annotation from VST"
          link: "https://products.groupdocs.com/annotation/net/extract/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Extract Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/net/extract/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Extract Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/net/extract/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Extract Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/net/extract/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Extract Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/net/extract/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Extract Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/net/extract/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---