---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Interfejs API adnotacji Java DXF Adnotacja w języku C#"
head_description: "Java API do tworzenia i opisywania popularnych typów adnotacji z DXF, obrazów, rysunków i formatów plików dokumentów."

############################# Header ############################
title: "Adnotacja DXF z Javy"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Pobierz darmową wersję próbną"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Informacje o GroupDocs.Annotation dla interfejsu API języka Java"
    content: |
        GroupDocs.Annotation for Java API to biblioteka, która umożliwia dodawanie adnotacji do plików PDF, Word i innych dokumentów na komputerach Mac, Windows lub Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) to natywny interfejs API języka Java do zarządzania adnotacjami z kompleksową obsługą tworzenia, dodawania, edytowania, usuwania, wyodrębniania i eksportowania adnotacji z obrazów i różnych innych dokumentów. Pełną listę obsługiwanych formatów dokumentów można zobaczyć na tej [stronie](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ta biblioteka pozwala pracować nie tylko z dokumentem DXF, ale także z wieloma innymi typami dokumentów, takimi jak Word, Excel, PowerPoint, e-maile Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad i wiele innych.
        GroupDocs.Annotation for Java API umożliwia tworzenie i dodawanie nowych notatek, edytowanie adnotacji, wyodrębnianie komentarzy, adnotacji i usuwanie ich z dokumentów. Biblioteka obsługuje 13 różnych typów adnotacji, w tym tekst, polilinia, obszar, podkreślenie, punkt, znak wodny, strzałka, elipsa, zamiana tekstu, odległość, pole tekstowe, redakcja zasobów w plikach PDF, HTML, dokumentach Microsoft Word, arkuszach kalkulacyjnych, diagramach, prezentacjach, rysunki, obrazy i wiele innych formatów plików.
        Przykład (patrz poniżej) ilustruje pracę z dokumentem DXF, w tym przykładzie możesz zobaczyć główne kroki pracy z GroupDocs. Adnotacja: skonfiguruj licencję, otwórz dokument, z którym chcesz pracować, utwórz adnotację, dodanie obiektów danych w celu ustawienia właściwości adnotacji zgodnie z własnymi wymaganiami i zapisanie wyniku w odpowiednim miejscu. Możesz również przyjrzeć się bardziej szczegółowo obsługiwanym funkcjom na naszej [stronie] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) lub w naszej [dokumentacji] produktu (https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Kroki, aby dodać adnotacje do DXF w Javie"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ułatwia programistom Javy dodawanie różnych typów adnotacji do plików DXF w dowolnej aplikacji opartej na Javie, wykonując kilka prostych kroków.
        *   Utwórz obiekty odpowiedzi z komentarzem i datą.
        *   Utwórz obiekt AreaAnnotation, ustaw opcje obszaru i dodaj odpowiedzi.
        *   Utwórz obiekt Annotator i dodaj adnotację obszaru.
        *   Zapisz plik wyjściowy.
    title_right: "wymagania systemowe"
    content_right: |
        Interfejsy API GroupDocs.Annotation for Java są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że w systemie są zainstalowane następujące wymagania wstępne.
        *   Systemy operacyjne: Microsoft Windows, Linux, MacOS
        *   Środowisko programistyczne: NetBeans, Intellij IDEA, Eclipse itp
        *   Środowisko wykonawcze Java: Java 7 (1.7) i nowsze
        *   Pobierz najnowszą wersję GroupDocs.Annotation for Java z [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Podgląd adnotacji i przykładowy kod
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Create an instance of Reply class and add comments
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("This is area annotation");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Add annotation
        annotator.add(area);
        
        // Save to file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Kroki, aby usunąć adnotacje z DXF w Javie"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ułatwia programistom Javy usuwanie szczegółów adnotacji z plików DXF w dowolnej aplikacji opartej na Javie, wykonując kilka prostych kroków.
        *   Utwórz obiekty odpowiedzi z komentarzem i datą.
        *   Utwórz instancję obiektu SaveOptions i ustaw AnnotationTypes = AnnotationType.None.
        *   Wywołaj metodę zapisu z wynikową ścieżką lub strumieniem dokumentu i obiektem SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```java
        // Create an instance of Annotator class 
        Annotator annotator = new Annotator("C://input.bmp");

        // Remove annotation by set type None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Save annotation to output file
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Kroki, aby edytować adnotacje z DXF w Javie"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ułatwia programistom Java aktualizację różnych właściwości adnotacji z plików DXF w dowolnej aplikacji opartej na Javie, wykonując kilka prostych kroków.
        *   Utwórz instancję obiektu Annotator z wejściową ścieżką dokumentu lub strumieniem z instancją LoadOptions z ImportAnnotations = true.
        *   Utwórz implementację AnnotationBase i ustaw Id istniejącej adnotacji (jeśli adnotacja z tym Id nie zostanie znaleziona, nic nie zostanie zmienione) lub lista ścieżek adnotacji (wszystkie istniejące adnotacje zostaną usunięte).
        *   Wywołaj metodę aktualizacji obiektu Annotator z przekazanymi adnotacjami.
        *   Wywołaj metodę zapisu z wynikową ścieżką lub strumieniem dokumentu i obiektem SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Create an instance of Reply class for first example and add comments
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Create an instance of Reply class for update first example
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Update and save annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Kroki, aby wyodrębnić adnotacje z DXF w Javie"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ułatwia programistom Javy dodawanie adnotacji do dokumentów i wyodrębnianie informacji z adnotacji z plików DXF w dowolnej aplikacji opartej na Javie, wykonując kilka prostych kroków.
        *   Utwórz obiekty odpowiedzi z komentarzem i datą.
        *   Utwórz instancję obiektu LoadOptions i wywołaj SetImportAnnotations z prawdziwym argumentem.
        *   Zdefiniuj zmienną typu Lista.
        *   Wywołaj metodę get i zwróć wynik do zmiennej powyżej.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```java
        // For using this example input file ("annotated.bmp") must be with annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Create an instance of Annotator class and get annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Demo na żywo, aby dodawać, usuwać, edytować, wyodrębniać adnotacje do dokumentów i obrazów"
    content: |
        Dodawaj, usuwaj, edytuj i wyodrębniaj adnotacje do pliku DXF już teraz, odwiedzając witrynę [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Demo na żywo ma następujące zalety

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dxf"
          title: "Informacje o formacie pliku DXF"
          content: |
            DXF, Drawing Interchange Format lub Drawing Exchange Format, jest oznakowaną reprezentacją danych pliku rysunku programu AutoCAD. Każdy element w pliku ma przedrostek liczby całkowitej zwany kodem grupy. Ten kod grupy faktycznie reprezentuje element następujący po nim i wskazuje znaczenie elementu danych dla danego typu obiektu. DXF umożliwia reprezentację prawie wszystkich informacji określonych przez użytkownika w pliku rysunku. Format pliku DXF został opracowany przez firmę Autodesk jako format pliku danych CAD w celu zapewnienia współdziałania danych między programem AutoCAD a innymi aplikacjami. W ten sposób dane mogą być importowane z innych formatów do DXF do AutoCAD zgodnie ze specyfikacjami interoperacyjności formatu pliku DXF.

          link: "https://docs.fileformat.com/image/dxf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Praca z innymi popularnymi formatami dokumentów"
    content: |
        Zaktualizuj właściwości adnotacji z niektórych popularnych formatów plików, jak opisano poniżej.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/java/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/java/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/java/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/java/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/java/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/java/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/java/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/java/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/java/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/java/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/java/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/java/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/java/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/java/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/java/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/java/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/java/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/java/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/java/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/java/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/java/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/java/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/java/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/java/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/java/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/java/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/java/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/java/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/java/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/java/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/java/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/java/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/java/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/java/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/java/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---