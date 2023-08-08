---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net PPT Annotation API Anotácia v C#"
head_description: "Net API na vytváranie a komentovanie populárnych typov anotácií z PPT, obrázkov, nákresov a formátov súborov dokumentov."

############################# Header ############################
title: "Anotujte PPT zo siete Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Stiahnite si bezplatnú skúšobnú verziu"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API je knižnica, ktorá vám umožňuje pridávať anotácie do PDF, Wordu a iných dokumentov na Mac, Windows alebo Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) je natívne Net API na správu anotácií s komplexnou podporou pre vytváranie, pridávanie, upravovanie, odstraňovanie, extrahovanie a exportovanie anotácií z obrázkov a rôznych iných dokumentov. Úplný zoznam podporovaných formátov dokumentov si môžete pozrieť na tejto [stránke](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Táto knižnica vám umožňuje pracovať nielen s dokumentom PPT, ale aj s mnohými ďalšími typmi dokumentov, ako sú Word, Excel, PowerPoint, Outlook e-maily, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad a mnoho ďalších.
        GroupDocs.Annotation for Net API vám umožňuje vytvárať a pridávať nové poznámky, upravovať anotácie, extrahovať komentáre, anotácie a odstraňovať ich z dokumentov. Knižnica podporuje 13 rôznych typov anotácií vrátane textu, polyline, oblasti, podčiarknutia, bodu, vodoznaku, šípky, elipsy, nahradenia textu, vzdialenosti, textového poľa, úpravy zdrojov v PDF, HTML, dokumentov Microsoft Word, tabuliek, diagramov, prezentácií, kresby, obrázky a mnoho ďalších formátov súborov.
        Príklad (pozri nižšie) ukazuje prácu s dokumentom PPT, v tomto príklade môžete vidieť hlavné kroky, ako pracovať s GroupDocs. Anotácia: Nastavte licenciu, otvorte dokument, s ktorým chcete pracovať, vytvorte anotáciu, pridanie dátových objektov na nastavenie vlastností anotácie podľa vašich požiadaviek a uloženie výsledku na potrebné miesto. Môžete si tiež pozrieť podrobnejšie informácie o podporovaných funkciách na našej [stránke github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) alebo v našom produkte [dokumentácia](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Kroky na pridanie anotácií do súboru PPT v sieti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) uľahčuje vývojárom siete pridávanie rôznych typov anotácií k súborom PPT v akejkoľvek aplikácii založenej na sieti implementáciou niekoľkých jednoduchých krokov.
        *   Vytvorte objekty odpovede s komentárom a dátumom.
        *   Vytvorte objekt AreaAnnotation, nastavte možnosti oblasti a pridajte odpovede.
        *   Vytvorte objekt anotátora a pridajte anotáciu oblasti.
        *   Uložiť výstupný súbor.
    title_right: "Požiadavky na systém"
    content_right: |
        GroupDocs.Annotation for Net API sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.
        *   Operačné systémy: Microsoft Windows, Linux, MacOS
        *   Vývojové prostredia: Visual Studio, Xamarin, MonoDevelop
        *   Rámce: .NET Framework, .NET Standard, .NET Core, Mono
        *   Stiahnite si najnovšiu verziu GroupDocs.Annotation pre .NET z [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Ukážka anotácie a ukážka kódu
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
    title_left: "Kroky na odstránenie anotácií zo súboru PPT v sieti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) uľahčuje vývojárom siete odstraňovanie podrobností anotácií zo súborov PPT v akejkoľvek aplikácii založenej na sieti implementáciou niekoľkých jednoduchých krokov.
        *   Vytvorte objekty odpovede s komentárom a dátumom.
        *   Okamžite vytvorte objekt SaveOptions a nastavte AnnotationTypes = AnnotationType.None.
        *   Zavolajte metódu uloženia s výslednou cestou dokumentu alebo streamom a objektom SaveOptions.

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
    title_left: "Kroky na úpravu anotácií z PPT v sieti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) uľahčuje vývojárom siete aktualizovať rôzne vlastnosti anotácií zo súborov PPT v akejkoľvek aplikácii založenej na sieti implementáciou niekoľkých jednoduchých krokov.
        *   Okamžitý objekt Annotator so vstupnou cestou dokumentu alebo stream s inštanciou LoadOptions s ImportAnnotations = true.
        *   Vytvorte nejakú implementáciu AnnotationBase a nastavte Id existujúcej anotácie (ak sa anotácia s týmto Id nenájde, nič sa nezmení) alebo zoznam ciest anotácií (všetky existujúce anotácie budú odstránené).
        *   Zavolajte metódu aktualizácie objektu Annotator s odovzdanými anotáciami.
        *   Zavolajte metódu uloženia s výslednou cestou dokumentu alebo streamom a objektom SaveOptions.

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
    title_left: "Kroky na extrahovanie anotácií z PPT v sieti"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) umožňuje vývojárom siete anotovať dokumenty a extrahovať informácie o anotáciách zo súborov PPT v rámci ľubovoľnej aplikácie založenej na sieti implementáciou niekoľkých jednoduchých krokov.
        *   Vytvorte objekty odpovede s komentárom a dátumom.
        *   Vytvorte instanciu objektu LoadOptions a zavolajte SetImportAnnotations s argumentom true.
        *   Definujte premennú typom List.
        *   Zavolajte metódu get a vráťte výsledok do premennej vyššie.

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
    title: "Živé ukážky na pridanie, odstránenie, úpravu, extrahovanie anotácií do dokumentov a obrázkov"
    content: |
        Pridávajte, odstraňujte, upravujte a extrahujte anotácie do súboru PPT práve teraz na webovej lokalite [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Živá ukážka má nasledujúce výhody

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppt"
          title: "Informácie o formáte súboru PPT"
          content: |
            Súbor s príponou PPT predstavuje súbor programu PowerPoint, ktorý pozostáva z kolekcie snímok na zobrazenie vo forme prezentácie. Špecifikuje binárny formát súboru, ktorý používa Microsoft PowerPoint 97-2003. Súbor PPT môže obsahovať niekoľko rôznych typov informácií, ako je text, odrážky, obrázky, multimédiá a ďalšie vložené objekty OLE. Microsoft prišiel s novším formátom súborov pre PowerPoint, známym ako PPTX, od roku 2007, ktorý je založený na Office OpenXML a je odlišný od tohto binárneho formátu súboru. Súbory PPT môže vytvárať aj niekoľko ďalších aplikačných programov, ako napríklad OpenOffice Impress a Apple Keynote.

          link: "https://docs.fileformat.com/image/ppt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Práca s inými populárnymi formátmi dokumentov"
    content: |
        Aktualizujte vlastnosti anotácií z niektorých populárnych formátov súborov, ako je uvedené nižšie.
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