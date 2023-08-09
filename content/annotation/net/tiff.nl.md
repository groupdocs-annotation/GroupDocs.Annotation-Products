---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net TIFF Annotatie-API Annotatie in C#"
head_description: "Net API voor het maken en annoteren van populaire annotatietypen van TIFF, afbeeldingen, tekeningen en documentbestandsindelingen."

############################# Header ############################
title: "Annoteer TIFF van Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download gratis proefversie"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Over GroupDocs.Annotation voor Net API"
    content: |
        GroupDocs.Annotation for Net API is een bibliotheek waarmee u annotaties kunt toevoegen aan PDF, Word en andere documenten op Mac, Windows of Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) is een native Net API voor het beheren van annotaties met uitgebreide ondersteuning voor het maken, toevoegen, bewerken, verwijderen, extraheren en exporteren van annotaties van afbeeldingen en diverse andere documenten. De volledige lijst met ondersteunde documentindelingen die u kunt zien op deze [pagina](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Met deze bibliotheek kunt u niet alleen met TIFF-documenten werken, maar ook met vele andere soorten documenten, zoals Word, Excel, PowerPoint, Outlook-e-mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad en vele anderen.
        Met de GroupDocs.Annotation for Net API kunt u nieuwe notities maken en toevoegen, annotaties bewerken, opmerkingen en annotaties extraheren en ze uit documenten verwijderen. De bibliotheek ondersteunt 13 verschillende annotatietypen, waaronder tekst, polylijn, gebied, onderstreping, punt, watermerk, pijl, ellips, tekstvervanging, afstand, tekstveld, redactie van bronnen in PDF, HTML, Microsoft Word-documenten, spreadsheets, diagrammen, presentaties, tekeningen, afbeeldingen en vele andere bestandsformaten.
        Het voorbeeld (zie hieronder) demonstreert het werken met een TIFF-document, in dit voorbeeld kunt u de belangrijkste stappen zien van het werken met GroupDocs. Annotatie: stel een licentie in, open een document waarmee u wilt werken, maak een annotatie, gegevensobjecten toevoegen om annotatie-eigenschappen in te stellen volgens uw vereisten en het resultaat opslaan op de gewenste plaats. U kunt ook meer details bekijken over de ondersteunde functies op onze [github pagina](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), of in onze product [documentatie](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Stappen om annotaties toe te voegen aan TIFF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maakt het gemakkelijk voor internetontwikkelaars om verschillende annotatietypes toe te voegen aan TIFF-bestanden binnen elke op internet gebaseerde applicatie door een paar eenvoudige stappen te implementeren.
        *   Maak Reply-objecten met commentaar en datum.
        *   Maak een AreaAnnotation-object, stel gebiedsopties in en voeg antwoorden toe.
        *   Maak een Annotator-object en voeg een gebiedsannotatie toe.
        *   Sla uitvoerbestand op.
    title_right: "systeem vereisten"
    content_right: |
        GroupDocs.Annotation for Net API's worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.
        *   Besturingssystemen: Microsoft Windows, Linux, MacOS
        *   Ontwikkelomgevingen: Visual Studio, Xamarin, MonoDevelop
        *   Kaders: .NET Framework, .NET Standaard, .NET Core, Mono
        *   Download de nieuwste versie van GroupDocs.Annotation voor .NET van [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Annotatievoorbeeld en codevoorbeeld
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
    title_left: "Stappen om annotaties te verwijderen uit TIFF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maakt het gemakkelijker voor internetontwikkelaars om annotatiedetails te verwijderen uit TIFF-bestanden binnen elke op internet gebaseerde applicatie door een paar eenvoudige stappen te implementeren.
        *   Maak Reply-objecten met commentaar en datum.
        *   Maak een Instantie van het SaveOptions-object en stel AnnotationTypes = AnnotationType.None in.
        *   Roep de opslagmethode aan met het resulterende documentpad of -stroom en SaveOptions-object.

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
    title_left: "Stappen om annotaties te bewerken van TIFF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maakt het voor internetontwikkelaars gemakkelijker om verschillende annotatie-eigenschappen van TIFF-bestanden binnen elke op internet gebaseerde applicatie bij te werken door een paar eenvoudige stappen te implementeren.
        *   Maak een instantie van het Annotator-object met invoerdocumentpad of -stroom met geïnstantieerde LoadOptions met ImportAnnotations = true.
        *   Maak een AnnotationBase-implementatie en stel de id van de bestaande annotatie in (als de annotatie met die id niet wordt gevonden, wordt er niets gewijzigd) of de padlijst met annotaties (alle bestaande annotaties worden verwijderd).
        *   Roep de updatemethode van het Annotator-object aan met doorgegeven annotaties.
        *   Roep de opslagmethode aan met het resulterende documentpad of -stroom en SaveOptions-object.

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
    title_left: "Stappen om annotaties te extraheren uit TIFF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maakt het gemakkelijk voor internetontwikkelaars om documenten te annoteren en annotatie-informatie te extraheren uit TIFF-bestanden binnen elke op internet gebaseerde applicatie door een paar eenvoudige stappen te implementeren.
        *   Maak Reply-objecten met commentaar en datum.
        *   Maak een Instantie van het LoadOptions-object en roep SetImportAnnotations aan met het argument True.
        *   Definieer variabele met type Lijst.
        *   Roep de get-methode aan en retourneer het resultaat naar de bovenstaande variabele.

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
    title: "Live demo's om annotaties aan documenten en afbeeldingen toe te voegen, te verwijderen, te bewerken en te extraheren"
    content: |
        Voeg nu annotaties toe aan, verwijder, bewerk en extraheer annotaties naar het bestand TIFF door naar de website [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) te gaan. De live demo heeft de volgende voordelen

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-tiff"
          title: "Over TIFF bestandsindeling"
          content: |
            TIFF of TIF, Tagged Image File Format, vertegenwoordigt rasterafbeeldingen die bedoeld zijn voor gebruik op verschillende apparaten die voldoen aan deze standaard voor bestandsindelingen. Het is in staat bilevel-, grijswaarden-, paletkleur- en full-color afbeeldingsgegevens in verschillende kleurruimten te beschrijven. Het ondersteunt zowel lossy als lossless compressieschema's om te kiezen tussen ruimte en tijd voor toepassingen die het formaat gebruiken. Het formaat is uitbreidbaar en heeft verschillende herzieningen ondergaan waardoor een onbeperkte hoeveelheid privé- of speciale informatie kan worden opgenomen. Het formaat is niet machine-afhankelijk en is vrij van grenzen zoals processor, besturingssysteem of bestandssystemen.

          link: "https://docs.fileformat.com/image/tiff/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Werken met andere populaire documentindelingen"
    content: |
        Werk annotatie-eigenschappen bij van enkele van de populaire bestandsindelingen, zoals hieronder vermeld.
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