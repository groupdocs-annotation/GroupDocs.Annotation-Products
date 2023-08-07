---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "„Net XLSM“ komentarų API komentaras C#"
head_description: "Net API, skirta kurti ir komentuoti populiarius komentarų tipus iš XLSM, vaizdų, brėžinių ir dokumentų failų formatų."

############################# Header ############################
title: "Komentuoti XLSM iš tinklo"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Atsisiųskite nemokamą bandomąją versiją"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Apie GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API yra biblioteka, leidžianti pridėti komentarų į PDF, Word ir kitus dokumentus Mac, Windows ar Ubuntu. [GroupDocs.Annotation for Net] (/annotation/net) yra vietinė tinklo API, skirta komentarams tvarkyti, su visapusišku palaikymu kuriant, įtraukiant, redaguojant, trinant, ištraukiant ir eksportuojant komentarus iš vaizdų ir įvairių kitų dokumentų. Visą palaikomų dokumentų formatų sąrašą galite pamatyti šiame [puslapyje](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ši biblioteka leidžia dirbti ne tik su XLSM dokumentu, bet ir su daugelio kitų tipų dokumentais, tokiais kaip Word, Excel, PowerPoint, Outlook el. laiškai, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ir daugelis kitų.
        „GroupDocs.Annotation for Net“ API leidžia kurti ir pridėti naujų pastabų, redaguoti komentarus, išgauti komentarus, anotacijas ir pašalinti juos iš dokumentų. Biblioteka palaiko 13 skirtingų anotacijų tipų, įskaitant tekstą, poliliniją, sritį, pabraukimą, tašką, vandens ženklą, rodyklę, elipsę, teksto pakeitimą, atstumą, teksto lauką, išteklių redagavimą PDF, HTML, Microsoft Word dokumentuose, skaičiuokles, diagramas, pristatymus, brėžiniai, vaizdai ir daugelis kitų failų formatų.
        Pavyzdyje (žr. toliau) parodytas darbas su XLSM dokumentu. Šiame pavyzdyje galite pamatyti pagrindinius darbo su GroupDocs veiksmus. Anotacija: nustatykite licenciją, atidarykite dokumentą, su kuriuo norite dirbti, ir sukurkite anotacija, pridedant duomenų objektus, kad nustatytumėte anotacijos ypatybes pagal jūsų poreikius ir išsaugant rezultatą reikiamoje vietoje. Taip pat galite sužinoti daugiau apie palaikomas funkcijas mūsų „github“ [puslapyje] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) arba mūsų produkto [dokumentacijoje] (https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Veiksmai, kaip pridėti komentarus prie XLSM tinkle"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) „Net“ kūrėjai gali lengvai pridėti įvairių tipų komentarų prie XLSM failų bet kurioje „Net“ programoje, atlikdami kelis paprastus veiksmus.
        *   Sukurkite atsakymo objektus su komentaru ir data.
        *   Sukurkite AreaAnnotation objektą, nustatykite srities parinktis ir pridėkite atsakymus.
        *   Sukurkite komentatoriaus objektą ir pridėkite srities anotaciją.
        *   Išsaugoti išvesties failą.
    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Annotation for Net API palaikomos visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.
        *   Operacinės sistemos: Microsoft Windows, Linux, MacOS
        *   Kūrimo aplinkos: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Atsisiųskite naujausią GroupDocs.Annotation versiją .NET iš [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anotacijos peržiūra ir kodo pavyzdys
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
    title_left: "Veiksmai, kaip pašalinti komentarus iš XLSM tinkle"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) „Net“ kūrėjams lengviau pašalinti komentarų informaciją iš XLSM failų bet kurioje „Net“ programoje, atlikus kelis paprastus veiksmus.
        *   Sukurkite atsakymo objektus su komentaru ir data.
        *   Sukurkite objektą SaveOptions ir nustatykite AnnotationTypes = AnnotationType.None.
        *   Iškvieskite išsaugojimo metodą su gautu dokumento keliu arba srautu ir objektu „SaveOptions“.

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
    title_left: "Veiksmai, kaip redaguoti komentarus iš XLSM tinkle"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) „Net“ kūrėjams leidžia lengviau atnaujinti įvairias komentarų ypatybes iš XLSM failų bet kurioje „Net“ programoje, įgyvendinant kelis paprastus veiksmus.
        *   Sukurkite komentatoriaus objektą su įvesties dokumento keliu arba srautu su momentinėmis LoadOptions su ImportAnnotations = true.
        *   Sukurkite kokį nors AnnotationBase diegimą ir nustatykite esamo komentaro ID (jei komentaras su tuo ID nerastas, niekas nebus pakeistas) arba komentarų kelių sąrašą (visi esami komentarai bus pašalinti).
        *   Iškvieskite komentatoriaus objekto atnaujinimo metodą su priimtais komentarais.
        *   Iškvieskite išsaugojimo metodą su gautu dokumento keliu arba srautu ir objektu „SaveOptions“.

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
    title_left: "Veiksmai, kaip ištraukti komentarus iš XLSM tinkle"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) leidžia „Net“ kūrėjams lengvai komentuoti dokumentus ir išgauti komentarų informaciją iš XLSM failų bet kurioje „Net“ programoje, atlikus kelis paprastus veiksmus.
        *   Sukurkite atsakymo objektus su komentaru ir data.
        *   Sukurkite LoadOptions objektą ir iškvieskite SetImportAnnotations su tikru argumentu.
        *   Apibrėžkite kintamąjį naudodami tipą Sąrašas.
        *   Iškvieskite metodą gauti ir grąžinkite rezultatą į aukščiau esantį kintamąjį.

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
    title: "Tiesioginės demonstracinės versijos, skirtos dokumentų ir vaizdų komentarams pridėti, pašalinti, redaguoti, išgauti"
    content: |
        Pridėkite, pašalinkite, redaguokite ir išskleiskite komentarus prie XLSM failo dabar, apsilankę [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) svetainėje.
Tiesioginė demonstracinė versija turi šiuos privalumus

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsm"
          title: "Apie XLSM failo formatą"
          content: |
            Failai su XLSM plėtiniu yra skaičiuoklės failų tipas, palaikantis makrokomandas. Taikymo požiūriu makrokomanda yra instrukcijų rinkinys, naudojamas procesams automatizuoti. Makrokomanda naudojama pakartotinai atliekamiems veiksmams įrašyti ir palengvina veiksmų atlikimą dar kartą paleidžiant makrokomandą. Makrokomandos programuojamos naudojant „Microsoft Visual Basic for Applications“ (VBA) iš „Excel“ darbaknygės, naudojant „Visual Basic“ rengyklę, ir jas galima paleisti / derinti tiesiai iš ten.

          link: "https://docs.fileformat.com/image/xlsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Darbas su kitais populiariais dokumentų formatais"
    content: |
        Atnaujinkite komentarų ypatybes iš kai kurių populiarių failų formatų, kaip nurodyta toliau.
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