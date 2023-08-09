---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Нето POTX Annotation API Annotate во C#"
head_description: "Net API за создавање и забележување популарни типови прибелешки од POTX, слики, цртежи и формати на датотеки на документи."

############################# Header ############################
title: "Забелешка POTX од Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Преземете бесплатен пробен период"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "За GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation за Net API е библиотека која ви овозможува да додавате прибелешки во PDF, Word и други документи на Mac, Windows или Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) е мајчин Net API за управување со прибелешки со сеопфатна поддршка за создавање, додавање, уредување, бришење, извлекување и извоз на прибелешки од слики и разни други документи. Целосната листа на поддржани формати на документи што може да ги видите на оваа [страница](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Оваа библиотека ви овозможува да работите не само со документи POTX туку и со многу други видови документи како што се Word, Excel, PowerPoint, Outlook е-пошта, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad и многу други.
        АПИ на GroupDocs.Annotation за Net ви овозможува да креирате и додавате нови белешки, да уредувате прибелешки, да извлекувате коментари, прибелешки и да ги отстранувате од документите. Библиотеката поддржува 13 различни типови на прибелешки, вклучувајќи текст, полилинија, област, подвлечен, точка, воден печат, стрелка, елипса, замена на текст, растојание, поле за текст, редакција на ресурси во PDF, HTML, Microsoft Word документи, табеларни пресметки, дијаграми, презентации, цртежи, слики и многу други формати на датотеки.
        Примерот (видете подолу) покажува работа со документот POTX, во овој пример можете да ги видите главните чекори како да работите со GroupDocs. Забелешка: Поставете лиценца, отворете документ со кој сакате да работите, креирајте прибелешка, додавање податочни објекти за поставување на својствата на прибелешка според вашите барања и зачувување на резултатот на потребното место. Исто така, можете подетално да ги погледнете поддржаните функции на нашата [github страница](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) или во нашиот производ [документација](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Чекори за додавање прибелешки на POTX во мрежата"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) им олеснува на развивачите на Net да додаваат различни типови на прибелешки на датотеките POTX во која било апликација базирана на мрежа со спроведување на неколку лесни чекори.
        *   Креирајте објекти за одговор со коментар и датум.
        *   Креирајте објект AreaAnnotation, поставете опции за областа и додајте одговори.
        *   Креирајте објект Annotator и додајте прибелешка за областа.
        *   Зачувајте ја излезната датотека.
    title_right: "Системски барања"
    content_right: |
        GroupDocs.Annotation за Net API се поддржани на сите главни платформи и оперативни системи. Пред да го извршите кодот подолу, проверете дали ги имате инсталирано следните предуслови на вашиот систем.
        *   Оперативни системи: Microsoft Windows, Linux, MacOS
        *   Развојни средини: Visual Studio, Xamarin, MonoDevelop
        *   Рамки: .NET Framework, .NET Standard, .NET Core, Mono
        *   Преземете ја најновата верзија на GroupDocs.Annotation за .NET од [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Преглед на прибелешки и примерок на код
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
    title_left: "Чекори за отстранување на прибелешки од POTX во мрежата"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) им олеснува на развивачите на Net да ги отстранат деталите за прибелешки од датотеките POTX во која било апликација базирана на мрежа со спроведување на неколку лесни чекори.
        *   Креирајте објекти за одговор со коментар и датум.
        *   Инстантирајте го објектот SaveOptions и поставете AnnotationTypes = AnnotationType.None.
        *   Повикајте го методот за зачувување со резултат на патеката или преносот на документот и објектот SaveOptions.

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
    title_left: "Чекори за уредување прибелешки од POTX во Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) им олеснува на развивачите на Net да ажурираат различни својства на прибелешки од датотеките POTX во која било апликација базирана на мрежа со спроведување на неколку лесни чекори.
        *   Instantiate Annotator објект со патека на влезен документ или пренос со инстанцирани LoadOptions со ImportAnnotations = точно.
        *   Направете некоја имплементација на AnnotationBase и поставете ИД на постоечка прибелешка (ако прибелешката со таа ИД не е пронајдена, ништо нема да се смени) или листа на патеки со прибелешки (сите постојни прибелешки ќе бидат отстранети).
        *   Начин на ажурирање повик на објект Annotator со поминати прибелешки.
        *   Повикајте го методот за зачувување со резултат на патеката или преносот на документот и објектот SaveOptions.

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
    title_left: "Чекори за екстракција на прибелешки од POTX во мрежата"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) им олеснува на програмерите на Net да ставаат прибелешки и да извлечат информации за прибелешки од датотеките POTX во која било апликација базирана на мрежа со спроведување на неколку лесни чекори.
        *   Креирајте објекти за одговор со коментар и датум.
        *   Инстантирајте го објектот LoadOptions и повикајте SetImportAnnotations со вистински аргумент.
        *   Дефинирајте ја променливата со тип Листа.
        *   Повикајте го методот за добивање и вратете го резултатот на променливата погоре.

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
    title: "Живи демонстрации за додавање, отстранување, уредување, екстракција на прибелешки на документи и слики"
    content: |
        Додајте, отстранувајте, уредувајте и извлечете прибелешки во датотеката POTX во моментов со посета на веб-локацијата [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Демото во живо ги има следните предности

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-potx"
          title: "За форматот на датотеката POTX"
          content: |
            Датотеките со екстензија .POTX претставуваат презентации на шаблоните на Microsoft PowerPoint што се креирани со Microsoft PowerPoint 2007 и погоре. Овој формат е создаден за да го замени форматот на датотеката POT кој се базира на бинарниот формат на датотека и е поддржан со PowerPoint 97-2003. Генерираните датотеки може да се користат за креирање презентации кои имаат ист распоред и други поставки кои се потребни за да се применат на нови датотеки. Овие поставки може да вклучуваат стилови, позадини, палета на бои, фонтови и стандардни поставки. Таквите датотеки се генерираат со цел да се создадат датотеки со шаблони подготвени за употреба за официјална употреба.

          link: "https://docs.fileformat.com/image/potx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Работа со други популарни формати на документи"
    content: |
        Ажурирајте ги својствата на прибелешките од некои од популарните формати на датотеки како што е наведено подолу.
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