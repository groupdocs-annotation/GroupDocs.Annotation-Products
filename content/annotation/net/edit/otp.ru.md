---
############################# Static ############################
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:57+03:00
draft: false
############################# Head ############################
head_title: "Прочитать и усилить Редактирование аннотаций в файлах OTP в приложениях C# .NET"
head_description: "API-интерфейс редактора аннотаций C# .NET для обновления популярных типов аннотаций до файлов OTP, изображений, файлов чертежей и документов."
############################# Header ############################
title: "Редактировать аннотации в файле OTP в .NET"
description: ".NET редактор аннотаций для изображений, Microsoft Office и других форматов файлов документов. Аннотируйте документы, используя 13 различных типов аннотаций, таких как; область, текст, заметки, водяной знак и т. д."
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
        [GroupDocs.Annotation for .NET](/ru/annotation/net/) — это собственный API-интерфейс управления и редактирования аннотаций .NET для чтения, [добавления](/annotation/net/add/otp/), обновления, [удаления](/annotation/net/remove/otp/) и [извлечения](/annotation/net/extract/otp/) аннотаций из изображений и форматов файлов документов. Пользователи могут легко обновлять комментарии, примечания, примечания и различные типы аннотаций, включая текст, графику и водяные знаки, в PDF, HTML, Word, Excel, схемах Visio, презентациях, рисунках, изображениях и многих других форматах файлов. Функция обработки аннотаций может точно считывать аннотации из импортированных документов и позволяет экспортировать обратно в исходный или желаемый формат файла после выполнения настройки.
