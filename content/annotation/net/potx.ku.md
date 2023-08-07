---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net POTX Annotation API Annotate in C#"
head_description: "Net API ku ji POTX, wêne, xêzkirin û formatên pelên pelgeyê celebên annotasyonên populer biafirîne û şîrove bike."

############################# Header ############################
title: "Nîşe POTX ji Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Daxistina Doza Belaş"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Der barê GroupDocs.Annotation ji bo Net API"
    content: |
        GroupDocs.Annotation ji bo Net API pirtûkxaneyek e ku dihêle hûn li ser Mac, Windows an Ubuntu şîroveyan li PDF, Word û belgeyên din zêde bikin. [GroupDocs.Annotation for Net](/annotation/net) API-ya Net-ê ya xwemalî ye ji bo birêvebirina annotasyonên bi piştgirîya berfireh ji bo afirandin, zêdekirin, guherandin, jêbirin, derxistin û hinartina annotasyonên ji wêne û belgeyên din ên cihêreng. Navnîşa tevahî ya formên belgeyên piştgirî yên ku hûn dikarin li ser vê [rûpelê] bibînin (https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ev pirtûkxane dihêle hûn ne tenê bi belgeya POTX re lê her weha bi gelek celeb belgeyên din ên wekî Word, Excel, PowerPoint, e-nameyên Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad û gelekên din re bixebitin.
        GroupDocs.Annotation ji bo Net API destûrê dide te ku hûn notên nû biafirînin û lê zêde bikin, şîroveyan biguherînin, şîroveyan, şîroveyan derxînin û wan ji belgeyan derxînin. Pirtûkxane 13 celebên annotasyonê yên cihêreng piştgirî dike, di nav de Nivîsar, Polyline, Herêm, Binxêz, Xal, Nîşan, Tîrek, Ellipse, Veguheztina Nivîsan, Dûrbûn, Qada Nivîsarê, Veguhastina Çavkaniyê di PDF, HTML, belgeyên Microsoft Word de, pelgeyên berbelav, diagram, pêşkêşî, xêzkirin, wêne û gelek formatên pelan ên din.
        Nimûne (ji kerema xwe li jêr binêre) nîşan dide ku bi belgeya POTX re dixebite, di vê nimûneyê de hûn dikarin gavên sereke yên çawa bi GroupDocs re bixebitin bibînin.Annotation: Destûrnameyek saz bikin, belgeyek ku hûn dixwazin pê re bixebitin vekin, vekin annotation, lê zêdekirina tiştên daneyê da ku taybetmendiyên annotasyonê li gorî hewcedariyên we bicîh bikin û encamê li cîhê hewce hilînin. Di heman demê de hûn dikarin li ser taybetmendiyên piştgirîkirî yên li ser github me [rûpel](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) an jî di hilberê me de [belge](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Gavên Zêdekirina Şîroveyan li POTX di Net-ê de"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ji bo pêşdebirên Net-ê hêsan dike ku bi pêkanîna çend gavên hêsan ve cûrbecûr şîrovekirina pelan li pelên POTX zêde bikin.
        *   Tiştên Bersiv bi şîrove û tarîxê biafirînin.
        *   Tişta AreaAnnotation biafirînin, vebijarkên deverê bicîh bikin û bersivan lê zêde bikin.
        *   Tişta Annotator biafirînin û şirovekirina deverê lê zêde bikin.
        *   Pelê derketinê tomar bike.
    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Annotation ji bo API-yên Net-ê li ser hemî platformên sereke û pergalên xebitandinê têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.
        *   Pergalên Xebatê: Microsoft Windows, Linux, MacOS
        *   Jîngehên Pêşveçûnê: Visual Studio, Xamarin, MonoDevelop
        *   Çarçove: .NET Framework, .NET Standard, .NET Core, Mono
        *   Guhertoya herî dawî ya GroupDocs.Annotation ji bo .NET ji [NuGet] dakêşin (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Pêşdîtina annotation û nimûneya kodê
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
    title_left: "Gavên Rakirina Şîroveyan ji POTX li Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Ji pêşdebirên Net-ê re hêsantir dike ku hûrguliyên annotasyonê ji pelên POTX di nav her serîlêdana Net-ê de bi cîbicîkirina çend gavên hêsan rakin.
        *   Tiştên Bersiv bi şîrove û tarîxê biafirînin.
        *   Tişta SaveOptions destnîşan bikin û AnnotationTypes = AnnotationType.None saz bikin.
        *   Rêbaza hilanînê bi rêça belgeya encam an tîrêjê û tiştê SaveOptions re bang bikin.

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
    title_left: "Gavên Guherandinên Şîrove ji POTX li Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Ji pêşdebirên Net-ê re hêsantir dike ku bi pêkanîna çend gavên hêsan ve nûvekirina taybetmendiyên cûrbecûr şîrovekirinê ji pelên POTX di nav her serlêdanek Net-ê de nûve bikin.
        *   Tişta Annotatorê bi rêça belgeya têketinê ve bişopînin an bi Vebijarkên Loadê yên destnîşankirî bi ImportAnnotations re biherikînin = rast.
        *   Hin pêkanîna AnnotationBase biafirînin û Nasnameya annotationê ya heyî destnîşan bikin (heke şîroveya bi wê Nasnameyê re neyê dîtin, dê tiştek neyê guheztin) an navnîşa rêgezên şîroveyan (hemû şîroveyên heyî dê werin rakirin).
        *   Rêbaza nûvekirina tiştê Annotator bi şîroveyên derbasbûyî re bang bikin.
        *   Rêbaza hilanînê bi rêça belgeya encam an tîrêjê û tiştê SaveOptions re bang bikin.

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
    title_left: "Gavên Derxistina Şîroveyan ji POTX li Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ji bo pêşdebirên Net-ê hêsan dike ku bi pêkanîna çend gavên hêsan ve belgeyan şîrove bikin û agahdariya şîrovekirinê ji pelên POTX derxînin.
        *   Tiştên Bersiv bi şîrove û tarîxê biafirînin.
        *   Objektîfên LoadOptions destnîşan bikin û bi argumana rast bangî SetImportAnnotations bikin.
        *   Guherbar bi tîpa Lîsteyê pênase bikin.
        *   Banga rêbaza wergirtinê bikin û encamê vegerînin guhêrbara jorîn.

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
    title: "Demoyên Zindî ku lê zêde bikin, jêbirin, biguherînin, şîroveyan ji belge û wêneyan derxin"
    content: |
        Bi seredana malpera [GroupDocs.Annotation Demos Zindî](https://products.groupdocs.app/annotation/family) niha li pelê POTX şîroveyan zêde bikin, jêbikin, biguherînin û derxin. Demoya zindî xwedî feydeyên jêrîn e

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-potx"
          title: "Derbarê POTX Forma Pelê"
          content: |
            Pelên bi dirêjkirina .POTX pêşandanên şablonên Microsoft PowerPoint yên ku bi Microsoft PowerPoint 2007 û jor ve hatine afirandin temsîl dikin. Ev format ji bo şûna pelê pelê POT-ê ku li ser bingeha forma pelê binaryê ye û bi PowerPoint 97-2003 ve tê piştgirî kirin, hate afirandin. Pelên ku têne çêkirin dikarin ji bo afirandina pêşandanên ku xwedan heman sêwiranê ne û mîhengên din ên ku ji bo pelên nû werin sepandin têne bikar anîn. Van mîhengan dikarin şêwaz, paşxane, paleta rengan, font û pêşnumayan pêk bînin. Pelên weha têne çêkirin ku ji bo karanîna fermî pelên şablonê amade-bikaranîna biafirînin.

          link: "https://docs.fileformat.com/image/potx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi Formên Belgeya Din ên populer re dixebitin"
    content: |
        Taybetmendiyên annotasyonê ji hin formatên pelê yên populer ên ku li jêr têne destnîşan kirin nûve bikin.
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