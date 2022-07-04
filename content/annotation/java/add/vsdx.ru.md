---
############################# Static ############################
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:26+03:00
draft: false
############################# Head ############################
head_title: "Добавить аннотации к VSDX в приложениях Java"
head_description: "Java API для создания и добавления популярных типов аннотаций в VSDX, изображения, чертежи и форматы файлов документов."
############################# Header ############################
title: "Аннотировать файлы VSDX в Java"
description: "Добавляйте аннотации к VSDX, документам Microsoft Office, изображениям, HTML, рисункам и другим форматам файлов в любых типах приложений Java."
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
    title_left: "Шаги по добавлению аннотаций в VSDX в Java"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/java/) позволяет разработчикам Java легко добавлять различные типы аннотаций в файлы VSDX в любом приложении на основе Java, выполняя несколько простых шагов.
        * Создание объектов ответа с комментарием и датой.
        * Создайте объект AreaAnnotation, установите параметры области и добавьте ответы.
        * Создайте объект Annotator и добавьте аннотацию области.
        * Сохранить выходной файл.
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
    title: "Annotation preview and code sample"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
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
        Annotator annotator = new Annotator("input.vsdx");
        annotator.add(area);
        annotator.save("output.vsdx");
        annotator.dispose();
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для добавления аннотаций к документам и изображениям"
    content: |
        Создавайте и добавляйте аннотации к файлу VSDX прямо сейчас, посетив веб-сайт [живые демо](https://products.groupdocs.app/annotation/family).  
        Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsdx"
          title: "О формате файла VSDX"
          content: |
            Файлы с расширением .VSDX представляют формат файлов Microsoft Visio, появившийся в Microsoft Office 2013 и более поздних версиях. Он был разработан для замены формата двоичных файлов .VSD, который поддерживается более ранними версиями Microsoft Visio. Он также поддерживается службами Visio в Microsoft SharePoint Server 2013 и не требует промежуточного формата файла для публикации в SharePoint Server. Файлы Visio используются для создания чертежей, содержащих визуальные объекты, блок-схемы, диаграмму UML, информационный поток, организационные диаграммы, диаграммы программного обеспечения, схему сети, модели баз данных, сопоставление объектов и другую подобную информацию. Файлы, созданные с помощью Visio, также можно экспортировать в различные форматы файлов, такие как PNG, BMP, PDF и другие.
          link: "https://docs.fileformat.com/image/vsdx/"
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
