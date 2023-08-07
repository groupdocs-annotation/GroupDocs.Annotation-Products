---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Nett PPSX Annotation API Annotate i C#"
head_description: "Net API for å lage og kommentere populære merknadstyper fra PPSX, bilder, tegninger og dokumentfilformater."

############################# Header ############################
title: "Merk PPSX fra Nett"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Last ned gratis prøveversjon"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API er et bibliotek som lar deg legge til merknader til PDF, Word og andre dokumenter på Mac, Windows eller Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) er en innebygd Net API for å administrere merknader med omfattende støtte for å lage, legge til, redigere, slette, trekke ut og eksportere merknader fra bilder og diverse andre dokumenter. Den fullstendige listen over støttede dokumentformater kan du se på denne [siden](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Dette biblioteket lar deg jobbe ikke bare med PPSX-dokumenter, men også med mange andre typer dokumenter som Word, Excel, PowerPoint, Outlook-e-post, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad og mange andre.
        GroupDocs.Annotation for Net API lar deg opprette og legge til nye notater, redigere merknader, trekke ut kommentarer, merknader og fjerne dem fra dokumenter. Biblioteket støtter 13 forskjellige merknadstyper, inkludert tekst, polylinje, område, understreking, punkt, vannmerke, pil, ellipse, teksterstatning, avstand, tekstfelt, ressursredaksjon i PDF, HTML, Microsoft Word-dokumenter, regneark, diagrammer, presentasjoner, tegninger, bilder og mange andre filformater.
        Eksemplet (se nedenfor) viser hvordan du arbeider med PPSX-dokumentet. I dette eksemplet kan du se hovedtrinnene for hvordan du arbeider med GroupDocs. Merknad: Konfigurer en lisens, åpne et dokument du vil jobbe med, opprette en merknad, legge til dataobjekter for å angi merknadsegenskaper i henhold til dine krav og lagre resultatet på ønsket sted. Du kan også se mer detaljert på de støttede funksjonene på vår github [side](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), eller i vår produkt [dokumentasjon](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Trinn for å legge til merknader til PPSX i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gjør det enkelt for Net-utviklere å legge til ulike merknadstyper til PPSX-filer i en hvilken som helst Net-basert applikasjon ved å implementere noen få enkle trinn.
        *   Lag svarobjekter med kommentar og dato.
        *   Opprett AreaAnnotation-objekt, angi områdealternativer og legg til svar.
        *   Opprett Annotator-objekt og legg til områdeanmerkning.
        *   Lagre utdatafil.
    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Annotation for Net APIer støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.
        *   Operativsystemer: Microsoft Windows, Linux, MacOS
        *   Utviklingsmiljøer: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Last ned den nyeste versjonen av GroupDocs.Annotation for .NET fra [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Forhåndsvisning av merknader og kodeeksempel
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
    title_left: "Trinn for å fjerne merknader fra PPSX i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gjør det enklere for Net-utviklere å fjerne merknadsdetaljer fra PPSX-filer i en hvilken som helst Net-basert applikasjon ved å implementere noen få enkle trinn.
        *   Lag svarobjekter med kommentar og dato.
        *   Instantier SaveOptions-objektet og sett AnnotationTypes = AnnotationType.None.
        *   Anrop lagringsmetode med resulterende dokumentbane eller strøm og SaveOptions-objekt.

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
    title_left: "Trinn for å redigere merknader fra PPSX i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gjør det enklere for Net-utviklere å oppdatere ulike merknadsegenskaper fra PPSX-filer i en hvilken som helst Net-basert applikasjon ved å implementere noen få enkle trinn.
        *   Instantier Annotator-objekt med inndatadokumentbane eller strøm med instansierte LoadOptions med ImportAnnotations = true.
        *   Opprett en AnnotationBase-implementering og sett ID-en til den eksisterende merknaden (hvis merknaden med den ID-en ikke blir funnet, vil ingenting bli endret) eller stiliste med merknader (alle eksisterende merknader vil bli fjernet).
        *   Anrop oppdateringsmetode for Annotator-objekt med beståtte merknader.
        *   Anrop lagringsmetode med resulterende dokumentbane eller strøm og SaveOptions-objekt.

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
    title_left: "Trinn for å trekke ut merknader fra PPSX i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gjør det enkelt for Net-utviklere å kommentere dokumenter og trekke ut merknadsinformasjon fra PPSX-filer i en hvilken som helst Net-basert applikasjon ved å implementere noen få enkle trinn.
        *   Lag svarobjekter med kommentar og dato.
        *   Instantier LoadOptions-objektet og kall SetImportAnnotations med sant argument.
        *   Definer variabel med typen List.
        *   Ring hent-metoden og returner resultatet til variabelen ovenfor.

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
    title: "Live-demoer for å legge til, fjerne, redigere, trekke ut merknader til dokumenter og bilder"
    content: |
        Legg til, fjern, rediger og trekk ut merknader til PPSX-filen akkurat nå ved å gå til nettstedet [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
Live-demoen har følgende fordeler

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppsx"
          title: "Om PPSX filformat"
          content: |
            PPSX, Power Point Slide Show, filen er opprettet ved hjelp av Microsoft PowerPoint 2007 og nyere for Slide Show-formål. Det er en oppdatering til PPS-filformatet som ble støttet av Microsoft PowerPoint 97-2003-versjoner. Når en PPSX-fil deles med en annen bruker og åpnes, starter den som PowerPoint-show i motsetning til PPTX-filen som åpnes i redigerbar modus. Sekvensen for lysbildefremvisningen er den samme som i den originale presentasjonen. Alle lysbildene følger med bildene, lydene og andre innebygde medier følger presentasjonslysbildene til PPSX under lysbildefremvisningen.

          link: "https://docs.fileformat.com/image/ppsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbeide med andre populære dokumentformater"
    content: |
        Oppdater merknadsegenskaper fra noen av de populære filformatene som angitt nedenfor.
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