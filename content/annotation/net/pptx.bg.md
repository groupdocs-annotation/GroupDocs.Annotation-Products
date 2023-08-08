---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net PPTX Annotation API Annotate в C#"
head_description: "Net API за създаване и анотиране на популярни типове анотации от PPTX, изображения, чертежи и файлови формати на документи."

############################# Header ############################
title: "Анотирайте PPTX от Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Изтеглете безплатна пробна версия"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Относно GroupDocs.Annotation за Net API"
    content: |
        GroupDocs.Annotation for Net API е библиотека, която ви позволява да добавяте анотации към PDF, Word и други документи на Mac, Windows или Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) е собствен Net API за управление на анотации с цялостна поддръжка за създаване, добавяне, редактиране, изтриване, извличане и експортиране на анотации от изображения и различни други документи. Пълният списък на поддържаните формати на документи можете да видите на тази [страница](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Тази библиотека ви позволява да работите не само с документ PPTX, но и с много други типове документи като Word, Excel, PowerPoint, Outlook имейли, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad и много други.
        GroupDocs.Annotation for Net API ви позволява да създавате и добавяте нови бележки, да редактирате анотации, да извличате коментари, анотации и да ги премахвате от документи. Библиотеката поддържа 13 различни типа анотации, включително текст, полилиния, област, подчертаване, точка, воден знак, стрелка, елипса, замяна на текст, разстояние, текстово поле, редакция на ресурси в PDF, HTML, документи на Microsoft Word, електронни таблици, диаграми, презентации, чертежи, изображения и много други файлови формати.
        Примерът (моля, вижте по-долу) демонстрира работа с документ PPTX, в този пример можете да видите основните стъпки за това как да работите с GroupDocs. Анотация: Настройте лиценз, отворете документ, с който искате да работите, създаване на анотация, добавяне на обекти с данни, за да зададете свойства на анотация според вашите изисквания и запазване на резултата на необходимото място. Също така бихте могли да разгледате по-подробно поддържаните функции на нашата [страница] в github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) или в [документацията] на нашия продукт (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Стъпки за добавяне на анотации към PPTX в Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) улеснява Net разработчиците да добавят различни типове анотации към PPTX файлове в рамките на всяко Net-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте обекти за отговор с коментар и дата.
        *   Създайте обект AreaAnnotation, задайте опции за областта и добавете отговори.
        *   Създайте обект Annotator и добавете анотация на областта.
        *   Запазете изходния файл.
    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Annotation for Net API се поддържат на всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.
        *   Операционни системи: Microsoft Windows, Linux, MacOS
        *   Среди за разработка: Visual Studio, Xamarin, MonoDevelop
        *   Рамки: .NET Framework, .NET Standard, .NET Core, Mono
        *   Изтеглете най-новата версия на GroupDocs.Annotation за .NET от [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Визуализация на анотация и примерен код
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
    title_left: "Стъпки за премахване на анотации от PPTX в Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) улеснява разработчиците на Net да премахнат подробности за анотация от PPTX файлове в рамките на всяко Net-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте обекти за отговор с коментар и дата.
        *   Създайте обект SaveOptions и задайте AnnotationTypes = AnnotationType.None.
        *   Извикване на метод за запазване с резултатен път на документ или поток и обект SaveOptions.

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
    title_left: "Стъпки за редактиране на анотации от PPTX в Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) улеснява разработчиците на Net да актуализират различни свойства на анотации от PPTX файлове в рамките на всяко Net-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте екземпляр на обект Annotator с входен път на документа или поток с инстанцирани LoadOptions с ImportAnnotations = true.
        *   Създайте реализация на AnnotationBase и задайте идентификатор на съществуваща анотация (ако анотация с този идентификатор не бъде намерена, нищо няма да бъде променено) или списък с пътеки на анотации (всички съществуващи анотации ще бъдат премахнати).
        *   Извикване на метод за актуализиране на обект Annotator с предадени анотации.
        *   Извикване на метод за запазване с резултатен път на документ или поток и обект SaveOptions.

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
    title_left: "Стъпки за извличане на анотации от PPTX в Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) улеснява разработчиците на Net да анотират документи и да извличат информация за анотации от PPTX файлове в рамките на всяко Net-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте обекти за отговор с коментар и дата.
        *   Създайте обект LoadOptions и извикайте SetImportAnnotations с аргумент true.
        *   Дефинирайте променлива с тип List.
        *   Извикайте метода get и върнете резултата към променливата по-горе.

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
    title: "Демонстрации на живо за добавяне, премахване, редактиране, извличане на анотации към документи и изображения"
    content: |
        Добавяйте, премахвайте, редактирайте и извличайте анотации към файла PPTX точно сега, като посетите уебсайта [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Демото на живо има следните предимства

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pptx"
          title: "Относно файловия формат PPTX"
          content: |
            Файловете с разширение PPTX са презентационни файлове, създадени с популярно приложение Microsoft PowerPoint. За разлика от предишната версия на формата на презентационния файл PPT, който беше двоичен, форматът PPTX се основава на отворения XML презентационен формат на Microsoft PowerPoint. Презентационният файл е колекция от слайдове, където всеки слайд може да съдържа текст, изображения, форматиране, анимации и други медии. Тези слайдове се представят на публиката под формата на слайдшоу с персонализирани настройки за представяне.

          link: "https://docs.fileformat.com/image/pptx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Работа с други популярни формати на документи"
    content: |
        Актуализирайте свойствата на анотацията от някои от популярните файлови формати, както е посочено по-долу.
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