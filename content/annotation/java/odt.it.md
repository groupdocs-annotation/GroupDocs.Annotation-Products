---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java ODT API di annotazione Annota in C#"
head_description: "API Java per creare e annotare tipi di annotazioni popolari da ODT, immagini, disegni e formati di file di documenti."

############################# Header ############################
title: "Annota ODT da Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Scarica la prova gratuita"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Annotation per l'API Java"
    content: |
        GroupDocs.Annotation for Java API è una libreria che ti consente di aggiungere annotazioni a PDF, Word e altri documenti su Mac, Windows o Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) è un'API Java nativa per la gestione delle annotazioni con supporto completo per la creazione, l'aggiunta, la modifica, l'eliminazione, l'estrazione e l'esportazione di annotazioni da immagini e vari altri documenti. L'elenco completo dei formati di documenti supportati è disponibile in questa [pagina](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Questa libreria ti consente di lavorare non solo con il documento ODT ma anche con molti altri tipi di documenti come Word, Excel, PowerPoint, e-mail di Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad e molti altri.
        L'API GroupDocs.Annotation per Java consente di creare e aggiungere nuove note, modificare annotazioni, estrarre commenti, annotazioni e rimuoverle dai documenti. La libreria supporta 13 diversi tipi di annotazione, tra cui Testo, Polilinea, Area, Sottolineato, Punto, Filigrana, Freccia, Ellisse, Sostituzione testo, Distanza, Campo di testo, Redazione risorsa in PDF, HTML, documenti Microsoft Word, fogli di calcolo, diagrammi, presentazioni, disegni, immagini e molti altri formati di file.
        L'esempio (vedi sotto) mostra come lavorare con il documento ODT, in questo esempio puoi vedere i passaggi principali di come lavorare con GroupDocs. Annotazione: impostare una licenza, aprire un documento con cui vuoi lavorare, creare un annotazione, aggiunta di oggetti dati per impostare le proprietà di annotazione in base alle proprie esigenze e salvataggio del risultato nella posizione necessaria. Inoltre, puoi dare un'occhiata più dettagliata alle funzionalità supportate sulla nostra [pagina] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) o nella [documentazione] del nostro prodotto (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Passaggi per aggiungere annotazioni a ODT in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende facile per gli sviluppatori Java aggiungere vari tipi di annotazioni ai file ODT all'interno di qualsiasi applicazione basata su Java implementando pochi semplici passaggi.
        *   Crea oggetti Reply con commento e data.
        *   Crea un oggetto AreaAnnotation, imposta le opzioni dell'area e aggiungi le risposte.
        *   Crea un oggetto Annotator e aggiungi l'annotazione dell'area.
        *   Salva il file di output.
    title_right: "Requisiti di sistema"
    content_right: |
        Le API GroupDocs.Annotation per Java sono supportate su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.
        *   Sistemi operativi: Microsoft Windows, Linux, MacOS
        *   Ambiente di sviluppo: NetBeans, Intellij IDEA, Eclipse ecc
        *   Java Runtime Environment: Java 7 (1.7) e versioni successive
        *   Ottieni l'ultima versione di GroupDocs.Annotation per Java da [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anteprima dell'annotazione ed esempio di codice
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
    title_left: "Passaggi per rimuovere le annotazioni da ODT in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende più facile per gli sviluppatori Java rimuovere i dettagli delle annotazioni dai file ODT all'interno di qualsiasi applicazione basata su Java implementando alcuni semplici passaggi.
        *   Crea oggetti Reply con commento e data.
        *   Crea un'istanza dell'oggetto SaveOptions e imposta AnnotationTypes = AnnotationType.None.
        *   Chiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

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
    title_left: "Passaggi per modificare le annotazioni da ODT in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende più facile per gli sviluppatori Java aggiornare varie proprietà di annotazione da file ODT all'interno di qualsiasi applicazione basata su Java implementando alcuni semplici passaggi.
        *   Crea un'istanza dell'oggetto Annotator con il percorso o il flusso del documento di input con LoadOptions istanziato con ImportAnnotations = true.
        *   Crea un'implementazione AnnotationBase e imposta l'ID dell'annotazione esistente (se l'annotazione con quell'ID non viene trovata, non verrà modificato nulla) o l'elenco dei percorsi delle annotazioni (tutte le annotazioni esistenti verranno rimosse).
        *   Chiama il metodo di aggiornamento dell'oggetto Annotator con annotazioni passate.
        *   Chiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

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
    title_left: "Passaggi per estrarre annotazioni da ODT in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende facile per gli sviluppatori Java annotare documenti ed estrarre informazioni di annotazione da file ODT all'interno di qualsiasi applicazione basata su Java implementando pochi semplici passaggi.
        *   Crea oggetti Reply con commento e data.
        *   Crea un'istanza dell'oggetto LoadOptions e chiama SetImportAnnotations con argomento vero.
        *   Definisci variabile con tipo List.
        *   Chiama il metodo get e restituisci il risultato alla variabile sopra.

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
    title: "Demo dal vivo per aggiungere, rimuovere, modificare ed estrarre annotazioni a documenti e immagini"
    content: |
        Aggiungi, rimuovi, modifica ed estrai subito le annotazioni dal file ODT visitando il sito web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
La demo dal vivo ha i seguenti vantaggi

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odt"
          title: "Informazioni sul formato file ODT"
          content: |
            I file ODT sono tipi di documenti creati con applicazioni di elaborazione testi basate sul formato OpenDocument Text File. Questi vengono creati con applicazioni di elaborazione testi come OpenOffice Writer gratuito e possono contenere contenuti come testo, immagini, oggetti e stili. Il file ODT è per l'elaboratore di testi di Writer ciò che il DOCX è per Microsoft Word. Diverse applicazioni, tra cui Google Docs e l'elaboratore di testi basato sul Web di Google incluso in Google Drive, possono aprire i file ODT per la modifica. Microsoft Word può anche aprire file ODT e salvarli in altri formati come DOC e DOCX.

          link: "https://docs.fileformat.com/image/odt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Lavorare con altri formati di documenti popolari"
    content: |
        Aggiorna le proprietà delle annotazioni da alcuni dei formati di file più diffusi come indicato di seguito.
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