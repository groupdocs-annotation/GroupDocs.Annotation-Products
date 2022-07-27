
---
############################# Static ############################
layout: "auto-gen"
date: 2022-07-05T12:44:18+03:00
draft: false

############################# Head ############################
head_title: "Remove Annotations from DOTM in Net Application"
head_description: "Net API to create and Remove popular annotation types from DOTM, images, drawings and document file formats."

############################# Header ############################
title: "Remove DOTM Files from Net"
description: "Add annotations from DOTM, Microsoft Office documents, images, HTML, drawings and other file formats in any type of Net application."
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

        This library allows you to work not only with DOTM document but also with many other types documents such as Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad and many others.

        The GroupDocs.Annotation for Net API allows you to create and [add](/annotation/net/add/dotm/) new notes, [edit](/annotation/net/edit/dotm/) annotations, [extract](/annotation/[PLATFORM_URL]/extract/dotm/) comments, annotations, and remove them from documents. The library supports 13 different annotation types, including Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction in PDF, HTML, Microsoft Word documents, spreadsheets, diagrams, presentations, drawings, images and many other file formats.

        The example (please see below) demonstrates working with DOTM document, in this example you could see the main steps of how to work with GroupDocs.Annotation: Setup a license, open a document you want to work with, creating an annotation, adding data objects to set annotation properties according to your requirements and saving the result to the needed place. Also you could have a look more detailed on the supported features on our github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), or in our product [documentation](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps to Remove Annotations from DOTM in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easier for Net developers to remove annotation details from DOTM files within any Net-based application by implementing a few easy steps.
        
        *   Create Reply objects with comment and date.
        *   Instantiate SaveOptions object and set AnnotationTypes = AnnotationType.None.
        *   Call save method with resultant document path or stream and SaveOptions object.
    
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for Net APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installed on your system.
        
        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Annotation for .NET from [NuGet](https://www.nuget.org/packages/groupdocs.annotation)
    
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

############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Extract Annotations"
    content: |
        View and remove annotations from DOTM file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.
        The live demo has the following benefits

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dotm"
          title: "About DOTM File Format"
          content: |
            
          link: "https://docs.fileformat.com/image/dotm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Annotating From Other Popular File Formats"
    content: |
        Java annotations editor API for documents and image formats. Update annotation properties from some of the popular file formats as stated below.
    format:
        # format loop
        - name: "Remove Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/net/remove/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Remove Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/net/remove/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Remove Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/net/remove/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Remove Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/net/remove/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Remove Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/net/remove/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Remove Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/net/remove/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Remove Annotation from DOTM"
          link: "https://products.groupdocs.com/annotation/net/remove/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Remove Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/net/remove/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Remove Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/net/remove/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Remove Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/net/remove/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Remove Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Remove Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/net/remove/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Remove Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/net/remove/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/net/remove/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Remove Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/net/remove/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Remove Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/net/remove/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Remove Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/net/remove/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/net/remove/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Remove Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/net/remove/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Remove Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/net/remove/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Remove Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/net/remove/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Remove Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/net/remove/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Remove Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/net/remove/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Remove Annotation from EML"
          link: "https://products.groupdocs.com/annotation/net/remove/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Remove Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/net/remove/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Remove Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/net/remove/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Remove Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/net/remove/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Remove Annotation from VSS"
          link: "https://products.groupdocs.com/annotation/net/remove/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Remove Annotation from VST"
          link: "https://products.groupdocs.com/annotation/net/remove/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Remove Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/net/remove/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Remove Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/net/remove/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Remove Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/net/remove/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Remove Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/net/remove/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Remove Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/net/remove/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---