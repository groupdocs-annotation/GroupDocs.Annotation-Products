---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:57+03:00
draft: false

############################# Head ############################
head_title: "Read &amp; Edit Annotations in POTM Files in C# .NET Applications"
head_description: "C# .NET annotation editor API to update popular annotation types to POTM files, images, drawing and document file formats."

############################# Header ############################
title: "Edit Annotations in POTM File in .NET"
description: ".NET annotation editor for images, Microsoft Office and other document file formats. Annotate documents using 13 different annotation types like; area, text, notes, watermark etc."
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
        [GroupDocs.Annotation for .NET](https://products.groupdocs.com/annotation/net) is a native .NET annotation management & editor API read, add, update, remove and extract annotations from images and document file formats. Users can easily update comments, notes, remarks and various annotation types including text, graphics and watermark in PDF, HTML, Word, Excel, Visio diagrams, presentations, drawings, images, and many other file formats. The annotation-processing feature can precisely read the annotations from imported documents and allows exporting back into the original or desired file format after implementing the customization.

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps for Editing Annotations from POTM in C#"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/net) makes it easy for .NET developers to edit annotation details from POTM files within their applications by implementing a few easy steps.

        *   Instantiate Annotator object with input document path or stream.
        *   Create some AnnotationBase implementation and set Id of existed annotation (if annotation with that Id not found, nothing will be changed) or path list of annotations (all existed annotations will be removed).
        *   Call Update method of Annotator object with passed annotations.
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
        // open annotated document
        using (Annotator annotator = new Annotator("result.potm"))
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
                annotator.Save("result.potm");
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Update Annotations"
    content: |
        Edit annotation in POTM file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-potm"
          title: "About POTM File Format"
          content: |
            Files with POTM extension are Microsoft PowerPoint template files with support for Macros. POTM files are created with PowerPoint 2007 or above and contains default settings that can be used to create further presentation files. These settings can include styles, backgrounds, colour palette, fonts and defaults along with macros that consist of custom functions for doing particular task. They may also be opened by a previous version of PowerPoint with Open XML document support installed. POTM files can be opened in Microsoft PowerPoint for editing like any other PowerPoint file.

          link: "https://docs.fileformat.com/presentation/potm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Annotations Within Other File Formats"
    content: |
        Multi format documents and images annotation editor API for .NET. Update annotation from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Edit Annotation in PDF"
          link: "https://products.groupdocs.com/annotation/net/edit/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Edit Annotation in DOC"
          link: "https://products.groupdocs.com/annotation/net/edit/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Edit Annotation in DOCM"
          link: "https://products.groupdocs.com/annotation/net/edit/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Edit Annotation in DOCX"
          link: "https://products.groupdocs.com/annotation/net/edit/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Edit Annotation in DOT"
          link: "https://products.groupdocs.com/annotation/net/edit/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Edit Annotation in DOTX"
          link: "https://products.groupdocs.com/annotation/net/edit/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Edit Annotation in DOTM"
          link: "https://products.groupdocs.com/annotation/net/edit/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Edit Annotation in RTF"
          link: "https://products.groupdocs.com/annotation/net/edit/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Edit Annotation in ODT"
          link: "https://products.groupdocs.com/annotation/net/edit/odt"
          description: "Open Document Text"

        # format loop
        - name: "Edit Annotation in XLS"
          link: "https://products.groupdocs.com/annotation/net/edit/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Edit Annotation in XLSX"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Edit Annotation in XLSM"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit Annotation in XLSB"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Edit Annotation in ODS"
          link: "https://products.groupdocs.com/annotation/net/edit/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Edit Annotation in PPT"
          link: "https://products.groupdocs.com/annotation/net/edit/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Edit Annotation in PPTX"
          link: "https://products.groupdocs.com/annotation/net/edit/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Edit Annotation in PPSX"
          link: "https://products.groupdocs.com/annotation/net/edit/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Edit Annotation in POTM"
          link: "https://products.groupdocs.com/annotation/net/edit/potm"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Edit Annotation in PPTM"
          link: "https://products.groupdocs.com/annotation/net/edit/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Edit Annotation in PPS"
          link: "https://products.groupdocs.com/annotation/net/edit/pps"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Edit Annotation in ODP"
          link: "https://products.groupdocs.com/annotation/net/edit/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Edit Annotation in HTML"
          link: "https://products.groupdocs.com/annotation/net/edit/html"
          description: "HyperText Markup Language"

        # format loop
        - name: "Edit Annotation in TIFF"
          link: "https://products.groupdocs.com/annotation/net/edit/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Edit Annotation in JPEG"
          link: "https://products.groupdocs.com/annotation/net/edit/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Edit Annotation in PNG"
          link: "https://products.groupdocs.com/annotation/net/edit/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Edit Annotation in BMP"
          link: "https://products.groupdocs.com/annotation/net/edit/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Edit Annotation in EML"
          link: "https://products.groupdocs.com/annotation/net/edit/eml"
          description: "E-mail Message"

        # format loop
        - name: "Edit Annotation in MSG"
          link: "https://products.groupdocs.com/annotation/net/edit/msg"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Edit Annotation in VSD"
          link: "https://products.groupdocs.com/annotation/net/edit/vsd"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Edit Annotation in VSDX"
          link: "https://products.groupdocs.com/annotation/net/edit/vsdx"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Edit Annotation in VSS"
          link: "https://products.groupdocs.com/annotation/net/edit/vss"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Edit Annotation in VST"
          link: "https://products.groupdocs.com/annotation/net/edit/vst"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Edit Annotation in DWG"
          link: "https://products.groupdocs.com/annotation/net/edit/dwg"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Edit Annotation in DXF"
          link: "https://products.groupdocs.com/annotation/net/edit/dxf"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Edit Annotation in DCM"
          link: "https://products.groupdocs.com/annotation/net/edit/dcm"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Edit Annotation in WMF"
          link: "https://products.groupdocs.com/annotation/net/edit/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Edit Annotation in EMF"
          link: "https://products.groupdocs.com/annotation/net/edit/emf"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
