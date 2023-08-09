---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net DOTX Annotation API märkused C#-s"
head_description: "Net API populaarsete annotatsioonitüüpide DOTX, piltide, jooniste ja dokumendifailivormingute loomiseks ja märkuste tegemiseks."

############################# Header ############################
title: "Märkige Netist DOTX"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Laadige alla tasuta prooviversioon"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Teave GroupDocs.Annotation kohta Net API jaoks"
    content: |
        GroupDocs.Annotation for Net API on teek, mis võimaldab teil lisada märkusi PDF-i, Wordi ja muudele Maci, Windowsi või Ubuntu dokumentidele. [GroupDocs.Annotation for Net](/annotation/net) on natiivne Net API märkuste haldamiseks, mis toetab igakülgset annotatsioonide loomist, lisamist, redigeerimist, kustutamist, ekstraheerimist ja eksportimist piltidelt ja mitmesugustest muudest dokumentidest. Toetatud dokumendivormingute täielikku loendit näete sellel [lehel](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        See teek võimaldab teil töötada mitte ainult DOTX dokumendiga, vaid ka palju muud tüüpi dokumentidega, nagu Word, Excel, PowerPoint, Outlooki meilid, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ja paljud teised.
        GroupDocs.Annotation for Net API võimaldab teil luua ja lisada uusi märkmeid, redigeerida märkusi, ekstraktida kommentaare, märkusi ja neid dokumentidest eemaldada. Teek toetab 13 erinevat märkuste tüüpi, sealhulgas tekst, rida, ala, allajoon, punkt, vesimärk, nool, ellips, teksti asendamine, kaugus, tekstiväli, ressursi redigeerimine PDF-is, HTML-is, Microsoft Wordi dokumentides, arvutustabelites, diagrammides, esitlustes, joonised, pildid ja paljud muud failivormingud.
        Näide (vt allpool) demonstreerib töötamist dokumendiga DOTX, selles näites näete GroupDocsiga töötamise peamisi samme. Annotatsioon: seadistage litsents, avage dokument, millega soovite töötada, luues annotatsioon, andmeobjektide lisamine annotatsiooni omaduste määramiseks vastavalt teie vajadustele ja tulemuse salvestamine vajalikku kohta. Samuti võite toetatud funktsioonide kohta üksikasjalikumalt tutvuda meie [Githubi lehel](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) või meie toote [dokumentatsioonis](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Toimingud võrgus faili DOTX märkuste lisamiseks"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) teeb võrgu arendajatel lihtsaks lisada erinevaid märkuste tüüpe DOTX failidele mis tahes võrgupõhises rakenduses, rakendades mõnda lihtsat sammu.
        *   Looge vastuseobjektid koos kommentaari ja kuupäevaga.
        *   Looge AreaAnnotation objekt, määrake ala valikud ja lisage vastuseid.
        *   Loo annotaatori objekt ja lisa ala märkus.
        *   Salvestage väljundfail.
    title_right: "Nõuded süsteemile"
    content_right: |
        GroupDocs.Annotation for Net API-sid toetatakse kõigil suurematel platvormidel ja operatsioonisüsteemidel. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.
        *   Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        *   Arenduskeskkonnad: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Laadige alla .NET-i jaoks mõeldud GroupDocs.Annotation uusim versioon saidilt [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Annotatsiooni eelvaade ja koodinäidis
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
    title_left: "Toimingud märkuste eemaldamiseks võrgus failist DOTX"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) muudab Neti arendajatel lihtsamaks annotatsiooni üksikasjade eemaldamise mis tahes võrgupõhises rakenduses olevast failist DOTX, rakendades mõnda lihtsat sammu.
        *   Looge vastuseobjektid koos kommentaari ja kuupäevaga.
        *   Käivitage objekt SaveOptions ja määrake AnnotationTypes = AnnotationType.None.
        *   Helistage salvestamismeetodile tulemuseks oleva dokumendi tee või voo ja SaveOptions objektiga.

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
    title_left: "Toimingud võrgus faili DOTX märkuste muutmiseks"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) muudab võrgu arendajatel lihtsamaks erinevate annotatsioonide atribuutide värskendamise DOTX failidest mis tahes võrgupõhises rakenduses, rakendades mõnda lihtsat sammu.
        *   Eksperimenteerige annotaatori objekt sisenddokumendi tee või vooga koos korduvate LoadOptionsiga koos ImportAnnotations = true.
        *   Looge AnnotationBase'i teostus ja määrake olemasoleva annotatsiooni ID (kui selle ID-ga annotatsiooni ei leitud, ei muudeta midagi) või märkuste teede loend (kõik olemasolevad annotatsioonid eemaldatakse).
        *   Kutsuge läbitud märkustega annotaatori objekti värskendusmeetodit.
        *   Helistage salvestamismeetodile tulemuseks oleva dokumendi tee või voo ja SaveOptions objektiga.

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
    title_left: "Toimingud võrgus olevast failist DOTX märkuste ekstraheerimiseks"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) muudab Neti arendajatel lihtsaks dokumentidele märkuste lisamise ja annotatsiooniteabe ekstraktimise DOTX-failidest mis tahes võrgupõhises rakenduses, rakendades mõnda lihtsat sammu.
        *   Looge vastuseobjektid koos kommentaari ja kuupäevaga.
        *   Esitage objekt LoadOptions ja kutsuge välja SetImportAnnotations tõese argumendiga.
        *   Määratle muutuja tüübiga List.
        *   Kutsuge meetod hankima ja tagastage tulemus ülaltoodud muutujale.

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
    title: "Reaalajas demod dokumentide ja piltide märkuste lisamiseks, eemaldamiseks, redigeerimiseks ja ekstraktimiseks"
    content: |
        Lisage, eemaldage, muutke ja ekstraktige faili DOTX märkusi kohe, külastades veebisaiti [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Reaalajas demol on järgmised eelised

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dotx"
          title: "Teave failivormingu DOTX kohta"
          content: |
            DOTX-laiendiga failid on Microsoft Wordi loodud mallifailid, millel on eelvormindatud sätted edasiste DOCX-failide genereerimiseks. Mallfail luuakse konkreetsete kasutajasätete saamiseks, mida tuleks rakendada järgmistele nende põhjal loodud kärbestele. Need seaded hõlmavad lehe veerisid, ääriseid, päiseid, jalusi ja muid lehe seadeid. Selliseid malle kasutatakse ametlikes dokumentides, nagu ettevõtte kirjaplangid ja standardvormid. DOTX-failivorming võeti kasutusele koos Microsoft Office 2007 väljalaskega, et asendada binaarne DOT-failivorming, kuid seda toetavad ka kõrgemad versioonid. Microsoft Word avab vaikimisi kõik uued dokumendid faili normal.dot alusel. Kui seda muudetakse, on kõigi uute loodud failide tulemuseks samad sätted, mis mallifailis. Microsoft Word 2007-s on DOT-failivorming asendatud Office OpenXML-põhise DOTX-failivorminguga.

          link: "https://docs.fileformat.com/image/dotx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muude populaarsete dokumendivormingutega töötamine"
    content: |
        Värskendage mõne populaarse failivormingu annotatsiooni atribuute, nagu allpool kirjeldatud.
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