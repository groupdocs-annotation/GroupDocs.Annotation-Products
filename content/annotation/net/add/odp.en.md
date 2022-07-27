
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/add/odp"/>

############################# Head ############################
head_title: "Add Annotations to ODP in Net Application"
head_description: "Net API to create and Add popular annotation types to ODP, images, drawings and document file formats."

############################# Header ############################
title: "Add ODP Files to Net"
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
        GroupDocs.Annotation for Net API is a library that allows you to add annotations to PDF, Word and other documents on Mac, Windows or Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) is a native Net API for managing annotations with comprehensive support for creating, adding, editing, deleting, extracting and exporting annotations from images and various other documents. The full list of supported document formats you could see on this [page](https://docs.groupdocs.com/annotation/net/supported-document-formats/).

        This library allows you to work not only with ODP document but also with many other types documents such as Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad and many others.

        The GroupDocs.Annotation for Net API allows you to create and add new notes, [edit](/annotation/net/edit/odp/) annotations, [extract](/annotation/net/extract/odp/) comments, annotations, and [remove](/annotation/net/remove/odp/) them from documents. The library supports 13 different annotation types, including Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction in PDF, HTML, Microsoft Word documents, spreadsheets, diagrams, presentations, drawings, images and many other file formats.

        The example (please see below) demonstrates working with ODP document, in this example you could see the main steps of how to work with GroupDocs.Annotation: Setup a license, open a document you want to work with, creating an annotation, adding data objects to set annotation properties according to your requirements and saving the result to the needed place. Also you could have a look more detailed on the supported features on our github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), or in our product [documentation](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps to Add Annotations to ODP in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easy for Net developers to add various annotation types to ODP files within any Net-based application by implementing a few easy steps.
        
        *   Create Reply objects with comment and date.
        *   Create AreaAnnotation object, set area options and add replies.
        *   Create Annotator object and add area annotation.
        *   Save output file.
    
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
    title: "Annotation preview and code sample"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
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
                Message = "This is text field annotation",
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
                        Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Add Annotations to Documents and Images"
    content: |
        Create and add annotations to ODP file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.
        The live demo has the following benefits

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odp"
          title: "About ODP File Format"
          content: |
            Files with ODP extension represent presentation file format used by OpenOffice.org in the OASISOpen standard. A presentation file is a collection of slides where each slide can comprise of text, images, formatting, animations, and other media. These slides are presented to audience in the form of slideshows with custom presentation settings. ODP files can be opened by applications that conform to the OpenDocument format (such as OpenOffice or StarOffice).
          link: "https://docs.fileformat.com/image/odp/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Annotating Other Popular File Formats"
    content: |
        Java annotations editor API for documents and image formats. Update annotation properties from some of the popular file formats as stated below.
    format:
        # format loop
        - name: "Add Annotation to PDF"
          link: "https://products.groupdocs.com/annotation/net/add/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add Annotation to DOC"
          link: "https://products.groupdocs.com/annotation/net/add/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add Annotation to DOCM"
          link: "https://products.groupdocs.com/annotation/net/add/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add Annotation to DOCX"
          link: "https://products.groupdocs.com/annotation/net/add/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add Annotation to DOT"
          link: "https://products.groupdocs.com/annotation/net/add/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add Annotation to DOTX"
          link: "https://products.groupdocs.com/annotation/net/add/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add Annotation to RTF"
          link: "https://products.groupdocs.com/annotation/net/add/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Add Annotation to ODT"
          link: "https://products.groupdocs.com/annotation/net/add/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Add Annotation to XLS"
          link: "https://products.groupdocs.com/annotation/net/add/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add Annotation to XLSX"
          link: "https://products.groupdocs.com/annotation/net/add/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add Annotation to XLSM"
          link: "https://products.groupdocs.com/annotation/net/add/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add Annotation to XLSB"
          link: "https://products.groupdocs.com/annotation/net/add/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add Annotation to ODS"
          link: "https://products.groupdocs.com/annotation/net/add/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add Annotation to PPT"
          link: "https://products.groupdocs.com/annotation/net/add/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add Annotation to PPTX"
          link: "https://products.groupdocs.com/annotation/net/add/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add Annotation to PPSX"
          link: "https://products.groupdocs.com/annotation/net/add/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Add Annotation to POTM"
          link: "https://products.groupdocs.com/annotation/net/add/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Add Annotation to PPTM"
          link: "https://products.groupdocs.com/annotation/net/add/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Add Annotation to PPS"
          link: "https://products.groupdocs.com/annotation/net/add/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add Annotation to ODP"
          link: "https://products.groupdocs.com/annotation/net/add/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add Annotation to HTML"
          link: "https://products.groupdocs.com/annotation/net/add/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Add Annotation to TIFF"
          link: "https://products.groupdocs.com/annotation/net/add/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add Annotation to JPEG"
          link: "https://products.groupdocs.com/annotation/net/add/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Add Annotation to PNG"
          link: "https://products.groupdocs.com/annotation/net/add/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add Annotation to EML"
          link: "https://products.groupdocs.com/annotation/net/add/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Add Annotation to MSG"
          link: "https://products.groupdocs.com/annotation/net/add/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Add Annotation to VSD"
          link: "https://products.groupdocs.com/annotation/net/add/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Add Annotation to VSDX"
          link: "https://products.groupdocs.com/annotation/net/add/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Add Annotation to VSS"
          link: "https://products.groupdocs.com/annotation/net/add/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Add Annotation to VST"
          link: "https://products.groupdocs.com/annotation/net/add/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Add Annotation to DWG"
          link: "https://products.groupdocs.com/annotation/net/add/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Add Annotation to DXF"
          link: "https://products.groupdocs.com/annotation/net/add/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Add Annotation to DCM"
          link: "https://products.groupdocs.com/annotation/net/add/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Add Annotation to WMF"
          link: "https://products.groupdocs.com/annotation/net/add/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Add Annotation to EMF"
          link: "https://products.groupdocs.com/annotation/net/add/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---