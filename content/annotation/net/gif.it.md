---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net GIF API di annotazione Annota in C#"
head_description: "Net API per creare e annotare tipi di annotazioni popolari da GIF, immagini, disegni e formati di file di documenti."

############################# Header ############################
title: "Annota GIF da Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Scarica la prova gratuita"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Informazioni su GroupDocs.Annotation per Net API"
    content: |
        GroupDocs.Annotation for Net API è una libreria che consente di aggiungere annotazioni a PDF, Word e altri documenti su Mac, Windows o Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) è un'API Net nativa per la gestione delle annotazioni con supporto completo per la creazione, l'aggiunta, la modifica, l'eliminazione, l'estrazione e l'esportazione di annotazioni da immagini e vari altri documenti. L'elenco completo dei formati di documenti supportati è disponibile in questa [pagina](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Questa libreria ti consente di lavorare non solo con il documento GIF ma anche con molti altri tipi di documenti come Word, Excel, PowerPoint, e-mail di Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad e molti altri.
        L'API GroupDocs.Annotation per Net consente di creare e aggiungere nuove note, modificare annotazioni, estrarre commenti, annotazioni e rimuoverle dai documenti. La libreria supporta 13 diversi tipi di annotazione, tra cui Testo, Polilinea, Area, Sottolineato, Punto, Filigrana, Freccia, Ellisse, Sostituzione testo, Distanza, Campo di testo, Redazione risorsa in PDF, HTML, documenti Microsoft Word, fogli di calcolo, diagrammi, presentazioni, disegni, immagini e molti altri formati di file.
        L'esempio (vedi sotto) mostra come lavorare con il documento GIF, in questo esempio puoi vedere i passaggi principali di come lavorare con GroupDocs. Annotazione: impostare una licenza, aprire un documento con cui vuoi lavorare, creare un annotazione, aggiunta di oggetti dati per impostare le proprietà di annotazione in base alle proprie esigenze e salvataggio del risultato nella posizione necessaria. Inoltre, puoi dare un'occhiata più dettagliata alle funzionalità supportate sulla nostra [pagina github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) o nella [documentazione del nostro prodotto](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Passaggi per aggiungere annotazioni a GIF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) rende facile per gli sviluppatori Net aggiungere vari tipi di annotazioni ai file GIF all'interno di qualsiasi applicazione basata su Net implementando pochi semplici passaggi.
        *   Crea oggetti Reply con commento e data.
        *   Crea un oggetto AreaAnnotation, imposta le opzioni dell'area e aggiungi le risposte.
        *   Crea un oggetto Annotator e aggiungi l'annotazione dell'area.
        *   Salva il file di output.
    title_right: "Requisiti di sistema"
    content_right: |
        GroupDocs.Annotation for Net APIs è supportato su tutte le principali piattaforme e sistemi operativi. Prima di eseguire il codice seguente, assicurati di avere i seguenti prerequisiti installati sul tuo sistema.
        *   Sistemi operativi: Microsoft Windows, Linux, MacOS
        *   Ambienti di sviluppo: Visual Studio, Xamarin, MonoDevelop
        *   Framework: .NET Framework, .NET Standard, .NET Core, Mono
        *   Scarica l'ultima versione di GroupDocs.Annotation per .NET da [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anteprima dell'annotazione ed esempio di codice
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
    title_left: "Passaggi per rimuovere le annotazioni da GIF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) rende più facile per gli sviluppatori Net rimuovere i dettagli delle annotazioni dai file GIF all'interno di qualsiasi applicazione basata su Net implementando alcuni semplici passaggi.
        *   Crea oggetti Reply con commento e data.
        *   Crea un'istanza dell'oggetto SaveOptions e imposta AnnotationTypes = AnnotationType.None.
        *   Chiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

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
    title_left: "Passaggi per modificare le annotazioni da GIF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) rende più facile per gli sviluppatori Net aggiornare varie proprietà di annotazione dai file GIF all'interno di qualsiasi applicazione basata su Net implementando alcuni semplici passaggi.
        *   Crea un'istanza dell'oggetto Annotator con il percorso o il flusso del documento di input con LoadOptions istanziato con ImportAnnotations = true.
        *   Crea un'implementazione AnnotationBase e imposta l'ID dell'annotazione esistente (se l'annotazione con quell'ID non viene trovata, non verrà modificato nulla) o l'elenco dei percorsi delle annotazioni (tutte le annotazioni esistenti verranno rimosse).
        *   Chiama il metodo di aggiornamento dell'oggetto Annotator con annotazioni passate.
        *   Chiama il metodo di salvataggio con il percorso o il flusso del documento risultante e l'oggetto SaveOptions.

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
    title_left: "Passaggi per estrarre le annotazioni da GIF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) rende facile per gli sviluppatori Net annotare documenti ed estrarre informazioni di annotazione da file GIF all'interno di qualsiasi applicazione basata su Net implementando pochi semplici passaggi.
        *   Crea oggetti Reply con commento e data.
        *   Crea un'istanza dell'oggetto LoadOptions e chiama SetImportAnnotations con argomento vero.
        *   Definisci variabile con tipo List.
        *   Chiama il metodo get e restituisci il risultato alla variabile sopra.

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
    title: "Demo dal vivo per aggiungere, rimuovere, modificare ed estrarre annotazioni a documenti e immagini"
    content: |
        Aggiungi, rimuovi, modifica ed estrai subito le annotazioni dal file GIF visitando il sito web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). La demo dal vivo ha i seguenti vantaggi

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-gif"
          title: "Informazioni sul formato file GIF"
          content: |
            Un formato GIF o Graphical Interchange Format è un tipo di immagine altamente compressa. Di proprietà di Unisys, GIF utilizza l'algoritmo di compressione LZW che non degrada la qualità dell'immagine. Per ogni immagine GIF in genere consente fino a 8 bit per pixel e sono consentiti fino a 256 colori nell'immagine. A differenza di un'immagine JPEG, che può visualizzare fino a 16 milioni di colori e tocca abbastanza i limiti dell'occhio umano. Ai tempi in cui è emerso Internet, le GIF sono rimaste la scelta migliore perché richiedevano una larghezza di banda ridotta e erano compatibili con la grafica che consuma aree di colore solide. Una GIF animata combina numerose immagini o fotogrammi in un singolo file e li visualizza in sequenza per generare una clip animata o un breve video. I limiti di colore sono fino a 256 per ogni fotogramma e sono probabilmente i meno adatti per riprodurre altre immagini e fotografie con gradiente di colore.

          link: "https://docs.fileformat.com/image/gif/"

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