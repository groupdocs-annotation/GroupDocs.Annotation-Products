---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:25+03:00
draft: false

############################# Head ############################
head_title: "Add Annotations to PPS in Java Applications"
head_description: "Java API to create and add popular annotation types to PPS, images, drawings and document file formats."

############################# Header ############################
title: "Annotate PPS Files in Java"
description: "Add annotations to PPS, Microsoft Office documents, images, HTML, drawings and other file formats in any type of Java application."
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
        [GroupDocs.Annotation for Java](/annotation/java/) is a native Java API for annotations management with a comprehensive support to create, add, edit, delete, extract and export annotations from images and document file formats. Users can easily extract comments, notes, remarks and 13 different annotation types including text, graphics and watermarks in PDF, HTML, Microsoft Word documents, Excel spreadsheets, Visio diagrams, PowerPoint presentations, drawings, images, and many other file formats. The annotation-processing feature can accurately read the annotations from the imported documents and allows exporting back into the original or desired file format after implementing the annotations customization.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Steps to Add Annotations to PPS in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) makes it easy for Java developers to add various annotation types to PPS files within any Java-based application by implementing a few easy steps.

        *   Create Reply objects with comment and date.
        *   Create AreaAnnotation object, set area options and add replies.
        *   Create Annotator object and add area annotation.
        *   Save output file.
        
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
    title: "Annotation preview and code sample"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("This is area annotation");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        Annotator annotator = new Annotator("input.pps");
        annotator.add(area);
        annotator.save("output.pps");
        annotator.dispose();
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Add Annotations to Documents and Images"
    content: |
        Create and add annotations to PPS file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pps"
          title: "About PPS File Format"
          content: |
            PPS, PowerPoint Slide Show, files are created using Microsoft PowerPoint for Slide Show purpose. PPS file reading and creation is supported by Microsoft PowerPoint 97-2003. The more latest version of this file format is PPSX which is based on Office OpenXML standards. PPS files can still be read by latest versions of Microsoft PowerPoint, but newly created files can only be saved in PPSX file format. When a PPS file is shared with another user and opened, it starts as Powerpoint show unlike PPT file which opens in editable mode.

          link: "https://docs.fileformat.com/presentation/pps/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Annotating Other Popular File Formats"
    content: |
        Java annotation management library for documents and image formats. Add annotation properties to some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Add Annotation to PDF"
          link: "https://products.groupdocs.com/annotation/java/add/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Add Annotation to DOC"
          link: "https://products.groupdocs.com/annotation/java/add/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Add Annotation to DOCM"
          link: "https://products.groupdocs.com/annotation/java/add/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Add Annotation to DOCX"
          link: "https://products.groupdocs.com/annotation/java/add/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Add Annotation to DOT"
          link: "https://products.groupdocs.com/annotation/java/add/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Add Annotation to DOTX"
          link: "https://products.groupdocs.com/annotation/java/add/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Add Annotation to DOTM"
          link: "https://products.groupdocs.com/annotation/java/add/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Add Annotation to RTF"
          link: "https://products.groupdocs.com/annotation/java/add/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Add Annotation to ODT"
          link: "https://products.groupdocs.com/annotation/java/add/odt"
          description: "Open Document Text"

        # format loop
        - name: "Add Annotation to XLS"
          link: "https://products.groupdocs.com/annotation/java/add/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Add Annotation to XLSX"
          link: "https://products.groupdocs.com/annotation/java/add/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Add Annotation to XLSM"
          link: "https://products.groupdocs.com/annotation/java/add/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Add Annotation to XLSB"
          link: "https://products.groupdocs.com/annotation/java/add/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Add Annotation to ODS"
          link: "https://products.groupdocs.com/annotation/java/add/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Add Annotation to PPT"
          link: "https://products.groupdocs.com/annotation/java/add/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Add Annotation to PPTX"
          link: "https://products.groupdocs.com/annotation/java/add/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Add Annotation to PPSX"
          link: "https://products.groupdocs.com/annotation/java/add/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Add Annotation to POTM"
          link: "https://products.groupdocs.com/annotation/java/add/potm"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Add Annotation to PPTM"
          link: "https://products.groupdocs.com/annotation/java/add/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Add Annotation to ODP"
          link: "https://products.groupdocs.com/annotation/java/add/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Add Annotation to HTML"
          link: "https://products.groupdocs.com/annotation/java/add/html"
          description: "HyperText Markup Language"

        # format loop
        - name: "Add Annotation to TIFF"
          link: "https://products.groupdocs.com/annotation/java/add/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Add Annotation to JPEG"
          link: "https://products.groupdocs.com/annotation/java/add/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Add Annotation to PNG"
          link: "https://products.groupdocs.com/annotation/java/add/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Add Annotation to BMP"
          link: "https://products.groupdocs.com/annotation/java/add/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Add Annotation to EML"
          link: "https://products.groupdocs.com/annotation/java/add/eml"
          description: "E-mail Message"

        # format loop
        - name: "Add Annotation to MSG"
          link: "https://products.groupdocs.com/annotation/java/add/msg"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Add Annotation to VSD"
          link: "https://products.groupdocs.com/annotation/java/add/vsd"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Add Annotation to VSDX"
          link: "https://products.groupdocs.com/annotation/java/add/vsdx"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Add Annotation to VSS"
          link: "https://products.groupdocs.com/annotation/java/add/vss"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Add Annotation to VST"
          link: "https://products.groupdocs.com/annotation/java/add/vst"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Add Annotation to DWG"
          link: "https://products.groupdocs.com/annotation/java/add/dwg"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Add Annotation to DXF"
          link: "https://products.groupdocs.com/annotation/java/add/dxf"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Add Annotation to DCM"
          link: "https://products.groupdocs.com/annotation/java/add/dcm"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Add Annotation to WMF"
          link: "https://products.groupdocs.com/annotation/java/add/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Add Annotation to EMF"
          link: "https://products.groupdocs.com/annotation/java/add/emf"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
