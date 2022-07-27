
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/edit/vst"/>

############################# Head ############################
head_title: "Редактирование Аннотаций в VST в Java приложении"
head_description: "Java API для создания и Редактирование популярных типов аннотаций в VST, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Редактирование VST файла в Java"
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

        Эта библиотека позволяет работать не только с VST но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Java API позволяет создавать и [добавлять](/ru/annotation/java/add/vst/) новые заметки, редактировать аннотации, [извлекать](/ru/annotation/java/extract/vst/) комментарии, примечания и [удалять](/ru/annotation/java/remove/vst/) их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с VST документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/java/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Редактирование аннотаций в VST in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/java/) упрощает разработчикам Java обновление различных свойств аннотаций из файлов VST в любом приложении на основе Java за счет выполнения нескольких простых шагов.
        
        * Создание экземпляра объекта Annotator с входным путем к документу или потоком с экземпляром LoadOptions с ImportAnnotations = true.
        * Создайте некоторую реализацию AnnotationBase и установите идентификатор существующей аннотации (если аннотация с этим идентификатором не найдена, ничего не изменится) или список путей аннотаций (все существующие аннотации будут удалены).
        * Вызвать метод обновления объекта Annotator с переданными аннотациями.
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
        String outputPath = "UpdateAnnotation.bmp";
        
        // Создание экземпляра класса Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Создание экземпляра класса Reply для первого примера и добавляем комментарии
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Создание экземпляра класса AreaAnnotation и устанавка параметров
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Добавление исходной аннотации
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        LoadOptions loadOptions = new LoadOptions();
        
        // Открытие аннотированного документа
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Создание экземпляра класса Reply для обновления первого примера
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);
        
        // Изменяем некоторые свойства существующей аннотации
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Обновляем аннотацию
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для изменения аннотаций из документов и изображений"
    content: |
        Читайте и редактируйте аннотации из файла VST прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vst"
          title: "О формате файла VST"
          content: |
            Файлы с расширением VST представляют собой файлы векторных изображений, созданные с помощью Microsoft Visio, и служат шаблоном для создания дополнительных файлов. Эти файлы шаблонов имеют двоичный формат и содержат макет и параметры по умолчанию, которые используются для создания новых рисунков Visio. Когда файл VST открывается в Microsoft Visio, он содержит существующие настройки для продолжения работы с документом. Как правило, файлы Visio используются для создания рисунков, содержащих визуальные объекты, блок-схемы, диаграмму UML, информационный поток, организационные диаграммы, диаграммы программного обеспечения, схему сети, модели баз данных, сопоставление объектов и другую подобную информацию. Файлы, созданные с помощью Visio, также можно экспортировать в различные форматы файлов, такие как PNG, BMP, PDF и другие.
          link: "https://docs.fileformat.com/image/vst/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Редактирование аннотаций из файлов других популярных форматов"
    content: |
        Библиотека управления аннотациями Java для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Редактирование Annotation в PDF"
          link: "https://products.groupdocs.com/annotation/java/edit/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Редактирование Annotation в DOC"
          link: "https://products.groupdocs.com/annotation/java/edit/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Редактирование Annotation в DOCM"
          link: "https://products.groupdocs.com/annotation/java/edit/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Редактирование Annotation в DOCX"
          link: "https://products.groupdocs.com/annotation/java/edit/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Редактирование Annotation в DOT"
          link: "https://products.groupdocs.com/annotation/java/edit/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Редактирование Annotation в DOTX"
          link: "https://products.groupdocs.com/annotation/java/edit/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Редактирование Annotation в RTF"
          link: "https://products.groupdocs.com/annotation/java/edit/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Редактирование Annotation в ODT"
          link: "https://products.groupdocs.com/annotation/java/edit/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Редактирование Annotation в XLS"
          link: "https://products.groupdocs.com/annotation/java/edit/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Редактирование Annotation в XLSX"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Редактирование Annotation в XLSM"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Редактирование Annotation в XLSB"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Редактирование Annotation в ODS"
          link: "https://products.groupdocs.com/annotation/java/edit/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Редактирование Annotation в PPT"
          link: "https://products.groupdocs.com/annotation/java/edit/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Редактирование Annotation в PPTX"
          link: "https://products.groupdocs.com/annotation/java/edit/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Редактирование Annotation в PPSX"
          link: "https://products.groupdocs.com/annotation/java/edit/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Редактирование Annotation в POTM"
          link: "https://products.groupdocs.com/annotation/java/edit/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Редактирование Annotation в PPTM"
          link: "https://products.groupdocs.com/annotation/java/edit/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Редактирование Annotation в PPS"
          link: "https://products.groupdocs.com/annotation/java/edit/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Редактирование Annotation в ODP"
          link: "https://products.groupdocs.com/annotation/java/edit/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Редактирование Annotation в HTML"
          link: "https://products.groupdocs.com/annotation/java/edit/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Редактирование Annotation в TIFF"
          link: "https://products.groupdocs.com/annotation/java/edit/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Редактирование Annotation в JPEG"
          link: "https://products.groupdocs.com/annotation/java/edit/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Редактирование Annotation в PNG"
          link: "https://products.groupdocs.com/annotation/java/edit/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Редактирование Annotation в EML"
          link: "https://products.groupdocs.com/annotation/java/edit/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Редактирование Annotation в MSG"
          link: "https://products.groupdocs.com/annotation/java/edit/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Редактирование Annotation в VSD"
          link: "https://products.groupdocs.com/annotation/java/edit/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Редактирование Annotation в VSDX"
          link: "https://products.groupdocs.com/annotation/java/edit/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Редактирование Annotation в VSS"
          link: "https://products.groupdocs.com/annotation/java/edit/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Редактирование Annotation в VST"
          link: "https://products.groupdocs.com/annotation/java/edit/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Редактирование Annotation в DWG"
          link: "https://products.groupdocs.com/annotation/java/edit/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Редактирование Annotation в DXF"
          link: "https://products.groupdocs.com/annotation/java/edit/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Редактирование Annotation в DCM"
          link: "https://products.groupdocs.com/annotation/java/edit/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Редактирование Annotation в WMF"
          link: "https://products.groupdocs.com/annotation/java/edit/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Редактирование Annotation в EMF"
          link: "https://products.groupdocs.com/annotation/java/edit/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---