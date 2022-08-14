
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/edit/cad"/>

############################# Head ############################
head_title: "Edit Annotations in CAD in Net Application"
head_description: "Net API to create and Edit popular annotation types in CAD, images, drawings and document file formats."

############################# Header ############################
title: "Edit CAD Files in Net"
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

        This library allows you to work not only with CAD document but also with many other types documents such as Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad and many others.

        The GroupDocs.Annotation for Net API allows you to create and [add](/annotation/net/add/cad/) new notes, edit annotations, [extract](/annotation/net/extract/cad/) comments, annotations, and [remove](/annotation/net/remove/cad/) them from documents. The library supports 13 different annotation types, including Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction in PDF, HTML, Microsoft Word documents, spreadsheets, diagrams, presentations, drawings, images and many other file formats.

        The example (please see below) demonstrates working with CAD document, in this example you could see the main steps of how to work with GroupDocs.Annotation: Setup a license, open a document you want to work with, creating an annotation, adding data objects to set annotation properties according to your requirements and saving the result to the needed place. Also you could have a look more detailed on the supported features on our github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), or in our product [documentation](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps to Edit Annotations in CAD in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easier for Net developers to update various annotation properties from CAD files within any Net-based application by implementing a few easy steps.
        
        *   Instantiate Annotator object with input document path or stream with instantiated LoadOptions with ImportAnnotations = true.
        *   Create some AnnotationBase implementation and set Id of existed annotation (if annotation with that Id not found, nothing will be changed) or path list of annotations (all existed annotations will be removed).
        *   Call update method of Annotator object with passed annotations.
        *   Call save method with resultant document path or stream and SaveOptions object.
    
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
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Updated first comment",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Updated second comment",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Annotate Documents and Images"
    content: |
        Read and edit annotations from CAD file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.
        The live demo has the following benefits

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-cad"
          title: "About CAD File Format"
          content: |
            CAD stands for Computer Aided Design. The term CADD (for Computer Aided Design and Drafting) is also used. It is used for a 3D graphics file format and may contain 2D or 3D designs. CAD file is a digital file format of an object generated and used by CAD software. A CAD file contains a technical drawing, blueprint, schematic, or 3D rendering of an object. There may be other CAD tools that can be used to create, open, edit and export these .cad files to more widely used CAD drawing file formats.
          link: "https://docs.fileformat.com/image/cad/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Annotating From Other Popular File Formats"
    content: |
        Java annotations editor API for documents and image formats. Update annotation properties from some of the popular file formats as stated below.
    format:
        # format loop
        - name: "Edit Annotation in PDF"
          link: "https://products.groupdocs.com/annotation/net/edit/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Edit Annotation in DOC"
          link: "https://products.groupdocs.com/annotation/net/edit/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Edit Annotation in DOCM"
          link: "https://products.groupdocs.com/annotation/net/edit/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Edit Annotation in DOCX"
          link: "https://products.groupdocs.com/annotation/net/edit/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Edit Annotation in DOT"
          link: "https://products.groupdocs.com/annotation/net/edit/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Edit Annotation in DOTX"
          link: "https://products.groupdocs.com/annotation/net/edit/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Edit Annotation in RTF"
          link: "https://products.groupdocs.com/annotation/net/edit/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Edit Annotation in ODT"
          link: "https://products.groupdocs.com/annotation/net/edit/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Edit Annotation in XLS"
          link: "https://products.groupdocs.com/annotation/net/edit/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Edit Annotation in XLSX"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Edit Annotation in XLSM"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit Annotation in XLSB"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Edit Annotation in ODS"
          link: "https://products.groupdocs.com/annotation/net/edit/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Edit Annotation in PPT"
          link: "https://products.groupdocs.com/annotation/net/edit/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Edit Annotation in PPTX"
          link: "https://products.groupdocs.com/annotation/net/edit/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Edit Annotation in PPSX"
          link: "https://products.groupdocs.com/annotation/net/edit/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Edit Annotation in POTM"
          link: "https://products.groupdocs.com/annotation/net/edit/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Edit Annotation in PPTM"
          link: "https://products.groupdocs.com/annotation/net/edit/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Edit Annotation in PPS"
          link: "https://products.groupdocs.com/annotation/net/edit/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Edit Annotation in ODP"
          link: "https://products.groupdocs.com/annotation/net/edit/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Edit Annotation in HTML"
          link: "https://products.groupdocs.com/annotation/net/edit/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Edit Annotation in TIFF"
          link: "https://products.groupdocs.com/annotation/net/edit/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Edit Annotation in JPEG"
          link: "https://products.groupdocs.com/annotation/net/edit/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Edit Annotation in PNG"
          link: "https://products.groupdocs.com/annotation/net/edit/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Edit Annotation in EML"
          link: "https://products.groupdocs.com/annotation/net/edit/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Edit Annotation in MSG"
          link: "https://products.groupdocs.com/annotation/net/edit/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Edit Annotation in VSD"
          link: "https://products.groupdocs.com/annotation/net/edit/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Edit Annotation in VSDX"
          link: "https://products.groupdocs.com/annotation/net/edit/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Edit Annotation in VSS"
          link: "https://products.groupdocs.com/annotation/net/edit/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Edit Annotation in VST"
          link: "https://products.groupdocs.com/annotation/net/edit/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Edit Annotation in DWG"
          link: "https://products.groupdocs.com/annotation/net/edit/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Edit Annotation in DXF"
          link: "https://products.groupdocs.com/annotation/net/edit/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Edit Annotation in DCM"
          link: "https://products.groupdocs.com/annotation/net/edit/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Edit Annotation in WMF"
          link: "https://products.groupdocs.com/annotation/net/edit/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Edit Annotation in EMF"
          link: "https://products.groupdocs.com/annotation/net/edit/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---