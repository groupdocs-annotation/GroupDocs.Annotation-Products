---
############################# Static ############################
layout: "auto-gen-annotation"
date: 2021-05-13T12:45:06+03:00
draft: false
############################# Head ############################
head_title: "Удаление аннотаций из файлов DOTX в приложениях C# .NET"
head_description: "API аннотаций C# .NET для удаления популярных типов аннотаций в файлы DOTX, изображения, форматы файлов чертежей и документов."
############################# Header ############################
title: "Удалить аннотации из DOTX в C#"
description: "Удалите все ранее добавленные аннотации из Microsoft Office, изображений, Интернета, рисунков и других форматов файлов документов в любом типе приложения .NET."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
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
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: ".NET"
    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "Справочник по API"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Примеры кода"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Живые демонстрации"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Цены"
    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"
############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Annotation для .NET API"
    content: |
        [GroupDocs.Annotation for .NET](/ru/annotation/net/) — это собственный API обработки аннотаций .NET для просмотра, [добавления](/annotation/net/add/dotx/), [изменения](/annotation/net/edit/dotx), удаления и [извлечения](/annotation/net/extract/dotx/) аннотаций из изображений и форматов файлов документов. Пользователи могут легко удалять комментарии, заметки, примечания и различные типы аннотаций, включая текст, графику и водяные знаки, в PDF, HTML, Word, Excel, диаграммах Visio, презентациях, рисунках, изображениях и многих других форматах файлов. Функция обработки аннотаций может точно считывать аннотации из импортированных документов и позволяет экспортировать обратно в исходный или желаемый формат файла после выполнения настройки.
