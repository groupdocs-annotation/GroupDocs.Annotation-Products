---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net PPSX Annotation API Annotate C#"
head_description: "Net API, lai izveidotu un anotētu populārus anotāciju veidus no PPSX, attēliem, zīmējumiem un dokumentu failu formātiem."

############################# Header ############################
title: "Anotējiet PPSX no tīkla"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Lejupielādēt bezmaksas izmēģinājuma versiju"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Par GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API ir bibliotēka, kas ļauj pievienot anotācijas PDF, Word un citiem dokumentiem operētājsistēmā Mac, Windows vai Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) ir vietēja tīkla API anotāciju pārvaldībai ar visaptverošu atbalstu anotāciju izveidei, pievienošanai, rediģēšanai, dzēšanai, izvilkšanai un eksportēšanai no attēliem un dažādiem citiem dokumentiem. Pilnu atbalstīto dokumentu formātu sarakstu varat skatīt šajā [lapā](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Šī bibliotēka ļauj strādāt ne tikai ar PPSX dokumentu, bet arī ar daudziem cita veida dokumentiem, piemēram, Word, Excel, PowerPoint, Outlook e-pastiem, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad un daudziem citiem.
        GroupDocs.Annotation for Net API ļauj izveidot un pievienot jaunas piezīmes, rediģēt anotācijas, iegūt komentārus, anotācijas un noņemt tos no dokumentiem. Bibliotēka atbalsta 13 dažādus anotāciju veidus, tostarp tekstu, daudzlīniju, apgabalu, pasvītrojumu, punktu, ūdenszīmi, bultiņu, elipsi, teksta aizstāšanu, attālumu, teksta lauku, resursu rediģēšanu PDF, HTML, Microsoft Word dokumentos, izklājlapās, diagrammās, prezentācijās, zīmējumi, attēli un daudzi citi failu formāti.
        Piemērā (lūdzu, skatiet tālāk) ir parādīts darbs ar PPSX dokumentu, šajā piemērā var redzēt galvenās darbības, kā strādāt ar GroupDocs. Anotācija: iestatiet licenci, atveriet dokumentu, ar kuru vēlaties strādāt, izveidojot anotācija, datu objektu pievienošana anotācijas rekvizītu iestatīšanai atbilstoši jūsu prasībām un rezultāta saglabāšana vajadzīgajā vietā. Varat arī skatīt sīkāku informāciju par atbalstītajām funkcijām mūsu github [lapā](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) vai mūsu produkta [dokumentācijā](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Darbības, lai pievienotu anotācijas failam PPSX pakalpojumā Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Tas ļauj Net izstrādātājiem viegli pievienot dažādus anotāciju veidus PPSX failiem jebkurā uz tīklu balstītā lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidojiet atbildes objektus ar komentāru un datumu.
        *   Izveidojiet AreaAnnotation objektu, iestatiet apgabala opcijas un pievienojiet atbildes.
        *   Izveidojiet anotatora objektu un pievienojiet apgabala anotāciju.
        *   Saglabājiet izvades failu.
    title_right: "Sistēmas prasības"
    content_right: |
        GroupDocs.Annotation for Net API tiek atbalstītas visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.
        *   Operētājsistēmas: Microsoft Windows, Linux, MacOS
        *   Izstrādes vides: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Lejupielādējiet jaunāko GroupDocs.Annotation versiju .NET no [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anotācijas priekšskatījums un koda paraugs
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
    title_left: "Darbības, lai noņemtu anotācijas no PPSX pakalpojumā Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Izmantojot dažas vienkāršas darbības, Net izstrādātājiem ir vieglāk noņemt anotāciju informāciju no PPSX failiem jebkurā Net lietojumprogrammā.
        *   Izveidojiet atbildes objektus ar komentāru un datumu.
        *   Izveidojiet objektu SaveOptions un iestatiet AnnotationTypes = AnnotationType.None.
        *   Izsauciet saglabāšanas metodi ar iegūto dokumenta ceļu vai straumi un SaveOptions objektu.

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
    title_left: "Darbības, lai rediģētu anotācijas no PPSX pakalpojumā Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ļauj Net izstrādātājiem vieglāk atjaunināt dažādus anotāciju rekvizītus no PPSX failiem jebkurā Net lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidot Annotatora objektu ar ievades dokumenta ceļu vai straumi ar instantierētām LoadOptions ar ImportAnnotations = true.
        *   Izveidojiet kādu AnnotationBase implementāciju un iestatiet esošās anotācijas ID (ja anotācija ar šo ID nav atrasta, nekas netiks mainīts) vai anotāciju ceļu sarakstu (visas esošās anotācijas tiks noņemtas).
        *   Izsaukt Annotator objekta atjaunināšanas metodi ar nodotām anotācijām.
        *   Izsauciet saglabāšanas metodi ar iegūto dokumenta ceļu vai straumi un SaveOptions objektu.

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
    title_left: "Darbības, lai izvilktu anotācijas no PPSX pakalpojumā Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ļauj Net izstrādātājiem viegli anotēt dokumentus un izvilkt anotāciju informāciju no PPSX failiem jebkurā Net lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidojiet atbildes objektus ar komentāru un datumu.
        *   Izveidojiet LoadOptions objektu un izsauciet SetImportAnnotations ar patiesu argumentu.
        *   Definējiet mainīgo ar tipu Saraksts.
        *   Izsauciet metodi get un atgrieziet rezultātu iepriekš norādītajam mainīgajam.

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
    title: "Tiešraides demonstrācijas, lai pievienotu, noņemtu, rediģētu un izvilktu anotācijas dokumentiem un attēliem"
    content: |
        Pievienojiet, noņemiet, rediģējiet un izvelciet anotācijas failam PPSX tūlīt, apmeklējot vietni [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Tiešraides demonstrācijai ir šādas priekšrocības

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppsx"
          title: "Par PPSX faila formātu"
          content: |
            PPSX, Power Point slaidrāde, fails ir izveidots, izmantojot Microsoft PowerPoint 2007 un jaunāku versiju slaidrādes nolūkos. Tas ir PPS faila formāta atjauninājums, ko atbalstīja Microsoft PowerPoint 97-2003 versijas. Kad PPSX fails tiek koplietots ar citu lietotāju un tiek atvērts, tas tiek sākts kā PowerPoint rādījums atšķirībā no PPTX faila, kas tiek atvērts rediģēšanas režīmā. Slaidrādes secība ir tāda pati kā sākotnējā prezentācijā. Visi slaidi tiek pievienoti attēliem, skaņas un citi iegultie datu nesēji tiek pievienoti prezentācijas slaidiem uz PPSX slaidrādes laikā.

          link: "https://docs.fileformat.com/image/ppsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Darbs ar citiem populāriem dokumentu formātiem"
    content: |
        Atjauniniet anotācijas rekvizītus no dažiem populāriem failu formātiem, kā norādīts tālāk.
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