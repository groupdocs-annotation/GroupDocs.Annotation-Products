---
############################# Static ############################
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:44+03:00
draft: false
############################# Head ############################
head_title: "Удалить аннотации из HTML в приложениях Java"
head_description: "Javaannotation API для удаления популярных типов аннотаций из HTML, изображений, рисунков и форматов файлов документов."
############################# Header ############################
title: "Удалить аннотации из HTML в Java"
description: "Удаляйте уже добавленные аннотации из Microsoft Office, изображений, рисунков, HTML и других форматов файлов документов в любом типе приложения Java."
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
        [GroupDocs.Annotation for Java](/ru/annotation/java/) — это встроенная библиотека управления аннотациями Java для просмотра, [добавления](/annotation/java/add/html/), обновления, удаления, [извлечения](/annotation/java/extract/html/) или экспорта аннотаций из изображений и форматов файлов документов. Пользователи могут легко удалять комментарии, заметки, примечания и различные типы аннотаций, включая текст, графику и водяные знаки, в файлах PDF, HTML, Word, Excel, Visio, презентациях, рисунках, изображениях и многих других форматах. Функция обработки аннотаций может точно считывать аннотации из импортированных документов и позволяет экспортировать обратно в исходный или желаемый формат файла после выполнения настройки.
############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по удалению аннотаций из HTML в Java"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/java/) упрощает разработчикам Java удаление деталей аннотаций из файлов HTML в любом приложении на основе Java за счет выполнения нескольких простых шагов.
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
    code: |
        ```java
        Annotator annotator = new Annotator("C://input.html");
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);
        annotator.save("C://output.html", saveOptions);
        annotator.dispose();
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для удаления аннотаций из документов и изображений"
    content: |
        Просмотрите и удалите аннотации из файла HTML прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family). 
        Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-html"
          title: "О формате файла HTML"
          content: |
            HTML (Hyper Text Markup Language) — это расширение для веб-страниц, созданных для отображения в браузерах. HTML, известный как язык Интернета, развивался с учетом новых требований к информации, которая должна отображаться как часть веб-страниц. Последний вариант известен как HTML 5, что дает большую гибкость для работы с языком. HTML-страницы либо принимаются с сервера, на котором они размещены, либо также могут быть загружены из локальной системы. Каждая HTML-страница состоит из HTML-элементов, таких как формы, текст, изображения, анимация, ссылки и т. д. Эти элементы представлены такими тегами, как img, a, p и некоторыми другими, где каждый тег имеет начало и конец. Он также может встраивать приложения, написанные на языках сценариев, таких как JavaScript и таблицы стилей (CSS), для общего представления макета.
          link: "https://docs.fileformat.com/web/html/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Редактирование аннотаций из файлов других популярных форматов"
    content: |
        Java API для удаления аннотаций из документов и форматов файлов изображений. Удалите свойства аннотаций из некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Удалить аннотацию из PDF"
          link: "/annotation/java/remove/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Удалить аннотацию из DOC"
          link: "/annotation/java/remove/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Удалить аннотацию из DOCM"
          link: "/annotation/java/remove/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Удалить аннотацию из DOCX"
          link: "/annotation/java/remove/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Удалить аннотацию из DOT"
          link: "/annotation/java/remove/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Удалить аннотацию из DOTX"
          link: "/annotation/java/remove/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Удалить аннотацию из RTF"
          link: "/annotation/java/remove/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Удалить аннотацию из ODT"
          link: "/annotation/java/remove/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Удалить аннотацию из XLS"
          link: "/annotation/java/remove/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Удалить аннотацию из XLSX"
          link: "/annotation/java/remove/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Удалить аннотацию из XLSM"
          link: "/annotation/java/remove/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить аннотацию из XLSB"
          link: "/annotation/java/remove/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Удалить аннотацию из ODS"
          link: "/annotation/java/remove/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Удалить аннотацию из PPT"
          link: "/annotation/java/remove/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Удалить аннотацию из PPTX"
          link: "/annotation/java/remove/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Удалить аннотацию из PPSX"
          link: "/annotation/java/remove/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Удалить аннотацию из POTM"
          link: "/annotation/java/remove/potm/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Удалить аннотацию из PPTM"
          link: "/annotation/java/remove/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Удалить аннотацию из PPS"
          link: "/annotation/java/remove/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Удалить аннотацию из ODP"
          link: "/annotation/java/remove/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Удалить аннотацию из TIFF"
          link: "/annotation/java/remove/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Удалить аннотацию из JPEG"
          link: "/annotation/java/remove/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Удалить аннотацию из PNG"
          link: "/annotation/java/remove/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Удалить аннотацию из BMP"
          link: "/annotation/java/remove/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Удалить аннотацию из EML"
          link: "/annotation/java/remove/eml/"
          description: "Сообщение электронной почты"
        # format loop
        - name: "Удалить аннотацию из MSG"
          link: "/annotation/java/remove/msg/"
          description: "Сообщение электронной почты Microsoft Outlook"
        # format loop
        - name: "Удалить аннотацию из VSD"
          link: "/annotation/java/remove/vsd/"
          description: "Чертеж Microsoft Visio 2003-2010"
        # format loop
        - name: "Удалить аннотацию из VSDX"
          link: "/annotation/java/remove/vsdx/"
          description: "Рисование Microsoft Visio"
        # format loop
        - name: "Удалить аннотацию из VSS"
          link: "/annotation/java/remove/vss/"
          description: "Трафарет Microsoft Visio 2003-2010"
        # format loop
        - name: "Удалить аннотацию из VST"
          link: "/annotation/java/remove/vst/"
          description: "Трафарет Microsoft Visio 2013"
        # format loop
        - name: "Удалить аннотацию из DWG"
          link: "/annotation/java/remove/dwg/"
          description: "Форматы проектных данных Autodesk"
        # format loop
        - name: "Удалить аннотацию из DXF"
          link: "/annotation/java/remove/dxf/"
          description: "Обмен чертежами AutoCAD"
        # format loop
        - name: "Удалить аннотацию из DCM"
          link: "/annotation/java/remove/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
        # format loop
        - name: "Удалить аннотацию из WMF"
          link: "/annotation/java/remove/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Удалить аннотацию из EMF"
          link: "/annotation/java/remove/emf/"
          description: "Расширенный формат метафайла"
############################# Back to top ###############################
back_to_top:
    enable: true
---
