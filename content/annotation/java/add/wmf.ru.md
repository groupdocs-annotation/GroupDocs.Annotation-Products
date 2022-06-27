---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:27+03:00
draft: false
############################# Head ############################
head_title: "Добавить аннотации к WMF в приложениях Java"
head_description: "Java API для создания и добавления популярных типов аннотаций в WMF, изображения, чертежи и форматы файлов документов."
############################# Header ############################
title: "Аннотировать файлы WMF в Java"
description: "Добавляйте аннотации к документам WMF, Microsoft Office, изображениям, HTML, рисункам и другим форматам файлов в любых типах приложений Java."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
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
              text: "Справочник по API"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Примеры кода"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Живые демонстрации"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Цены"
    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Annotation для Java API"
    content: |
        [GroupDocs.Annotation for Java](/ru/annotation/java/) — это собственный Java API для управления аннотациями с комплексной поддержкой для создания, добавления, редактирования, удаления, извлечения и экспорта аннотаций из изображений и форматов файлов документов. Пользователи могут легко извлекать комментарии, заметки, примечания и 13 различных типов аннотаций, включая текст, графику и водяные знаки, в документах PDF, HTML, Microsoft Word, электронных таблицах Excel, диаграммах Visio, презентациях PowerPoint, рисунках, изображениях и многих других форматах файлов. Функция обработки аннотаций может точно считывать аннотации из импортированных документов и позволяет экспортировать обратно в исходный или желаемый формат файла после реализации настройки аннотаций.
############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по добавлению аннотаций в WMF в Java"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/java/) позволяет разработчикам Java легко добавлять различные типы аннотаций в файлы WMF в любом приложении на основе Java, выполняя несколько простых шагов.
        * Создание экземпляра объекта Annotator с входным путем или потоком документа.
        * Создайте экземпляр объекта TextFieldAnnotation с нужными свойствами (позиция, номер страницы и т. д.).
        * Вызвать метод добавления и передать объект TextFieldAnnotation.
        * Метод сохранения вызова с результирующим путем документа или потоком.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среда разработки: NetBeans, Intellij IDEA, Eclipse и т. д.
        * Среда выполнения Java: J2SE 6.0 и выше
        * Получите последнюю версию GroupDocs.Annotation для Java от [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-conversion)
