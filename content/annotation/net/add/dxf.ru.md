
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/add/dxf"/>

############################# Head ############################
head_title: "Добавление Аннотаций в DXF в Net приложении"
head_description: "Net API для создания и Добавление популярных типов аннотаций в DXF, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Добавление DXF файла в Net"
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

        Эта библиотека позволяет работать не только с DXF но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Net API позволяет создавать и добавлять новые заметки, [редактировать](/ru/annotation/net/edit/dxf/) аннотации, [извлекать](/ru/annotation/net/extract/dxf/) комментарии, примечания и [удалять](/ru/annotation/net/remove/dxf/) их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с DXF документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/net/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Добавление аннотаций в DXF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/net/) позволяет разработчикам Net легко добавлять различные типы аннотаций к файлам DXF в любом приложении на основе Net, выполняя несколько простых шагов.
        
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
    

############################# Preview ############################
preview:
    enable: true
    title: "Предварительный просмотр аннотации и пример кода"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        // Добавляем аннотацию текстового поля к документу с локального диска
        using (Annotator annotator = new Annotator("input.bmp"))
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "This is text field annotation",
                Opacity = 0.7,
                PageNumber = 0,
                PenStyle = PenStyle.Dot,
                PenWidth = 3,
                FontFamily = "Arial",
                TextHorizontalAlignment = HorizontalAlignment.Center,
                Replies = new List
                {
                    new Reply
                    {
                        Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для добавления аннотаций к документам и изображениям"
    content: |
        Создавайте и добавляйте аннотации к файлу DXF прямо сейчас, посетив веб-сайт [живые демо](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dxf"
          title: "О формате файла DXF"
          content: |
            DXF, формат обмена чертежами или формат обмена чертежами — это теговое представление данных файла чертежа AutoCAD. Каждый элемент в файле имеет префикс целого числа, называемый групповым кодом. Этот групповой код фактически представляет следующий за ним элемент и указывает значение элемента данных для данного типа объекта. DXF позволяет представить почти всю указанную пользователем информацию в файле чертежа. Формат файла DXF был разработан Autodesk как формат файла данных САПР для взаимодействия данных между AutoCAD и другими приложениями. Таким образом, данные могут быть импортированы из других форматов в DXF в AutoCAD в соответствии со спецификациями совместимости форматов файлов DXF.
          link: "https://docs.fileformat.com/image/dxf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Аннотирование других популярных форматов файлов"
    content: |
        Библиотека управления аннотациями Net для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Добавление Annotation в PDF"
          link: "https://products.groupdocs.com/annotation/net/add/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Добавление Annotation в DOC"
          link: "https://products.groupdocs.com/annotation/net/add/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Добавление Annotation в DOCM"
          link: "https://products.groupdocs.com/annotation/net/add/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Добавление Annotation в DOCX"
          link: "https://products.groupdocs.com/annotation/net/add/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Добавление Annotation в DOT"
          link: "https://products.groupdocs.com/annotation/net/add/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Добавление Annotation в DOTX"
          link: "https://products.groupdocs.com/annotation/net/add/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Добавление Annotation в RTF"
          link: "https://products.groupdocs.com/annotation/net/add/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Добавление Annotation в ODT"
          link: "https://products.groupdocs.com/annotation/net/add/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Добавление Annotation в XLS"
          link: "https://products.groupdocs.com/annotation/net/add/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Добавление Annotation в XLSX"
          link: "https://products.groupdocs.com/annotation/net/add/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Добавление Annotation в XLSM"
          link: "https://products.groupdocs.com/annotation/net/add/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Добавление Annotation в XLSB"
          link: "https://products.groupdocs.com/annotation/net/add/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Добавление Annotation в ODS"
          link: "https://products.groupdocs.com/annotation/net/add/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Добавление Annotation в PPT"
          link: "https://products.groupdocs.com/annotation/net/add/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Добавление Annotation в PPTX"
          link: "https://products.groupdocs.com/annotation/net/add/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Добавление Annotation в PPSX"
          link: "https://products.groupdocs.com/annotation/net/add/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Добавление Annotation в POTM"
          link: "https://products.groupdocs.com/annotation/net/add/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Добавление Annotation в PPTM"
          link: "https://products.groupdocs.com/annotation/net/add/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Добавление Annotation в PPS"
          link: "https://products.groupdocs.com/annotation/net/add/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Добавление Annotation в ODP"
          link: "https://products.groupdocs.com/annotation/net/add/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Добавление Annotation в HTML"
          link: "https://products.groupdocs.com/annotation/net/add/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Добавление Annotation в TIFF"
          link: "https://products.groupdocs.com/annotation/net/add/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Добавление Annotation в JPEG"
          link: "https://products.groupdocs.com/annotation/net/add/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Добавление Annotation в PNG"
          link: "https://products.groupdocs.com/annotation/net/add/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Добавление Annotation в EML"
          link: "https://products.groupdocs.com/annotation/net/add/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Добавление Annotation в MSG"
          link: "https://products.groupdocs.com/annotation/net/add/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Добавление Annotation в VSD"
          link: "https://products.groupdocs.com/annotation/net/add/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Добавление Annotation в VSDX"
          link: "https://products.groupdocs.com/annotation/net/add/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Добавление Annotation в VSS"
          link: "https://products.groupdocs.com/annotation/net/add/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Добавление Annotation в VST"
          link: "https://products.groupdocs.com/annotation/net/add/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Добавление Annotation в DWG"
          link: "https://products.groupdocs.com/annotation/net/add/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Добавление Annotation в DXF"
          link: "https://products.groupdocs.com/annotation/net/add/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Добавление Annotation в DCM"
          link: "https://products.groupdocs.com/annotation/net/add/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Добавление Annotation в WMF"
          link: "https://products.groupdocs.com/annotation/net/add/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Добавление Annotation в EMF"
          link: "https://products.groupdocs.com/annotation/net/add/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---