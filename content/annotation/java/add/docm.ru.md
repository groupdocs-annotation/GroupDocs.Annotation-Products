
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/add/docm"/>

############################# Head ############################
head_title: "Добавление Аннотаций в DOCM в Java приложении"
head_description: "Java API для создания и Добавление популярных типов аннотаций в DOCM, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Добавление DOCM файла в Java"
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

        GroupDocs.Annotation for Java API позволяет создавать и добавлять новые заметки, [редактировать](/ru/annotation/java/edit/docm/) аннотации, [извлекать](/ru/annotation/java/extract/docm/) комментарии, примечания и [удалять](/ru/annotation/java/remove/docm/) их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с DOCM документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/java/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Добавление аннотаций в DOCM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/java/) позволяет разработчикам Java легко добавлять различные типы аннотаций к файлам DOCM в любом приложении на основе Java, выполняя несколько простых шагов.
        
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
    title: "Предварительный просмотр аннотации и пример кода"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Создаем экземпляр класса Reply и добавляем комментарии
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Создаем экземпляр класса AreaAnnotation и устанавливаем параметры
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
        
        // Создаем экземпляр класса Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Добавляем аннотацию
        annotator.add(area);
        
        // Сохраняем в файл
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для добавления аннотаций к документам и изображениям"
    content: |
        Создавайте и добавляйте аннотации к файлу DOCM прямо сейчас, посетив веб-сайт [живые демо](https://products.groupdocs.app/annotation/family).
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
    title: "Аннотирование других популярных форматов файлов"
    content: |
        Библиотека управления аннотациями Java для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Добавление Annotation в PDF"
          link: "https://products.groupdocs.com/annotation/java/add/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Добавление Annotation в DOC"
          link: "https://products.groupdocs.com/annotation/java/add/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Добавление Annotation в DOCM"
          link: "https://products.groupdocs.com/annotation/java/add/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Добавление Annotation в DOCX"
          link: "https://products.groupdocs.com/annotation/java/add/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Добавление Annotation в DOT"
          link: "https://products.groupdocs.com/annotation/java/add/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Добавление Annotation в DOTX"
          link: "https://products.groupdocs.com/annotation/java/add/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Добавление Annotation в RTF"
          link: "https://products.groupdocs.com/annotation/java/add/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Добавление Annotation в ODT"
          link: "https://products.groupdocs.com/annotation/java/add/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Добавление Annotation в XLS"
          link: "https://products.groupdocs.com/annotation/java/add/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Добавление Annotation в XLSX"
          link: "https://products.groupdocs.com/annotation/java/add/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Добавление Annotation в XLSM"
          link: "https://products.groupdocs.com/annotation/java/add/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Добавление Annotation в XLSB"
          link: "https://products.groupdocs.com/annotation/java/add/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Добавление Annotation в ODS"
          link: "https://products.groupdocs.com/annotation/java/add/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Добавление Annotation в PPT"
          link: "https://products.groupdocs.com/annotation/java/add/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Добавление Annotation в PPTX"
          link: "https://products.groupdocs.com/annotation/java/add/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Добавление Annotation в PPSX"
          link: "https://products.groupdocs.com/annotation/java/add/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Добавление Annotation в POTM"
          link: "https://products.groupdocs.com/annotation/java/add/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Добавление Annotation в PPTM"
          link: "https://products.groupdocs.com/annotation/java/add/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Добавление Annotation в PPS"
          link: "https://products.groupdocs.com/annotation/java/add/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Добавление Annotation в ODP"
          link: "https://products.groupdocs.com/annotation/java/add/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Добавление Annotation в HTML"
          link: "https://products.groupdocs.com/annotation/java/add/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Добавление Annotation в TIFF"
          link: "https://products.groupdocs.com/annotation/java/add/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Добавление Annotation в JPEG"
          link: "https://products.groupdocs.com/annotation/java/add/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Добавление Annotation в PNG"
          link: "https://products.groupdocs.com/annotation/java/add/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Добавление Annotation в EML"
          link: "https://products.groupdocs.com/annotation/java/add/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Добавление Annotation в MSG"
          link: "https://products.groupdocs.com/annotation/java/add/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Добавление Annotation в VSD"
          link: "https://products.groupdocs.com/annotation/java/add/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Добавление Annotation в VSDX"
          link: "https://products.groupdocs.com/annotation/java/add/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Добавление Annotation в VSS"
          link: "https://products.groupdocs.com/annotation/java/add/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Добавление Annotation в VST"
          link: "https://products.groupdocs.com/annotation/java/add/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Добавление Annotation в DWG"
          link: "https://products.groupdocs.com/annotation/java/add/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Добавление Annotation в DXF"
          link: "https://products.groupdocs.com/annotation/java/add/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Добавление Annotation в DCM"
          link: "https://products.groupdocs.com/annotation/java/add/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Добавление Annotation в WMF"
          link: "https://products.groupdocs.com/annotation/java/add/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Добавление Annotation в EMF"
          link: "https://products.groupdocs.com/annotation/java/add/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---