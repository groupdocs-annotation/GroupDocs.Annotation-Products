
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/wmf"/>

############################# Head ############################
head_title: "Rimuovere Annotazioni da WMF nell'applicazione Net"
head_description: "Net API per creare e Rimuovere tipi di annotazioni popolari da WMF, immagini, disegni e formati di file di documenti."

############################# Header ############################
title: "Annota {{FORMATO}} {{azione.preposizioni}} {{Piattaforma}}"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Annotation per Net"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Annotation per Net API"
    content: |
        GroupDocs.Annotation for Net API è una libreria che ti consente di aggiungere annotazioni a PDF, Word e altri documenti su Mac, Windows o Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) è un'API nativa di Net per la gestione delle annotazioni con supporto completo per la creazione, l'aggiunta, la modifica, l'eliminazione, l'estrazione e l'esportazione di annotazioni da immagini e vari altri documenti. L'elenco completo dei formati di documenti supportati è disponibile in questa [pagina](https://docs.groupdocs.com/annotation/net/supported-document-formats/).

        Questa libreria ti consente di lavorare non solo con il documento WMF ma anche con molti altri tipi di documenti come Word, Excel, PowerPoint, email di Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad e molti altri.

        L'API GroupDocs.Annotation per Net ti consente di creare e aggiungere nuove note, edit annotazioni, extract commenti, annotazioni e remove dai documenti. La libreria supporta 13 diversi tipi di annotazione, tra cui Testo, Polilinea, Area, Sottolineato, Punto, Filigrana, Freccia, Ellisse, Sostituzione testo, Distanza, Campo di testo, Redazione risorsa in PDF, HTML, documenti Microsoft Word, fogli di calcolo, diagrammi, presentazioni, disegni, immagini e molti altri formati di file.

        L'esempio (vedi sotto) mostra come lavorare con il documento WMF, in questo esempio puoi vedere i passaggi principali di come lavorare con GroupDocs. Annotazione: imposta una licenza, apri un documento con cui vuoi lavorare, crea un annotazione, aggiunta di oggetti dati per impostare le proprietà di annotazione in base alle proprie esigenze e salvataggio del risultato nella posizione necessaria. Inoltre puoi dare uno sguardo più dettagliato alle funzionalità supportate sulla nostra github [pagina](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), o nella nostra [documentazione](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Passaggi per aggiungere annotazioni da WMF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende facile per gli sviluppatori Net aggiungere vari tipi di annotazioni ai file WMF all'interno di qualsiasi applicazione basata su Net implementando pochi semplici passaggi.
        * Crea oggetti di risposta con commento e data.
        * Crea un oggetto AreaAnnotation, imposta le opzioni dell'area e aggiungi risposte.
        * Crea un oggetto Annotator e aggiungi un'annotazione dell'area.
        * Salva il file di output.
    title_right: "Requisiti di sistema"
    content_right: |
        Le API GroupDocs.Annotation per Net sono supportate su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.
        * Sistemi operativi: Microsoft Windows, Linux, MacOS
        * Ambienti di sviluppo: Visual Studio, Xamarin, MonoDevelop
        * Framework: .NET Framework, .NET Standard, .NET Core, Mono
        * Scarica l'ultima versione di GroupDocs.Annotation per .NET da [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: "Anteprima dell'annotazione ed esempio di codice"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Aggiungi l'annotazione del campo di testo al documento dal disco locale
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
                Message = "Questa è un'annotazione del campo di testo",
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
                        Comment = "Primo commento",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Secondo commento",
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
    title_left: "Passaggi per rimuovere le annotazioni da WMF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende più facile per gli sviluppatori Net rimuovere i dettagli delle annotazioni dai file WMF all'interno di qualsiasi applicazione basata su Net implementando alcuni semplici passaggi.
        * Crea oggetti di risposta con commento e data.
        * Crea un'istanza dell'oggetto SaveOptions e imposta AnnotationTypes = AnnotationType.None.
        * Richiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```cs
        // 1- Come rimuovere l'annotazione dal documento utilizzando l'indice di annotazione
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- Come rimuovere l'annotazione dal documento utilizzando l'oggetto annotazione
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- Come rimuovere alcune annotazioni dal documento utilizzando l'elenco degli ID
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- Come rimuovere alcune annotazioni dal documento utilizzando l'elenco di annotazioni
        
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
    title_left: "Passaggi per modificare le annotazioni da WMF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende più facile per gli sviluppatori Net aggiornare varie proprietà di annotazione da file WMF all'interno di qualsiasi applicazione basata su Net implementando pochi semplici passaggi.
        * Crea un'istanza dell'oggetto Annotator con il percorso o il flusso del documento di input con LoadOptions istanziato con ImportAnnotations = true.
        * Crea un'implementazione AnnotationBase e imposta l'ID dell'annotazione esistente (se l'annotazione con quell'ID non viene trovata, non verrà modificato nulla) o l'elenco dei percorsi delle annotazioni (tutte le annotazioni esistenti verranno rimosse).
        * Chiama il metodo di aggiornamento dell'oggetto Annotator con annotazioni passate.
        * Richiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```cs
        // apre il documento annotato
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assumendo che cambieremo alcune proprietà dell'annotazione esistente
                AreaAnnotation updated = nuova AreaAnnotation
                    {
                            // È importante impostare l'ID dell'annotazione esistente
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Messaggio = "Questa è un'annotazione aggiornata",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Primo commento aggiornato",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Secondo commento aggiornato",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // aggiorna l'annotazione
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Passaggi per estrarre le annotazioni da WMF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) rende facile per gli sviluppatori Net annotare documenti ed estrarre informazioni di annotazione da file WMF all'interno di qualsiasi applicazione basata su Net implementando pochi semplici passaggi.
        * Crea oggetti di risposta con commento e data.
        * Crea un'istanza dell'oggetto LoadOptions e chiama SetImportAnnotations con argomento vero.
        * Definire variabile con tipo List.
        * Chiama il metodo get e restituisci il risultato alla variabile sopra.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```cs
        // per utilizzare questo file di input di esempio ("annotated.bmp") deve essere con annotazioni
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
    title: "Demo dal vivo per estrarre annotazioni"
    content: |
        Visualizza e rimuovi subito le annotazioni dal file WMF visitando il sito web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        La demo dal vivo ha i seguenti vantaggi

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-wmf"
          title: "Informazioni sul formato file WMF"
          content: |
            I file con estensione WMF rappresentano Microsoft Windows Metafile (WMF) per la memorizzazione di dati di immagini in formato vettoriale e bitmap. Per essere più precisi, WMF appartiene alla categoria dei formati di file vettoriali dei formati di file grafici indipendenti dal dispositivo. Windows Graphical Device Interface (GDI) utilizza le funzioni memorizzate in un file WMF per visualizzare un'immagine sullo schermo. Successivamente è stata pubblicata una versione più avanzata di WMF, nota come Enhanced Meta Files (EMF), che rende il formato più ricco di funzionalità. In pratica, WMF è simile a SVG.
          link: "https://docs.fileformat.com/image/wmf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Lavorare con altri formati di documenti popolari"
    content: |
        Aggiorna le proprietà delle annotazioni da alcuni dei formati di file più diffusi come indicato di seguito.
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