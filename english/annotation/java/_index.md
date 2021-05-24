---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Document Annotation API | View & Annotate PDF Word Excel PPTX Images"
head_description: "Java Document Annotation API. View, tag, comment & annotate PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAD, EMF WMF & image file formats."

############################# Header ############################
title: "Document Annotation via Java API"
description: "‎Build Java Applications with capabilities to View & Annotate PDF, HTML, MS Office and other document formats without installing any external software.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation for Java API provides easy to use document, annotation management, and manipulation functionality to be used in your Java-based business applications. Our Java annotator library allows you to work with many types of annotations, which include text, polyline, area, underline, point, watermark, arrow, ellipse, text replacement, distance, text field, resource redaction etc. It also offers a comprehensive set of data objects to customize annotation properties as per your requirements within all supported document formats including: PDF, HTML, Microsoft Office Word, Excel spreadsheets, PowerPoint presentations, Visio, Outlook emails, images, metafiles, CAD drawing and various other formats.  
        
      The API provides the ability to get thumbnails of document pages and supports importing and exporting annotation to and from PDF files.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Annotation for Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Overview"
          content: |
            * Add Annotations
            * Export Annotations
            * Import Annotations
            * User Management
            * Reply Based Comments
            * Annotation Compatibility
            * Abstract Storage
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation for Java supports all popular [document file formats](https://docs.groupdocs.com/annotation/java/supported-document-formats/) including: Microsoft Office, PDF, images and many others.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **Excel**: XLS, XLSX, XLSB, XLSM
                * **PowerPoint**: PPT, PPTX, PPTM, POTX, POTM, PPS, PPSX, PPSM
                * **Outlook**: EML, EMLX
                * **Visio**: VSS, VST, VSD, VSDX

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **Portable**: PDF (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: ODT, ODS, ODP
                * **Images**: BMP, JPG, TIFF, TIF, PNG
                * **AutoCAD**: DWG, DXF
                * **Other**: HTML, DCM

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Java supports following Operating Systems, Frameworks & Package Managers:
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Annotation for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Add Area Annotation in Document and Link Simple & Nested Comments"

      # feature loop
      - icon: "fas fa-eye"
        content: "Point to a Particular Content using Arrow Annotation"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Set Text Watermarks to PDF, Slides, Excel Worksheets, Images & Diagrams at Angled Position"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Add Popup Comments to any Place in the Document using Point Annotation"

      # feature loop
      - icon: "fas fa-code"
        content: "Use Polyline Annotation to Connect Sequence of Line Segments, Arc Segments or both"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Add Ellipse Annotation to PDF, Word Documents, Spreadsheets, Presentations, Diagrams & Images"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Add Angled Watermarks for PDF, PowerPoint, Excel, Images & Diagrams"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Fetch Coordinates of Text Annotation in Image Representation of a Document‎"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Underline, Strikethrough or Modify Specific Text in a Document"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Add Text Stamp or Watermark & Text Field in a Document"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Import & Export Annotations among Word Documents & PowerPoint Presentations"

      # feature loop
      - icon: "fas fa-columns"
        content: "Annotate Excel Spreadsheets with Text, TextReplacement, Watermark & Resource Redaction Annotation types"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Add Polyline, Strikethrough, Underline or Text Annotations to PowerPoint Presentations and Slides"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Mark Point Annotation in Presentations using X, Y Coordinates"

      # feature loop
      - icon: "fas fa-print"
        content: "Add Strikethrough, Text, Underline or Polyline Annotations to Images"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Fetch Document Information & Images for Visio Diagrams, such as VSS & VSD"

      # feature loop
      - icon: "fas fa-lock"
        content: "Perform Annotation Management (Add, Modify & Delete Annotations) Tasks using Data Storage"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Get Thumbnails of the Document Pages & Work with Multi-page TIFF files"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Assign Access Rights to Users for Allowed Annotation Actions"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Fetch all Annotation of a Document with a Single Function Call"

      # feature loop
      - icon: "fas fa-heading"
        content: "Add Link Annotations to PDF, Word & PowerPoint Presentations"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "SVG Path Parsing support for PDF, Word, Diagrams, Slides and other major document formats"

      # feature loop
      - icon: "fas fa-cube"
        content: "Support for adding Watermark Annotation to Word documents and cleanup for Text Replacement"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Shape Processing support in Diagrams for Text Annotations"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Save Time by Caching Page Previews of Documents for Faster Processing"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Easily Annotate Word, Excel and PowerPoint Documents even with Older Formats"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Display Distance Annotation Captions for Excel, PowerPoint and Diagrams"

    more_feature:
      # more_feature_loop
      - title: "Configurable Data Object Properties"
        content: |
          GroupDocs.Annotation for Java API consists of an extensive collection of data objects with configurable properties, used in data storage. These properties include, Annotation (coordinates, dimensions, type, color, frame style, background color etc.), Annotation Collaborator (ID, document, access rights etc.), Annotation Reply (reply, parent annotation, GUID, message, time etc.), Document (GUID, name, owner, type, access rights etc.), User (ID, nick, email, password, photo etc.).

      # more_feature_loop
      - title: "User Rights Access Management"
        content: "GroupDocs.Annotation for Java API empowers you to easily manage user rights for accessing annotations. You can assign or revoke user access rights by configuring properties, such as View, Annotate, Download, Export, Delete etc."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net"

############################# Back to top ###############################
back_to_top:
  enable: true
---