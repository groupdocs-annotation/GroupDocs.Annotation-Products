---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java VSS Annotation API Annotate i C#"
head_description: "Java API til at oprette og kommentere populære annoteringstyper fra VSS, billeder, tegninger og dokumentfilformater."

############################# Header ############################
title: "Anmærk VSS fra Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download gratis prøveversion"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API er et bibliotek, der giver dig mulighed for at tilføje anmærkninger til PDF, Word og andre dokumenter på Mac, Windows eller Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) er en indbygget Java API til håndtering af annoteringer med omfattende understøttelse af oprettelse, tilføjelse, redigering, sletning, udtrækning og eksport af annoteringer fra billeder og forskellige andre dokumenter. Den fulde liste over understøttede dokumentformater kan du se på denne [side](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Dette bibliotek giver dig mulighed for ikke kun at arbejde med VSS-dokumenter, men også med mange andre typer dokumenter, såsom Word, Excel, PowerPoint, Outlook-e-mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad og mange andre.
        GroupDocs.Annotation for Java API giver dig mulighed for at oprette og tilføje nye noter, redigere anmærkninger, udtrække kommentarer, anmærkninger og fjerne dem fra dokumenter. Biblioteket understøtter 13 forskellige annotationstyper, inklusive tekst, polylinje, område, understregning, punkt, vandmærke, pil, ellipse, teksterstatning, afstand, tekstfelt, ressourceredaktion i PDF, HTML, Microsoft Word-dokumenter, regneark, diagrammer, præsentationer, tegninger, billeder og mange andre filformater.
        Eksemplet (se nedenfor) demonstrerer arbejdet med VSS-dokumentet, i dette eksempel kan du se hovedtrinene i, hvordan man arbejder med GroupDocs.Annotation: Konfigurer en licens, åbn et dokument, du vil arbejde med, opret en annotering, tilføjelse af dataobjekter for at indstille annoteringsegenskaber i henhold til dine krav og gemme resultatet på det nødvendige sted. Du kan også se mere detaljeret om de understøttede funktioner på vores github [side](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), eller i vores produkt [dokumentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Trin til at tilføje annoteringer til VSS i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gør det nemt for Java-udviklere at tilføje forskellige annotationstyper til VSS-filer i enhver Java-baseret applikation ved at implementere nogle få nemme trin.
        *   Opret svarobjekter med kommentar og dato.
        *   Opret AreaAnnotation-objekt, indstil områdeindstillinger og tilføj svar.
        *   Opret annotatorobjekt og tilføj områdeannotering.
        *   Gem outputfil.
    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Annotation til Java API'er understøttes på alle større platforme og operativsystemer. Før du udfører koden nedenfor, skal du sørge for, at du har følgende forudsætninger installeret på dit system.
        *   Operativsystemer: Microsoft Windows, Linux, MacOS
        *   Udviklingsmiljø: NetBeans, Intellij IDEA, Eclipse osv
        *   Java Runtime Environment: Java 7 (1.7) og nyere
        *   Hent den seneste version af GroupDocs.Annotation for Java fra [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Forhåndsvisning af annotering og kodeeksempel
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
    title_left: "Trin til fjernelse af annoteringer fra VSS i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gør det nemmere for Java-udviklere at fjerne anmærkningsdetaljer fra VSS-filer i enhver Java-baseret applikation ved at implementere nogle få nemme trin.
        *   Opret svarobjekter med kommentar og dato.
        *   Instantiér SaveOptions-objektet og indstil AnnotationTypes = AnnotationType.None.
        *   Kald gemmemetode med resulterende dokumentsti eller strøm og SaveOptions-objekt.

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
    title_left: "Trin til redigering af annoteringer fra VSS i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gør det lettere for Java-udviklere at opdatere forskellige annoteringsegenskaber fra VSS-filer i enhver Java-baseret applikation ved at implementere nogle få nemme trin.
        *   Instantiér Annotator-objekt med input-dokumentsti eller -strøm med instansierede LoadOptions med ImportAnnotations = true.
        *   Opret en AnnotationBase-implementering og sæt Id for eksisterende annotering (hvis annotering med dette Id ikke findes, vil intet blive ændret) eller stiliste over annoteringer (alle eksisterende annoteringer vil blive fjernet).
        *   Kald opdateringsmetode for annotatorobjekt med beståede annoteringer.
        *   Kald gemmemetode med resulterende dokumentsti eller strøm og SaveOptions-objekt.

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
    title_left: "Trin til at udtrække annoteringer fra VSS i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gør det nemt for Java-udviklere at annotere dokumenter og udtrække anmærkningsoplysninger fra VSS-filer i enhver Java-baseret applikation ved at implementere nogle få nemme trin.
        *   Opret svarobjekter med kommentar og dato.
        *   Instantiér LoadOptions-objektet og kald SetImportAnnotations med sandt argument.
        *   Definer variabel med typen Liste.
        *   Kald get-metoden og returner resultatet til variabel ovenfor.

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
    title: "Live-demoer til at tilføje, fjerne, redigere, udtrække annoteringer til dokumenter og billeder"
    content: |
        Tilføj, fjern, rediger og udpak annoteringer til filen VSS lige nu ved at besøge webstedet [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Livedemoen har følgende fordele

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vss"
          title: "Om VSS filformat"
          content: |
            VSS er stencilfiler oprettet med Microsoft Visio 2007 og tidligere. Et relativt nyt filformat er .VSSX, der blev introduceret med Microsoft Visio 2013. Stencilfiler giver tegneobjekter, der kan inkluderes i en .VSD Visio-tegning. Microsoft Visio selv er kendt for at skabe tegneelementer såsom samling af figurer, forbindelser, flowcharts, netværkslayout, UML-diagrammer, softwarediagrammer, databasemodeller, objektkortlægning og anden lignende information. Det har også rige konverteringsfunktioner fra Visio-dokumenter til andre filformater såsom PNG, BMP, PDF og andre. Visio er tilgængelig til både Windows og Mac OS.

          link: "https://docs.fileformat.com/image/vss/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbejde med andre populære dokumentformater"
    content: |
        Opdater annoteringsegenskaber fra nogle af de populære filformater som angivet nedenfor.
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