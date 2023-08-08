---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net DCM Annotation API Annotate в C#"
head_description: "Net API для создания и аннотирования популярных типов аннотаций из DCM, изображений, рисунков и форматов файлов документов."

############################# Header ############################
title: "Аннотировать DCM из сети"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Annotation для Net API"
    content: |
        GroupDocs.Annotation for Net API — это библиотека, позволяющая добавлять аннотации в PDF, Word и другие документы на Mac, Windows или Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) — это собственный Net API для управления аннотациями с комплексной поддержкой создания, добавления, редактирования, удаления, извлечения и экспорта аннотаций из изображений и различных других документов. Полный список поддерживаемых форматов документов вы можете увидеть на этой [странице](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Эта библиотека позволяет работать не только с документом DCM, но и со многими другими типами документов, такими как Word, Excel, PowerPoint, сообщения электронной почты Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad и многими другими.
        GroupDocs.Annotation for Net API позволяет создавать и добавлять новые заметки, редактировать аннотации, извлекать комментарии, аннотации и удалять их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая текст, полилинию, область, подчеркивание, точку, водяной знак, стрелку, эллипс, замену текста, расстояние, текстовое поле, редактирование ресурсов в PDF, HTML, документах Microsoft Word, электронных таблицах, диаграммах, презентациях, чертежи, изображения и многие другие форматы файлов.
        Пример (см. ниже) демонстрирует работу с документом DCM, в этом примере вы можете увидеть основные шаги работы с GroupDocs. аннотацию, добавляя объекты данных для установки свойств аннотации в соответствии с вашими требованиями и сохраняя результат в нужном месте. Также вы можете более подробно ознакомиться с поддерживаемыми функциями на нашей [странице] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) или в [документации] нашего продукта (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Действия по добавлению аннотаций к DCM в сети"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) позволяет сетевым разработчикам легко добавлять различные типы аннотаций к файлам DCM в любом сетевом приложении, выполняя несколько простых шагов.
        *   Создайте объекты ответа с комментарием и датой.
        *   Создайте объект AreaAnnotation, установите параметры области и добавьте ответы.
        *   Создайте объект Annotator и добавьте аннотацию области.
        *   Сохраните выходной файл.
    title_right: "Системные Требования"
    content_right: |
        GroupDocs.Annotation for Net API поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        *   Операционные системы: Microsoft Windows, Linux, MacOS
        *   Среды разработки: Visual Studio, Xamarin, MonoDevelop.
        *   Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        *   Загрузите последнюю версию GroupDocs.Annotation для .NET из [NuGet](https://www.nuget.org/packages/groupdocs.annotation).

############################# Preview ############################
preview_Add:
    enable: true
    title: Предварительный просмотр аннотации и пример кода
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
        using (Annotator annotator = new Annotator("input.bmp"))
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
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Действия по удалению аннотаций из DCM в сети"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) упрощает сетевым разработчикам удаление деталей аннотаций из файлов DCM в любом сетевом приложении путем выполнения нескольких простых шагов.
        *   Создайте объекты ответа с комментарием и датой.
        *   Создайте экземпляр объекта SaveOptions и установите AnnotationTypes = AnnotationType.None.
        *   Вызовите метод сохранения с результирующим путем или потоком документа и объектом SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Действия по редактированию аннотаций из DCM в сети"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) упрощает сетевым разработчикам обновление различных свойств аннотаций из файлов DCM в любом сетевом приложении за счет выполнения нескольких простых шагов.
        *   Создайте экземпляр объекта Annotator с путем или потоком входного документа с созданным экземпляром LoadOptions с ImportAnnotations = true.
        *   Создайте некоторую реализацию AnnotationBase и установите идентификатор существующей аннотации (если аннотация с этим идентификатором не найдена, ничего не изменится) или список путей аннотаций (все существующие аннотации будут удалены).
        *   Вызвать метод обновления объекта Annotator с переданными аннотациями.
        *   Вызовите метод сохранения с результирующим путем или потоком документа и объектом SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```cs
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
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
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Действия по извлечению аннотаций из DCM в сети"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) позволяет сетевым разработчикам легко аннотировать документы и извлекать аннотационную информацию из DCM файлов в любом сетевом приложении, выполняя несколько простых шагов.
        *   Создайте объекты ответа с комментарием и датой.
        *   Создайте экземпляр объекта LoadOptions и вызовите SetImportAnnotations с аргументом true.
        *   Определите переменную с типом List.
        *   Вызовите метод get и верните результат в переменную выше.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```cs
        // for using this example input file ("annotated.bmp") must be with annotations
        using (Annotator annotator = new Annotator("annotated.bmp"))
        {
            List annotations = annotator.Get();
            XmlSerializer formatter = new XmlSerializer(typeof(List));
            using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
                fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Живые демонстрации для добавления, удаления, редактирования, извлечения аннотаций к документам и изображениям"
    content: |
        Добавляйте, удаляйте, редактируйте и извлекайте аннотации к файлу DCM прямо сейчас, посетив веб-сайт [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dcm"
          title: "О формате файла DCM"
          content: |
            Файлы с расширением .DCM представляют собой цифровые изображения, в которых хранится медицинская информация о пациентах, такая как МРТ, компьютерная томография и ультразвуковые изображения. Он был разработан Национальной ассоциацией производителей электрооборудования (NEMA) и предназначался для стандартизации формата файлов изображений для распространения и просмотра медицинских изображений. Он похож на формат файла DICOM и может включать информацию о пациенте для справки.

          link: "https://docs.fileformat.com/image/dcm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Работа с другими популярными форматами документов"
    content: |
        Обновите свойства аннотаций из некоторых популярных форматов файлов, как указано ниже.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/net/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/net/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/net/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/net/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/net/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/net/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/net/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/net/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/net/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/net/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/net/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/net/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/net/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/net/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/net/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/net/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/net/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/net/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/net/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/net/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/net/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/net/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/net/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/net/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/net/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/net/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/net/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/net/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/net/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/net/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/net/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/net/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/net/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/net/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/net/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---