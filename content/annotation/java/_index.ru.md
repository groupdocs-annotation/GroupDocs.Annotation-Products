---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
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
description: "Создавайте приложения Java с возможностями просмотра и комментирования документов PDF, HTML, MS Office и других форматов без установки какого-либо внешнего программного обеспечения.."
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
        image: "/border/groupdocs-annotation-java.svg"
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
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation for Java API предоставляет простые в использовании функции управления документами, аннотациями и манипулирования, которые можно использовать в ваших бизнес-приложениях на основе Java. Наша библиотека аннотаторов Java позволяет работать со многими типами аннотаций, включая текст, полилинию, область, подчеркивание, точку, водяной знак, стрелку, эллипс, замену текста, расстояние, текстовое поле, редактирование ресурсов и т. д. Она также предлагает полный набор объектов данных для настройки свойств аннотаций в соответствии с вашими требованиями во всех поддерживаемых форматах документов, включая: PDF, HTML, Microsoft Office Word, электронные таблицы Excel, презентации PowerPoint, Visio, сообщения электронной почты Outlook, изображения, метафайлы, чертежи САПР и различные другие форматы.
        
      API предоставляет возможность получать миниатюры страниц документа и поддерживает импорт и экспорт аннотаций в файлы PDF и из них.
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
            - title: "Форматы Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **Excel**: XLS, XLSX, XLSB, XLSM
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Outlook**: EML, EMLX
                * **Visio**: VSS, VST, VSD, VSDX

        right:
          enable: true
          table:
            # table loop
            - title: "Другие форматы"
              content: |
                * **Портативный**: PDF (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: ODT, ODS, ODP
                * **Изображения**: BMP, JPG, TIFF, TIF, PNG
                * **AutoCAD**: DWG, DXF
                * **Другое**: HTML

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

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Annotation для функций Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Добавить аннотацию области в документ и связать простые и вложенные комментарии"

      # feature loop
      - icon: "fas fa-eye"
        content: "Укажите на определенный контент с помощью аннотации со стрелкой"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Установите текстовые водяные знаки в PDF, слайды, рабочие листы Excel, изображения и диаграммы в угловом положении"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Добавьте всплывающие комментарии в любое место в документе с помощью точечной аннотации"

      # feature loop
      - icon: "fas fa-code"
        content: "Используйте аннотацию полилинии для соединения последовательности сегментов линии, сегментов дуги или того и другого"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Добавить аннотацию эллипса в PDF, документы Word, электронные таблицы, презентации, диаграммы и изображения"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Добавляйте угловые водяные знаки для PDF, PowerPoint, Excel, изображений и диаграмм"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Получить координаты текстовой аннотации в графическом представлении документа"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Подчеркивание, зачеркивание или изменение определенного текста в документе"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Добавить текстовую марку или водяной знак и текстовое поле в документ"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Экспорт аннотаций Word & PowerPoint"

      # feature loop
      - icon: "fas fa-columns"
        content: "Аннотируйте электронные таблицы Excel с помощью типов аннотаций Text, TextReplacement, Watermark и Resource Redaction."

      # feature loop
      - icon: "fas fa-file-word"
        content: "Добавляйте полилинию, зачеркивание, подчеркивание или текстовые аннотации к презентациям и слайдам PowerPoint."

      # feature loop
      - icon: "fas fa-envelope"
        content: "Отметить аннотацию точки в презентациях с использованием координат X, Y"

      # feature loop
      - icon: "fas fa-print"
        content: "Добавляйте зачеркнутые, текстовые, подчеркнутые или ломаные аннотации к изображениям"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Получение сведений о документе и изображений для диаграмм Visio, таких как VSS и VSD"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Получите миниатюры страниц документа и работайте с многостраничными файлами TIFF"
      
      # feature loop
      - icon: "fas fa-file-excel"
        content: "Получить всю аннотацию документа с помощью одного вызова функции"

      # feature loop
      - icon: "fas fa-heading"
        content: "Добавление аннотаций ссылок в презентации PDF, Word и PowerPoint"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Поддержка анализа пути SVG для PDF, Word, диаграмм, слайдов и других основных форматов документов."

      # feature loop
      - icon: "fas fa-cube"
        content: "Поддержка добавления аннотации водяного знака к документам Word и очистки для замены текста."

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Поддержка обработки фигур в диаграммах для текстовых аннотаций"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Экономьте время за счет кэширования предварительных просмотров страниц документов для более быстрой обработки"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Легко комментируйте документы Word, Excel и PowerPoint даже в старых форматах"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Отображение заголовков аннотаций расстояния для Excel, PowerPoint и диаграмм"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation предлагает API для просмотра документов для других популярных сред разработки."

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
