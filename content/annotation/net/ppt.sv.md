---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net PPT Annotation API Annotate i C#"
head_description: "Net API för att skapa och kommentera populära anteckningstyper från PPT, bilder, ritningar och dokumentfilformat."

############################# Header ############################
title: "Annotera PPT från Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ladda ner gratis provversion"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API är ett bibliotek som låter dig lägga till kommentarer till PDF, Word och andra dokument på Mac, Windows eller Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) är ett inbyggt Net API för att hantera kommentarer med omfattande stöd för att skapa, lägga till, redigera, ta bort, extrahera och exportera kommentarer från bilder och olika andra dokument. Den fullständiga listan över dokumentformat som stöds kan du se på denna [sida](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Detta bibliotek låter dig arbeta inte bara med PPT dokument utan också med många andra typer av dokument som Word, Excel, PowerPoint, Outlook e-post, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad och många andra.
        GroupDocs.Annotation for Net API låter dig skapa och lägga till nya anteckningar, redigera kommentarer, extrahera kommentarer, anteckningar och ta bort dem från dokument. Biblioteket stöder 13 olika anteckningstyper, inklusive text, polylinje, område, understrykning, punkt, vattenstämpel, pil, ellips, textersättning, avstånd, textfält, resursredigering i PDF, HTML, Microsoft Word-dokument, kalkylblad, diagram, presentationer, ritningar, bilder och många andra filformat.
        Exemplet (se nedan) visar hur du arbetar med PPT-dokument, i det här exemplet kan du se huvudstegen för hur du arbetar med GroupDocs. Annotation: Konfigurera en licens, öppna ett dokument du vill arbeta med, skapa en annotering, lägga till dataobjekt för att ställa in anteckningsegenskaper enligt dina krav och spara resultatet på önskad plats. Du kan också titta mer detaljerat på de funktioner som stöds på vår github [sida](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), eller i vår produkt [dokumentation](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Steg för att lägga till kommentarer till PPT i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gör det enkelt för Net-utvecklare att lägga till olika anteckningstyper till PPT-filer inom alla nätbaserade program genom att implementera några enkla steg.
        *   Skapa svarsobjekt med kommentar och datum.
        *   Skapa AreaAnnotation-objekt, ställ in områdesalternativ och lägg till svar.
        *   Skapa Annotator-objekt och lägg till områdesanteckning.
        *   Spara utdatafil.
    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Annotation for Net API:er stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.
        *   Operativsystem: Microsoft Windows, Linux, MacOS
        *   Utvecklingsmiljöer: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Ladda ner den senaste versionen av GroupDocs.Annotation för .NET från [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Förhandsgranskning av anteckningar och kodexempel
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
    title_left: "Steg för att ta bort anteckningar från PPT i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gör det enklare för Net-utvecklare att ta bort anteckningsdetaljer från PPT-filer i valfri nätbaserad applikation genom att implementera några enkla steg.
        *   Skapa svarsobjekt med kommentar och datum.
        *   Instantiera SaveOptions-objektet och ställ in AnnotationTypes = AnnotationType.None.
        *   Anropa sparmetoden med resulterande dokumentsökväg eller ström och SaveOptions-objekt.

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
    title_left: "Steg för att redigera kommentarer från PPT i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gör det enklare för Net-utvecklare att uppdatera olika annoteringsegenskaper från PPT-filer i alla nätbaserade program genom att implementera några enkla steg.
        *   Instantiera Annotator-objekt med indatadokumentsökväg eller -ström med instansierade LoadOptions med ImportAnnotations = true.
        *   Skapa en AnnotationBase-implementering och ange Id för existerande anteckning (om anteckning med det Id inte hittas, kommer ingenting att ändras) eller sökvägslista med anteckningar (alla existerande anteckningar kommer att tas bort).
        *   Anrop uppdateringsmetod för Annotator-objekt med godkända anteckningar.
        *   Anropa sparmetoden med resulterande dokumentsökväg eller ström och SaveOptions-objekt.

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
    title_left: "Steg för att extrahera kommentarer från PPT i Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gör det enkelt för Net-utvecklare att kommentera dokument och extrahera anteckningsinformation från PPT-filer i alla Net-baserade applikationer genom att implementera några enkla steg.
        *   Skapa svarsobjekt med kommentar och datum.
        *   Instantiera LoadOptions-objektet och anrop SetImportAnnotations med sant argument.
        *   Definiera variabel med typen List.
        *   Anrop get-metoden och returnera resultatet till variabeln ovan.

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
    title: "Live-demos att lägga till, ta bort, redigera, extrahera kommentarer till dokument och bilder"
    content: |
        Lägg till, ta bort, redigera och extrahera kommentarer till filen PPT just nu genom att besöka webbplatsen [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Livedemon har följande fördelar

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppt"
          title: "Om filformatet PPT"
          content: |
            En fil med PPT-tillägg representerar en PowerPoint-fil som består av en samling bilder för visning som SlideShow. Den anger det binära filformatet som används av Microsoft PowerPoint 97-2003. En PPT-fil kan innehålla flera olika typer av information som text, punktpunkter, bilder, multimedia och andra inbäddade OLE-objekt. Microsoft kom med nyare filformat för PowerPoint, känt som PPTX, från 2007 och framåt som är baserat på Office OpenXML och skiljer sig från detta binära filformat. Flera andra applikationsprogram som OpenOffice Impress och Apple Keynote kan också skapa PPT-filer.

          link: "https://docs.fileformat.com/image/ppt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbeta med andra populära dokumentformat"
    content: |
        Uppdatera annoteringsegenskaper från några av de populära filformaten enligt nedan.
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