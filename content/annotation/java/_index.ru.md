---
############################# Static ############################
layout: "product"
date: 2022-07-05T12:44:18+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API аннотации документов Java | Просмотр и комментирование изображений PDF Word Excel PPTX"
head_description: "API аннотаций документов Java. Просмотр, теги, комментарии и аннотации PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAD и форматы файлов изображений."

############################# Header ############################
title: "Аннотации документов через Java API"
description: "Создавайте приложения Java с возможностями просмотра и комментирования документов PDF, HTML, MS Office и других форматов без установки какого-либо внешнего программного обеспечения."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation для Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Обзор"

            # button loop
            - link: "#features"
              text: "Функции"

            # button loop
            - link: "#support"
              text: "Поддержка"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "Демонстрация"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Цена"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Java API это продукт который дает возможность работать с аннотациями в документах на разных платформах и в разных операционных системах, таких как: Android, MacOS, Linux, Windows. GroupDocs.Annotation предоставляет библиотеку с простым и понятным API. Вы можете работать с защищенными паролем документами, генерировать графические представления документов разных разрешений, вращать документы, скрывать части документов, гибко манипулировать с параметрами аннотаций и многое другое.

        GroupDocs.Annotation for Java API повзовляет  работать с разными типами аннотаций такими как: Text, Polyline, Area, Underline, Point, Watermark, Arrow, Ellipse, Text Replacement, Distance, Text Field, Resource Redaction etc. Для таких наиболее популярных форматов документов как: PDF, HTML, Microsoft Office Word, Excel spreadsheets, PowerPoint presentations, Visio, Outlook emails, images, metafiles, CAD drawing and various other formats. API предоставляет возможность получать миниатюры страниц документа и поддерживает импорт и экспорт аннотаций в файлы PDF и из них.

        С помощью библиотеки вы можете [добавлять](/annotation/java/add/bmp/) новые аннотации, [редактировать](/annotation/java/edit/bmp/), [извлекать](/annotation/[PLATFORM_URL]/extract/bmp/), [удалять](/annotation/java/remove/bmp/) из документов - вот это далеко не полный список всех возможностей. Также библиотека предоставляет полный набор объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями во всех поддерживаемых форматах документов. 

        Работа с GroupDocs.Annotation for Java API очень простая, и состоит всего из нескольких основных шагов. Для начала вам нужно установить лицензию, потом выбрать файл с которым вы хотите работать, дальше выбрать нужное действие с аннотацией (удалить/редактировать/извлечь/удалить) и сохранить в нужное место. Так же у нас есть [документация](https://docs.groupdocs.com/annotation/java/getting-started/) по продутку и много [примеров](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) по работе с аннотациями.

        GroupDocs.Annotation регулярно обновляется и предоставляет для своих клиентов поддержку, вы можете задавать нам вопросы или присылать свои идеи или рассказывать про свои потребновсть в чем то новом и мы с радостью это реализуем в наших новых версиях.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приводится обзор GroupDocs.Annotation для Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Обзор"
          content: |
            * Добавить аннотации
            * Экспорт аннотаций
            * Импорт аннотаций
            * Комментарии на основе ответов
            * Совместимость аннотаций
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation для Java поддерживает все популярные [форматы файлов документов](https://docs.groupdocs.com/annotation/java/supported-document-formats/), включая: Microsoft Office, PDF, изображения и многие другие.
        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: [DOC](/annotation/java/add/doc/), [DOCX](/annotation/java/add/docx/), [DOCM](/annotation/java/add/docm/), [DOT](/annotation/java/add/dot/), [DOTX](/annotation/java/add/dotx/), [RTF](/annotation/java/add/rtf/)
                * **Excel**: [XLS](/annotation/java/add/xls/), [XLSX](/annotation/java/add/xlsx/), [XLSB](/annotation/java/add/xlsb/), [XLSM](/annotation/java/add/xlsm/)
                * **PowerPoint**: [PPT](/annotation/java/add/ppt/), [PPTX](/annotation/java/add/pptx/), [PPS](/annotation/java/add/pps/), [PPSX](/annotation/java/add/ppsx/), [POTM](/annotation/java/add/potm/), [POTX](/annotation/java/add/potx/), [PPSM](/annotation/java/add/ppsm/), [PPTM](/annotation/java/add/pptm/), [WMF](/annotation/java/add/wmf/), [EMF](/annotation/java/add/emf/)
                * **Outlook**: [EML](/annotation/java/add/eml/), [EMLX](/annotation/java/add/emlx/), [MSG](/annotation/java/add/msg/)
                * **Visio**: [VSS](/annotation/java/add/vss/), [VST](/annotation/java/add/vst/), [VSD](/annotation/java/add/vsd/), [VSDX](/annotation/java/add/vsdx/), [VSX](/annotation/java/add/vsx/)

        right:
          enable: true
          table:
            # table loop
            - title: "Другие форматы"
              content: |
                * **Portable**: [PDF](/annotation/java/add/pdf/) (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: [ODT](/annotation/java/add/odt/), [ODS](/annotation/java/add/ods/), [ODP](/annotation/java/add/odp/)
                * **Images**: [BMP](/annotation/java/add/bmp/), [JPG](/annotation/java/add/jpg/), [JPEG](/annotation/java/add/jpeg/), [TIFF](/annotation/java/add/tiff/), [TIF](/annotation/java/add/tif/), [PNG](/annotation/java/add/png/), [GIF](/annotation/java/add/gif/), [DCM](/annotation/java/add/dcm/), [DICOM](/annotation/java/add/dicom/)
                * **AutoCAD**: [DWG](/annotation/java/add/dwg/), [DXF](/annotation/java/add/dxf/), [CAD](/annotation/java/add/cad/)
                * **Other**: [HTM](/annotation/java/add/htm/), [HTML](/annotation/java/add/html/), [CSV](/annotation/java/add/csv/), [DJVU](/annotation/java/add/djvu/), [OTP](/annotation/java/add/otp/), [OTT](/annotation/java/add/ott/)

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation для Java поддерживает следующие операционные системы, платформы и менеджеры пакетов:
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Microsoft Windows
                * Сервер Microsoft Windows
                * линукс
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * Java 7 (1.7) и выше

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Среды разработки"
              content: |
                * NetBeans
                * IntelliJ ИДЕЯ
                * Затмение
            # table loop
            - icon: "fas fa-tools"
              title: "Инструмент автоматизации сборки"
              content: |
                * Мавен

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Annotation для функций Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/java/add-area-annotation/"
        content: "Добавить аннотацию области в документ и связать простые и вложенные комментарии"

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/java/add-arrow-annotation/"
        content: "Укажите на определенный контент с помощью аннотации со стрелкой"

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: "Установите текстовые водяные знаки в PDF, слайды, рабочие листы Excel, изображения и диаграммы в угловом положении"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Добавьте всплывающие комментарии в любое место в документе с помощью точечной аннотации"

      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/java/add-polyline-annotation/"
        content: "Используйте аннотацию полилинии для соединения последовательности сегментов линии, сегментов дуги или того и другого"

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/java/add-ellipse-annotation/"
        content: "Добавить аннотацию эллипса в PDF, документы Word, электронные таблицы, презентации, диаграммы и изображения"

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: "Добавляйте угловые водяные знаки для PDF, PowerPoint, Excel, изображений и диаграмм"

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/java/extract-annotations-from-document/"
        content: "Получить координаты текстовой аннотации в графическом представлении документа"

      # feature loop
      - icon: "fas fa-location-arrow"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Подчеркивание, зачеркивание или изменение определенного текста в документе"

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Добавить текстовую марку или водяной знак и текстовое поле в документ"

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/advanced-usage/"
        content: "Экспорт аннотаций Word & PowerPoint"

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Аннотируйте электронные таблицы Excel с помощью типов аннотаций Text, TextReplacement, Watermark и Resource Redaction."

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Добавляйте полилинию, зачеркивание, подчеркивание или текстовые аннотации к презентациям и слайдам PowerPoint."

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Отметить аннотацию точки в презентациях с использованием координат X, Y"

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Добавляйте зачеркнутые, текстовые, подчеркнутые или ломаные аннотации к изображениям"

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: "Получение сведений о документе и изображений для диаграмм Visio, таких как VSS и VSD"

      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/java/basic-usage/"
        content: "Получите миниатюры страниц документа и работайте с многостраничными файлами TIFF"
      
      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: "Получить всю аннотацию документа с помощью одного вызова функции"

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/java/add-link-annotation/"
        content: "Добавление аннотаций ссылок в презентации PDF, Word и PowerPoint"

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Поддержка анализа пути SVG для PDF, Word, диаграмм, слайдов и других основных форматов документов."

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: "Поддержка добавления аннотации водяного знака к документам Word и очистки для замены текста."

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: "Поддержка обработки фигур в диаграммах для текстовых аннотаций"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/advanced-usage/"
        content: "Экономьте время за счет кэширования предварительных просмотров страниц документов для более быстрой обработки"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Легко комментируйте документы Word, Excel и PowerPoint даже в старых форматах"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-distance-annotation/"
        content: "Отображение заголовков аннотаций расстояния для Excel, PowerPoint и диаграмм"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for .NET"
          image: "/border/groupdocs-annotation-net.svg"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---