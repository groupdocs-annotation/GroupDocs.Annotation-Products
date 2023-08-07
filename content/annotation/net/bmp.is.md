---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net BMP Annotation API Annotate í C#"
head_description: "Net API til að búa til og athugasemda við vinsælar athugasemdagerðir úr BMP, myndum, teikningum og skjalaskráarsniðum."

############################# Header ############################
title: "Skýrðu BMP frá Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Sækja ókeypis prufuáskrift"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Um GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API er bókasafn sem gerir þér kleift að bæta við athugasemdum við PDF, Word og önnur skjöl á Mac, Windows eða Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) er innbyggt Net API til að stjórna athugasemdum með alhliða stuðningi við að búa til, bæta við, breyta, eyða, draga út og flytja út athugasemdir úr myndum og ýmsum öðrum skjölum. Allur listi yfir studd skjalasnið sem þú gætir séð á þessari [síðu](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Þetta bókasafn gerir þér kleift að vinna ekki aðeins með BMP skjölum heldur einnig með mörgum öðrum skjölum eins og Word, Excel, PowerPoint, Outlook tölvupósti, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad og mörgum öðrum.
        GroupDocs.Annotation for Net API gerir þér kleift að búa til og bæta við nýjum athugasemdum, breyta athugasemdum, draga út athugasemdir, athugasemdir og fjarlægja þær úr skjölum. Bókasafnið styður 13 mismunandi skýringargerðir, þar á meðal texta, fjöllínu, svæði, undirstrik, punkt, vatnsmerki, ör, sporbaug, textaskipti, fjarlægð, textareit, tilföng klippingu í PDF, HTML, Microsoft Word skjölum, töflureiknum, skýringarmyndum, kynningum, teikningar, myndir og mörg önnur skráarsnið.
        Dæmið (vinsamlegast sjáðu hér að neðan) sýnir að þú vinnur með BMP skjal, í þessu dæmi gætirðu séð helstu skrefin í því hvernig á að vinna með GroupDocs.Athugasemd: Setja upp leyfi, opna skjal sem þú vilt vinna með, búa til athugasemd, bæta við gagnahlutum til að stilla athugasemdareiginleika í samræmi við kröfur þínar og vista niðurstöðuna á nauðsynlegum stað. Þú gætir líka skoðað studdu eiginleikana á github [síðu] okkar (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), eða í vörunni okkar [skjölum](https) ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Skref til að bæta athugasemdum við BMP í Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gerir það auðvelt fyrir Net forritara að bæta ýmsum athugasemdategundum við BMP skrár innan hvaða net-undirstaða forrits sem er með því að útfæra nokkur auðveld skref.
        *   Búðu til svarhluti með athugasemd og dagsetningu.
        *   Búðu til AreaAnnotation hlut, stilltu svæðisvalkosti og bættu við svörum.
        *   Búðu til Annotator hlut og bættu við svæðisskýringum.
        *   Vista úttaksskrá.
    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Annotation for Net API eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.
        *   Stýrikerfi: Microsoft Windows, Linux, MacOS
        *   Þróunarumhverfi: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Sæktu nýjustu útgáfuna af GroupDocs.Annotation fyrir .NET frá [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Forskoðun athugasemda og kóðasýni
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
    title_left: "Skref til að fjarlægja athugasemdir úr BMP í Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gerir það auðveldara fyrir Net forritara að fjarlægja athugasemdaupplýsingar úr BMP skrám innan hvaða net-undirstaða forrits sem er með því að útfæra nokkur auðveld skref.
        *   Búðu til svarhluti með athugasemd og dagsetningu.
        *   Staðfestu SaveOptions hlutinn og stilltu AnnotationTypes = AnnotationType.None.
        *   Hringdu í vistunaraðferð með skjalaslóð eða straumi og SaveOptions hlut.

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
    title_left: "Skref til að breyta athugasemdum frá BMP í Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gerir það auðveldara fyrir Net forritara að uppfæra ýmsa skýringaeiginleika úr BMP skrám innan hvaða Net-undirstaða forrits sem er með því að útfæra nokkur auðveld skref.
        *   Staðfestu Annotator hlut með innsláttarskjalsslóð eða straumi með instantiated LoadOptions með ImportAnnotations = true.
        *   Búðu til einhverja AnnotationBase útfærslu og stilltu auðkenni þeirra skýringa sem fyrir voru (ef athugasemd með því auðkenni finnst ekki verður engu breytt) eða slóðalista yfir athugasemdir (allar skýringar sem til eru verða fjarlægðar).
        *   Kalla uppfærsluaðferð á Annotator hlut með samþykktum athugasemdum.
        *   Hringdu í vistunaraðferð með skjalaslóð eða straumi og SaveOptions hlut.

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
    title_left: "Skref til að draga út athugasemdir úr BMP í Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) gerir það auðvelt fyrir Net forritara að skrifa athugasemdir við skjöl og draga út athugasemdaupplýsingar úr BMP skrám innan hvaða net-undirstaða forrits sem er með því að útfæra nokkur auðveld skref.
        *   Búðu til svarhluti með athugasemd og dagsetningu.
        *   Staðfestu LoadOptions hlut og hringdu í SetImportAnnotations með sannri röksemdafærslu.
        *   Skilgreindu breytu með gerð List.
        *   Hringdu í fá aðferð og skilaðu niðurstöðunni í breytuna hér að ofan.

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
    title: "Lifandi kynningar til að bæta við, fjarlægja, breyta, draga út athugasemdir við skjöl og myndir"
    content: |
        Bættu við, fjarlægðu, breyttu og dragðu út athugasemdir við BMP skrána núna með því að fara á vefsíðu [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Lifandi kynningin hefur eftirfarandi kosti

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-bmp"
          title: "Um BMP skráarsnið"
          content: |
            Skrár með endinguna .BMP tákna Bitmap Image skrár sem eru notaðar til að geyma bitmap stafrænar myndir. Þessar myndir eru óháðar skjákortum og eru einnig kallaðar tækisóháð bitamynd (DIB) skráarsnið. Þetta sjálfstæði þjónar þeim tilgangi að opna skrána á mörgum kerfum eins og Microsoft Windows og Mac. BMP skráarsniðið getur geymt gögn sem tvívíddar stafrænar myndir í bæði einlita og litasniði með mismunandi litadýpt.

          link: "https://docs.fileformat.com/image/bmp/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vinna með önnur vinsæl skjalasnið"
    content: |
        Uppfærðu athugasemdareiginleika frá sumum af vinsælustu skráarsniðunum eins og fram kemur hér að neðan.
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