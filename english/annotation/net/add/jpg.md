---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:50+03:00
draft: false

############################# Head ############################
head_title: "Add Annotation to JPG Files in C# .NET Applications"
head_description: "C# .NET annotation processing &amp; management API to add popular annotation types to JPG files, images, drawing and document file formats."

############################# Header ############################
title: "Add Annotation to JPG in .NET"
description: "Annotate images, Microsoft Office and other document file formats using 13 different annotation types including text, comments, notes etc."
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
        [GroupDocs.Annotation for .NET](https://products.groupdocs.com/annotation/net) is a native .NET API that enables users to add, edit and remove annotations from images and document file formats. You can easily employ comments, notes, remarks and various annotation types including text, graphics and watermark to PDF, HTML, Word, Excel, Visio diagrams, presentations, drawings, images, and many other file formats. The annotation-processing feature can precisely read the annotations from imported documents and allows exporting back into the original or desired file format after implementing the customization.

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps for Adding Annotations to JPG in C#"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/net) makes it easy for .NET developers to add annotation properties to JPG files from within their applications by implementing a few easy steps.

        *   Instantiate Annotator object with input document path or stream.
        *   Instantiate TextFieldAnnotation object with desired properties (position, page number etc).
        *   Call Add method and pass TextFieldAnnotation object.
        *   Call Save method with resultant document path or stream.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for .NET APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environments: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download the latest version of GroupDocs.Annotation for .NET from [Nuget](https://www.nuget.org/packages/groupdocs.annotation)
        
    code: |
        ```cs
        //Add text field annotation to the document from local disk
        using (Annotator annotator = new Annotator("input.jpg"))
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
            annotator.Save("result.jpg");
        }
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Add Annotations"
    content: |
        Add annotation to JPG file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpg"
          title: "About JPG File Format"
          content: |
            A JPEG is a type of image format that is saved using the method of lossy compression. The output image, as result of compression, is a trade-off between storage size and image quality. Users can adjust the compression level to achieve the desired quality level while at the same time reduce the storage size. Image quality is negligibly affected if 10:1 compression is applied to the image. The higher the compression value, the higher the degradation in image quality.

          link: "https://docs.fileformat.com/image/jpeg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Adding Annotations To Other File Formats"
    content: |
        Multi format documents and images annotation processing API for .NET. Add annotation to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add Annotation to PDF"
          link: "https://products.groupdocs.com/annotation/net/add/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add Annotation to DOC"
          link: "https://products.groupdocs.com/annotation/net/add/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add Annotation to DOCM"
          link: "https://products.groupdocs.com/annotation/net/add/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add Annotation to DOCX"
          link: "https://products.groupdocs.com/annotation/net/add/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add Annotation to DOT"
          link: "https://products.groupdocs.com/annotation/net/add/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add Annotation to DOTX"
          link: "https://products.groupdocs.com/annotation/net/add/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add Annotation to DOTM"
          link: "https://products.groupdocs.com/annotation/net/add/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add Annotation to RTF"
          link: "https://products.groupdocs.com/annotation/net/add/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Add Annotation to ODT"
          link: "https://products.groupdocs.com/annotation/net/add/odt"
          description: "Open Document Text"

        # format loop
        - name: "Add Annotation to XLS"
          link: "https://products.groupdocs.com/annotation/net/add/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add Annotation to XLSX"
          link: "https://products.groupdocs.com/annotation/net/add/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add Annotation to XLSM"
          link: "https://products.groupdocs.com/annotation/net/add/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add Annotation to XLSB"
          link: "https://products.groupdocs.com/annotation/net/add/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add Annotation to ODS"
          link: "https://products.groupdocs.com/annotation/net/add/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add Annotation to PPT"
          link: "https://products.groupdocs.com/annotation/net/add/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add Annotation to PPTX"
          link: "https://products.groupdocs.com/annotation/net/add/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add Annotation to PPSX"
          link: "https://products.groupdocs.com/annotation/net/add/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Add Annotation to POTM"
          link: "https://products.groupdocs.com/annotation/net/add/potm"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Add Annotation to PPTM"
          link: "https://products.groupdocs.com/annotation/net/add/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Add Annotation to PPS"
          link: "https://products.groupdocs.com/annotation/net/add/pps"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Add Annotation to ODP"
          link: "https://products.groupdocs.com/annotation/net/add/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add Annotation to HTML"
          link: "https://products.groupdocs.com/annotation/net/add/html"
          description: "HyperText Markup Language"

        # format loop
        - name: "Add Annotation to TIFF"
          link: "https://products.groupdocs.com/annotation/net/add/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add Annotation to JPEG"
          link: "https://products.groupdocs.com/annotation/net/add/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Add Annotation to PNG"
          link: "https://products.groupdocs.com/annotation/net/add/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add Annotation to BMP"
          link: "https://products.groupdocs.com/annotation/net/add/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Add Annotation to EML"
          link: "https://products.groupdocs.com/annotation/net/add/eml"
          description: "E-mail Message"

        # format loop
        - name: "Add Annotation to MSG"
          link: "https://products.groupdocs.com/annotation/net/add/msg"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Add Annotation to VSD"
          link: "https://products.groupdocs.com/annotation/net/add/vsd"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Add Annotation to VSDX"
          link: "https://products.groupdocs.com/annotation/net/add/vsdx"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Add Annotation to VSS"
          link: "https://products.groupdocs.com/annotation/net/add/vss"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Add Annotation to VST"
          link: "https://products.groupdocs.com/annotation/net/add/vst"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Add Annotation to DWG"
          link: "https://products.groupdocs.com/annotation/net/add/dwg"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Add Annotation to DXF"
          link: "https://products.groupdocs.com/annotation/net/add/dxf"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Add Annotation to DCM"
          link: "https://products.groupdocs.com/annotation/net/add/dcm"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Add Annotation to WMF"
          link: "https://products.groupdocs.com/annotation/net/add/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Add Annotation to EMF"
          link: "https://products.groupdocs.com/annotation/net/add/emf"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
