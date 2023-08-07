---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net XLSM Annotation API Annotate in C#"
head_description: "Net-sovellusliittymä suosittujen merkintätyyppien luomiseen ja merkitsemiseen XLSM, kuvista, piirustuksista ja asiakirjatiedostomuodoista."

############################# Header ############################
title: "Merkitse XLSM Netistä"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Lataa ilmainen kokeiluversio"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Tietoja GroupDocs.Annotation for Net API:sta"
    content: |
        GroupDocs.Annotation for Net API on kirjasto, jonka avulla voit lisätä huomautuksia PDF-, Word- ja muihin asiakirjoihin Macissa, Windowsissa tai Ubuntussa. [GroupDocs.Annotation for Net](/annotation/net) on natiivi Net-sovellusliittymä merkintöjen hallintaan, ja siinä on kattava tuki merkintöjen luomiseen, lisäämiseen, muokkaamiseen, poistamiseen, poimimiseen ja vientiin kuvista ja useista muista asiakirjoista. Täydellinen luettelo tuetuista asiakirjamuodoista, jotka voit nähdä tällä [sivulla](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Tämän kirjaston avulla voit työskennellä XLSM-asiakirjan lisäksi myös monien muiden asiakirjojen kanssa, kuten Word, Excel, PowerPoint, Outlook-sähköpostit, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ja monet muut.
        GroupDocs.Annotation for Net -sovellusliittymän avulla voit luoda ja lisätä uusia muistiinpanoja, muokata huomautuksia, poimia kommentteja, merkintöjä ja poistaa niitä asiakirjoista. Kirjasto tukee 13 erilaista merkintätyyppiä, mukaan lukien teksti, polyline, alue, alleviivaus, piste, vesileima, nuoli, ellipsi, tekstin vaihto, etäisyys, tekstikenttä, resurssien muokkaus PDF-, HTML-, Microsoft Word -asiakirjoissa, laskentataulukoissa, kaavioissa, esityksissä, piirustuksia, kuvia ja monia muita tiedostomuotoja.
        Esimerkki (katso alla) havainnollistaa työskentelyä asiakirjan XLSM kanssa. Tässä esimerkissä voit nähdä GroupDocsin työskentelyn päävaiheet. Huomautus: Määritä lisenssi, avaa dokumentti, jota haluat käsitellä, ja luo huomautus, tietoobjektien lisääminen merkintöjen ominaisuuksien määrittämiseksi tarpeidesi mukaan ja tuloksen tallentaminen haluttuun paikkaan. Voit myös tutustua tarkemmin tuettuihin ominaisuuksiin github-sivullamme [sivulla](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) tai tuotteessamme [dokumentaatiossa](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET). ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Vaiheet huomautusten lisäämiseksi Netin tiedostoon XLSM"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net-kehittäjien on helppo lisätä erilaisia ​​merkintätyyppejä XLSM-tiedostoihin missä tahansa Net-pohjaisessa sovelluksessa muutaman helpon vaiheen avulla.
        *   Luo vastausobjekteja kommentilla ja päivämäärällä.
        *   Luo AreaAnnotation-objekti, aseta alueasetukset ja lisää vastauksia.
        *   Luo Annotator-objekti ja lisää alueen huomautus.
        *   Tallenna tulostiedosto.
    title_right: "Laitteistovaatimukset"
    content_right: |
        GroupDocs.Annotation for Net API:t ovat tuettuja kaikilla tärkeimmillä alustoilla ja käyttöjärjestelmillä. Ennen kuin suoritat alla olevan koodin, varmista, että sinulla on seuraavat edellytykset asennettuna järjestelmääsi.
        *   Käyttöjärjestelmät: Microsoft Windows, Linux, MacOS
        *   Kehitysympäristöt: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Lataa GroupDocs.Annotationin uusin versio .NETille osoitteesta [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Huomautuksen esikatselu ja koodinäyte
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
    title_left: "Ohjeet merkintöjen poistamiseen Netin XLSM-tiedostosta"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Helpottaa Net-kehittäjien merkintöjen tietojen poistamista XLSM-tiedostoista missä tahansa Net-pohjaisessa sovelluksessa muutaman helpon vaiheen avulla.
        *   Luo vastausobjekteja kommentilla ja päivämäärällä.
        *   Luo SaveOptions-objekti ja aseta AnnotationTypes = AnnotationType.None.
        *   Kutsu tallennusmenetelmää tuloksena olevalla asiakirjapolulla tai -virralla ja SaveOptions-objektilla.

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
    title_left: "Ohjeet merkintöjen muokkaamiseen XLSM Netissä"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Helpottaa Net-kehittäjien merkintöjen ominaisuuksien päivittämistä XLSM-tiedostoista missä tahansa Net-pohjaisessa sovelluksessa muutaman helpon vaiheen avulla.
        *   Instantoi Annotator-objekti syöteasiakirjan polulla tai virralla instantoiduilla LoadOptions-toiminnoilla, kun ImportAnnotations = true.
        *   Luo jokin AnnotationBase-toteutus ja aseta olemassa olevan merkinnän tunnus (jos merkintää tällä tunnuksella ei löydy, mitään ei muuteta) tai merkintöjen polkuluettelo (kaikki olemassa olevat merkinnät poistetaan).
        *   Kutsu Annotator-objektin päivitysmenetelmä hyväksytyillä huomautuksilla.
        *   Kutsu tallennusmenetelmää tuloksena olevalla asiakirjapolulla tai -virralla ja SaveOptions-objektilla.

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
    title_left: "Ohjeet huomautusten poimimiseen Netin XLSM-tiedostosta"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Helpottaa Net-kehittäjien merkintää asiakirjoja ja poimia huomautustietoja XLSM-tiedostoista missä tahansa Net-pohjaisessa sovelluksessa muutaman helpon vaiheen avulla.
        *   Luo vastausobjekteja kommentilla ja päivämäärällä.
        *   Luo LoadOptions-objekti ja kutsu SetImportAnnotations tosi-argumentilla.
        *   Määrittele muuttuja tyypillä List.
        *   Kutsu get-metodi ja palauta tulos yllä olevaan muuttujaan.

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
    title: "Live-esittelyt asiakirjojen ja kuvien huomautusten lisäämiseen, poistamiseen, muokkaamiseen ja poimimiseen"
    content: |
        Lisää, poista, muokkaa ja pura merkintöjä tiedostoon XLSM heti käymällä [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) -sivustolla. Live-demolla on seuraavat edut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsm"
          title: "Tietoja tiedostomuodosta XLSM"
          content: |
            XLSM-laajennuksella varustetut tiedostot ovat eräänlaisia ​​taulukkolaskentatiedostoja, jotka tukevat makroja. Sovelluksen näkökulmasta makro on joukko ohjeita, joita käytetään prosessien automatisointiin. Makroa käytetään tallentamaan toistuvasti suoritetut vaiheet ja helpottaa toimintojen suorittamista suorittamalla makro uudelleen. Makrot ohjelmoidaan Microsoftin Visual Basic for Applications (VBA) -ohjelmalla Excel-työkirjasta Visual Basic Editorin avulla, ja ne voidaan suorittaa/virheenkorjata suoraan sieltä.

          link: "https://docs.fileformat.com/image/xlsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Työskentely muiden suosittujen asiakirjamuotojen kanssa"
    content: |
        Päivitä merkintöjen ominaisuudet joistakin suosituista tiedostomuodoista alla kuvatulla tavalla.
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