############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по удалению аннотаций из DOTX"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/net/) позволяет разработчикам .NET легко удалять детали аннотаций из файлов DOTX в своих приложениях, выполняя несколько простых шагов.
        * Создание экземпляра объекта Annotator с входным путем или потоком документа.
        * Создайте экземпляр объекта SaveOptions и установите AnnotationTypes = AnnotationType.None.
        * Вызовите метод Save с результирующим путем или потоком документа и объектом SaveOptions.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Annotation для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.annotation).
    code: |
        ```cs
        // 1- Как удалить аннотацию из документа, используя индекс аннотации
        using (Annotator annotator = new Annotator("result.dotx"))
        {
        	annotator.Remove(0);
        	annotator.Save("removed.dotx");
        }
        // 2- Как удалить аннотацию из документа с помощью объекта аннотации
        using (Annotator annotator = new Annotator("result.dotx"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp[0]);
        	annotator.Save("removed.dotx");
        }
        // 3- Как удалить некоторые аннотации из документа, используя список идентификаторов
        using (Annotator annotator = new Annotator("result.dotx"))
        {
        	var idList = new List{1, 2, 3};
        	annotator.Remove(idList);
        	annotator.Save("removed.dotx");
        }
        // 4- Как удалить некоторые аннотации из документа, используя список аннотаций
        using (Annotator annotator = new Annotator("result.dotx"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp);
        	annotator.Save("removed.dotx");
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для удаления аннотаций"
    content: |
        Удалите аннотацию из файла DOTX прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family). Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dotx"
          title: "О формате файла DOTX"
          content: |
            Файлы с расширением DOTX представляют собой файлы шаблонов, созданные Microsoft Word с предварительно отформатированными настройками для создания дополнительных файлов DOCX. Файл шаблона создается для того, чтобы иметь определенные пользовательские настройки, которые должны применяться к последующим мухам, созданным на их основе. Эти параметры включают поля страницы, границы, верхние и нижние колонтитулы и другие параметры страницы. Такие шаблоны используются в официальных документах, таких как бланки компаний и стандартизированные формы. Формат файла DOTX был представлен в выпуске Microsoft Office 2007 для замены двоичного формата файла DOT, но поддерживается и более поздними версиями. Microsoft Word по умолчанию открывает каждый новый документ на основе файла normal.dot. В случае изменения все новые созданные файлы будут иметь те же настройки, что и в файле шаблона. В Microsoft Word 2007 формат файла DOT был заменен форматом файла DOTX на основе Office OpenXML.
          link: "https://docs.fileformat.com/word-processing/dotx/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Удаление аннотаций из файлов других поддерживаемых форматов"
    content: |
        API для удаления аннотаций мультиформатных документов и изображений для .NET. Удалите аннотацию из некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Удалить аннотацию из PDF"
          link: "/annotation/net/remove/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Удалить аннотацию из DOC"
          link: "/annotation/net/remove/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Удалить аннотацию из DOCM"
          link: "/annotation/net/remove/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Удалить аннотацию из DOCX"
          link: "/annotation/net/remove/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Удалить аннотацию из DOT"
          link: "/annotation/net/remove/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Удалить аннотацию из RTF"
          link: "/annotation/net/remove/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Удалить аннотацию из ODT"
          link: "/annotation/net/remove/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Удалить аннотацию из XLS"
          link: "/annotation/net/remove/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Удалить аннотацию из XLSX"
          link: "/annotation/net/remove/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Удалить аннотацию из XLSM"
          link: "/annotation/net/remove/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Удалить аннотацию из XLSB"
          link: "/annotation/net/remove/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Удалить аннотацию из ODS"
          link: "/annotation/net/remove/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Удалить аннотацию из PPT"
          link: "/annotation/net/remove/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Удалить аннотацию из PPTX"
          link: "/annotation/net/remove/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Удалить аннотацию из PPSX"
          link: "/annotation/net/remove/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Удалить аннотацию из POTM"
          link: "/annotation/net/remove/potm/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Удалить аннотацию из PPTM"
          link: "/annotation/net/remove/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Удалить аннотацию из PPS"
          link: "/annotation/net/remove/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Удалить аннотацию из ODP"
          link: "/annotation/net/remove/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Удалить аннотацию из HTML"
          link: "/annotation/net/remove/html/"
          description: "Язык гипертекстовой разметки"
        # format loop
        - name: "Удалить аннотацию из TIFF"
          link: "/annotation/net/remove/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Удалить аннотацию из JPEG"
          link: "/annotation/net/remove/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Удалить аннотацию из PNG"
          link: "/annotation/net/remove/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Удалить аннотацию из BMP"
          link: "/annotation/net/remove/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Удалить аннотацию из EML"
          link: "/annotation/net/remove/eml/"
          description: "Сообщение электронной почты"
        # format loop
        - name: "Удалить аннотацию из MSG"
          link: "/annotation/net/remove/msg/"
          description: "Сообщение электронной почты Microsoft Outlook"
        # format loop
        - name: "Удалить аннотацию из VSD"
          link: "/annotation/net/remove/vsd/"
          description: "Чертеж Microsoft Visio 2003-2010"
        # format loop
        - name: "Удалить аннотацию из VSDX"
          link: "/annotation/net/remove/vsdx/"
          description: "Рисование Microsoft Visio"
        # format loop
        - name: "Удалить аннотацию из VSS"
          link: "/annotation/net/remove/vss/"
          description: "Трафарет Microsoft Visio 2003-2010"
        # format loop
        - name: "Удалить аннотацию из VST"
          link: "/annotation/net/remove/vst/"
          description: "Трафарет Microsoft Visio 2013"
        # format loop
        - name: "Удалить аннотацию из DWG"
          link: "/annotation/net/remove/dwg/"
          description: "Форматы проектных данных Autodesk"
        # format loop
        - name: "Удалить аннотацию из DXF"
          link: "/annotation/net/remove/dxf/"
          description: "Обмен чертежами AutoCAD"
        # format loop
        - name: "Удалить аннотацию из DCM"
          link: "/annotation/net/remove/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
        # format loop
        - name: "Удалить аннотацию из WMF"
          link: "/annotation/net/remove/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Удалить аннотацию из EMF"
          link: "/annotation/net/remove/emf/"
          description: "Расширенный формат метафайла"
############################# Back to top ###############################
back_to_top:
    enable: true
---
