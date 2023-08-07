---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "C# тіліндегі Net OTT Annotation API Annotate"
head_description: "OTT, кескіндер, сызбалар және құжат файл пішімінен танымал аннотация түрлерін жасауға және аннотациялауға арналған Net API."

############################# Header ############################
title: "Net сайтынан OTT аннотациясын жазыңыз"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Тегін сынақ нұсқасын жүктеп алыңыз"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "GroupDocs туралы. Net API үшін аннотация"
    content: |
        GroupDocs.Annotation for Net API — PDF, Word және Mac, Windows немесе Ubuntu жүйелеріндегі басқа құжаттарға аннотациялар қосуға мүмкіндік беретін кітапхана. [GroupDocs.Annotation for Net](/annotation/net) — кескіндерден және басқа да әртүрлі құжаттардан аннотацияларды жасауға, қосуға, өңдеуге, жоюға, шығарып алуға және экспорттауға жан-жақты қолдау көрсететін аннотацияларды басқаруға арналған жергілікті Net API. Қолдау көрсетілетін құжат пішімдерінің толық тізімін осы [бетте](https://docs.groupdocs.com/annotation/net/supported-document-formats/) көруге болады.
        Бұл кітапхана тек OTT құжатымен ғана емес, Word, Excel, PowerPoint, Outlook электрондық пошталары, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad және т.б. сияқты көптеген құжаттар түрлерімен жұмыс істеуге мүмкіндік береді.
        GroupDocs.Annotation for Net API сізге жаңа ескертпелер жасауға және қосуға, аннотацияларды өңдеуге, түсініктемелерді, аннотацияларды шығарып алуға және оларды құжаттардан жоюға мүмкіндік береді. Кітапхана 13 түрлі аннотация түрлерін қолдайды, соның ішінде мәтін, полисызық, аймақ, астын сызу, нүкте, су таңбасы, көрсеткі, эллипс, мәтінді ауыстыру, қашықтық, мәтін өрісі, PDF, HTML, Microsoft Word құжаттарындағы ресурстарды өңдеу, электрондық кестелер, диаграммалар, презентациялар, сызбалар, кескіндер және басқа да көптеген файл пішімдері.
        Мысал (төменде қараңыз) OTT құжатымен жұмыс істеуді көрсетеді, бұл мысалда GroupDocs бағдарламасымен жұмыс істеудің негізгі қадамдарын көруге болады. Аннотация: Лицензияны орнату, жұмыс істегіңіз келетін құжатты ашу, файл жасау аннотация, талаптарыңызға сәйкес аннотация сипаттарын орнату үшін деректер нысандарын қосу және нәтижені қажетті орынға сақтау. Сондай-ақ қолдау көрсетілетін мүмкіндіктерді github [бет](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) немесе [documentation](https) өнімінен толығырақ қарауға болады. ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Net жүйесінде OTT файлына аннотацияларды қосу қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) желі әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген желіге негізделген қолданбадағы OTT файлдарына әртүрлі аннотация түрлерін қосуды жеңілдетеді.
        *   Түсініктеме мен күні бар Жауап нысандарын жасаңыз.
        *   AreaAnnotation нысанын жасаңыз, аймақ опцияларын орнатыңыз және жауаптарды қосыңыз.
        *   Аннотатор нысанын жасаңыз және аймаққа аннотация қосыңыз.
        *   Шығару файлын сақтаңыз.
    title_right: "Жүйе талаптары"
    content_right: |
        Net API үшін GroupDocs.Аннотацияға барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетіледі. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.
        *   Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        *   Әзірлеу орталары: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   .NET үшін GroupDocs.Annotation бағдарламасының соңғы нұсқасын [NuGet] сайтынан жүктеп алыңыз (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Аннотацияны алдын ала қарау және код үлгісі
    content: |
        ![Annotation preview image]https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png
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
    title_left: "Net жүйесіндегі OTT файлынан аннотацияларды жою қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген желіге негізделген қолданбадағы OTT файлдарынан аннотация мәліметтерін жоюды жеңілдетеді.
        *   Түсініктеме мен күні бар Жауап нысандарын жасаңыз.
        *   SaveOptions нысанын жасаңыз және AnnotationTypes = AnnotationType.None орнатыңыз.
        *   Нәтижелік құжат жолы немесе ағыны және SaveOptions нысаны бар қоңырауды сақтау әдісі.

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
    title_left: "Net жүйесінде OTT аннотацияларын өңдеу қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген желіге негізделген қолданбадағы OTT файлдарының әртүрлі аннотация сипаттарын жаңартуды жеңілдетеді.
        *   Кіріс құжат жолы бар аннотатор нысанын құру немесе ImportAnnotations көмегімен даналық LoadOptions ағыны = шын.
        *   Кейбір AnnotationBase енгізуін жасаңыз және бар аннотацияның идентификаторын орнатыңыз (егер бұл идентификаторы бар аннотация табылмаса, ештеңе өзгертілмейді) немесе аннотациялардың жол тізімін (барлық аннотациялар жойылады).
        *   Өткізілген аннотациялары бар Annotator нысанының қоңырауды жаңарту әдісі.
        *   Нәтижелік құжат жолы немесе ағыны және SaveOptions нысаны бар қоңырауды сақтау әдісі.

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
    title_left: "Net жүйесіндегі OTT файлынан аннотацияларды шығару қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Желілік әзірлеушілерге бірнеше оңай қадамдарды орындау арқылы кез келген желіге негізделген қолданбадағы OTT файлдарынан құжаттарға түсініктеме беруді және аннотация ақпаратын шығаруды жеңілдетеді.
        *   Түсініктеме мен күні бар Жауап нысандарын жасаңыз.
        *   LoadOptions нысанын іске қосыңыз және шынайы аргументпен SetImportAnnotations шақырыңыз.
        *   Тізім түрімен айнымалыны анықтаңыз.
        *   Get әдісіне қоңырау шалыңыз және нәтижені жоғарыдағы айнымалыға қайтарыңыз.

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
    title: "Құжаттар мен кескіндерге аннотацияларды қосу, жою, өңдеу, шығару үшін тікелей көрсетілімдер"
    content: |
        Дәл қазір [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) веб-сайтына кіру арқылы OTT файлына аннотацияларды қосу, жою, өңдеу және шығару.
Тікелей демонстрацияның келесі артықшылықтары бар

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ott"
          title: "OTT Файл пішімі туралы"
          content: |
            OTT кеңейтімі бар файлдар OASIS OpenDocument стандартты пішіміне сәйкес қолданбалармен жасалған үлгілік құжаттарды білдіреді. Олар тегін OpenOffice Writer сияқты мәтіндік процессор қолданбаларымен жасалады және осы үлгі файлдарынан жаңа құжаттарды жасау үшін пайдалануға болатын параметрлерді сақтай алады. Бұл параметрлерге бет жиектері, жиектер, үстіңгі деректемелер, төменгі деректемелер және басқа бет параметрлері кіреді. Мұндай шаблондар компанияның бланкілері мен стандартталған бланкілері сияқты ресми құжаттарда қолданылады.

          link: "https://docs.fileformat.com/image/ott/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Басқа танымал құжат пішімдерімен жұмыс істеу"
    content: |
        Төменде көрсетілгендей кейбір танымал файл пішімдерінің аннотация сипаттарын жаңартыңыз.
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