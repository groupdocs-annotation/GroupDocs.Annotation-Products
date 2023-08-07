---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net XLS Annotation API Annotate u C#"
head_description: "Net API za stvaranje i označavanje popularnih vrsta komentara iz XLS, slika, crteža i formata datoteka dokumenata."

############################# Header ############################
title: "Označite XLS s Neta"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Preuzmite besplatnu probnu verziju"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation za Net API"
    content: |
        GroupDocs.Annotation for Net API je biblioteka koja vam omogućuje dodavanje komentara u PDF, Word i druge dokumente na Macu, Windowsu ili Ubuntuu. [GroupDocs.Annotation for Net](/annotation/net) izvorni je Net API za upravljanje komentarima sa sveobuhvatnom podrškom za stvaranje, dodavanje, uređivanje, brisanje, izdvajanje i izvoz komentara iz slika i raznih drugih dokumenata. Potpuni popis podržanih formata dokumenata možete vidjeti na ovoj [stranici](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ova biblioteka vam omogućuje rad ne samo s dokumentom XLS već i s mnogim drugim vrstama dokumenata kao što su Word, Excel, PowerPoint, Outlook e-pošta, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad i mnogi drugi.
        GroupDocs.Annotation for Net API omogućuje stvaranje i dodavanje novih bilješki, uređivanje komentara, izdvajanje komentara, komentara i njihovo uklanjanje iz dokumenata. Knjižnica podržava 13 različitih vrsta komentara, uključujući tekst, poliliniju, područje, podcrtavanje, točku, vodeni žig, strelicu, elipsu, zamjenu teksta, udaljenost, tekstualno polje, redakciju resursa u PDF-u, HTML-u, Microsoft Word dokumentima, proračunskim tablicama, dijagramima, prezentacijama, crteži, slike i mnogi drugi formati datoteka.
        Primjer (pogledajte dolje) demonstrira rad s XLS dokumentom, u ovom primjeru možete vidjeti glavne korake rada s GroupDocs. Napomena: Postavite licencu, otvorite dokument s kojim želite raditi, kreirajte bilježenje, dodavanje podatkovnih objekata za postavljanje svojstava bilježaka prema vašim zahtjevima i spremanje rezultata na potrebno mjesto. Također možete detaljnije pogledati podržane značajke na našoj github [stranici](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) ili u [dokumentaciji] našeg proizvoda (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Koraci za dodavanje komentara u XLS u Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) olakšava Net programerima dodavanje raznih vrsta komentara XLS datotekama unutar bilo koje Net-bazirane aplikacije implementacijom nekoliko jednostavnih koraka.
        *   Stvorite objekte odgovora s komentarom i datumom.
        *   Stvorite objekt AreaAnnotation, postavite opcije područja i dodajte odgovore.
        *   Stvorite objekt Annotator i dodajte oznaku područja.
        *   Spremi izlaznu datoteku.
    title_right: "Zahtjevi sustava"
    content_right: |
        API-ji GroupDocs.Annotation za Net podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.
        *   Operativni sustavi: Microsoft Windows, Linux, MacOS
        *   Razvojna okruženja: Visual Studio, Xamarin, MonoDevelop
        *   Okviri: .NET Framework, .NET Standard, .NET Core, Mono
        *   Preuzmite najnoviju verziju GroupDocs.Annotation za .NET s [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Pregled komentara i uzorak koda
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
    title_left: "Koraci za uklanjanje komentara iz XLS u Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) olakšava Net programerima uklanjanje detalja komentara iz XLS datoteka unutar bilo koje Net-bazirane aplikacije implementacijom nekoliko jednostavnih koraka.
        *   Stvorite objekte odgovora s komentarom i datumom.
        *   Instancirajte objekt SaveOptions i postavite AnnotationTypes = AnnotationType.None.
        *   Pozovite metodu spremanja s rezultirajućom putanjom dokumenta ili tokom i objektom SaveOptions.

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
    title_left: "Koraci za uređivanje komentara iz XLS u Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) olakšava Net programerima ažuriranje različitih svojstava zabilješki iz XLS datoteka unutar bilo koje Net-bazirane aplikacije implementacijom nekoliko jednostavnih koraka.
        *   Instancirajte Annotator objekt s ulaznom putanjom dokumenta ili tok s instanciranim LoadOptions s ImportAnnotations = true.
        *   Napravite implementaciju AnnotationBase i postavite ID postojeće zabilješke (ako zabilješka s tim ID-om nije pronađena, ništa se neće promijeniti) ili popis puta zabilješki (sve postojeće zabilješke bit će uklonjene).
        *   Pozovite metodu ažuriranja objekta Annotator s proslijeđenim komentarima.
        *   Pozovite metodu spremanja s rezultirajućom putanjom dokumenta ili tokom i objektom SaveOptions.

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
    title_left: "Koraci za izdvajanje komentara iz XLS u Netu"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) olakšava Net programerima da dodaju bilješke dokumentima i izvuku informacije o bilješkama iz XLS datoteka unutar bilo koje aplikacije temeljene na Netu implementacijom nekoliko jednostavnih koraka.
        *   Stvorite objekte odgovora s komentarom i datumom.
        *   Instancirajte objekt LoadOptions i pozovite SetImportAnnotations s argumentom true.
        *   Definirajte varijablu tipom List.
        *   Pozovi metodu get i vrati rezultat gornjoj varijabli.

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
    title: "Demonstracije uživo za dodavanje, uklanjanje, uređivanje, izdvajanje komentara na dokumente i slike"
    content: |
        Dodajte, uklonite, uredite i ekstrahirajte komentare u datoteku XLS odmah tako da posjetite [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) web mjesto. Demo uživo ima sljedeće prednosti

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xls"
          title: "O formatu datoteke XLS"
          content: |
            Datoteke s ekstenzijom XLS predstavljaju Excel binarni format datoteke. Takve datoteke može izraditi Microsoft Excel kao i drugi slični programi za proračunske tablice kao što su OpenOffice Calc ili Apple Numbers. Datoteka koju sprema Excel poznata je kao radna knjiga gdje svaka radna knjiga može imati jedan ili više radnih listova. Podaci se pohranjuju i prikazuju korisnicima u obliku tablice na radnom listu i mogu obuhvatiti numeričke vrijednosti, tekstualne podatke, formule, vanjske podatkovne veze, slike i grafikone. Aplikacije kao što je Microsoft Excel omogućuju izvoz podataka radne knjige u nekoliko različitih formata uključujući PDF, CSV, XLSX, TXT, HTML, XPS i nekoliko drugih. XLS format datoteke zamijenjen je otvorenijim i strukturiranim formatom, XLSX, s izdavanjem Microsoft Excela 2007. Najnovije verzije još uvijek pružaju podršku za stvaranje i čitanje XLS datoteka, iako je XLSX sada prvi izbor za upotrebu.

          link: "https://docs.fileformat.com/image/xls/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Rad s drugim popularnim formatima dokumenata"
    content: |
        Ažurirajte svojstva zabilješki iz nekih od popularnih formata datoteka kao što je navedeno u nastavku.
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