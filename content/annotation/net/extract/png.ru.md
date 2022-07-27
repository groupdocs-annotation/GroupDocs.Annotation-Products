
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/extract/png"/>

############################# Head ############################
head_title: "Извличение Аннотаций с PNG в Net приложении"
head_description: "Net API для создания и Извличение популярных типов аннотаций с PNG, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Извличение PNG файла с Net"
description: ""
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

        Эта библиотека позволяет работать не только с PNG но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Net API позволяет создавать и [добавлять](/ru/annotation/net/add/png/) новые заметки, [редактировать](/ru/annotation/net/edit/png/) аннотации, извлекать комментарии, примечания и [удалять](/ru/annotation/net/remove/png/) их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с PNG документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/net/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Извличение аннотаций с PNG in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/net/) позволяет разработчикам Net легко аннотировать документы и извлекать аннотационную информацию из файлов PNG в любом приложении на основе Net, выполняя несколько простых шагов.
        
        * Создание объектов ответа с комментарием и датой.
        * Создайте экземпляр объекта LoadOptions и вызовите SetImportAnnotations с аргументом true.
        * Определите переменную с типом List.
        * Вызвать метод get и вернуть результат в переменную выше.
    
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для Net поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Annotation для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.annotation).
    

############################# Preview ############################
preview:
    enable: true
    
    code: |
        ```cs
        // Для использования этого примера входной файл ("annotated.bmp") должен быть с аннотациями
        using (Annotator annotator = new Annotator("annotated.bmp"))
        {
            List annotations = annotator.Get();
            XmlSerializer formatter = new XmlSerializer(typeof(List));
            using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
                fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для аннотирования документов и изображений"
    content: |
        Извлеките аннотацию из файла PNG прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-png"
          title: "О формате файла PNG"
          content: |
            PNG, переносимая сетевая графика, относится к типу формата файла растрового изображения, в котором используется сжатие без потерь. Этот формат файла был создан в качестве замены формата обмена графикой (GIF) и не имеет ограничений авторского права. Однако формат файла PNG не поддерживает анимацию. Формат файлов PNG поддерживает сжатие изображений без потерь, что делает его популярным среди пользователей. С течением времени PNG превратился в один из наиболее часто используемых форматов файлов изображений. Почти все операционные системы поддерживают открытие файлов PNG. Например, средство просмотра Microsoft Windows имеет возможность открывать файлы PNG, поскольку ОС по умолчанию поддерживает эту поддержку, доступную как часть установки.
          link: "https://docs.fileformat.com/image/png/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Извлечение аннотаций из файлов других поддерживаемых форматов"
    content: |
        Библиотека управления аннотациями Net для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Извличение Annotation с PDF"
          link: "https://products.groupdocs.com/annotation/net/extract/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Извличение Annotation с DOC"
          link: "https://products.groupdocs.com/annotation/net/extract/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Извличение Annotation с DOCM"
          link: "https://products.groupdocs.com/annotation/net/extract/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Извличение Annotation с DOCX"
          link: "https://products.groupdocs.com/annotation/net/extract/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Извличение Annotation с DOT"
          link: "https://products.groupdocs.com/annotation/net/extract/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Извличение Annotation с DOTX"
          link: "https://products.groupdocs.com/annotation/net/extract/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Извличение Annotation с RTF"
          link: "https://products.groupdocs.com/annotation/net/extract/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Извличение Annotation с ODT"
          link: "https://products.groupdocs.com/annotation/net/extract/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Извличение Annotation с XLS"
          link: "https://products.groupdocs.com/annotation/net/extract/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Извличение Annotation с XLSX"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Извличение Annotation с XLSM"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Извличение Annotation с XLSB"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Извличение Annotation с ODS"
          link: "https://products.groupdocs.com/annotation/net/extract/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Извличение Annotation с PPT"
          link: "https://products.groupdocs.com/annotation/net/extract/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Извличение Annotation с PPTX"
          link: "https://products.groupdocs.com/annotation/net/extract/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Извличение Annotation с PPSX"
          link: "https://products.groupdocs.com/annotation/net/extract/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Извличение Annotation с POTM"
          link: "https://products.groupdocs.com/annotation/net/extract/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Извличение Annotation с PPTM"
          link: "https://products.groupdocs.com/annotation/net/extract/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Извличение Annotation с PPS"
          link: "https://products.groupdocs.com/annotation/net/extract/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Извличение Annotation с ODP"
          link: "https://products.groupdocs.com/annotation/net/extract/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Извличение Annotation с HTML"
          link: "https://products.groupdocs.com/annotation/net/extract/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Извличение Annotation с TIFF"
          link: "https://products.groupdocs.com/annotation/net/extract/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Извличение Annotation с JPEG"
          link: "https://products.groupdocs.com/annotation/net/extract/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Извличение Annotation с PNG"
          link: "https://products.groupdocs.com/annotation/net/extract/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Извличение Annotation с EML"
          link: "https://products.groupdocs.com/annotation/net/extract/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Извличение Annotation с MSG"
          link: "https://products.groupdocs.com/annotation/net/extract/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Извличение Annotation с VSD"
          link: "https://products.groupdocs.com/annotation/net/extract/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Извличение Annotation с VSDX"
          link: "https://products.groupdocs.com/annotation/net/extract/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Извличение Annotation с VSS"
          link: "https://products.groupdocs.com/annotation/net/extract/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Извличение Annotation с VST"
          link: "https://products.groupdocs.com/annotation/net/extract/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Извличение Annotation с DWG"
          link: "https://products.groupdocs.com/annotation/net/extract/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Извличение Annotation с DXF"
          link: "https://products.groupdocs.com/annotation/net/extract/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Извличение Annotation с DCM"
          link: "https://products.groupdocs.com/annotation/net/extract/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Извличение Annotation с WMF"
          link: "https://products.groupdocs.com/annotation/net/extract/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Извличение Annotation с EMF"
          link: "https://products.groupdocs.com/annotation/net/extract/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---