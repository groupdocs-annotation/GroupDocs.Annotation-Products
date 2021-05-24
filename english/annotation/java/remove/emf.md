---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:44+03:00
draft: false

############################# Head ############################
head_title: "Remove Annotations from EMF in Java Applications"
head_description: "Javaannotation API to remove popular annotation types from EMF, images, drawings and document file formats."

############################# Header ############################
title: "Remove Annotations from EMF in Java"
description: "Delete already added annotations from Microsoft Office, images, drawings, HTML and other document file formats in any type of Java application."
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
        [GroupDocs.Annotation for Java](https://products.groupdocs.com/annotation/java) is a native Java annotations management library to view, add, update, erase, extract or export annotations from images and document file formats. Users can easily delete comments, notes, remarks and various annotation types including text, graphics and watermarks in PDF, HTML, Word, Excel, Visio diagrams, presentations, drawings, images, and many other file formats. The annotation-processing feature can precisely read the annotations from imported documents and allows exporting back into the original or desired file format after implementing the customization.

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to Delete Annotations from EMF in Java"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/java) makes it easier for Java developers to remove annotation details from EMF files within any Java-based application by implementing a few easy steps.

        *   Instantiate Annotator object with input document path or stream.
        *   Instantiate SaveOptions object and set AnnotationTypes = AnnotationType.None.
        *   Call save method with resultant document path or stream and SaveOptions object.
        
    title_right: "System Requirements"
    content_right: |
        GroupDocs.Annotation for Java APIs are supported on all major platforms and operating systems. Before executing the code below, please make sure that you have the following prerequisites installled on your system.

        *   Operating Systems: Microsoft Windows, Linux, MacOS
        *   Development Environment: NetBeans, Intellij IDEA, Eclipse etc
        *   Java Runtime Environment: J2SE 6.0 and above
        *   Get the latest version of GroupDocs.Annotation for Java from [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-conversion)
        
    code: |
        ```java
        Annotator annotator = new Annotator("C://input.emf");
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);
        annotator.save("C://output.emf", saveOptions);
        annotator.dispose();
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Delete Annotations from Documents and Images"
    content: |
        View and remove annotations from EMF file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-emf"
          title: "About EMF File Format"
          content: |
            Enhanced metafile format (EMF) stores graphical images device-independently. Metafiles of EMF comprises of variable-length records in chronological order that can render the stored image after parsing on any output device. These variable-length records can be definitions of enclosed objects, commands for drawing, and graphics properties critical to render the image accurately. When a device opens an EMF metafile using its own graphics environment, the proportions, dimensions, colors and other graphic properties of original image remains same regardless of the opening device platform.

          link: "https://docs.fileformat.com/image/emf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Annotating From Other Popular File Formats"
    content: |
        Java API to remove annotations from documents and image file formats. Erase annotation properties from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Remove Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/java/remove/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Remove Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/java/remove/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Remove Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/java/remove/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Remove Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/java/remove/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Remove Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/java/remove/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Remove Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/java/remove/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Remove Annotation from DOTM"
          link: "https://products.groupdocs.com/annotation/java/remove/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Remove Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/java/remove/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Remove Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/java/remove/odt"
          description: "Open Document Text"

        # format loop
        - name: "Remove Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/java/remove/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Remove Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Remove Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Remove Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/java/remove/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Remove Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/java/remove/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/java/remove/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Remove Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/java/remove/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Remove Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/java/remove/potm"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Remove Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/java/remove/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Remove Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/java/remove/pps"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Remove Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/java/remove/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Remove Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/java/remove/html"
          description: "HyperText Markup Language"

        # format loop
        - name: "Remove Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/java/remove/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Remove Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/java/remove/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Remove Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/java/remove/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Remove Annotation from BMP"
          link: "https://products.groupdocs.com/annotation/java/remove/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Remove Annotation from EML"
          link: "https://products.groupdocs.com/annotation/java/remove/eml"
          description: "E-mail Message"

        # format loop
        - name: "Remove Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/java/remove/msg"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Remove Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/java/remove/vsd"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Remove Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/java/remove/vsdx"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Remove Annotation from VSS"
          link: "https://products.groupdocs.com/annotation/java/remove/vss"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Remove Annotation from VST"
          link: "https://products.groupdocs.com/annotation/java/remove/vst"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Remove Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/java/remove/dwg"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Remove Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/java/remove/dxf"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Remove Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/java/remove/dcm"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Remove Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/java/remove/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Remove Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/java/remove/emf"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
