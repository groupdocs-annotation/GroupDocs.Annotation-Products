---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net EMLX Anotace API Anotace v C#"
head_description: "Net API pro vytváření a komentování oblíbených typů anotací z EMLX, obrázků, nákresů a formátů souborů dokumentů."

############################# Header ############################
title: "Anotace EMLX ze sítě"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Stáhněte si zkušební verzi zdarma"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API je knihovna, která umožňuje přidávat anotace do PDF, Wordu a dalších dokumentů na Macu, Windows nebo Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) je nativní Net API pro správu anotací s komplexní podporou pro vytváření, přidávání, úpravy, mazání, extrahování a export anotací z obrázků a různých dalších dokumentů. Úplný seznam podporovaných formátů dokumentů můžete vidět na této [stránce](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Tato knihovna vám umožňuje pracovat nejen s dokumentem EMLX, ale také s mnoha dalšími typy dokumentů, jako jsou Word, Excel, PowerPoint, Outlook e-maily, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad a mnoho dalších.
        GroupDocs.Annotation for Net API umožňuje vytvářet a přidávat nové poznámky, upravovat anotace, extrahovat komentáře, anotace a odstraňovat je z dokumentů. Knihovna podporuje 13 různých typů anotací, včetně textu, křivky, plochy, podtržení, bodu, vodoznaku, šipky, elipsy, nahrazení textu, vzdálenosti, textového pole, úpravy zdrojů v PDF, HTML, dokumentů Microsoft Word, tabulek, diagramů, prezentací, výkresy, obrázky a mnoho dalších formátů souborů.
        Příklad (viz níže) ukazuje práci s dokumentem EMLX, v tomto příkladu můžete vidět hlavní kroky, jak pracovat s GroupDocs. Anotace: Nastavte licenci, otevřete dokument, se kterým chcete pracovat, vytvořte anotace, přidání datových objektů pro nastavení vlastností anotace podle vašich požadavků a uložení výsledku na potřebné místo. Také se můžete podrobněji podívat na podporované funkce na naší github [stránce](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), nebo v našem produktu [dokumentace](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Kroky k přidání anotací do EMLX v síti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) usnadňuje vývojářům sítě přidávání různých typů anotací k souborům EMLX v jakékoli aplikaci založené na síti pomocí několika jednoduchých kroků.
        *   Vytvořte objekty odpovědi s komentářem a datem.
        *   Vytvořte objekt AreaAnnotation, nastavte možnosti oblasti a přidejte odpovědi.
        *   Vytvořte objekt Annotator a přidejte popis oblasti.
        *   Uložit výstupní soubor.
    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Annotation for Net API jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.
        *   Operační systémy: Microsoft Windows, Linux, MacOS
        *   Vývojová prostředí: Visual Studio, Xamarin, MonoDevelop
        *   Frameworky: .NET Framework, .NET Standard, .NET Core, Mono
        *   Stáhněte si nejnovější verzi GroupDocs.Annotation pro .NET z [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Náhled anotace a ukázka kódu
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
    title_left: "Kroky k odstranění anotací z EMLX v síti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) usnadňuje vývojářům sítě odstranění podrobností anotací ze souborů EMLX v jakékoli aplikaci založené na síti pomocí několika jednoduchých kroků.
        *   Vytvořte objekty odpovědi s komentářem a datem.
        *   Vytvořte instanci objektu SaveOptions a nastavte AnnotationTypes = AnnotationType.None.
        *   Volejte metodu uložení s výslednou cestou dokumentu nebo streamem a objektem SaveOptions.

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
    title_left: "Kroky k úpravě anotací z EMLX v síti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) usnadňuje vývojářům sítě aktualizaci různých vlastností anotací ze souborů EMLX v jakékoli aplikaci založené na síti implementací několika jednoduchých kroků.
        *   Vytvořte instanci objektu Annotator se vstupní cestou dokumentu nebo streamu s instancí LoadOptions s ImportAnnotations = true.
        *   Vytvořte nějakou implementaci AnnotationBase a nastavte Id existující anotace (pokud anotace s tímto Id nebude nalezena, nic se nezmění) nebo seznam cest anotací (všechny existující anotace budou odstraněny).
        *   Zavolejte metodu aktualizace objektu Annotator s předanými anotacemi.
        *   Volejte metodu uložení s výslednou cestou dokumentu nebo streamem a objektem SaveOptions.

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
    title_left: "Kroky k extrahování anotací z EMLX v síti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) usnadňuje vývojářům sítě anotaci dokumentů a extrahování anotačních informací ze souborů EMLX v jakékoli aplikaci založené na síti pomocí několika jednoduchých kroků.
        *   Vytvořte objekty odpovědi s komentářem a datem.
        *   Vytvořte instanci objektu LoadOptions a zavolejte SetImportAnnotations s argumentem true.
        *   Definujte proměnnou typem List.
        *   Zavolejte metodu get a vraťte výsledek do proměnné výše.

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
    title: "Živé ukázky pro přidání, odebrání, úpravu, extrahování anotací do dokumentů a obrázků"
    content: |
        Přidávejte, odebírejte, upravujte a extrahujte anotace do souboru EMLX právě teď na webu [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Živé demo má následující výhody

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-emlx"
          title: "O formátu souboru EMLX"
          content: |
            Formát souboru EMLX je implementován a vyvinut společností Apple. Aplikace Apple Mail používá pro export e-mailů souborový formát EMLX. Existují i ​​další aplikace, které mohou otevřít soubory EMLX a převést je do jiných formátů souborů.

          link: "https://docs.fileformat.com/image/emlx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Práce s jinými oblíbenými formáty dokumentů"
    content: |
        Aktualizujte vlastnosti anotace z některých oblíbených formátů souborů, jak je uvedeno níže.
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