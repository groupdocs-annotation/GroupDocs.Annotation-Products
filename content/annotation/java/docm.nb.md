---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DOCM Annotation API Annotate i C#"
head_description: "Java API for å lage og kommentere populære merknadstyper fra DOCM, bilder, tegninger og dokumentfilformater."

############################# Header ############################
title: "Merk DOCM fra Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Last ned gratis prøveversjon"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API er et bibliotek som lar deg legge til merknader til PDF, Word og andre dokumenter på Mac, Windows eller Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) er et innebygd Java API for å administrere merknader med omfattende støtte for å lage, legge til, redigere, slette, trekke ut og eksportere merknader fra bilder og diverse andre dokumenter. Den fullstendige listen over støttede dokumentformater kan du se på denne [siden](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Dette biblioteket lar deg jobbe ikke bare med DOCM-dokumenter, men også med mange andre typer dokumenter som Word, Excel, PowerPoint, Outlook-e-post, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad og mange andre.
        GroupDocs.Annotation for Java API lar deg opprette og legge til nye notater, redigere merknader, trekke ut kommentarer, merknader og fjerne dem fra dokumenter. Biblioteket støtter 13 forskjellige merknadstyper, inkludert tekst, polylinje, område, understreking, punkt, vannmerke, pil, ellipse, teksterstatning, avstand, tekstfelt, ressursredaksjon i PDF, HTML, Microsoft Word-dokumenter, regneark, diagrammer, presentasjoner, tegninger, bilder og mange andre filformater.
        Eksemplet (se nedenfor) viser hvordan du arbeider med DOCM-dokumentet. I dette eksemplet kan du se hovedtrinnene for hvordan du arbeider med GroupDocs. Merknad: Konfigurer en lisens, åpne et dokument du vil jobbe med, opprette en merknad, legge til dataobjekter for å angi merknadsegenskaper i henhold til dine krav og lagre resultatet på ønsket sted. Du kan også se mer detaljert på de støttede funksjonene på vår github [side](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), eller i produkt [dokumentasjon](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Trinn for å legge til merknader til DOCM i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gjør det enkelt for Java-utviklere å legge til ulike merknadstyper til DOCM-filer i enhver Java-basert applikasjon ved å implementere noen få enkle trinn.
        *   Lag svarobjekter med kommentar og dato.
        *   Opprett AreaAnnotation-objekt, angi områdealternativer og legg til svar.
        *   Opprett Annotator-objekt og legg til områdeanmerkning.
        *   Lagre utdatafil.
    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Annotation for Java APIer støttes på alle større plattformer og operativsystemer. Før du utfører koden nedenfor, sørg for at du har følgende forutsetninger installert på systemet ditt.
        *   Operativsystemer: Microsoft Windows, Linux, MacOS
        *   Utviklingsmiljø: NetBeans, Intellij IDEA, Eclipse etc
        *   Java Runtime Environment: Java 7 (1.7) og nyere
        *   Få den nyeste versjonen av GroupDocs.Annotation for Java fra [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Forhåndsvisning av merknader og kodeeksempel
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
    title_left: "Trinn for å fjerne merknader fra DOCM i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gjør det enklere for Java-utviklere å fjerne merknadsdetaljer fra DOCM-filer i enhver Java-basert applikasjon ved å implementere noen få enkle trinn.
        *   Lag svarobjekter med kommentar og dato.
        *   Instantier SaveOptions-objektet og sett AnnotationTypes = AnnotationType.None.
        *   Anrop lagringsmetode med resulterende dokumentbane eller strøm og SaveOptions-objekt.

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
    title_left: "Trinn for å redigere merknader fra DOCM i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gjør det enklere for Java-utviklere å oppdatere ulike merknadsegenskaper fra DOCM-filer i enhver Java-basert applikasjon ved å implementere noen få enkle trinn.
        *   Instantier Annotator-objekt med inndatadokumentbane eller strøm med instansierte LoadOptions med ImportAnnotations = true.
        *   Opprett en AnnotationBase-implementering og sett ID-en til den eksisterende merknaden (hvis merknaden med den ID-en ikke blir funnet, vil ingenting bli endret) eller stiliste med merknader (alle eksisterende merknader vil bli fjernet).
        *   Anrop oppdateringsmetode for Annotator-objekt med beståtte merknader.
        *   Anrop lagringsmetode med resulterende dokumentbane eller strøm og SaveOptions-objekt.

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
    title_left: "Trinn for å trekke ut merknader fra DOCM i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gjør det enkelt for Java-utviklere å kommentere dokumenter og trekke ut merknadsinformasjon fra DOCM-filer i enhver Java-basert applikasjon ved å implementere noen få enkle trinn.
        *   Lag svarobjekter med kommentar og dato.
        *   Instantier LoadOptions-objektet og kall SetImportAnnotations med sant argument.
        *   Definer variabel med typen List.
        *   Ring hent-metoden og returner resultatet til variabelen ovenfor.

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
    title: "Live-demoer for å legge til, fjerne, redigere, trekke ut merknader til dokumenter og bilder"
    content: |
        Legg til, fjern, rediger og trekk ut merknader til DOCM-filen akkurat nå ved å gå til nettstedet [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Live-demoen har følgende fordeler

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docm"
          title: "Om DOCM filformat"
          content: |
            DOCM-filer er Microsoft Word 2007 eller høyere genererte dokumenter med muligheten til å kjøre makroer. Det ligner på DOCX-filformatet, men muligheten til å kjøre makroer gjør det forskjellig fra DOCX. I likhet med DOCX kan DOCM-filer være lagringstekst, bilder, tabeller, former, diagrammer og annet innhold. Muligheten til å kjøre makroer gjør det enkelt å spare tid ved å utføre serien med kommandoer i form av registrerte handlinger for automatisk fullføring av en oppgave . DOCM-filer kan åpnes og redigeres i Microsoft Word 2007 og nyere.

          link: "https://docs.fileformat.com/image/docm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbeide med andre populære dokumentformater"
    content: |
        Oppdater merknadsegenskaper fra noen av de populære filformatene som angitt nedenfor.
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