---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net TIF Annotation API Annotate у C#"
head_description: "Net API для створення та анотування популярних типів анотацій із TIF, зображень, малюнків і форматів файлів документів."

############################# Header ############################
title: "Примітка TIF з мережі"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Завантажте безкоштовну пробну версію"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Про GroupDocs.Annotation для Net API"
    content: |
        GroupDocs.Annotation for Net API — це бібліотека, яка дозволяє додавати анотації до PDF, Word та інших документів на Mac, Windows або Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) — це власний API Net для керування анотаціями з повною підтримкою створення, додавання, редагування, видалення, вилучення й експорту анотацій із зображень та різних інших документів. Повний список підтримуваних форматів документів можна переглянути на цій [сторінці](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ця бібліотека дозволяє вам працювати не лише з документом TIF, а й з багатьма іншими типами документів, такими як Word, Excel, PowerPoint, електронні листи Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad та багато інших.
        GroupDocs.Annotation for Net API дозволяє створювати та додавати нові нотатки, редагувати анотації, отримувати коментарі, анотації та видаляти їх із документів. Бібліотека підтримує 13 різних типів анотацій, зокрема текст, ламана лінія, область, підкреслення, точка, водяний знак, стрілка, еліпс, заміна тексту, відстань, текстове поле, редакція ресурсу в документах PDF, HTML, Microsoft Word, електронних таблицях, діаграмах, презентаціях, малюнки, зображення та багато інших форматів файлів.
        Приклад (див. нижче) демонструє роботу з документом TIF, у цьому прикладі ви можете побачити основні кроки роботи з GroupDocs. Анотація: налаштуйте ліцензію, відкрийте документ, з яким хочете працювати, створіть анотація, додавання об’єктів даних для встановлення властивостей анотації відповідно до ваших вимог і збереження результату в потрібному місці. Також ви можете детальніше ознайомитися з підтримуваними функціями на нашій [сторінці] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) або в [документації] нашого продукту (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Кроки для додавання анотацій до TIF у мережі"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) дозволяє розробникам Net легко додавати різні типи анотацій до файлів TIF у будь-якій програмі на основі Net, реалізувавши кілька простих кроків.
        *   Створення об’єктів відповіді з коментарем і датою.
        *   Створіть об’єкт AreaAnnotation, установіть параметри області та додайте відповіді.
        *   Створіть об’єкт Annotator і додайте анотацію області.
        *   Зберегти вихідний файл.
    title_right: "Системні вимоги"
    content_right: |
        GroupDocs.Annotation for Net API підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.
        *   Операційні системи: Microsoft Windows, Linux, MacOS
        *   Середовища розробки: Visual Studio, Xamarin, MonoDevelop
        *   Фреймворки: .NET Framework, .NET Standard, .NET Core, Mono
        *   Завантажте останню версію GroupDocs.Annotation для .NET із [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Попередній перегляд анотації та приклад коду
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
    title_left: "Кроки для видалення анотацій із TIF у мережі"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) спрощує розробникам Net видаляти деталі анотації з файлів TIF у будь-якій програмі на базі Net, виконавши кілька простих кроків.
        *   Створення об’єктів відповіді з коментарем і датою.
        *   Створіть об’єкт SaveOptions і встановіть AnnotationTypes = AnnotationType.None.
        *   Виклик методу збереження з кінцевим шляхом або потоком документа та об’єктом SaveOptions.

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
    title_left: "Кроки для редагування анотацій із TIF у мережі"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) полегшує розробникам Net оновлення різноманітних властивостей анотацій із файлів TIF у будь-якій програмі на основі Net, реалізувавши кілька простих кроків.
        *   Створення екземпляра об’єкта Annotator із вхідним шляхом документа або потоку з екземпляром LoadOptions із ImportAnnotations = true.
        *   Створіть деяку реалізацію AnnotationBase та встановіть ідентифікатор наявної анотації (якщо анотація з таким ідентифікатором не знайдена, нічого не буде змінено) або список шляхів анотацій (усі існуючі анотації буде видалено).
        *   Виклик методу оновлення об’єкта Annotator із переданими анотаціями.
        *   Виклик методу збереження з кінцевим шляхом або потоком документа та об’єктом SaveOptions.

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
    title_left: "Кроки для вилучення анотацій із TIF у мережі"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) полегшує розробникам Net коментувати документи та видобувати анотаційну інформацію з файлів TIF у будь-якій програмі на базі Net, виконавши кілька простих кроків.
        *   Створення об’єктів відповіді з коментарем і датою.
        *   Створення екземпляра об’єкта LoadOptions і виклику SetImportAnnotations з аргументом true.
        *   Визначте змінну з типом List.
        *   Виклик методу get і повернення результату до змінної вище.

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
    title: "Живі демонстрації для додавання, видалення, редагування та вилучення анотацій до документів і зображень"
    content: |
        Додавайте, видаляйте, редагуйте та витягуйте анотації до файлу TIF прямо зараз, відвідавши веб-сайт [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Жива демонстрація має такі переваги

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-tif"
          title: "Про формат файлу TIF"
          content: |
            TIFF або TIF, Tagged Image File Format, представляє растрові зображення, які призначені для використання на різних пристроях, які відповідають цьому стандарту формату файлів. Він здатний описувати дані дворівневого зображення, відтінків сірого, кольору палітри та повнокольорового зображення в кількох колірних просторах. Він підтримує схеми стиснення як із втратами, так і без втрат, щоб вибрати між простором і часом для програм, які використовують формат. Формат не залежить від машини та не залежить від процесора, операційної системи чи файлових систем.

          link: "https://docs.fileformat.com/image/tif/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Робота з іншими популярними форматами документів"
    content: |
        Оновіть властивості анотації з деяких популярних форматів файлів, як зазначено нижче.
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