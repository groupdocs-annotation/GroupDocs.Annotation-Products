---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:45:06+03:00
draft: false

############################# Head ############################
head_title: "Remove Annotations from DOCM Files in C# .NET Applications"
head_description: "C# .NET annotation API to remove popular annotation types to DOCM files, images, drawing and document file formats."

############################# Header ############################
title: "Remove Annotations from DOCM in C#"
description: "Delete all previously added annotations from Microsoft Office, images, web, drawings and other document file formats in any type of .NET application."
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
        img_alt: "GroupDocs.Annotation for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: ".NET"

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
    title: "About GroupDocs.Annotation for .NET API"
    content: |
        [GroupDocs.Annotation for .NET](https://products.groupdocs.com/annotation/net) is a native .NET annotation processing API to view, add, modify, remove and extract annotations from images and document file formats. Users can easily delete comments, notes, remarks and various annotation types including text, graphics and watermarks in PDF, HTML, Word, Excel, Visio diagrams, presentations, drawings, images, and many other file formats. The annotation-processing feature can precisely read the annotations from imported documents and allows exporting back into the original or desired file format after implementing the customization.

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps for Removing Annotations from DOCM"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/net) makes it easy for .NET developers to remove annotation details from DOCM files within their applications by implementing a few easy steps.

        *   Instantiate Annotator object with input document path or stream.
        *   Instantiate SaveOptions object and set AnnotationTypes = AnnotationType.None.
        *   Call Save method with resultant document path or stream and SaveOptions object.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Annotation for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.annotation)
        
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.docm"))
        {
        	annotator.Remove(0);
        	annotator.Save("removed.docm");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.docm"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp[0]);
        	annotator.Save("removed.docm");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.docm"))
        {
        	var idList = new List{1, 2, 3};
        	annotator.Remove(idList);
        	annotator.Save("removed.docm");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
        using (Annotator annotator = new Annotator("result.docm"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp);
        	annotator.Save("removed.docm");
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Remove Annotations"
    content: |
        Delete annotation from DOCM file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docm"
          title: "About DOCM File Format"
          content: |
            DOCM files are Microsoft Word 2007 or higher generated documents with the ability to run macros. It is similar to DOCX file format but the ability to run macros makes it different from DOCX. Like DOCX, DOCM files can be store text, images, tables, shapes, charts and other contents.The capability to run macros make it easy to save time by executing the series of commands in the form of recorded actions for automatic completion of a task. DOCM files can be opened and edited in Microsoft Word 2007 and above.

          link: "https://docs.fileformat.com/word-processing/docm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Erasing Annotations From Other Supported File Formats"
    content: |
        Multi format documents and images annotation removing API for .NET. Delete annotation from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Remove Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/net/remove/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Remove Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/net/remove/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Remove Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/net/remove/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Remove Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/net/remove/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Remove Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/net/remove/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Remove Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/net/remove/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Remove Annotation from DOTM"
          link: "https://products.groupdocs.com/annotation/net/remove/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Remove Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/net/remove/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Remove Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/net/remove/odt"
          description: "Open Document Text"

        # format loop
        - name: "Remove Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/net/remove/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Remove Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Remove Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/net/remove/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Remove Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/net/remove/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/net/remove/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Remove Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/net/remove/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Remove Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/net/remove/potm"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Remove Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/net/remove/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/net/remove/pps"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Remove Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/net/remove/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Remove Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/net/remove/html"
          description: "HyperText Markup Language"

        # format loop
        - name: "Remove Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/net/remove/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Remove Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/net/remove/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Remove Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/net/remove/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Remove Annotation from BMP"
          link: "https://products.groupdocs.com/annotation/net/remove/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Remove Annotation from EML"
          link: "https://products.groupdocs.com/annotation/net/remove/eml"
          description: "E-mail Message"

        # format loop
        - name: "Remove Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/net/remove/msg"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Remove Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/net/remove/vsd"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Remove Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/net/remove/vsdx"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Remove Annotation from VSS"
          link: "https://products.groupdocs.com/annotation/net/remove/vss"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Remove Annotation from VST"
          link: "https://products.groupdocs.com/annotation/net/remove/vst"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Remove Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/net/remove/dwg"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Remove Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/net/remove/dxf"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Remove Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/net/remove/dcm"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Remove Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/net/remove/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Remove Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/net/remove/emf"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
