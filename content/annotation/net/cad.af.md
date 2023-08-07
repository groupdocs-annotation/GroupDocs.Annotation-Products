---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net CAD Annotation API Annotate in C#"
head_description: "Net API om gewilde annotasietipes van CAD, beelde, tekeninge en dokumentlêerformate te skep en te annoteer."

############################# Header ############################
title: "Annoteer CAD vanaf Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Laai gratis proeflopie af"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Oor GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API is 'n biblioteek wat jou toelaat om aantekeninge by PDF, Word en ander dokumente op Mac, Windows of Ubuntu te voeg. [GroupDocs.Annotation for Net](/annotation/net) is 'n inheemse Net API vir die bestuur van aantekeninge met omvattende ondersteuning vir die skep, byvoeging, redigeer, uitvee, onttrek en uitvoer van aantekeninge van beelde en verskeie ander dokumente. Die volledige lys van ondersteunde dokumentformate wat jy op hierdie [bladsy] kan sien (https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Hierdie biblioteek laat jou toe om nie net met CAD dokument te werk nie, maar ook met baie ander tipe dokumente soos Word, Excel, PowerPoint, Outlook-e-posse, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad en vele ander.
        Die GroupDocs.Annotation for Net API laat jou toe om nuwe notas te skep en by te voeg, aantekeninge te wysig, opmerkings, annotasies te onttrek en dit uit dokumente te verwyder. Die biblioteek ondersteun 13 verskillende aantekeningtipes, insluitend teks, polilyn, area, onderstreep, punt, watermerk, pyl, ellips, teksvervanging, afstand, teksveld, hulpbronredaksie in PDF, HTML, Microsoft Word-dokumente, sigblaaie, diagramme, aanbiedings, tekeninge, beelde en baie ander lêerformate.
        Die voorbeeld (sien asseblief hieronder) demonstreer werk met CAD dokument, in hierdie voorbeeld kan jy die hoofstappe sien van hoe om met GroupDocs te werk. Aantekening: Stel 'n lisensie op, maak 'n dokument oop waarmee jy wil werk, skep 'n annotasie, byvoeging van data-objekte om annotasie-eienskappe volgens u vereistes te stel en die resultaat op die nodige plek te stoor. Jy kan ook meer gedetailleerd kyk na die ondersteunde kenmerke op ons github [bladsy](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), of in ons produk [dokumentasie](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Stappe om aantekeninge by CAD in Net te voeg"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maak dit maklik vir Net-ontwikkelaars om verskeie aantekeningtipes by CAD-lêers binne enige Net-gebaseerde toepassing by te voeg deur 'n paar maklike stappe te implementeer.
        *   Skep Antwoord-objekte met kommentaar en datum.
        *   Skep AreaAnnotation-objek, stel area-opsies in en voeg antwoorde by.
        *   Skep Annotator-objek en voeg area-aantekening by.
        *   Stoor uitvoerlêer.
    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Annotation for Net API's word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.
        *   Bedryfstelsels: Microsoft Windows, Linux, MacOS
        *   Ontwikkelingsomgewings: Visual Studio, Xamarin, MonoDevelop
        *   Raamwerke: .NET Framework, .NET Standard, .NET Core, Mono
        *   Laai die nuutste weergawe van GroupDocs.Annotation vir .NET af van [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Aantekeningvoorskou en kodevoorbeeld
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
    title_left: "Stappe om aantekeninge van CAD in Net te verwyder"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maak dit makliker vir Net-ontwikkelaars om aantekeningbesonderhede van CAD-lêers binne enige Net-gebaseerde toepassing te verwyder deur 'n paar maklike stappe te implementeer.
        *   Skep Antwoord-objekte met kommentaar en datum.
        *   Instantieer SaveOptions-objek en stel AnnotationTypes = AnnotationType.None.
        *   Oproep stoor metode met gevolglike dokument pad of stroom en SaveOptions voorwerp.

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
    title_left: "Stappe om aantekeninge van CAD in Net te wysig"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maak dit makliker vir Net-ontwikkelaars om verskeie annotasie-eienskappe vanaf CAD-lêers binne enige Net-gebaseerde toepassing op te dateer deur 'n paar maklike stappe te implementeer.
        *   Instansieer Annotator-objek met invoerdokumentpad of stroom met geïnstantieerde LoadOptions met ImportAnnotations = true.
        *   Skep 'n paar AnnotationBase-implementering en stel Id van bestaande aantekening (indien aantekening met daardie Id nie gevind word nie, sal niks verander word nie) of padlys van aantekeninge (alle bestaande aantekeninge sal verwyder word).
        *   Roep opdateringsmetode van Annotator-voorwerp met geslaagde aantekeninge op.
        *   Oproep stoor metode met gevolglike dokument pad of stroom en SaveOptions voorwerp.

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
    title_left: "Stappe om aantekeninge uit CAD in Net te onttrek"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) maak dit maklik vir Net-ontwikkelaars om dokumente te annoteer en annotasie-inligting uit CAD-lêers binne enige Net-gebaseerde toepassing te onttrek deur 'n paar maklike stappe te implementeer.
        *   Skep Antwoord-objekte met kommentaar en datum.
        *   Instansieer LoadOptions-voorwerp en noem SetImportAnnotations met ware argument.
        *   Definieer veranderlike met tipe Lys.
        *   Roep kry metode en gee resultaat terug na veranderlike hierbo.

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
    title: "Regstreekse demonstrasies om by te voeg, te verwyder, te wysig, aantekeninge by dokumente en prente te onttrek"
    content: |
        Voeg, verwyder, redigeer en onttrek aantekeninge by CAD-lêer op die oomblik deur [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) webwerf te besoek. Die lewendige demo het die volgende voordele

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-cad"
          title: "Oor CAD Lêerformaat"
          content: |
            CAD staan ​​vir Computer Aided Design. Die term CADD (vir Computer Aided Design and Drafting) word ook gebruik. Dit word gebruik vir 'n 3D-grafiese lêerformaat en kan 2D- of 3D-ontwerpe bevat. CAD-lêer is 'n digitale lêerformaat van 'n voorwerp wat deur CAD-sagteware gegenereer en gebruik word. 'n CAD-lêer bevat 'n tegniese tekening, bloudruk, skematiese of 3D-weergawe van 'n voorwerp. Daar kan ander CAD-instrumente wees wat gebruik kan word om hierdie .cad-lêers te skep, oop te maak, te redigeer en uit te voer na meer algemeen gebruikte CAD-tekenlêerformate.

          link: "https://docs.fileformat.com/image/cad/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Werk met ander gewilde dokumentformate"
    content: |
        Dateer annotasie-eienskappe op vanaf sommige van die gewilde lêerformate soos hieronder vermeld.
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