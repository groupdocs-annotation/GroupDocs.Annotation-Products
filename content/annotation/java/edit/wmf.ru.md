---
############################# Static ############################
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:34+03:00
draft: false
############################# Head ############################
head_title: "Редактировать аннотации файлов WMF в приложениях Java"
head_description: "API редактора аннотаций Java для обновления популярных типов аннотаций из WMF, изображений, рисунков и форматов файлов документов."
############################# Header ############################
title: "Редактировать аннотации в файле WMF в Java"
description: "Редактор аннотаций Java для изображений, Microsoft Office и других форматов файлов документов. Аннотируйте файлы WMF, используя 13 различных типов аннотаций, таких как; область, текст, заметки, водяной знак и т. д."
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
        [GroupDocs.Annotation for Java](/ru/annotation/java/) — это собственное решение для управления аннотациями Java, позволяющее эффективно просматривать, [добавлять](/annotation/java/add/wmf/), обновлять, [удалять](/annotation/java/remove/wmf/) и [извлекать](/annotation/java/extract/wmf/) аннотации из изображений и форматов файлов документов. Пользователи могут легко редактировать комментарии, заметки, примечания и различные типы аннотаций, включая текст, графику и водяные знаки, в PDF, HTML, Word, Excel, диаграммах Visio, презентациях, рисунках, изображениях и многих других форматах файлов. Функция обработки аннотаций может точно считывать аннотации из импортированных документов и позволяет экспортировать обратно в исходный или желаемый формат файла после выполнения настройки.
############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по редактированию аннотаций из WMF в Java"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/java/) упрощает разработчикам Java обновление различных свойств аннотаций из файлов WMF в любом приложении на основе Java за счет выполнения нескольких простых шагов.
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
    code: |
        ```java
        String outputPath = "UpdateAnnotation.wmf";
        Annotator annotator = new Annotator("input.wmf");
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        // добавить исходную аннотацию
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        LoadOptions loadOptions = new LoadOptions();
        loadOptions.setImportAnnotations(true);
        // открыть аннотированный документ
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);
        // предлагаем изменить некоторые свойства существующей аннотации
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        // обновить аннотацию
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для изменения аннотаций из документов и изображений"
    content: |
        Читайте и редактируйте аннотации из файла WMF прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family).  
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
    title: "Редактирование аннотаций из файлов других популярных форматов"
    content: |
        API редактора аннотаций Java для документов и форматов изображений. Обновите свойства аннотаций из некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Редактировать аннотацию из PDF"
          link: "/annotation/java/edit/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Редактировать аннотацию из DOC"
          link: "/annotation/java/edit/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Редактировать аннотацию из DOCM"
          link: "/annotation/java/edit/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать аннотацию из DOCX"
          link: "/annotation/java/edit/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Редактировать аннотацию из DOT"
          link: "/annotation/java/edit/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Редактировать аннотацию из DOTX"
          link: "/annotation/java/edit/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Редактировать аннотацию из RTF"
          link: "/annotation/java/edit/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Редактировать аннотацию из ODT"
          link: "/annotation/java/edit/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Редактировать аннотацию из XLS"
          link: "/annotation/java/edit/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Редактировать аннотацию из XLSX"
          link: "/annotation/java/edit/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Редактировать аннотацию из XLSM"
          link: "/annotation/java/edit/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать аннотацию из XLSB"
          link: "/annotation/java/edit/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Редактировать аннотацию из ODS"
          link: "/annotation/java/edit/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Редактировать аннотацию из PPT"
          link: "/annotation/java/edit/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Редактировать аннотацию из PPTX"
          link: "/annotation/java/edit/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Редактировать аннотацию из PPSX"
          link: "/annotation/java/edit/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Редактировать аннотацию из POTM"
          link: "/annotation/java/edit/potm/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Редактировать аннотацию из PPTM"
          link: "/annotation/java/edit/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Редактировать аннотацию из PPS"
          link: "/annotation/java/edit/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Редактировать аннотацию из ODP"
          link: "/annotation/java/edit/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Редактировать аннотацию из HTML"
          link: "/annotation/java/edit/html/"
          description: "Язык гипертекстовой разметки"
        # format loop
        - name: "Редактировать аннотацию из TIFF"
          link: "/annotation/java/edit/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Редактировать аннотацию из JPEG"
          link: "/annotation/java/edit/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Редактировать аннотацию из PNG"
          link: "/annotation/java/edit/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Редактировать аннотацию из BMP"
          link: "/annotation/java/edit/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Редактировать аннотацию из EML"
          link: "/annotation/java/edit/eml/"
          description: "Сообщение электронной почты"
        # format loop
        - name: "Редактировать аннотацию из MSG"
          link: "/annotation/java/edit/msg/"
          description: "Сообщение электронной почты Microsoft Outlook"
        # format loop
        - name: "Редактировать аннотацию из VSD"
          link: "/annotation/java/edit/vsd/"
          description: "Чертеж Microsoft Visio 2003-2010"
        # format loop
        - name: "Редактировать аннотацию из VSDX"
          link: "/annotation/java/edit/vsdx/"
          description: "Рисование Microsoft Visio"
        # format loop
        - name: "Редактировать аннотацию из VSS"
          link: "/annotation/java/edit/vss/"
          description: "Трафарет Microsoft Visio 2003-2010"
        # format loop
        - name: "Редактировать аннотацию из VST"
          link: "/annotation/java/edit/vst/"
          description: "Трафарет Microsoft Visio 2013"
        # format loop
        - name: "Редактировать аннотацию из DWG"
          link: "/annotation/java/edit/dwg/"
          description: "Форматы проектных данных Autodesk"
        # format loop
        - name: "Редактировать аннотацию из DXF"
          link: "/annotation/java/edit/dxf/"
          description: "Обмен чертежами AutoCAD"
        # format loop
        - name: "Редактировать аннотацию из DCM"
          link: "/annotation/java/edit/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
        # format loop
        - name: "Редактировать аннотацию из EMF"
          link: "/annotation/java/edit/emf/"
          description: "Расширенный формат метафайла"
############################# Back to top ###############################
back_to_top:
    enable: true
---
