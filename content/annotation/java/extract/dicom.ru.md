
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/extract/dicom"/>

############################# Head ############################
head_title: "Извличение Аннотаций с DICOM в Java приложении"
head_description: "Java API для создания и Извличение популярных типов аннотаций с DICOM, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Извличение DICOM файла с Java"
description: ""
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
        img_alt: "GroupDocs.Annotation для Java"
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
    title: "О GroupDocs.Annotation для Java API"
    content: |
        GroupDocs.Annotation for Java API это библиотека которая позволяет добавлять аннотации к файлам PDF, Word и другим документам на Mac, Windows или Ubuntu. [GroupDocs.Annotation для [PLATFORM]](/ru/annotation/java/) это собственный Java API для управления аннотациями с комплексной поддержкой для создания, добавления, редактирования, удаления, извлечения и экспорта аннотаций из изображений и других документов, весь список поддерживаемых документов вы можете посмотреть на [странице](https://docs.groupdocs.com/annotation/java/supported-document-formats/).

        Эта библиотека позволяет работать не только с DICOM но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Java API позволяет создавать и [добавлять](/ru/annotation/java/add/dicom/) новые заметки, [редактировать](/ru/annotation/java/edit/dicom/) аннотации, извлекать комментарии, примечания и [удалять](/ru/annotation/java/remove/dicom/) их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с DICOM документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/java/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Извличение аннотаций с DICOM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/java/) позволяет разработчикам Java легко аннотировать документы и извлекать аннотационную информацию из файлов DICOM в любом приложении на основе Java, выполняя несколько простых шагов.
        
        * Создание объектов ответа с комментарием и датой.
        * Создайте экземпляр объекта LoadOptions и вызовите SetImportAnnotations с аргументом true.
        * Определите переменную с типом List.
        * Вызвать метод get и вернуть результат в переменную выше.
    
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среда разработки: NetBeans, Intellij IDEA, Eclipse и т. д.
        * Среда выполнения Java: Java 7 (1.7) и выше
        * Получите последнюю версию GroupDocs.Annotation для Java из [репозитория артефактов GroupDocs](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)
    

############################# Preview ############################
preview:
    enable: true
    
    code: |
        ```java
        // Для использования этого примера входной файл ("annotated.bmp") должен быть с аннотациями
        LoadOptions loadOptions = new LoadOptions();

        // Создание экземпляра класса Annotator и получиние аннотации
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для аннотирования документов и изображений"
    content: |
        Извлеките аннотацию из файла DICOM прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dicom"
          title: "О формате файла DICOM"
          content: |
            
          link: "https://docs.fileformat.com/image/dicom/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Извлечение аннотаций из файлов других поддерживаемых форматов"
    content: |
        Библиотека управления аннотациями Java для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Извличение Annotation с PDF"
          link: "https://products.groupdocs.com/annotation/java/extract/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Извличение Annotation с DOC"
          link: "https://products.groupdocs.com/annotation/java/extract/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Извличение Annotation с DOCM"
          link: "https://products.groupdocs.com/annotation/java/extract/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Извличение Annotation с DOCX"
          link: "https://products.groupdocs.com/annotation/java/extract/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Извличение Annotation с DOT"
          link: "https://products.groupdocs.com/annotation/java/extract/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Извличение Annotation с DOTX"
          link: "https://products.groupdocs.com/annotation/java/extract/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Извличение Annotation с RTF"
          link: "https://products.groupdocs.com/annotation/java/extract/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Извличение Annotation с ODT"
          link: "https://products.groupdocs.com/annotation/java/extract/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Извличение Annotation с XLS"
          link: "https://products.groupdocs.com/annotation/java/extract/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Извличение Annotation с XLSX"
          link: "https://products.groupdocs.com/annotation/java/extract/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Извличение Annotation с XLSM"
          link: "https://products.groupdocs.com/annotation/java/extract/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Извличение Annotation с XLSB"
          link: "https://products.groupdocs.com/annotation/java/extract/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Извличение Annotation с ODS"
          link: "https://products.groupdocs.com/annotation/java/extract/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Извличение Annotation с PPT"
          link: "https://products.groupdocs.com/annotation/java/extract/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Извличение Annotation с PPTX"
          link: "https://products.groupdocs.com/annotation/java/extract/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Извличение Annotation с PPSX"
          link: "https://products.groupdocs.com/annotation/java/extract/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Извличение Annotation с POTM"
          link: "https://products.groupdocs.com/annotation/java/extract/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Извличение Annotation с PPTM"
          link: "https://products.groupdocs.com/annotation/java/extract/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Извличение Annotation с PPS"
          link: "https://products.groupdocs.com/annotation/java/extract/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Извличение Annotation с ODP"
          link: "https://products.groupdocs.com/annotation/java/extract/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Извличение Annotation с HTML"
          link: "https://products.groupdocs.com/annotation/java/extract/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Извличение Annotation с TIFF"
          link: "https://products.groupdocs.com/annotation/java/extract/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Извличение Annotation с JPEG"
          link: "https://products.groupdocs.com/annotation/java/extract/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Извличение Annotation с PNG"
          link: "https://products.groupdocs.com/annotation/java/extract/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Извличение Annotation с EML"
          link: "https://products.groupdocs.com/annotation/java/extract/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Извличение Annotation с MSG"
          link: "https://products.groupdocs.com/annotation/java/extract/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Извличение Annotation с VSD"
          link: "https://products.groupdocs.com/annotation/java/extract/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Извличение Annotation с VSDX"
          link: "https://products.groupdocs.com/annotation/java/extract/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Извличение Annotation с VSS"
          link: "https://products.groupdocs.com/annotation/java/extract/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Извличение Annotation с VST"
          link: "https://products.groupdocs.com/annotation/java/extract/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Извличение Annotation с DWG"
          link: "https://products.groupdocs.com/annotation/java/extract/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Извличение Annotation с DXF"
          link: "https://products.groupdocs.com/annotation/java/extract/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Извличение Annotation с DCM"
          link: "https://products.groupdocs.com/annotation/java/extract/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Извличение Annotation с WMF"
          link: "https://products.groupdocs.com/annotation/java/extract/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Извличение Annotation с EMF"
          link: "https://products.groupdocs.com/annotation/java/extract/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---