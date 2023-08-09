---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net MSG Annotation API Annotate v C#"
head_description: "Net API za ustvarjanje in označevanje priljubljenih vrst opomb iz MSG, slik, risb in formatov dokumentov."

############################# Header ############################
title: "Opomba MSG iz Neta"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Prenesite brezplačno preskusno različico"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API je knjižnica, ki vam omogoča dodajanje opomb v dokumente PDF, Word in druge dokumente v sistemu Mac, Windows ali Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) je izvorni Net API za upravljanje opomb s celovito podporo za ustvarjanje, dodajanje, urejanje, brisanje, ekstrahiranje in izvažanje opomb iz slik in različnih drugih dokumentov. Celoten seznam podprtih formatov dokumentov si lahko ogledate na tej [strani](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ta knjižnica vam omogoča delo ne samo z dokumentom MSG, ampak tudi z mnogimi drugimi vrstami dokumentov, kot so Word, Excel, PowerPoint, Outlookova e-pošta, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad in mnogi drugi.
        GroupDocs.Annotation for Net API vam omogoča ustvarjanje in dodajanje novih opomb, urejanje opomb, ekstrahiranje komentarjev, opomb in njihovo odstranjevanje iz dokumentov. Knjižnica podpira 13 različnih vrst opomb, vključno z besedilom, poličrtijo, območjem, podčrtajem, točko, vodnim žigom, puščico, elipso, zamenjavo besedila, razdaljo, besedilnim poljem, redakcijo virov v dokumentih PDF, HTML, Microsoft Word, preglednicah, diagramih, predstavitvah, risbe, slike in številne druge oblike datotek.
        Primer (glejte spodaj) prikazuje delo z dokumentom MSG, v tem primeru si lahko ogledate glavne korake dela z GroupDocs. Opomba: nastavite licenco, odprite dokument, s katerim želite delati, ustvarite opombo, dodajanje podatkovnih objektov za nastavitev lastnosti opombe glede na vaše zahteve in shranjevanje rezultata na potrebno mesto. Prav tako si lahko podrobneje ogledate podprte funkcije na naši [strani github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) ali v [dokumentaciji](https://docs.groupdocs.com/annotation/net/getting-started/) našega izdelka.

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Koraki za dodajanje opomb v MSG v Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net razvijalcem olajša dodajanje različnih vrst opomb datotekam MSG znotraj katere koli Net temelječe aplikacije z implementacijo nekaj preprostih korakov.
        *   Ustvarite objekte odgovora s komentarjem in datumom.
        *   Ustvarite predmet AreaAnnotation, nastavite možnosti območja in dodajte odgovore.
        *   Ustvarite objekt Annotator in dodajte opombo območja.
        *   Shrani izhodno datoteko.
    title_right: "Sistemske zahteve"
    content_right: |
        API-ji GroupDocs.Annotation za Net so podprti na vseh glavnih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.
        *   Operacijski sistemi: Microsoft Windows, Linux, MacOS
        *   Razvojna okolja: Visual Studio, Xamarin, MonoDevelop
        *   Ogrodja: .NET Framework, .NET Standard, .NET Core, Mono
        *   Prenesite najnovejšo različico GroupDocs.Annotation za .NET iz [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Predogled pripisov in vzorec kode
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
    title_left: "Koraki za odstranitev opomb iz MSG v Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) omogoča razvijalcem Neta lažje odstranjevanje podrobnosti opomb iz datotek MSG v kateri koli aplikaciji, ki temelji na Netu, z implementacijo nekaj preprostih korakov.
        *   Ustvarite objekte odgovora s komentarjem in datumom.
        *   Instanciirajte objekt SaveOptions in nastavite AnnotationTypes = AnnotationType.None.
        *   Pokličite metodo shranjevanja z nastalo potjo dokumenta ali tokom in objektom SaveOptions.

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
    title_left: "Koraki za urejanje opomb iz MSG v Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) razvijalcem Neta olajša posodabljanje različnih lastnosti opomb iz datotek MSG znotraj katere koli aplikacije, ki temelji na Netu, z implementacijo nekaj preprostih korakov.
        *   Instanciirajte objekt Annotator s potjo vhodnega dokumenta ali tok z instanciranimi LoadOptions z ImportAnnotations = true.
        *   Ustvarite implementacijo AnnotationBase in nastavite ID obstoječe opombe (če opomba s tem ID-jem ni najdena, ne bo nič spremenjeno) ali seznam poti opomb (vse obstoječe opombe bodo odstranjene).
        *   Pokličite metodo posodobitve objekta Annotator s posredovanimi opombami.
        *   Pokličite metodo shranjevanja z nastalo potjo dokumenta ali tokom in objektom SaveOptions.

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
    title_left: "Koraki za ekstrahiranje opomb iz MSG v Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net razvijalcem olajša dodajanje opomb dokumentom in pridobivanje informacij o opombah iz datotek MSG znotraj katere koli aplikacije, ki temelji na Netu, z implementacijo nekaj preprostih korakov.
        *   Ustvarite objekte odgovora s komentarjem in datumom.
        *   Instanciirajte objekt LoadOptions in pokličite SetImportAnnotations z argumentom true.
        *   Definirajte spremenljivko s tipom List.
        *   Pokličite metodo get in vrnite rezultat zgornji spremenljivki.

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
    title: "Predstavitve v živo za dodajanje, odstranjevanje, urejanje, ekstrahiranje opomb v dokumente in slike"
    content: |
        Takoj dodajte, odstranite, uredite in izvlecite opombe v datoteko MSG tako, da obiščete spletno mesto [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Predstavitev v živo ima naslednje prednosti

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-msg"
          title: "O formatu datoteke MSG"
          content: |
            MSG je oblika datoteke, ki jo uporabljata Microsoft Outlook in Exchange za shranjevanje e-poštnih sporočil, stikov, sestankov ali drugih opravil. Takšna sporočila lahko vsebujejo eno ali več e-poštnih polj s pošiljateljem, prejemnikom, zadevo, datumom in telesom sporočila ali kontaktnimi podatki, podrobnostmi o sestanku in eno ali več specifikacijami opravil. Lastnosti, ki sestavljajo predmet sporočila, so tudi del datoteke MSG. Datoteka MSG ima glave, glavno telo sporočila in hiperpovezave kot navadno besedilo ASCII. Datoteke MSG so primerne tudi s programi, ki potrebujejo Microsoftov vmesnik za programiranje sporočilnih aplikacij (MAPI).

          link: "https://docs.fileformat.com/image/msg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Delo z drugimi priljubljenimi formati dokumentov"
    content: |
        Posodobite lastnosti pripisov iz nekaterih priljubljenih formatov datotek, kot je navedeno spodaj.
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