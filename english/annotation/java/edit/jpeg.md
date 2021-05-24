---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:31+03:00
draft: false

############################# Head ############################
head_title: "Edit JPEG File Annotations in Java Applications"
head_description: "Java annotations editor API to update popular annotation types from JPEG, images, drawings and document file formats."

############################# Header ############################
title: "Edit Annotations in JPEG File in Java"
description: "Java annotation editor for images, Microsoft Office and other document file formats. Annotate JPEG files using 13 different annotation types like; area, text, notes, watermark etc."
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
        [GroupDocs.Annotation for Java](https://products.groupdocs.com/annotation/java) is a native Java annotations manipulation solution to efficiently view, add, update, delete and extract annotations from images and document file formats. Users can easily edit comments, notes, remarks and various annotation types including text, graphics and watermark in PDF, HTML, Word, Excel, Visio diagrams, presentations, drawings, images, and many other file formats. The annotation-processing feature can precisely read the annotations from imported documents and allows exporting back into the original or desired file format after implementing the customization.

############################# Steps ############################
steps:
    enable: true
    title_left: "Steps to Edit Annotations from JPEG in Java"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/java) makes it easier for Java developers to update various annotation properties from JPEG files within any Java-based application by implementing a few easy steps.

        *   Instantiate Annotator object with input document path or stream with instantiated LoadOptions with ImportAnnotations = true.
        *   Create some AnnotationBase implementation and set Id of existed annotation (if annotation with that Id not found, nothing will be changed) or path list of annotations (all existed annotations will be removed).
        *   Call update method of Annotator object with passed annotations.
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
        String outputPath = "UpdateAnnotation.jpeg";
        Annotator annotator = new Annotator("input.jpeg");
        
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        loadOptions.setImportAnnotations(true);
        
        // open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);
        
        // suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // update annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```
        
############################# Demos ############################
demos:
    enable: true
    title: "Live Demos to Modify Annotations from Documents and Images"
    content: |
        Read and edit annotations from JPEG file right now by visiting [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) website.  
        The live demo has the following benefits
        
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpeg"
          title: "About JPEG File Format"
          content: |
            A JPEG is a type of image format that is saved using the method of lossy compression. The output image, as result of compression, is a trade-off between storage size and image quality. Users can adjust the compression level to achieve the desired quality level while at the same time reduce the storage size. Image quality is negligibly affected if 10:1 compression is applied to the image. The higher the compression value, the higher the degradation in image quality. JPEG image file format was standardized by the Joint Photographic Experts Group and, hence, the name JPEG. The format has been the choice of storing and transmitting photographic images on the web. Almost all Operating systems now have viewers that support visualization of JPEG images, which are often stored with JPG extension as well. Even the web browsers support visualization of JPEG images.

          link: "https://docs.fileformat.com/image/jpeg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Editing Annotating From Other Popular File Formats"
    content: |
        Java annotations editor API for documents and image formats. Update annotation properties from some of the popular file formats as stated below.
    format: 
        # format loop
        - name: "Edit Annotation from PDF"
          link: "https://products.groupdocs.com/annotation/java/edit/pdf"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Edit Annotation from DOC"
          link: "https://products.groupdocs.com/annotation/java/edit/doc"
          description: "Microsoft Word Document"

        # format loop
        - name: "Edit Annotation from DOCM"
          link: "https://products.groupdocs.com/annotation/java/edit/docm"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Edit Annotation from DOCX"
          link: "https://products.groupdocs.com/annotation/java/edit/docx"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Edit Annotation from DOT"
          link: "https://products.groupdocs.com/annotation/java/edit/dot"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Edit Annotation from DOTX"
          link: "https://products.groupdocs.com/annotation/java/edit/dotx"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Edit Annotation from DOTM"
          link: "https://products.groupdocs.com/annotation/java/edit/dotm"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Edit Annotation from RTF"
          link: "https://products.groupdocs.com/annotation/java/edit/rtf"
          description: "Rich Text Document"

        # format loop
        - name: "Edit Annotation from ODT"
          link: "https://products.groupdocs.com/annotation/java/edit/odt"
          description: "Open Document Text"

        # format loop
        - name: "Edit Annotation from XLS"
          link: "https://products.groupdocs.com/annotation/java/edit/xls"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Edit Annotation from XLSX"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsx"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Edit Annotation from XLSM"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsm"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Edit Annotation from XLSB"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsb"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Edit Annotation from ODS"
          link: "https://products.groupdocs.com/annotation/java/edit/ods"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Edit Annotation from PPT"
          link: "https://products.groupdocs.com/annotation/java/edit/ppt"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Edit Annotation from PPTX"
          link: "https://products.groupdocs.com/annotation/java/edit/pptx"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Edit Annotation from PPSX"
          link: "https://products.groupdocs.com/annotation/java/edit/ppsx"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Edit Annotation from POTM"
          link: "https://products.groupdocs.com/annotation/java/edit/potm"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Edit Annotation from PPTM"
          link: "https://products.groupdocs.com/annotation/java/edit/pptm"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Edit Annotation from PPS"
          link: "https://products.groupdocs.com/annotation/java/edit/pps"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Edit Annotation from ODP"
          link: "https://products.groupdocs.com/annotation/java/edit/odp"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Edit Annotation from HTML"
          link: "https://products.groupdocs.com/annotation/java/edit/html"
          description: "HyperText Markup Language"

        # format loop
        - name: "Edit Annotation from TIFF"
          link: "https://products.groupdocs.com/annotation/java/edit/tiff"
          description: "Tagged Image File Format"

        # format loop
        - name: "Edit Annotation from JPEG"
          link: "https://products.groupdocs.com/annotation/java/edit/jpeg"
          description: "JPEG Image"

        # format loop
        - name: "Edit Annotation from PNG"
          link: "https://products.groupdocs.com/annotation/java/edit/png"
          description: "Portable Network Graphic"

        # format loop
        - name: "Edit Annotation from BMP"
          link: "https://products.groupdocs.com/annotation/java/edit/bmp"
          description: "Bitmap File Format"

        # format loop
        - name: "Edit Annotation from EML"
          link: "https://products.groupdocs.com/annotation/java/edit/eml"
          description: "E-mail Message"

        # format loop
        - name: "Edit Annotation from MSG"
          link: "https://products.groupdocs.com/annotation/java/edit/msg"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Edit Annotation from VSD"
          link: "https://products.groupdocs.com/annotation/java/edit/vsd"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Edit Annotation from VSDX"
          link: "https://products.groupdocs.com/annotation/java/edit/vsdx"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Edit Annotation from VSS"
          link: "https://products.groupdocs.com/annotation/java/edit/vss"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Edit Annotation from VST"
          link: "https://products.groupdocs.com/annotation/java/edit/vst"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Edit Annotation from DWG"
          link: "https://products.groupdocs.com/annotation/java/edit/dwg"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Edit Annotation from DXF"
          link: "https://products.groupdocs.com/annotation/java/edit/dxf"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Edit Annotation from DCM"
          link: "https://products.groupdocs.com/annotation/java/edit/dcm"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Edit Annotation from WMF"
          link: "https://products.groupdocs.com/annotation/java/edit/wmf"
          description: "Windows Metafile"

        # format loop
        - name: "Edit Annotation from EMF"
          link: "https://products.groupdocs.com/annotation/java/edit/emf"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---
