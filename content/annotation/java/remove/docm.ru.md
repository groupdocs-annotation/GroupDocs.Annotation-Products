
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/remove/docm"/>

############################# Head ############################
head_title: "Удаление Аннотаций с DOCM в Java приложении"
head_description: "Java API для создания и Удаление популярных типов аннотаций с DOCM, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Удаление DOCM файла с Java"
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

        Эта библиотека позволяет работать не только с DOCM но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Java API позволяет создавать и [добавлять](/ru/annotation/java/add/docm/) новые заметки, [редактировать](/ru/annotation/java/edit/docm/) аннотации, [извлекать](/ru/annotation/java/extract/docm/) комментарии, примечания и удалять их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с DOCM документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/java/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Удаление аннотаций с DOCM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/java упрощает разработчикам Java удаление деталей аннотаций из файлов DOCM в любом приложении на основе Java за счет выполнения нескольких простых шагов.
        
        * Создание объектов ответа с комментарием и датой.
        * Создайте экземпляр объекта SaveOptions и установите AnnotationTypes = AnnotationType.None.
        * Вызовите метод сохранения с результирующим путем или потоком документа и объектом SaveOptions.
    
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
        // Создание экземпляра класса Annotator
        Annotator annotator = new Annotator("C://input.bmp");
        
        // Удаление аннотации по заданному типу None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);
        
        // Сохранение аннотации в выходном файле
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для удаления аннотаций из документов и изображений"
    content: |
        Просмотрите и удалите аннотации из файла DOCM прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docm"
          title: "О формате файла DOCM"
          content: |
            Файлы DOCM представляют собой документы, сгенерированные Microsoft Word 2007 или более поздней версии, с возможностью запуска макросов. Он похож на формат файла DOCX, но возможность запускать макросы отличает его от DOCX. Как и DOCX, файлы DOCM могут хранить текст, изображения, таблицы, формы, диаграммы и другое содержимое. Возможность запуска макросов позволяет легко сэкономить время, выполняя серию команд в виде записанных действий для автоматического завершения задачи. . Файлы DOCM можно открывать и редактировать в Microsoft Word 2007 и более поздних версиях.
          link: "https://docs.fileformat.com/image/docm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Удвление аннотаций из файлов других популярных форматов"
    content: |
        Библиотека управления аннотациями Java для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Удаление Annotation с PDF"
          link: "https://products.groupdocs.com/annotation/java/remove/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Удаление Annotation с DOC"
          link: "https://products.groupdocs.com/annotation/java/remove/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Удаление Annotation с DOCM"
          link: "https://products.groupdocs.com/annotation/java/remove/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Удаление Annotation с DOCX"
          link: "https://products.groupdocs.com/annotation/java/remove/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Удаление Annotation с DOT"
          link: "https://products.groupdocs.com/annotation/java/remove/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Удаление Annotation с DOTX"
          link: "https://products.groupdocs.com/annotation/java/remove/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Удаление Annotation с RTF"
          link: "https://products.groupdocs.com/annotation/java/remove/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Удаление Annotation с ODT"
          link: "https://products.groupdocs.com/annotation/java/remove/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Удаление Annotation с XLS"
          link: "https://products.groupdocs.com/annotation/java/remove/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Удаление Annotation с XLSX"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Удаление Annotation с XLSM"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Удаление Annotation с XLSB"
          link: "https://products.groupdocs.com/annotation/java/remove/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Удаление Annotation с ODS"
          link: "https://products.groupdocs.com/annotation/java/remove/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Удаление Annotation с PPT"
          link: "https://products.groupdocs.com/annotation/java/remove/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Удаление Annotation с PPTX"
          link: "https://products.groupdocs.com/annotation/java/remove/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Удаление Annotation с PPSX"
          link: "https://products.groupdocs.com/annotation/java/remove/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Удаление Annotation с POTM"
          link: "https://products.groupdocs.com/annotation/java/remove/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Удаление Annotation с PPTM"
          link: "https://products.groupdocs.com/annotation/java/remove/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Удаление Annotation с PPS"
          link: "https://products.groupdocs.com/annotation/java/remove/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Удаление Annotation с ODP"
          link: "https://products.groupdocs.com/annotation/java/remove/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Удаление Annotation с HTML"
          link: "https://products.groupdocs.com/annotation/java/remove/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Удаление Annotation с TIFF"
          link: "https://products.groupdocs.com/annotation/java/remove/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Удаление Annotation с JPEG"
          link: "https://products.groupdocs.com/annotation/java/remove/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Удаление Annotation с PNG"
          link: "https://products.groupdocs.com/annotation/java/remove/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Удаление Annotation с EML"
          link: "https://products.groupdocs.com/annotation/java/remove/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Удаление Annotation с MSG"
          link: "https://products.groupdocs.com/annotation/java/remove/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Удаление Annotation с VSD"
          link: "https://products.groupdocs.com/annotation/java/remove/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Удаление Annotation с VSDX"
          link: "https://products.groupdocs.com/annotation/java/remove/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Удаление Annotation с VSS"
          link: "https://products.groupdocs.com/annotation/java/remove/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Удаление Annotation с VST"
          link: "https://products.groupdocs.com/annotation/java/remove/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Удаление Annotation с DWG"
          link: "https://products.groupdocs.com/annotation/java/remove/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Удаление Annotation с DXF"
          link: "https://products.groupdocs.com/annotation/java/remove/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Удаление Annotation с DCM"
          link: "https://products.groupdocs.com/annotation/java/remove/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Удаление Annotation с WMF"
          link: "https://products.groupdocs.com/annotation/java/remove/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Удаление Annotation с EMF"
          link: "https://products.groupdocs.com/annotation/java/remove/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---