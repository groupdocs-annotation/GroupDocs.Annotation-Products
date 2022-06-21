---
############################# Static ############################
layout: "auto-gen"
date: 2021-05-13T12:44:50+03:00
draft: false
############################# Head ############################
head_title: "Добавление аннотации к файлам JPEG в приложениях C# .NET"
head_description: "Обработка аннотаций C# .NET &amp; API управления для добавления популярных типов аннотаций к файлам JPEG, изображениям, форматам файлов чертежей и документов."
############################# Header ############################
title: "Добавить аннотацию к JPEG в .NET"
description: "Аннотируйте изображения, документы Microsoft Office и другие форматы файлов, используя 13 различных типов аннотаций, включая текст, комментарии, заметки и т. д."
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
        [GroupDocs.Annotation for .NET](/ru/annotation/net/) — это собственный API .NET, который позволяет пользователям добавлять, редактировать и удалять аннотации к изображениям и форматам файлов документов. Вы можете легко использовать комментарии, заметки, примечания и различные типы аннотаций, включая текст, графику и водяные знаки, в PDF, HTML, Word, Excel, диаграммы Visio, презентации, рисунки, изображения и файлы многих других форматов. Функция обработки аннотаций может точно считывать аннотации из импортированных документов и позволяет экспортировать обратно в исходный или желаемый формат файла после выполнения настройки.
############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по добавлению аннотаций к JPEG в C#"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/net/) позволяет разработчикам .NET легко добавлять свойства аннотаций к файлам JPEG из своих приложений, выполняя несколько простых шагов.
        * Создание экземпляра объекта Annotator с входным путем или потоком документа.
        * Создание экземпляра объекта TextFieldAnnotation с желаемыми свойствами (позиция, номер страницы и т. д.).
        * Вызвать метод Add и передать объект TextFieldAnnotation.
        * Вызовите метод Save с результирующим путем или потоком документа.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для .NET поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        * Операционные системы: Microsoft Windows, Linux, MacOS
        * Среды разработки: Visual Studio, Xamarin, MonoDevelop
        * Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        * Загрузите последнюю версию GroupDocs.Annotation для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.annotation).
    code: |
        ```cs
        // Добавляем аннотацию текстового поля к документу с локального диска
        using (Annotator annotator = new Annotator("input.jpeg"))
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
            annotator.Save("result.jpeg");
        }
        ```
############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для добавления аннотаций"
    content: |
        Добавьте аннотацию в файл JPEG прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family). 
        Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpeg"
          title: "О формате файла JPEG"
          content: |
            JPEG — это тип формата изображения, который сохраняется с использованием метода сжатия с потерями. Выходное изображение в результате сжатия представляет собой компромисс между размером хранилища и качеством изображения. Пользователи могут настроить уровень сжатия для достижения желаемого уровня качества и в то же время уменьшить размер хранилища. Качество изображения незначительно ухудшается, если к изображению применяется сжатие 10:1. Чем выше значение сжатия, тем выше ухудшение качества изображения. Формат файла изображения JPEG был стандартизирован Объединенной группой экспертов по фотографии, отсюда и название JPEG. Формат был выбран для хранения и передачи фотографических изображений в Интернете. Почти все операционные системы теперь имеют средства просмотра, поддерживающие визуализацию изображений JPEG, которые также часто хранятся с расширением JPG. Даже веб-браузеры поддерживают визуализацию изображений JPEG.
          link: "https://docs.fileformat.com/image/jpeg/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Добавление аннотаций к файлам других форматов"
    content: |
        API обработки мультиформатных документов и аннотаций изображений для .NET. Добавьте аннотацию к некоторым популярным форматам файлов, как указано ниже.
    format: 
        # format loop
        - name: "Добавить аннотацию в PDF"
          link: "/annotation/net/add/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Добавить аннотацию в DOC"
          link: "/annotation/net/add/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Добавить аннотацию в DOCM"
          link: "/annotation/net/add/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить аннотацию в DOCX"
          link: "/annotation/net/add/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Добавить аннотацию в DOT"
          link: "/annotation/net/add/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Добавить аннотацию в DOTX"
          link: "/annotation/net/add/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Добавить аннотацию в DOTM"
          link: "/annotation/net/add/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Добавить аннотацию в RTF"
          link: "/annotation/net/add/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Добавить аннотацию в ODT"
          link: "/annotation/net/add/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Добавить аннотацию в XLS"
          link: "/annotation/net/add/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Добавить аннотацию в XLSX"
          link: "/annotation/net/add/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Добавить аннотацию в XLSM"
          link: "/annotation/net/add/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Добавить аннотацию в XLSB"
          link: "/annotation/net/add/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Добавить аннотацию в ODS"
          link: "/annotation/net/add/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Добавить аннотацию в PPT"
          link: "/annotation/net/add/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Добавить аннотацию в PPTX"
          link: "/annotation/net/add/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Добавить аннотацию в PPSX"
          link: "/annotation/net/add/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Добавить аннотацию в POTM"
          link: "/annotation/net/add/potm/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Добавить аннотацию в PPTM"
          link: "/annotation/net/add/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Добавить аннотацию в PPS"
          link: "/annotation/net/add/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Добавить аннотацию в ODP"
          link: "/annotation/net/add/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Добавить аннотацию в HTML"
          link: "/annotation/net/add/html/"
          description: "Язык гипертекстовой разметки"
        # format loop
        - name: "Добавить аннотацию в TIFF"
          link: "/annotation/net/add/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Добавить аннотацию в PNG"
          link: "/annotation/net/add/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Добавить аннотацию в BMP"
          link: "/annotation/net/add/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Добавить аннотацию в EML"
          link: "/annotation/net/add/eml/"
          description: "Сообщение электронной почты"
        # format loop
        - name: "Добавить аннотацию в MSG"
          link: "/annotation/net/add/msg/"
          description: "Сообщение электронной почты Microsoft Outlook"
        # format loop
        - name: "Добавить аннотацию в VSD"
          link: "/annotation/net/add/vsd/"
          description: "Чертеж Microsoft Visio 2003-2010"
        # format loop
        - name: "Добавить аннотацию в VSDX"
          link: "/annotation/net/add/vsdx/"
          description: "Рисование Microsoft Visio"
        # format loop
        - name: "Добавить аннотацию в VSS"
          link: "/annotation/net/add/vss/"
          description: "Трафарет Microsoft Visio 2003-2010"
        # format loop
        - name: "Добавить аннотацию в VST"
          link: "/annotation/net/add/vst/"
          description: "Трафарет Microsoft Visio 2013"
        # format loop
        - name: "Добавить аннотацию в DWG"
          link: "/annotation/net/add/dwg/"
          description: "Форматы проектных данных Autodesk"
        # format loop
        - name: "Добавить аннотацию в DXF"
          link: "/annotation/net/add/dxf/"
          description: "Обмен чертежами AutoCAD"
        # format loop
        - name: "Добавить аннотацию в DCM"
          link: "/annotation/net/add/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
        # format loop
        - name: "Добавить аннотацию в WMF"
          link: "/annotation/net/add/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Добавить аннотацию в EMF"
          link: "/annotation/net/add/emf/"
          description: "Расширенный формат метафайла"
############################# Back to top ###############################
back_to_top:
    enable: true
---