############################# Steps ############################
howTo:
steps:
    enable: true
    title_left: "Шаги по редактированию аннотаций из OTP в C#"
    content_left: |
        [GroupDocs.Annotation](/ru/annotation/net/) позволяет разработчикам .NET легко редактировать детали аннотаций из файлов OTP в своих приложениях, выполняя несколько простых шагов.
        * Создание экземпляра объекта Annotator с входным путем или потоком документа.
        * Создайте некоторую реализацию AnnotationBase и установите идентификатор существующей аннотации (если аннотация с этим идентификатором не найдена, ничего не изменится) или список путей аннотаций (все существующие аннотации будут удалены).
        * Вызвать метод Update объекта Annotator с переданными аннотациями.
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
    title: "Живые демонстрации для обновления аннотаций"
    content: |
        Отредактируйте аннотацию в файле OTP прямо сейчас, посетив [живые демонстрации](https://products.groupdocs.app/annotation/family). 
        Живая демонстрация имеет следующие преимущества
############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-otp"
          title: "О формате файла OTP"
          content: |
            Файлы с расширением .OTP представляют собой файлы шаблонов презентаций, созданные приложениями в стандартном формате OASIS OpenDocument. Содержимое такого файла включает презентационную информацию в виде слайдов с текстом, изображениями, фигурами, мультимедийным содержимым, эффектами перехода и другими элементами слайдов. Эти файлы шаблонов используются для быстрого создания новых презентаций на основе информации о стилях, хранящейся в самом шаблоне. Файлы OTP можно создавать и сохранять с помощью нескольких различных приложений, таких как Impress, поставляемый с пакетом OpenOffice, и Microsoft PowerPoint. Формат файла OTP аналогичен файлам шаблонов Microsoft PowerPoint .POT и .POTX.
          link: "https://docs.fileformat.com/presentation/otp/"
############################# More Formats ############################
more_formats:
    enable: true
    title: "Редактирование аннотаций в файлах других форматов"
    content: |
        Многоформатный API редактора аннотаций к документам и изображениям для .NET. Обновите аннотацию из некоторых популярных форматов файлов, как указано ниже.
    format: 
        # format loop
        - name: "Редактировать аннотацию в PDF"
          link: "/annotation/net/edit/pdf/"
          description: "Adobe Portable Document Format"
        # format loop
        - name: "Редактировать аннотацию в DOC"
          link: "/annotation/net/edit/doc/"
          description: "Документ Microsoft Word"
        # format loop
        - name: "Редактировать аннотацию в DOCM"
          link: "/annotation/net/edit/docm/"
          description: "Документ Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать аннотацию в DOCX"
          link: "/annotation/net/edit/docx/"
          description: "Документ Microsoft Word с открытым XML"
        # format loop
        - name: "Редактировать аннотацию в DOT"
          link: "/annotation/net/edit/dot/"
          description: "Шаблон документа Microsoft Word"
        # format loop
        - name: "Редактировать аннотацию в DOTX"
          link: "/annotation/net/edit/dotx/"
          description: "Шаблон документа Word Open XML"
        # format loop
        - name: "Редактировать аннотацию в DOTM"
          link: "/annotation/net/edit/dotm/"
          description: "Шаблон Microsoft Word с поддержкой макросов"
        # format loop
        - name: "Редактировать аннотацию в RTF"
          link: "/annotation/net/edit/rtf/"
          description: "Форматированный текстовый документ"
        # format loop
        - name: "Редактировать аннотацию в ODT"
          link: "/annotation/net/edit/odt/"
          description: "Открыть текст документа"
        # format loop
        - name: "Редактировать аннотацию в XLS"
          link: "/annotation/net/edit/xls/"
          description: "Формат двоичного файла Microsoft Excel"
        # format loop
        - name: "Редактировать аннотацию в XLSX"
          link: "/annotation/net/edit/xlsx/"
          description: "Электронная таблица Microsoft Excel Open XML"
        # format loop
        - name: "Редактировать аннотацию в XLSM"
          link: "/annotation/net/edit/xlsm/"
          description: "Электронная таблица Microsoft Excel с поддержкой макросов"
        # format loop
        - name: "Редактировать аннотацию в XLSB"
          link: "/annotation/net/edit/xlsb/"
          description: "Двоичный лист Microsoft Excel"
        # format loop
        - name: "Редактировать аннотацию в ODS"
          link: "/annotation/net/edit/ods/"
          description: "Открыть электронную таблицу документов"
        # format loop
        - name: "Редактировать аннотацию в PPT"
          link: "/annotation/net/edit/ppt/"
          description: "Презентация PowerPoint"
        # format loop
        - name: "Редактировать аннотацию в PPTX"
          link: "/annotation/net/edit/pptx/"
          description: "Презентация PowerPoint Open XML"
        # format loop
        - name: "Редактировать аннотацию в PPSX"
          link: "/annotation/net/edit/ppsx/"
          description: "Слайд-шоу PowerPoint Open XML"
        # format loop
        - name: "Редактировать аннотацию в POTM"
          link: "/annotation/net/edit/potm/"
          description: "Шаблон Microsoft PowerPoint"
        # format loop
        - name: "Редактировать аннотацию в PPTM"
          link: "/annotation/net/edit/pptm/"
          description: "Презентация Microsoft PowerPoint"
        # format loop
        - name: "Редактировать аннотацию в PPS"
          link: "/annotation/net/edit/pps/"
          description: "Слайд-шоу Microsoft PowerPoint 97-2003"
        # format loop
        - name: "Редактировать аннотацию в ODP"
          link: "/annotation/net/edit/odp/"
          description: "Презентация OpenDocument"
        # format loop
        - name: "Редактировать аннотацию в HTML"
          link: "/annotation/net/edit/html/"
          description: "Язык гипертекстовой разметки"
        # format loop
        - name: "Редактировать аннотацию в TIFF"
          link: "/annotation/net/edit/tiff/"
          description: "Формат файла изображения с тегами"
        # format loop
        - name: "Редактировать аннотацию в JPEG"
          link: "/annotation/net/edit/jpeg/"
          description: "Изображение в формате JPEG"
        # format loop
        - name: "Редактировать аннотацию в PNG"
          link: "/annotation/net/edit/png/"
          description: "Портативная сетевая графика"
        # format loop
        - name: "Редактировать аннотацию в BMP"
          link: "/annotation/net/edit/bmp/"
          description: "Формат растрового файла"
        # format loop
        - name: "Редактировать аннотацию в EML"
          link: "/annotation/net/edit/eml/"
          description: "Сообщение электронной почты"
        # format loop
        - name: "Редактировать аннотацию в MSG"
          link: "/annotation/net/edit/msg/"
          description: "Сообщение электронной почты Microsoft Outlook"
        # format loop
        - name: "Редактировать аннотацию в VSD"
          link: "/annotation/net/edit/vsd/"
          description: "Чертеж Microsoft Visio 2003-2010"
        # format loop
        - name: "Редактировать аннотацию в VSDX"
          link: "/annotation/net/edit/vsdx/"
          description: "Рисование Microsoft Visio"
        # format loop
        - name: "Редактировать аннотацию в VSS"
          link: "/annotation/net/edit/vss/"
          description: "Трафарет Microsoft Visio 2003-2010"
        # format loop
        - name: "Редактировать аннотацию в VST"
          link: "/annotation/net/edit/vst/"
          description: "Трафарет Microsoft Visio 2013"
        # format loop
        - name: "Редактировать аннотацию в DWG"
          link: "/annotation/net/edit/dwg/"
          description: "Форматы проектных данных Autodesk"
        # format loop
        - name: "Редактировать аннотацию в DXF"
          link: "/annotation/net/edit/dxf/"
          description: "Обмен чертежами AutoCAD"
        # format loop
        - name: "Редактировать аннотацию в DCM"
          link: "/annotation/net/edit/dcm/"
          description: "Цифровая визуализация и коммуникации в медицине"
        # format loop
        - name: "Редактировать аннотацию в WMF"
          link: "/annotation/net/edit/wmf/"
          description: "Метафайл Windows"
        # format loop
        - name: "Редактировать аннотацию в EMF"
          link: "/annotation/net/edit/emf/"
          description: "Расширенный формат метафайла"
############################# Back to top ###############################
back_to_top:
    enable: true
---
