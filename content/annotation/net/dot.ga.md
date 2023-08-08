---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Glan DOT Anótáil API Anótála i C#"
head_description: "Net API chun cineálacha móréilimh anótála a chruthú agus a Anótáil ó DOT, íomhánna, líníochtaí agus formáidí comhaid doiciméad."

############################# Header ############################
title: "Anótáil DOT ó Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Íoslódáil Triail Saor in Aisce"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Maidir le GroupDocs.Annotation for Net API"
    content: |
        Is leabharlann é GroupDocs.Annotation for Net API a ligeann duit nótaí a chur le PDF, Word agus doiciméid eile ar Mac, Windows nó Ubuntu. Is éard atá i [GroupDocs.Annotation for Net](/annotation/net) ná Net API dúchais chun nótaí a bhainistiú le tacaíocht chuimsitheach chun nótaí a chruthú, a chur leis, a chur in eagar, a scriosadh, a bhaint agus a easpórtáil ó íomhánna agus doiciméid éagsúla eile. An liosta iomlán de na formáidí doiciméad tacaithe a d’fhéadfá a fheiceáil ar an [leathanach] seo(https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ligeann an leabharlann seo duit oibriú ní hamháin le doiciméad DOT ach freisin le go leor cineálacha doiciméad eile ar nós Word, Excel, PowerPoint, ríomhphoist Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad agus go leor eile.
        Ligeann an GroupDocs.Annotation for Net API duit nótaí nua a chruthú agus a chur leis, nótaí a chur in eagar, nótaí tráchta a bhaint as, agus iad a bhaint de dhoiciméid. Tacaíonn an leabharlann le 13 chineál nótaí éagsúla, lena n-áirítear Téacs, Polalíne, Achar, Líne Folaigh, Pointe, Comhartha Uisce, Arrow, Éilips, Athsholáthar Téacs, Fad, Réimse Téacs, Athchóiriú Acmhainní i bhformáid PDF, HTML, doiciméid Microsoft Word, scarbhileoga, léaráidí, cur i láthair, líníochtaí, íomhánna agus go leor formáidí comhaid eile.
        Léiríonn an sampla (féach thíos) oibriú le doiciméad DOT, sa sampla seo d'fhéadfá na príomhchéimeanna a fheiceáil maidir le conas oibriú le GroupDocs.Annotation: Socraigh ceadúnas, oscail doiciméad a bhfuil tú ag iarraidh oibriú leis, cruthaigh doiciméad anótáil, rudaí sonraí a chur leis chun airíonna anótála a shocrú de réir do riachtanas agus an toradh a shábháil chuig an áit atá ag teastáil. Chomh maith leis sin d'fhéadfá breathnú níos mionsonraithe a bheith agat ar na gnéithe tacaithe ar ár leathanach github [] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), nó inár dtáirge [doiciméadúchán] (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Céimeanna chun Anótálacha a Chur le DOT in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) éascaíonn sé d’fhorbróirí Net cineálacha éagsúla nótaí a chur le comhaid DOT laistigh d’fheidhmchlár Net-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cruthaigh oibiachtaí Freagra le trácht agus dáta.
        *   Cruthaigh réad AreaAnnotation, socraigh roghanna achair agus cuir freagraí leis.
        *   Cruthaigh réad Anótaire agus cuir anótáil achair leis.
        *   Sábháil an comhad aschuir.
    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Annotation for Net APIs ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.
        *   Córais Oibriúcháin: Microsoft Windows, Linux, MacOS
        *   Timpeallachtaí Forbartha: Visual Studio, Xamarin, MonoDevelop
        *   Creataí: .NET Framework, .NET Standard, .NET Core, Mona
        *   Íoslódáil an leagan is déanaí de GroupDocs.Annotation le haghaidh .NET ó [NuGet] (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Réamhamharc anótála agus sampla cód
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
    title_left: "Céimeanna chun Anótálacha a Bhaint de DOT in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) déanann sé níos éasca d’fhorbróirí Net sonraí anóta a bhaint de chomhaid DOT laistigh d’fheidhmchlár Net-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cruthaigh oibiachtaí Freagra le trácht agus dáta.
        *   Cuir réad SaveOptions ar bun agus socraigh AnnotationTypes = AnnotationType.None.
        *   Glaoigh ar an modh sábhála le cosán doiciméad nó sruth dá bharr agus réad SaveOptions.

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
    title_left: "Céimeanna chun Anótálacha ó DOT a chur in eagar in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) déanann sé níos éasca d’fhorbróirí Net airíonna anótála éagsúla ó chomhaid DOT a nuashonrú laistigh d’fheidhmchlár Net-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cuir réad Anótaire ar an toirt le conair doiciméid ionchuir nó sruth le LoadOptions meandrach le ImportAnnotations = fíor.
        *   Cruthaigh roinnt cur i bhfeidhm AnnotationBase agus socraigh Aitheantas an anótála a bhí ann (mura bhfuarthas anótáil leis an Aitheantas sin, ní athrófar aon rud) nó liosta cosáin na nótaí (bainfear gach anótáil atá ann).
        *   Modh nuashonraithe an ghlao ar réad Anótaire le nótaí a ritheadh.
        *   Glaoigh ar an modh sábhála le cosán doiciméad nó sruth dá bharr agus réad SaveOptions.

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
    title_left: "Céimeanna chun Anótálacha a Bhaint as DOT in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) déanann sé éasca d’fhorbróirí Glan doiciméid a anótáil agus faisnéis anótála a bhaint as comhaid DOT laistigh d’fheidhmchlár Net-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cruthaigh oibiachtaí Freagra le trácht agus dáta.
        *   Cuir oibiacht ar LoadOptions agus cuir glaoch ar SetImportAnnotations le fíorargóint.
        *   Sainmhínigh athróg le liosta cineáil.
        *   Modh faigh glao agus cuir an toradh ar ais chuig an athróg thuas.

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
    title: "Taispeántais Bheo le Cur Leis, Bain Amach, Cuir in Eagar, Anótálacha a Bhaint as Doiciméid agus Íomhánna"
    content: |
        Cuir nótaí le DOT leis, bain, cuir in eagar agus bain amach iad faoi láthair trí chuairt a thabhairt ar [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Tá na buntáistí seo a leanas ag an taispeántas beo

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dot"
          title: "Maidir le DOT Formáid Chomhaid"
          content: |
            Is comhaid teimpléid iad comhaid a bhfuil síneadh .DOT orthu a chruthaigh Microsoft Word chun socruithe réamhfhormáidithe a bheith acu le haghaidh tuilleadh comhaid DOC nó DOCX a ghiniúint. Cruthaítear comhad teimpléid chun go mbeidh socruithe úsáideora ar leith ann ba cheart a chur i bhfeidhm ar chomhaid ina dhiaidh sin a chruthaítear uathu seo. Áiríonn na socruithe seo imeall leathanaigh, teorainneacha, ceanntásca, buntásca, agus socruithe leathanaigh eile. Úsáidtear teimpléid dá leithéid i ndoiciméid oifigiúla mar chinn litreach cuideachta agus foirmeacha caighdeánaithe. Baineann formáid comhaid DOT go sonrach le Microsoft Word 2003 agus níos luaithe, ach tacaíonn leaganacha níos airde léi freisin. De réir réamhshocraithe osclaíonn Microsoft Word gach doiciméad nua bunaithe ar chomhad normal.dot. Má athraítear iad, beidh na socruithe céanna mar thoradh ar na comhaid nua go léir a chruthófar agus a bheidh sa chomhad teimpléid. I Microsoft Word 2007, cuireadh formáid comhaid DOTX bunaithe ar Office OpenXML in ionad fhormáid comhaid DOT.

          link: "https://docs.fileformat.com/image/dot/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ag Obair le Formáidí Doiciméad Coitianta Eile"
    content: |
        Nuashonraigh airíonna anótála ó chuid de na formáidí comhaid coitianta mar a luaitear thíos.
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