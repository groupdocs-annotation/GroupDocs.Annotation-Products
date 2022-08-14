
---
############################# Static ############################
layout: "auto-gen"
date: 2022-07-05T12:44:18+03:00
draft: false

############################# Head ############################
head_title: "Удаление Аннотаций с DOTM в Net приложении"
head_description: "Net API для создания и Удаление популярных типов аннотаций с DOTM, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Удаление DOTM файла с Net"
description: "Добавляйте аннотации с документы DOTM, Microsoft Office, изображениям, HTML, рисункам и другим форматам файлов в любых типах приложений Net."
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
        img_alt: "GroupDocs.Annotation для Net"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

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
    title: "О GroupDocs.Annotation для Net API"
    content: |
        GroupDocs.Annotation for Net API это библиотека которая позволяет добавлять аннотации к файлам PDF, Word и другим документам на Mac, Windows или Ubuntu. [GroupDocs.Annotation для [PLATFORM]](/ru/annotation/net/) это собственный Net API для управления аннотациями с комплексной поддержкой для создания, добавления, редактирования, удаления, извлечения и экспорта аннотаций из изображений и других документов, весь список поддерживаемых документов вы можете посмотреть на [странице](https://docs.groupdocs.com/annotation/net/supported-document-formats/).

        Эта библиотека позволяет работать не только с DOTM но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Net API позволяет создавать и [добавлять](/ru/annotation/net/add/dotm/) новые заметки, [редактировать](/ru/annotation/net/edit/dotm/) аннотации, [извлекать](/ru/annotation/net/extract/dotm/) комментарии, примечания и удалять их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с DOTM документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/net/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Удаление аннотаций с DOTM in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/net упрощает разработчикам Net удаление деталей аннотаций из файлов DOTM в любом приложении на основе Net за счет выполнения нескольких простых шагов.
        
        * Создание объектов ответа с комментарием и датой.
        * Создайте экземпляр объекта SaveOptions и установите AnnotationTypes = AnnotationType.None.
        * Вызовите метод сохранения с результирующим путем или потоком документа и объектом SaveOptions.
    
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для Net поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Annotation для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.annotation).
    
    code: |
        ```cs
        // 1- Как удалить аннотацию из документа, используя индекс аннотации
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        // 2- Как удалить аннотацию из документа с помощью объекта аннотации
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        // 3- Как удалить некоторые аннотации из документа, используя список идентификаторов
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        // 4- Как удалить некоторые аннотации из документа, используя список аннотаций
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для удаления аннотаций из документов и изображений"
    content: |
        Просмотрите и удалите аннотации из файла DOTM прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dotm"
          title: "О формате файла DOTM"
          content: |
            
          link: "https://docs.fileformat.com/image/dotm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Удвление аннотаций из файлов других популярных форматов"
    content: |
        Библиотека управления аннотациями Net для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Удаление Annotation с PDF"
          link: "https://products.groupdocs.com/annotation/net/remove/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Удаление Annotation с DOC"
          link: "https://products.groupdocs.com/annotation/net/remove/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Удаление Annotation с DOCM"
          link: "https://products.groupdocs.com/annotation/net/remove/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Удаление Annotation с DOCX"
          link: "https://products.groupdocs.com/annotation/net/remove/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Удаление Annotation с DOT"
          link: "https://products.groupdocs.com/annotation/net/remove/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Удаление Annotation с DOTX"
          link: "https://products.groupdocs.com/annotation/net/remove/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Удаление Annotation с DOTM"
          link: "https://products.groupdocs.com/annotation/net/remove/dotm/"
          description: "Microsoft Word Macro-Enabled Template"

        # format loop
        - name: "Удаление Annotation с RTF"
          link: "https://products.groupdocs.com/annotation/net/remove/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Удаление Annotation с ODT"
          link: "https://products.groupdocs.com/annotation/net/remove/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Удаление Annotation с XLS"
          link: "https://products.groupdocs.com/annotation/net/remove/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Удаление Annotation с XLSX"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Удаление Annotation с XLSM"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Удаление Annotation с XLSB"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Удаление Annotation с ODS"
          link: "https://products.groupdocs.com/annotation/net/remove/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Удаление Annotation с PPT"
          link: "https://products.groupdocs.com/annotation/net/remove/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Удаление Annotation с PPTX"
          link: "https://products.groupdocs.com/annotation/net/remove/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Удаление Annotation с PPSX"
          link: "https://products.groupdocs.com/annotation/net/remove/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Удаление Annotation с POTM"
          link: "https://products.groupdocs.com/annotation/net/remove/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Удаление Annotation с PPTM"
          link: "https://products.groupdocs.com/annotation/net/remove/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Удаление Annotation с PPS"
          link: "https://products.groupdocs.com/annotation/net/remove/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Удаление Annotation с ODP"
          link: "https://products.groupdocs.com/annotation/net/remove/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Удаление Annotation с HTML"
          link: "https://products.groupdocs.com/annotation/net/remove/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Удаление Annotation с TIFF"
          link: "https://products.groupdocs.com/annotation/net/remove/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Удаление Annotation с JPEG"
          link: "https://products.groupdocs.com/annotation/net/remove/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Удаление Annotation с PNG"
          link: "https://products.groupdocs.com/annotation/net/remove/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Удаление Annotation с EML"
          link: "https://products.groupdocs.com/annotation/net/remove/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Удаление Annotation с MSG"
          link: "https://products.groupdocs.com/annotation/net/remove/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Удаление Annotation с VSD"
          link: "https://products.groupdocs.com/annotation/net/remove/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Удаление Annotation с VSDX"
          link: "https://products.groupdocs.com/annotation/net/remove/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Удаление Annotation с VSS"
          link: "https://products.groupdocs.com/annotation/net/remove/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Удаление Annotation с VST"
          link: "https://products.groupdocs.com/annotation/net/remove/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Удаление Annotation с DWG"
          link: "https://products.groupdocs.com/annotation/net/remove/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Удаление Annotation с DXF"
          link: "https://products.groupdocs.com/annotation/net/remove/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Удаление Annotation с DCM"
          link: "https://products.groupdocs.com/annotation/net/remove/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Удаление Annotation с WMF"
          link: "https://products.groupdocs.com/annotation/net/remove/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Удаление Annotation с EMF"
          link: "https://products.groupdocs.com/annotation/net/remove/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---