############################# Preview ############################
preview:
    enable: true
    title: "Annotation preview and code sample"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-strikeout-annotation.png)
    code: |
        ```java
        String outputPath = Constants.getOutputFilePath("AddTextStrikeoutAnnotation", FilenameUtils.getExtension(input.wmf));
        final Annotator annotator = new Annotator(input.wmf);
        try {
            Reply reply1 = new Reply();
            reply1.setComment("First comment");
            reply1.setRepliedOn(Calendar.getInstance().getTime());
            Reply reply2 = new Reply();
            reply2.setComment("Second comment");
            reply2.setRepliedOn(Calendar.getInstance().getTime());
            java.util.List replies =  new ArrayList();
            replies.add(reply1);
            replies.add(reply2);
            Point point1 = new Point(80, 730);
            Point point2 = new Point(240, 730);
            Point point3 = new Point(80, 650);
            Point point4 = new Point(240, 650);
            List points = new ArrayList();
            points.add(point1);
            points.add(point2);
            points.add(point3);
            points.add(point4);
            StrikeoutAnnotation strikeout = new StrikeoutAnnotation();
            strikeout.setCreatedOn(Calendar.getInstance().getTime());
            strikeout.setFontColor(65535);
            strikeout.setMessage("This is strikeout annotation");
            strikeout.setOpacity(0.7);
            strikeout.setPageNumber(0);
            strikeout.setPoints(points);
            strikeout.setReplies(replies);
            annotator.add(strikeout);
            annotator.save(output.wmf);
        } finally {
            if (annotator != null) {
                annotator.dispose();
            }
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для добавления аннотаций к документам и изображениям"
    content: |
        Создавайте и добавляйте аннотации к файлу WMF прямо сейчас, посетив веб-сайт [живые демо](https://products.groupdocs.app/annotation/family).  
        Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-wmf"
          title: "О формате файла WMF"
          content: |
            Файлы с расширением WMF представляют собой метафайл Microsoft Windows (WMF) для хранения данных векторных и растровых изображений. Чтобы быть более точным, WMF принадлежит к категории форматов векторных файлов форматов графических файлов, которые не зависят от устройства. Интерфейс графических устройств Windows (GDI) использует функции, хранящиеся в файле WMF, для отображения изображения на экране. Более расширенная версия WMF, известная как Enhanced Meta Files (EMF), была опубликована позже, что делает формат более многофункциональным. Практически WMF похож на SVG.
          link: "https://docs.fileformat.com/image/wmf/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Аннотирование других популярных форматов файлов"
    content: |
        Библиотека управления аннотациями Java для документов и форматов изображений. Добавьте свойства аннотации к некоторым популярным форматам файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить аннотацию в PDF"
          link: "/annotation/java/add/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить аннотацию в DOC"
          link: "/annotation/java/add/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить аннотацию в DOCM"
          link: "/annotation/java/add/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить аннотацию в DOCX"
          link: "/annotation/java/add/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить аннотацию в DOT"
          link: "/annotation/java/add/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить аннотацию в DOTX"
          link: "/annotation/java/add/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить аннотацию в DOTM"
          link: "/annotation/java/add/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить аннотацию в RTF"
          link: "/annotation/java/add/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Добавить аннотацию в ODT"
          link: "/annotation/java/add/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить аннотацию в XLS"
          link: "/annotation/java/add/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить аннотацию в XLSX"
          link: "/annotation/java/add/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить аннотацию в XLSM"
          link: "/annotation/java/add/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить аннотацию в XLSB"
          link: "/annotation/java/add/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить аннотацию в ODS"
          link: "/annotation/java/add/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить аннотацию в PPT"
          link: "/annotation/java/add/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить аннотацию в PPTX"
          link: "/annotation/java/add/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить аннотацию в PPSX"
          link: "/annotation/java/add/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Добавить аннотацию в POTM"
          link: "/annotation/java/add/potm/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Добавить аннотацию в PPTM"
          link: "/annotation/java/add/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Добавить аннотацию в PPS"
          link: "/annotation/java/add/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить аннотацию в ODP"
          link: "/annotation/java/add/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить аннотацию в HTML"
          link: "/annotation/java/add/html/"
          description: "Язык гипертекстовой разметки"
        # format loop
        - name: "Добавить аннотацию в TIFF"
          link: "/annotation/java/add/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить аннотацию в JPEG"
          link: "/annotation/java/add/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Добавить аннотацию в PNG"
          link: "/annotation/java/add/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить аннотацию в BMP"
          link: "/annotation/java/add/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить аннотацию в EML"
          link: "/annotation/java/add/eml/"
          description: "Сообщение электронной почты"
        # format loop
        - name: "Добавить аннотацию в MSG"
          link: "/annotation/java/add/msg/"
          description: "Сообщение электронной почты Microsoft Outlook"
        # format loop
        - name: "Добавить аннотацию в VSD"
          link: "/annotation/java/add/vsd/"
          description: "Чертеж Microsoft Visio 2003-2010"
        # format loop
        - name: "Добавить аннотацию в VSDX"
          link: "/annotation/java/add/vsdx/"
          description: "Рисование Microsoft Visio"
        # format loop
        - name: "Добавить аннотацию в VSS"
          link: "/annotation/java/add/vss/"
          description: "Трафарет Microsoft Visio 2003-2010"
        # format loop
        - name: "Добавить аннотацию в VST"
          link: "/annotation/java/add/vst/"
          description: "Трафарет Microsoft Visio 2013"
        # format loop
        - name: "Добавить аннотацию в DWG"
          link: "/annotation/java/add/dwg/"
          description: "Форматы проектных данных Autodesk"
        # format loop
        - name: "Добавить аннотацию в DXF"
          link: "/annotation/java/add/dxf/"
          description: "Обмен чертежами AutoCAD"
        # format loop
        - name: "Добавить аннотацию в DCM"
          link: "/annotation/java/add/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
        # format loop
        - name: "Добавить аннотацию в WMF"
          link: "/annotation/java/add/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Добавить аннотацию в EMF"
          link: "/annotation/java/add/emf/"
          description: "Расширенный формат метафайла"
############################# Back to top ###############################
back_to_top:
    enable: true
---