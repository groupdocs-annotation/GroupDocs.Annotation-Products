---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API Anodi net VSX Anodi yn C#"
head_description: "API Net i greu ac Anodi mathau o anodiadau poblogaidd o VSX, delweddau, lluniadau a fformatau ffeil dogfen."

############################# Header ############################
title: "Anodwch VSX o Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Treial Am Ddim"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Ynglŷn â GroupDocs.Annotation ar gyfer API Net"
    content: |
        Mae GroupDocs.Annotation for Net API yn llyfrgell sy'n eich galluogi i ychwanegu anodiadau i PDF, Word a dogfennau eraill ar Mac, Windows neu Ubuntu. Mae [GroupDocs.Annotation for Net] (/anodiad/net) yn API Net brodorol ar gyfer rheoli anodiadau gyda chefnogaeth gynhwysfawr ar gyfer creu, ychwanegu, golygu, dileu, echdynnu ac allforio anodiadau o ddelweddau a dogfennau amrywiol eraill. Y rhestr lawn o fformatau dogfennau â chymorth y gallech eu gweld ar y [dudalen] hon(https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Mae'r llyfrgell hon yn eich galluogi i weithio nid yn unig gyda VSX dogfen ond hefyd gyda llawer o fathau eraill o ddogfennau megis Word, Excel, PowerPoint, e-byst Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad a llawer o rai eraill.
        Mae'r GroupDocs.Annotation for Net API yn eich galluogi i greu ac ychwanegu nodiadau newydd, golygu anodiadau, tynnu sylwadau, anodiadau, a'u tynnu o ddogfennau. Mae'r llyfrgell yn cefnogi 13 o wahanol fathau o anodi, gan gynnwys Testun, Polyline, Arwynebedd, Tanlinellu, Pwynt, Dyfrnod, Saeth, Ellipse, Amnewid Testun, Pellter, Maes Testun, Golygu Adnoddau mewn PDF, HTML, dogfennau Microsoft Word, taenlenni, diagramau, cyflwyniadau, lluniadau, delweddau a llawer o fformatau ffeil eraill.
        Mae'r enghraifft (gweler isod) yn dangos gweithio gyda dogfen VSX, yn yr enghraifft hon gallech weld y prif gamau o sut i weithio gyda GroupDocs.Annotation: Gosod trwydded, agor dogfen rydych am weithio gyda hi, creu a anodi, ychwanegu gwrthrychau data i osod priodweddau anodi yn unol â'ch gofynion ac arbed y canlyniad i'r lle sydd ei angen. Hefyd fe allech chi gael golwg fanylach ar y nodweddion a gefnogir ar ein tudalen github [tudalen] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), neu yn ein cynnyrch [dogfennaeth] (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Camau i Ychwanegu Anodiadau i VSX yn Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) yn ei gwneud hi'n hawdd i ddatblygwyr Net ychwanegu gwahanol fathau o anodiadau i VSX ffeil o fewn unrhyw raglen Net-seiliedig trwy weithredu ychydig o gamau hawdd.
        *   Creu gwrthrychau Ateb gyda sylw a dyddiad.
        *   Creu gwrthrych AreaAnnotation, gosod opsiynau ardal ac ychwanegu atebion.
        *   Creu gwrthrych Annotator ac ychwanegu anodiad ardal.
        *   Arbed ffeil allbwn.
    title_right: "Gofynion y System"
    content_right: |
        Cefnogir GroupDocs.Annotation for Net APIs ar bob prif lwyfan a system weithredu. Cyn gweithredu'r cod isod, gwnewch yn siŵr bod gennych y rhagofynion canlynol wedi'u gosod ar eich system.
        *   Systemau Gweithredu: Microsoft Windows, Linux, MacOS
        *   Amgylcheddau Datblygu: Visual Studio, Xamarin, MonoDevelop
        *   Fframweithiau: .NET Framework, .NET Standard, .NET Core, Mono
        *   Lawrlwythwch y fersiwn diweddaraf o GroupDocs.Annotation ar gyfer .NET o [NuGet]( https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Rhagolwg anodi a sampl cod
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
    title_left: "Camau i Dynnu Anodiadau o VSX yn Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) yn ei gwneud yn haws i ddatblygwyr Net dynnu manylion anodiad o VSX o ffeiliau o fewn unrhyw raglen Net-seiliedig trwy roi ychydig o gamau hawdd ar waith.
        *   Creu gwrthrychau Ateb gyda sylw a dyddiad.
        *   Instantiate SaveOptions object a gosod AnnotationTypes = AnnotationType.None.
        *   Dull arbed galwadau gyda llwybr dogfen canlyniadol neu ffrwd a gwrthrych SaveOptions.

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
    title_left: "Camau i Olygu Anodiadau o VSX yn Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) yn ei gwneud hi'n haws i ddatblygwyr Net ddiweddaru priodweddau anodi amrywiol o VSX ffeil o fewn unrhyw raglen Net-seiliedig trwy roi ychydig o gamau hawdd ar waith.
        *   Instantiate Annotator gwrthrych gyda llwybr dogfen mewnbwn neu ffrwd gyda LoadOptions instantiated gyda ImportAnnotations = gwir.
        *   Creu rhywfaint o weithrediad AnnotationBase a gosod ID o'r anodiadau sy'n bodoli (os na chanfuwyd yr anodiad gyda'r Id hwnnw, ni fydd unrhyw beth yn cael ei newid) neu restr llwybr o anodiadau (bydd yr holl anodiadau sy'n bodoli yn cael eu dileu).
        *   Dull diweddaru galwadau o wrthrych Annotator gydag anodiadau wedi'u pasio.
        *   Dull arbed galwadau gyda llwybr dogfen canlyniadol neu ffrwd a gwrthrych SaveOptions.

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
    title_left: "Camau i Echdynnu Anodiadau o VSX yn Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) yn ei gwneud hi'n hawdd i ddatblygwyr Net anodi dogfennau a thynnu gwybodaeth anodiad o VSX o ffeiliau o fewn unrhyw raglen Net-seiliedig trwy roi ychydig o gamau hawdd ar waith.
        *   Creu gwrthrychau Ateb gyda sylw a dyddiad.
        *   Cychwynnwch wrthrych LoadOptions a ffoniwch SetImportAnnotations gyda dadl wir.
        *   Diffinio newidyn gyda math Rhestr.
        *   Dull cael galwad a dychwelyd y canlyniad i'r newidyn uchod.

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
    title: "Demos Byw i'w Ychwanegu, Tynnu, Golygu, Tynnu Anodiadau i Ddogfennau a Delweddau"
    content: |
        Ychwanegu, dileu, golygu a thynnu anodiadau i ffeil VSX ar hyn o bryd drwy ymweld â gwefan [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Mae gan y demo byw y buddion canlynol

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsx"
          title: "Ynglŷn â VSX Fformat Ffeil"
          content: |
            Mae ffeiliau gydag estyniad .VSX yn cyfeirio at stensiliau sy'n cynnwys lluniadau a siapiau a ddefnyddir i greu diagramau yn Microsoft Visio. Mae ffeiliau VSX yn cael eu cadw mewn fformat ffeil XML ac fe'u cefnogwyd tan Visio 2013. Mae'r rhain yn wahanol i'r fformat ffeil VSDX cynradd a gyflwynwyd gyda Microsoft Visio 2013. Gellir agor ffeiliau VSX mewn unrhyw olygydd testun i weld y cynnwys.

          link: "https://docs.fileformat.com/image/vsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Gweithio gyda Fformatau Dogfennau Poblogaidd Eraill"
    content: |
        Diweddaru priodweddau anodi o rai o'r fformatau ffeil poblogaidd fel y nodir isod.
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