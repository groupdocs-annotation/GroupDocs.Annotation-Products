---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net PDF Annotation API Annotate i C#"
head_description: "Net API til at oprette og kommentere populære annotationstyper fra PDF, billeder, tegninger og dokumentfilformater."

############################# Header ############################
title: "Anmærk PDF fra Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download gratis prøveversion"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API er et bibliotek, der giver dig mulighed for at tilføje anmærkninger til PDF, Word og andre dokumenter på Mac, Windows eller Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) er en indbygget Net API til håndtering af annoteringer med omfattende understøttelse af oprettelse, tilføjelse, redigering, sletning, udtrækning og eksport af annoteringer fra billeder og forskellige andre dokumenter. Den fulde liste over understøttede dokumentformater kan du se på denne [side](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Dette bibliotek giver dig mulighed for ikke kun at arbejde med PDF-dokumenter, men også med mange andre typer dokumenter, såsom Word, Excel, PowerPoint, Outlook-e-mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad og mange andre.
        GroupDocs.Annotation for Net API giver dig mulighed for at oprette og tilføje nye noter, redigere annoteringer, udtrække kommentarer, anmærkninger og fjerne dem fra dokumenter. Biblioteket understøtter 13 forskellige annotationstyper, inklusive tekst, polylinje, område, understregning, punkt, vandmærke, pil, ellipse, teksterstatning, afstand, tekstfelt, ressourceredaktion i PDF, HTML, Microsoft Word-dokumenter, regneark, diagrammer, præsentationer, tegninger, billeder og mange andre filformater.
        Eksemplet (se nedenfor) demonstrerer arbejdet med PDF-dokumentet, i dette eksempel kan du se hovedtrinene i, hvordan man arbejder med GroupDocs.Annotation: Konfigurer en licens, åbn et dokument, du vil arbejde med, opret en annotering, tilføjelse af dataobjekter for at indstille annoteringsegenskaber i henhold til dine krav og gemme resultatet på det nødvendige sted. Du kan også se mere detaljeret om de understøttede funktioner på vores github [side](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), eller i vores produkt [dokumentation](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Trin til at tilføje annoteringer til PDF i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gør det nemt for Net-udviklere at tilføje forskellige annoteringstyper til PDF-filer i enhver net-baseret applikation ved at implementere nogle få nemme trin.
        *   Opret svarobjekter med kommentar og dato.
        *   Opret AreaAnnotation-objekt, indstil områdeindstillinger og tilføj svar.
        *   Opret annotatorobjekt og tilføj områdeannotering.
        *   Gem outputfil.
    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Annotation for Net API'er understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.
        *   Operativsystemer: Microsoft Windows, Linux, MacOS
        *   Udviklingsmiljøer: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Download den seneste version af GroupDocs.Annotation for .NET fra [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Forhåndsvisning af annotering og kodeeksempel
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
    title_left: "Trin til fjernelse af annoteringer fra PDF i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gør det nemmere for Net-udviklere at fjerne anmærkningsdetaljer fra PDF-filer i enhver Net-baseret applikation ved at implementere nogle få nemme trin.
        *   Opret svarobjekter med kommentar og dato.
        *   Instantiér SaveOptions-objektet og indstil AnnotationTypes = AnnotationType.None.
        *   Kald gemmemetode med resulterende dokumentsti eller strøm og SaveOptions-objekt.

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
    title_left: "Trin til redigering af annoteringer fra PDF i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gør det nemmere for Net-udviklere at opdatere forskellige annoteringsegenskaber fra PDF-filer i enhver Net-baseret applikation ved at implementere nogle få nemme trin.
        *   Instantiér Annotator-objekt med input-dokumentsti eller -strøm med instansierede LoadOptions med ImportAnnotations = true.
        *   Opret en AnnotationBase-implementering og sæt Id for eksisterende annotering (hvis annotering med dette Id ikke findes, vil intet blive ændret) eller stiliste over annoteringer (alle eksisterende annoteringer vil blive fjernet).
        *   Kald opdateringsmetode for annotatorobjekt med beståede annoteringer.
        *   Kald gemmemetode med resulterende dokumentsti eller strøm og SaveOptions-objekt.

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
    title_left: "Trin til at udtrække annoteringer fra PDF i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gør det nemt for Net-udviklere at kommentere dokumenter og udtrække anmærkningsoplysninger fra PDF-filer i enhver Net-baseret applikation ved at implementere nogle få nemme trin.
        *   Opret svarobjekter med kommentar og dato.
        *   Instantiér LoadOptions-objektet og kald SetImportAnnotations med sandt argument.
        *   Definer variabel med typen Liste.
        *   Kald get-metoden og returner resultatet til variabel ovenfor.

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
    title: "Live-demoer til at tilføje, fjerne, redigere, udtrække annoteringer til dokumenter og billeder"
    content: |
        Tilføj, fjern, rediger og udpak annoteringer til filen PDF lige nu ved at besøge webstedet [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Livedemoen har følgende fordele

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pdf"
          title: "Om PDF filformat"
          content: |
            Portable Document Format (PDF) er en type dokument skabt af Adobe tilbage i 1990'erne. Formålet med dette filformat var at indføre en standard for repræsentation af dokumenter og andet referencemateriale i et format, der er uafhængigt af applikationssoftware, hardware samt operativsystem. PDF-filer kan åbnes i Adobe Acrobat Reader/Writer samt i de fleste moderne browsere som Chrome, Safari, Firefox via udvidelser/plug-ins. De fleste af de kommercielt tilgængelige softwarepakker tilbyder også konvertering af deres dokumenter til PDF-filformat uden krav om yderligere softwarekomponent. PDF-filformatet har således fuld kapacitet til at indeholde information som tekst, billeder, hyperlinks, formularfelter, rige medier, digitale signaturer, vedhæftede filer, metadata, geospatiale funktioner og 3D-objekter i det, der kan blive en del af kildedokumentet.

          link: "https://docs.fileformat.com/image/pdf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbejde med andre populære dokumentformater"
    content: |
        Opdater annoteringsegenskaber fra nogle af de populære filformater som angivet nedenfor.
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