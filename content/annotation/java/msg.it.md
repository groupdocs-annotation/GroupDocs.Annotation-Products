
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/msg"/>

############################# Head ############################
head_title: "Rimuovere Annotazioni da MSG nell'applicazione Java"
head_description: "Java API per creare e Rimuovere tipi di annotazioni popolari da MSG, immagini, disegni e formati di file di documenti."

############################# Header ############################
title: "Annota MSG da Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Annotation per Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Annotation per Java API"
    content: |
        GroupDocs.Annotation for Java API è una libreria che ti consente di aggiungere annotazioni a PDF, Word e altri documenti su Mac, Windows o Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) è un'API nativa di Java per la gestione delle annotazioni con supporto completo per la creazione, l'aggiunta, la modifica, l'eliminazione, l'estrazione e l'esportazione di annotazioni da immagini e vari altri documenti. L'elenco completo dei formati di documenti supportati è disponibile in questa [pagina](https://docs.groupdocs.com/annotation/java/supported-document-formats/).

        Questa libreria ti consente di lavorare non solo con il documento MSG ma anche con molti altri tipi di documenti come Word, Excel, PowerPoint, email di Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad e molti altri.

        L'API GroupDocs.Annotation per Java ti consente di creare e aggiungere nuove note, edit annotazioni, extract commenti, annotazioni e remove dai documenti. La libreria supporta 13 diversi tipi di annotazione, tra cui Testo, Polilinea, Area, Sottolineato, Punto, Filigrana, Freccia, Ellisse, Sostituzione testo, Distanza, Campo di testo, Redazione risorsa in PDF, HTML, documenti Microsoft Word, fogli di calcolo, diagrammi, presentazioni, disegni, immagini e molti altri formati di file.

        L'esempio (vedi sotto) mostra come lavorare con il documento MSG, in questo esempio puoi vedere i passaggi principali di come lavorare con GroupDocs. Annotazione: imposta una licenza, apri un documento con cui vuoi lavorare, crea un annotazione, aggiunta di oggetti dati per impostare le proprietà di annotazione in base alle proprie esigenze e salvataggio del risultato nella posizione necessaria. Inoltre puoi dare uno sguardo più dettagliato alle funzionalità supportate sulla nostra github [pagina](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), o nella nostra [documentazione](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Passaggi per aggiungere annotazioni da MSG in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende facile per gli sviluppatori Java aggiungere vari tipi di annotazioni ai file MSG all'interno di qualsiasi applicazione basata su Java implementando pochi semplici passaggi.
        * Crea oggetti di risposta con commento e data.
        * Crea un oggetto AreaAnnotation, imposta le opzioni dell'area e aggiungi risposte.
        * Crea un oggetto Annotator e aggiungi un'annotazione dell'area.
        * Salva il file di output.
    title_right: "Requisiti di sistema"
    content_right: |
        Le API GroupDocs.Annotation per Java sono supportate su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.
        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambiente di sviluppo: NetBeans, Intellij IDEA, Eclipse ecc
        * Java Runtime Environment: Java 7 (1.7) e versioni successive
        * Ottieni l'ultima versione di GroupDocs.Annotation per Java da [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: "Anteprima dell'annotazione ed esempio di codice"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Crea un'istanza della classe Reply e aggiungi commenti
        Reply firstReply = new Reply();
        firstReply.setComment("Primo commento");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Secondo commento");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Crea un'istanza della classe AreaAnnotation e imposta le opzioni
        AreaAnnotation area = new AreaAnnotation();
        area.setColoreSfondo(65535);
        area.setBox(new Rettangolo(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("Questa è un'annotazione dell'area");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Crea un'istanza della classe Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Aggiungi annotazione
        annotator.add(area);
        
        // Salva nel file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Passaggi per rimuovere le annotazioni da MSG in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende più facile per gli sviluppatori Java rimuovere i dettagli delle annotazioni dai file MSG all'interno di qualsiasi applicazione basata su Java implementando alcuni semplici passaggi.
        * Crea oggetti di risposta con commento e data.
        * Crea un'istanza dell'oggetto SaveOptions e imposta AnnotationTypes = AnnotationType.None.
        * Richiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```java
        // Crea un'istanza della classe Annotator
        Annotator annotator = new Annotator("C://input.bmp");

        // Rimuovi l'annotazione per tipo di set Nessuno
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Salva l'annotazione nel file di output
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Passaggi per modificare le annotazioni da MSG in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende più facile per gli sviluppatori Java aggiornare varie proprietà di annotazione da file MSG all'interno di qualsiasi applicazione basata su Java implementando pochi semplici passaggi.
        * Crea un'istanza dell'oggetto Annotator con il percorso o il flusso del documento di input con LoadOptions istanziato con ImportAnnotations = true.
        * Crea un'implementazione AnnotationBase e imposta l'ID dell'annotazione esistente (se l'annotazione con quell'ID non viene trovata, non verrà modificato nulla) o l'elenco dei percorsi delle annotazioni (tutte le annotazioni esistenti verranno rimosse).
        * Chiama il metodo di aggiornamento dell'oggetto Annotator con annotazioni passate.
        * Richiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Crea un'istanza della classe Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Crea un'istanza della classe Reply per il primo esempio e aggiungi commenti
        Reply reply1 = new Reply();
        reply1.setComment("Primo commento originale");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Secondo commento originale");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Crea un'istanza della classe AreaAnnotation e imposta le opzioni
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("Questa è un'annotazione originale");
        original.setReplies(replies);
        
        // Aggiungi annotazione originale
        annotator.add(originale);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Apre il documento annotato
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Crea un'istanza della classe Reply per aggiornare il primo esempio
        Reply reply3 = new Reply();
        reply3.setComment("Primo commento aggiornato");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Secondo commento aggiornato");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggerisce di voler modificare alcune proprietà dell'annotazione esistente
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("Questa è un'annotazione aggiornata");
        updated.setReplies(replies1);
        
        // Aggiorna e salva l'annotazione
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Passaggi per estrarre le annotazioni da MSG in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende facile per gli sviluppatori Java annotare documenti ed estrarre informazioni di annotazione da file MSG all'interno di qualsiasi applicazione basata su Java implementando pochi semplici passaggi.
        * Crea oggetti di risposta con commento e data.
        * Crea un'istanza dell'oggetto LoadOptions e chiama SetImportAnnotations con argomento vero.
        * Definire variabile con tipo List.
        * Chiama il metodo get e restituisci il risultato alla variabile sopra.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```java
        // Per utilizzare questo esempio, il file di input ("annotated.bmp") deve contenere annotazioni
        LoadOptions loadOptions = new LoadOptions();
        
        // Crea un'istanza della classe Annotator e ottieni le annotazioni
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Demo dal vivo per estrarre annotazioni"
    content: |
        Visualizza e rimuovi subito le annotazioni dal file MSG visitando il sito web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        La demo dal vivo ha i seguenti vantaggi

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-msg"
          title: "Informazioni sul formato file MSG"
          content: |
            MSG è un formato di file utilizzato da Microsoft Outlook ed Exchange per archiviare messaggi di posta elettronica, contatti, appuntamenti o altre attività. Tali messaggi possono contenere uno o più campi e-mail, con il mittente, il destinatario, l'oggetto, la data e il corpo del messaggio, oppure le informazioni di contatto, i dettagli dell'appuntamento e una o più specifiche dell'attività. Le proprietà che costituiscono l'oggetto Message, incluso fanno anche parte del file MSG. Il file MSG ha intestazioni, corpo del messaggio principale e collegamenti ipertestuali come semplice testo ASCII. I file MSG sono adatti anche con i programmi che richiedono l'interfaccia MAPI (Messaging Applications Programming Interface) di Microsoft.
          link: "https://docs.fileformat.com/image/msg/"

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