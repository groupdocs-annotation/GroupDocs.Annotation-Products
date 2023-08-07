---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net DXF Annotation API Annotation in C#"
head_description: "Net-API zum Erstellen und Kommentieren beliebter Anmerkungstypen aus DXF, Bildern, Zeichnungen und Dokumentdateiformaten."

############################# Header ############################
title: "Kommentieren Sie DXF aus dem Netz"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download kostenlose Testversion"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Annotation für Net API"
    content: |
        GroupDocs.Annotation for Net API ist eine Bibliothek, mit der Sie Anmerkungen zu PDF-, Word- und anderen Dokumenten auf Mac, Windows oder Ubuntu hinzufügen können. [GroupDocs.Annotation for Net](/annotation/net) ist eine native Net-API zum Verwalten von Anmerkungen mit umfassender Unterstützung für das Erstellen, Hinzufügen, Bearbeiten, Löschen, Extrahieren und Exportieren von Anmerkungen aus Bildern und verschiedenen anderen Dokumenten. Die vollständige Liste der unterstützten Dokumentformate finden Sie auf dieser [Seite](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Mit dieser Bibliothek können Sie nicht nur mit DXF-Dokumenten arbeiten, sondern auch mit vielen anderen Dokumenttypen wie Word, Excel, PowerPoint, Outlook-E-Mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad und vielen anderen.
        Mit der GroupDocs.Annotation for Net-API können Sie neue Notizen erstellen und hinzufügen, Anmerkungen bearbeiten, Kommentare und Anmerkungen extrahieren und aus Dokumenten entfernen. Die Bibliothek unterstützt 13 verschiedene Anmerkungstypen, darunter Text, Polylinie, Fläche, Unterstreichung, Punkt, Wasserzeichen, Pfeil, Ellipse, Textersetzung, Abstand, Textfeld, Ressourcenschwärzung in PDF, HTML, Microsoft Word-Dokumenten, Tabellenkalkulationen, Diagrammen, Präsentationen, Zeichnungen, Bilder und viele andere Dateiformate.
        Das Beispiel (siehe unten) zeigt die Arbeit mit dem Dokument DXF. In diesem Beispiel können Sie die Hauptschritte für die Arbeit mit GroupDocs.Annotation sehen: Richten Sie eine Lizenz ein, öffnen Sie ein Dokument, mit dem Sie arbeiten möchten, und erstellen Sie ein Annotation, Hinzufügen von Datenobjekten zum Festlegen von Annotationseigenschaften gemäß Ihren Anforderungen und Speichern des Ergebnisses am erforderlichen Ort. Außerdem können Sie einen detaillierteren Blick auf die unterstützten Funktionen auf unserer Github-[Seite](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) oder in unserer Produkt-[Dokumentation](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) werfen ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Schritte zum Hinzufügen von Anmerkungen zu DXF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) macht es für Net-Entwickler einfach, verschiedene Annotationstypen zu DXF-Dateien in jeder Net-basierten Anwendung hinzuzufügen, indem sie ein paar einfache Schritte implementieren.
        *   Erstellen Sie Antwortobjekte mit Kommentar und Datum.
        *   Erstellen Sie ein AreaAnnotation-Objekt, legen Sie Bereichsoptionen fest und fügen Sie Antworten hinzu.
        *   Erstellen Sie ein Annotator-Objekt und fügen Sie eine Bereichsanmerkung hinzu.
        *   Ausgabedatei speichern.
    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Annotation for Net APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.
        *   Betriebssysteme: Microsoft Windows, Linux, MacOS
        *   Entwicklungsumgebungen: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Laden Sie die neueste Version von GroupDocs.Annotation für .NET von [NuGet] herunter (https://www.nuget.org/packages/groupdocs.annotation).

############################# Preview ############################
preview_Add:
    enable: true
    title: Anmerkungsvorschau und Codebeispiel
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
    title_left: "Schritte zum Entfernen von Anmerkungen aus DXF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) erleichtert Net-Entwicklern das Entfernen von Anmerkungsdetails aus DXF-Dateien in jeder Net-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        *   Erstellen Sie Antwortobjekte mit Kommentar und Datum.
        *   Instanziieren Sie das SaveOptions-Objekt und legen Sie AnnotationTypes = AnnotationType.None fest.
        *   Rufen Sie die Speichermethode mit dem resultierenden Dokumentpfad oder -stream und dem SaveOptions-Objekt auf.

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
    title_left: "Schritte zum Bearbeiten von Anmerkungen aus DXF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) erleichtert Net-Entwicklern das Aktualisieren verschiedener Annotationseigenschaften aus DXF-Dateien in jeder Net-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        *   Instanziieren Sie das Annotator-Objekt mit dem Pfad oder Stream des Eingabedokuments mit instanziierten LoadOptions mit ImportAnnotations = true.
        *   Erstellen Sie eine AnnotationBase-Implementierung und legen Sie die ID der vorhandenen Anmerkung fest (wenn die Anmerkung mit dieser ID nicht gefunden wird, wird nichts geändert) oder die Pfadliste der Anmerkungen (alle vorhandenen Anmerkungen werden entfernt).
        *   Rufen Sie die Update-Methode des Annotator-Objekts mit übergebenen Annotationen auf.
        *   Rufen Sie die Speichermethode mit dem resultierenden Dokumentpfad oder -stream und dem SaveOptions-Objekt auf.

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
    title_left: "Schritte zum Extrahieren von Anmerkungen aus DXF in Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) macht es Netzentwicklern leicht, Dokumente mit Anmerkungen zu versehen und Anmerkungsinformationen aus DXF-Dateien in jeder netzbasierten Anwendung zu extrahieren, indem sie ein paar einfache Schritte implementieren.
        *   Erstellen Sie Antwortobjekte mit Kommentar und Datum.
        *   Instanziieren Sie das LoadOptions-Objekt und rufen Sie SetImportAnnotations mit dem Argument true auf.
        *   Definieren Sie eine Variable vom Typ List.
        *   Rufen Sie die get-Methode auf und geben Sie das Ergebnis an die obige Variable zurück.

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
    title: "Live-Demos zum Hinzufügen, Entfernen, Bearbeiten und Extrahieren von Anmerkungen zu Dokumenten und Bildern"
    content: |
        Fügen Sie jetzt Anmerkungen zur Datei DXF hinzu, entfernen Sie sie, bearbeiten Sie sie und extrahieren Sie sie, indem Sie die Website [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) besuchen. Die Live-Demo bietet folgende Vorteile

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dxf"
          title: "Informationen zum Dateiformat DXF"
          content: |
            DXF, Drawing Interchange Format oder Drawing Exchange Format, ist eine getaggte Datendarstellung einer AutoCAD-Zeichnungsdatei. Jedes Element in der Datei hat eine vorangestellte Ganzzahl, die als Gruppencode bezeichnet wird. Dieser Gruppencode stellt tatsächlich das folgende Element dar und gibt die Bedeutung eines Datenelements für einen bestimmten Objekttyp an. DXF ermöglicht die Darstellung nahezu aller benutzerdefinierten Informationen in einer Zeichnungsdatei. Das DXF-Dateiformat wurde von Autodesk als CAD-Datendateiformat für die Dateninteroperabilität zwischen AutoCAD und anderen Anwendungen entwickelt. Somit können Daten aus anderen Formaten in DXF und AutoCAD gemäß den Interoperabilitätsspezifikationen für DXF-Dateiformate importiert werden.

          link: "https://docs.fileformat.com/image/dxf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbeiten mit anderen gängigen Dokumentformaten"
    content: |
        Aktualisieren Sie die Anmerkungseigenschaften einiger gängiger Dateiformate wie unten angegeben.
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