
---
############################# Static ############################
layout: "auto-gen" ###_DIMA_### layout: "auto-gen-annotation"
date: 2022-07-05T12:44:18+03:00
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/edit/docx"/>

############################# Head ############################
head_title: "Редактирование Аннотаций в DOCX в Net приложении"
head_description: "Net API для создания и Редактирование популярных типов аннотаций в DOCX, изображения, чертежи и форматы файлов документов."

############################# Header ############################
title: "Редактирование DOCX файла в Net"
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

        Эта библиотека позволяет работать не только с DOCX но также и со многими другими форматами, такими как Word, Excel, PowerPoint, Outlook emails, Visio, Adobe, OpenDocument, OpenOffice, AutoCad и еще множеством других форматов.

        GroupDocs.Annotation for Net API позволяет создавать и [добавлять](/ru/annotation/net/add/docx/) новые заметки, редактировать аннотации, [извлекать](/ru/annotation/net/extract/docx/) комментарии, примечания и [удалять](/ru/annotation/net/remove/docx/) их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction в документах PDF, HTML, Microsoft Word, электронных таблицах, диаграммах, презентациях, рисунках, изображениях и многих других форматах файлов.

        В примере ниже продемонстрирована работа с DOCX документом. В этом примере вы видите основные шаги в работе с GroupDocs.Annotation: установка лицензии, открытие файла для работы, создание аннотации, добавление объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями и сохранение результата в нужное место. Более детально ознакомиться с возможностями библиотеки вы можете посмотрев наш [github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net)-аккаунт, или в нашей [документации](https://docs.groupdocs.com/annotation/net/getting-started/) к продутку.

############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по Редактирование аннотаций в DOCX in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) [GroupDocs.Annotation](/ru/annotation/net/) упрощает разработчикам Net обновление различных свойств аннотаций из файлов DOCX в любом приложении на основе Net за счет выполнения нескольких простых шагов.
        
        * Создание экземпляра объекта Annotator с входным путем к документу или потоком с экземпляром LoadOptions с ImportAnnotations = true.
        * Создайте некоторую реализацию AnnotationBase и установите идентификатор существующей аннотации (если аннотация с этим идентификатором не найдена, ничего не изменится) или список путей аннотаций (все существующие аннотации будут удалены).
        * Вызвать метод обновления объекта Annotator с переданными аннотациями.
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
    
    code: |
        ```cs
        // открыть аннотированный документ
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            // предполагается, что мы собираемся изменить некоторые свойства существующей аннотации
                AreaAnnotation updated = new AreaAnnotation
                {
                      // Важно установить идентификатор существующей аннотации
                      Id = 1,
                      BackgroundColor = 255,
                      Box = new Rectangle(0, 0, 50, 200),
                      CreatedOn = DateTime.Now,
                      Message = "This is updated annotation",
                      Replies = new List
                      {
                           new Reply
                           {
                                Comment = "Updated first comment",
                                RepliedOn = DateTime.Now
                           },
                           new Reply
                           {
                                Comment = "Updated second comment",
                                RepliedOn = DateTime.Now
                           }
                    }
               };
               // обновить аннотацию
               annotator.Update(updated);
               annotator.Save("result.bmp");
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для изменения аннотаций из документов и изображений"
    content: |
        Читайте и редактируйте аннотации из файла DOCX прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).
        Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docx"
          title: "О формате файла DOCX"
          content: |
            DOCX — широко известный формат документов Microsoft Word. Представленный в 2007 году с выпуском Microsoft Office 2007, структура этого нового формата документа была изменена с простого двоичного файла на комбинацию XML и двоичных файлов. Файлы Docx можно открывать в Word 2007 и его более поздних версиях, но не в более ранних версиях MS Word, которые поддерживают расширения файлов DOC.
          link: "https://docs.fileformat.com/image/docx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Редактирование аннотаций из файлов других популярных форматов"
    content: |
        Библиотека управления аннотациями Net для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format:
        # format loop
        - name: "Редактирование Annotation в PDF"
          link: "https://products.groupdocs.com/annotation/net/edit/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Редактирование Annotation в DOC"
          link: "https://products.groupdocs.com/annotation/net/edit/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Редактирование Annotation в DOCM"
          link: "https://products.groupdocs.com/annotation/net/edit/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Редактирование Annotation в DOCX"
          link: "https://products.groupdocs.com/annotation/net/edit/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Редактирование Annotation в DOT"
          link: "https://products.groupdocs.com/annotation/net/edit/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Редактирование Annotation в DOTX"
          link: "https://products.groupdocs.com/annotation/net/edit/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Редактирование Annotation в RTF"
          link: "https://products.groupdocs.com/annotation/net/edit/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Редактирование Annotation в ODT"
          link: "https://products.groupdocs.com/annotation/net/edit/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Редактирование Annotation в XLS"
          link: "https://products.groupdocs.com/annotation/net/edit/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Редактирование Annotation в XLSX"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Редактирование Annotation в XLSM"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Редактирование Annotation в XLSB"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Редактирование Annotation в ODS"
          link: "https://products.groupdocs.com/annotation/net/edit/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Редактирование Annotation в PPT"
          link: "https://products.groupdocs.com/annotation/net/edit/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Редактирование Annotation в PPTX"
          link: "https://products.groupdocs.com/annotation/net/edit/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Редактирование Annotation в PPSX"
          link: "https://products.groupdocs.com/annotation/net/edit/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Редактирование Annotation в POTM"
          link: "https://products.groupdocs.com/annotation/net/edit/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Редактирование Annotation в PPTM"
          link: "https://products.groupdocs.com/annotation/net/edit/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Редактирование Annotation в PPS"
          link: "https://products.groupdocs.com/annotation/net/edit/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Редактирование Annotation в ODP"
          link: "https://products.groupdocs.com/annotation/net/edit/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Редактирование Annotation в HTML"
          link: "https://products.groupdocs.com/annotation/net/edit/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Редактирование Annotation в TIFF"
          link: "https://products.groupdocs.com/annotation/net/edit/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Редактирование Annotation в JPEG"
          link: "https://products.groupdocs.com/annotation/net/edit/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Редактирование Annotation в PNG"
          link: "https://products.groupdocs.com/annotation/net/edit/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Редактирование Annotation в EML"
          link: "https://products.groupdocs.com/annotation/net/edit/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Редактирование Annotation в MSG"
          link: "https://products.groupdocs.com/annotation/net/edit/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Редактирование Annotation в VSD"
          link: "https://products.groupdocs.com/annotation/net/edit/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Редактирование Annotation в VSDX"
          link: "https://products.groupdocs.com/annotation/net/edit/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Редактирование Annotation в VSS"
          link: "https://products.groupdocs.com/annotation/net/edit/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Редактирование Annotation в VST"
          link: "https://products.groupdocs.com/annotation/net/edit/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Редактирование Annotation в DWG"
          link: "https://products.groupdocs.com/annotation/net/edit/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Редактирование Annotation в DXF"
          link: "https://products.groupdocs.com/annotation/net/edit/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Редактирование Annotation в DCM"
          link: "https://products.groupdocs.com/annotation/net/edit/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Редактирование Annotation в WMF"
          link: "https://products.groupdocs.com/annotation/net/edit/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Редактирование Annotation в EMF"
          link: "https://products.groupdocs.com/annotation/net/edit/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---