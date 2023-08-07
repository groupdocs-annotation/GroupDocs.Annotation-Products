---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DCM Annotatie-API Annotatie in C#"
head_description: "Java API voor het maken en annoteren van populaire annotatietypen van DCM, afbeeldingen, tekeningen en documentbestandsindelingen."

############################# Header ############################
title: "Annoteer DCM vanuit Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download gratis proefversie"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Over GroupDocs.Annotatie voor Java API"
    content: |
        GroupDocs.Annotation for Java API is een bibliotheek waarmee u annotaties kunt toevoegen aan PDF, Word en andere documenten op Mac, Windows of Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) is een native Java API voor het beheren van annotaties met uitgebreide ondersteuning voor het maken, toevoegen, bewerken, verwijderen, extraheren en exporteren van annotaties van afbeeldingen en diverse andere documenten. De volledige lijst met ondersteunde documentindelingen die u kunt zien op deze [pagina](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Met deze bibliotheek kunt u niet alleen met DCM-documenten werken, maar ook met vele andere soorten documenten, zoals Word, Excel, PowerPoint, Outlook-e-mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad en vele anderen.
        Met de GroupDocs.Annotation for Java API kunt u nieuwe notities maken en toevoegen, annotaties bewerken, opmerkingen en annotaties extraheren en ze uit documenten verwijderen. De bibliotheek ondersteunt 13 verschillende annotatietypen, waaronder tekst, polylijn, gebied, onderstreping, punt, watermerk, pijl, ellips, tekstvervanging, afstand, tekstveld, redactie van bronnen in PDF, HTML, Microsoft Word-documenten, spreadsheets, diagrammen, presentaties, tekeningen, afbeeldingen en vele andere bestandsformaten.
        Het voorbeeld (zie hieronder) demonstreert het werken met een DCM-document, in dit voorbeeld kunt u de belangrijkste stappen zien van het werken met GroupDocs. Annotatie: stel een licentie in, open een document waarmee u wilt werken, maak een annotatie, gegevensobjecten toevoegen om annotatie-eigenschappen in te stellen volgens uw vereisten en het resultaat opslaan op de gewenste plaats. U kunt ook meer details bekijken over de ondersteunde functies op onze github [pagina](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), of in onze product [documentatie](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Stappen om annotaties toe te voegen aan DCM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maakt het gemakkelijk voor Java-ontwikkelaars om verschillende annotatietypes toe te voegen aan DCM-bestanden binnen elke op Java gebaseerde applicatie door een paar eenvoudige stappen te implementeren.
        *   Maak Reply-objecten met commentaar en datum.
        *   Maak een AreaAnnotation-object, stel gebiedsopties in en voeg antwoorden toe.
        *   Maak een Annotator-object en voeg een gebiedsannotatie toe.
        *   Sla uitvoerbestand op.
    title_right: "systeem vereisten"
    content_right: |
        GroupDocs.Annotation for Java API's worden ondersteund op alle belangrijke platforms en besturingssystemen. Voordat u de onderstaande code uitvoert, moet u ervoor zorgen dat de volgende vereisten op uw systeem zijn geïnstalleerd.
        *   Besturingssystemen: Microsoft Windows, Linux, MacOS
        *   Ontwikkelomgeving: NetBeans, Intellij IDEA, Eclipse etc
        *   Java Runtime Environment: Java 7 (1.7) en hoger
        *   Download de nieuwste versie van GroupDocs.Annotation voor Java van [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Annotatievoorbeeld en codevoorbeeld
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
    title_left: "Stappen om annotaties te verwijderen uit DCM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maakt het gemakkelijker voor Java-ontwikkelaars om annotatiedetails te verwijderen uit DCM-bestanden binnen elke op Java gebaseerde applicatie door een paar eenvoudige stappen te implementeren.
        *   Maak Reply-objecten met commentaar en datum.
        *   Maak een Instantie van het SaveOptions-object en stel AnnotationTypes = AnnotationType.None in.
        *   Roep de opslagmethode aan met het resulterende documentpad of -stroom en SaveOptions-object.

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
    title_left: "Stappen om annotaties van DCM in Java te bewerken"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maakt het gemakkelijker voor Java-ontwikkelaars om verschillende annotatie-eigenschappen van DCM-bestanden binnen elke op Java gebaseerde applicatie bij te werken door een paar eenvoudige stappen te implementeren.
        *   Maak een instantie van het Annotator-object met invoerdocumentpad of -stroom met geïnstantieerde LoadOptions met ImportAnnotations = true.
        *   Maak een AnnotationBase-implementatie en stel de id van de bestaande annotatie in (als de annotatie met die id niet wordt gevonden, wordt er niets gewijzigd) of de padlijst met annotaties (alle bestaande annotaties worden verwijderd).
        *   Roep de updatemethode van het Annotator-object aan met doorgegeven annotaties.
        *   Roep de opslagmethode aan met het resulterende documentpad of -stroom en SaveOptions-object.

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
    title_left: "Stappen om annotaties te extraheren uit DCM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maakt het gemakkelijk voor Java-ontwikkelaars om documenten te annoteren en annotatie-informatie te extraheren uit DCM-bestanden binnen elke op Java gebaseerde applicatie door een paar eenvoudige stappen te implementeren.
        *   Maak Reply-objecten met commentaar en datum.
        *   Maak een Instantie van het LoadOptions-object en roep SetImportAnnotations aan met het argument True.
        *   Definieer variabele met type Lijst.
        *   Roep de get-methode aan en retourneer het resultaat naar de bovenstaande variabele.

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
    title: "Live demo's om annotaties aan documenten en afbeeldingen toe te voegen, te verwijderen, te bewerken en te extraheren"
    content: |
        Voeg nu annotaties toe aan, verwijder, bewerk en extraheer annotaties naar het bestand DCM door naar de website [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) te gaan.
De live demo heeft de volgende voordelen

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dcm"
          title: "Over DCM bestandsindeling"
          content: |
            Bestanden met de extensie .DCM vertegenwoordigen een digitaal beeld waarin medische informatie van patiënten wordt opgeslagen, zoals MRI's, CT-scans en echografiebeelden. Het is ontwikkeld door de National Electrical Manufacturers Association (NEMA) en was bedoeld om het beeldvormingsbestandsformaat voor distributie en weergave van medische beelden te standaardiseren. Het is vergelijkbaar met het DICOM-bestandsformaat en kan patiëntinformatie bevatten ter referentie.

          link: "https://docs.fileformat.com/image/dcm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Werken met andere populaire documentindelingen"
    content: |
        Werk annotatie-eigenschappen bij van enkele van de populaire bestandsindelingen, zoals hieronder vermeld.
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