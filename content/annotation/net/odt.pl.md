---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Interfejs API adnotacji Net ODT Adnotacja w języku C#"
head_description: "Net API do tworzenia i opisywania popularnych typów adnotacji z ODT, obrazów, rysunków i formatów plików dokumentów."

############################# Header ############################
title: "Adnotacja ODT z sieci"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Pobierz darmową wersję próbną"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Informacje o GroupDocs.Annotation dla interfejsu API sieci"
    content: |
        GroupDocs.Annotation for Net API to biblioteka, która umożliwia dodawanie adnotacji do plików PDF, Word i innych dokumentów na komputerach Mac, Windows lub Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) to natywny interfejs API sieci do zarządzania adnotacjami z kompleksową obsługą tworzenia, dodawania, edytowania, usuwania, wyodrębniania i eksportowania adnotacji z obrazów i różnych innych dokumentów. Pełną listę obsługiwanych formatów dokumentów można zobaczyć na tej [stronie](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Ta biblioteka pozwala pracować nie tylko z dokumentem ODT, ale także z wieloma innymi typami dokumentów, takimi jak Word, Excel, PowerPoint, e-maile Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad i wiele innych.
        GroupDocs.Annotation for Net API umożliwia tworzenie i dodawanie nowych notatek, edytowanie adnotacji, wyodrębnianie komentarzy, adnotacji i usuwanie ich z dokumentów. Biblioteka obsługuje 13 różnych typów adnotacji, w tym tekst, polilinia, obszar, podkreślenie, punkt, znak wodny, strzałka, elipsa, zamiana tekstu, odległość, pole tekstowe, redakcja zasobów w plikach PDF, HTML, dokumentach Microsoft Word, arkuszach kalkulacyjnych, diagramach, prezentacjach, rysunki, obrazy i wiele innych formatów plików.
        Przykład (patrz poniżej) ilustruje pracę z dokumentem ODT, w tym przykładzie możesz zobaczyć główne kroki pracy z GroupDocs. Adnotacja: skonfiguruj licencję, otwórz dokument, z którym chcesz pracować, utwórz adnotację, dodanie obiektów danych w celu ustawienia właściwości adnotacji zgodnie z własnymi wymaganiami i zapisanie wyniku w odpowiednim miejscu. Możesz również przyjrzeć się bardziej szczegółowo obsługiwanym funkcjom na naszej [stronie github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) lub w naszej [dokumentacji produktu](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Kroki, aby dodać adnotacje do ODT w sieci"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ułatwia programistom sieciowym dodawanie różnych typów adnotacji do plików ODT w dowolnej aplikacji sieciowej poprzez wykonanie kilku prostych kroków.
        *   Utwórz obiekty odpowiedzi z komentarzem i datą.
        *   Utwórz obiekt AreaAnnotation, ustaw opcje obszaru i dodaj odpowiedzi.
        *   Utwórz obiekt Annotator i dodaj adnotację obszaru.
        *   Zapisz plik wyjściowy.
    title_right: "wymagania systemowe"
    content_right: |
        Interfejsy GroupDocs.Annotation for Net API są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że w systemie są zainstalowane następujące wymagania wstępne.
        *   Systemy operacyjne: Microsoft Windows, Linux, MacOS
        *   Środowiska programistyczne: Visual Studio, Xamarin, MonoDevelop
        *   Frameworki: .NET Framework, .NET Standard, .NET Core, Mono
        *   Pobierz najnowszą wersję GroupDocs.Annotation dla platformy .NET z [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Podgląd adnotacji i przykładowy kod
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
    title_left: "Kroki, aby usunąć adnotacje z ODT w sieci"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ułatwia programistom sieci usuwanie szczegółów adnotacji z plików ODT w dowolnej aplikacji sieciowej, wykonując kilka prostych kroków.
        *   Utwórz obiekty odpowiedzi z komentarzem i datą.
        *   Utwórz instancję obiektu SaveOptions i ustaw AnnotationTypes = AnnotationType.None.
        *   Wywołaj metodę zapisu z wynikową ścieżką lub strumieniem dokumentu i obiektem SaveOptions.

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
    title_left: "Kroki, aby edytować adnotacje z ODT w sieci"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ułatwia programistom sieci aktualizowanie różnych właściwości adnotacji z plików ODT w dowolnej aplikacji sieciowej poprzez wykonanie kilku prostych kroków.
        *   Utwórz instancję obiektu Annotator z wejściową ścieżką dokumentu lub strumieniem z instancją LoadOptions z ImportAnnotations = true.
        *   Utwórz implementację AnnotationBase i ustaw Id istniejącej adnotacji (jeśli adnotacja z tym Id nie zostanie znaleziona, nic nie zostanie zmienione) lub lista ścieżek adnotacji (wszystkie istniejące adnotacje zostaną usunięte).
        *   Wywołaj metodę aktualizacji obiektu Annotator z przekazanymi adnotacjami.
        *   Wywołaj metodę zapisu z wynikową ścieżką lub strumieniem dokumentu i obiektem SaveOptions.

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
    title_left: "Kroki, aby wyodrębnić adnotacje z ODT w sieci"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) ułatwia programistom sieci dodawanie adnotacji do dokumentów i wyodrębnianie informacji z adnotacji z plików {{FORMAT PLIKU}} w dowolnej aplikacji sieciowej, wykonując kilka prostych kroków.
        *   Utwórz obiekty odpowiedzi z komentarzem i datą.
        *   Utwórz instancję obiektu LoadOptions i wywołaj SetImportAnnotations z prawdziwym argumentem.
        *   Zdefiniuj zmienną typu Lista.
        *   Wywołaj metodę get i zwróć wynik do zmiennej powyżej.

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
    title: "Demo na żywo, aby dodawać, usuwać, edytować, wyodrębniać adnotacje do dokumentów i obrazów"
    content: |
        Dodawaj, usuwaj, edytuj i wyodrębniaj adnotacje do pliku ODT już teraz, odwiedzając witrynę [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Demo na żywo ma następujące zalety

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odt"
          title: "Informacje o formacie pliku ODT"
          content: |
            Pliki ODT to dokumenty tworzone za pomocą aplikacji do edycji tekstu, które są oparte na formacie pliku tekstowego OpenDocument. Są one tworzone za pomocą aplikacji edytora tekstu, takich jak bezpłatny OpenOffice Writer, i mogą przechowywać zawartość, taką jak tekst, obrazy, obiekty i style. Plik ODT jest dla edytora tekstu programu Writer tym, czym DOCX jest dla programu Microsoft Word. Kilka aplikacji, w tym Dokumenty Google i internetowy edytor tekstu Google zawarty w Dysku Google, może otwierać pliki ODT do edycji. Microsoft Word może również otwierać pliki ODT i zapisywać je w innych formatach, takich jak DOC i DOCX.

          link: "https://docs.fileformat.com/image/odt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Praca z innymi popularnymi formatami dokumentów"
    content: |
        Zaktualizuj właściwości adnotacji z niektórych popularnych formatów plików, jak opisano poniżej.
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