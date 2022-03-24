---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "API аннотации документов C# .NET | Аннотирование файлов изображений PDF Word Excel PPTX"
head_description: "API аннотации документов C# .NET. Просмотр, теги, комментарии и аннотации PDF Word DOC DOCX, Excel XLS XLSX, PPT PPTX, OTP, CAD, EMF WMF и файлы изображений."

############################# Header ############################
title: "Аннотировать текст или изображения в документах"
description: "Расширьте возможности своих приложений .NET, чтобы добавлять, редактировать и удалять все популярные типы аннотаций из более чем 50 форматов документов для более простой и эффективной совместной работы.."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for .NET"
        image: "/border/groupdocs-annotation-net.svg"
        product: "GroupDocs.Annotation"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Обзор ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation для .NET — это полный набор API-интерфейсов, который помогает создавать приложения для управления аннотациями документов на C#, ASP.NET и других связанных технологиях .NET. Вы можете создавать и работать со всеми популярными типами аннотаций, такими как область, точка, текст, эллипс, ссылка, подчеркивание, полилиния, стрелка, расстояние, водяной знак, изображение и т. д. для PDF, HTML, Microsoft Office Word, электронных таблиц Excel, презентаций PowerPoint, Visio, изображения, чертежи САПР и различные другие форматы. Библиотека аннотаторов документов позволяет экспортировать документы после добавления аннотаций, комментариев или выделенных заметок обратно в исходный формат. Он также дает вам удобный набор объектов данных, с помощью которых вы можете настраивать аннотации в соответствии с вашими требованиями.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Ниже приведен обзор GroupDocs.Annotation для .NET:

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
          GroupDocs.Annotation для .NET поддерживает все популярные [форматы файлов документов](https://docs.groupdocs.com/annotation/net/supported-document-formats/), включая: Microsoft Office, PDF, изображения и многие другие.

        left:
          enable: true
          table:
            # table loop
            - title: "Форматы Microsoft Office"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF 
                * **Microsoft Excel**: XLS, XLSX, XLSM, XLSB, CSV
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Microsoft Visio**: VSD, VSS, VSDX, VST, VSDM, VSSX, VSTM

        right:
          enable: true
          table:
            # table loop
            - title: "Другие форматы"
              content: |
                * **Портативный**: PDF (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: ODT, ODS, ODP
                * **Изображения**: BMP, JPEG, PNG, TIFF
                * **AutoCAD**: DWG, DXF
                * **Метафайлы**: EMF, WMF
                * **Электронная почта**: EML, EMLX
                * **Интернет**: HTM, HTML

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for .NET поддерживает следующие Операционные системы, Frameworks & Менеджер пакетовs:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Операционные системы"
              content: |
                * Рабочий стол Windows (x86 и x64)
                * Сервер Windows (x86 и x64)
                * Windows Azure
                * линукс
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Поддерживаемые платформы"
              content: |
                * .NET Стандарт 2.0
                * .NET Framework 2.0 или выше
                * .NET Core 2.0 или выше
                * Монофреймворк 1.2 или выше

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Менеджер пакетов"
              content: |
                * NuGet
            
            # table loop
            - icon: "fas fa-tools"
              title: "Среды разработки"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * МоноДевелопмент

############################# Функции ############################
features:
    enable: true
    title: "GroupDocs.Annotation для функций .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Добавляйте, редактируйте и удаляйте аннотации и ответы"

      # feature loop
      - icon: "fas fa-eye"
        content: "Экспорт аннотаций to Document"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Ограниченная лицензия — контролируемое выставление счетов путем оплаты в соответствии с использованием API"
      
      # feature loop
      - icon: "fas fa-code"
        content: "Вызов одной функции для извлечения всех аннотаций документа"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Присвоить значение аннотации точки или переместить существующее значение точки"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Добавьте аннотацию ссылки к слайдам PDF, Word и PowerPoint"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Установить цвет фона аннотации или удалить все аннотации из документа"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Аннотируйте PDF-файлы с точностью — получите представление изображения PDF-документа и предпросмотра страниц кэша"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Получить текстовые координаты текстовой аннотации в графическом представлении документа"

      # feature loop
      - icon: "fas fa-columns"
        content: "Связывание комментариев пользователей с аннотацией области и поддержка вложенных комментариев"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Используйте аннотацию со стрелкой для указания на определенный контент"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Используйте аннотацию расстояния, чтобы нарисовать линию, которая представляет расстояние между объектами"

      # feature loop
      - icon: "fas fa-print"
        content: "Аннотация на основе точек, которая при нажатии открывает окно для добавления комментариев"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Создайте соединенную последовательность сегментов линии, созданную как аннотацию полилинии"

      # feature loop
      - icon: "fas fa-lock"
        content: "Создайте сегменты прямой линии, сегменты дуги или их комбинацию."

      # feature loop
      - icon: "fas fa-file-code"
        content: "Пометить области документа, предложенные для редактирования"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Добавить аннотацию к изображению в PDF, диаграммы, Word, Excel, презентации и изображения"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Добавить текстовое поле и текстовый штамп или водяной знак в документ"

      # feature loop
      - icon: "fas fa-heading"
        content: "Зачеркивание, подчеркивание или замена определенного текста в документе"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Измените размер аннотации, назначив новые параметры высоты и ширины"

      # feature loop
      - icon: "fas fa-cube"
        content: "Получите миниатюры страниц документа. Управление множеством аннотированных документов для изображений и диаграмм"
  
      # feature loop
      - icon: "fab fa-uncharted"
        content: "Отрегулируйте вертикальное и горизонтальное выравнивание для аннотации водяного знака"
  
      # feature loop
      - icon: "fab fa-uncharted"
        content: "Добавить горизонтальное выравнивание текста для текстового поля"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Получить информацию о строках текста документа (текст, ширина, высота, отступы)"

    больше_функций:
      # more_feature_loop
      - title: "Поддержка нескольких типов аннотаций"
        content: |
          GroupDocs.Annotation для .NET позволяет работать с различными типами аннотаций. Это дает свободу и простоту общения при совместной работе с командой над задачами. Вы можете использовать аннотации, такие как аннотации области (отметить область как прямоугольник и добавить к ней примечания), аннотацию точки (прикрепить комментарии в любой точке документа), текстовую аннотацию (добавить комментарий к выделенному тексту), аннотацию зачеркивания/подчеркивания ( применяется к абзацу), аннотация в виде ломаной линии (рисование фигур и линий от руки), аннотация в виде стрелки (указатель в виде стрелки с присоединенными комментариями), аннотация в виде эллипса (отображение текста внутри эллипса), аннотация в виде расстояния (нарисуйте линию, которая представляет расстояние между объектами), ссылка аннотация (добавление веб-ссылок на поддерживаемые форматы документов) и аннотация водяного знака (текстовый штамп или водяной знак могут быть добавлены в документ).

          ```cs
          // Инициализировать список AnnotationInfo
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          // Инициализировать текстовую аннотацию
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          // Добавить аннотацию в список
          annotations.Add(textAnnotation);
          // Получить входной файловый поток
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          // Экспортировать аннотацию и сохранить выходной файл
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation предлагает API для просмотра документов для других популярных сред разработки."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for Java"
          image: "/border/groupdocs-annotation-java.svg"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
