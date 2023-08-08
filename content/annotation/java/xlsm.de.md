---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java XLSM Annotation API Annotieren in C#"
head_description: "Java-API zum Erstellen und Kommentieren beliebter Anmerkungstypen aus XLSM, Bildern, Zeichnungen und Dokumentdateiformaten."

############################# Header ############################
title: "Kommentieren Sie XLSM aus Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download kostenlose Testversion"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Annotation für Java API"
    content: |
        GroupDocs.Annotation for Java API ist eine Bibliothek, mit der Sie Anmerkungen zu PDF-, Word- und anderen Dokumenten auf Mac, Windows oder Ubuntu hinzufügen können. [GroupDocs.Annotation for Java](/annotation/java) ist eine native Java-API zum Verwalten von Anmerkungen mit umfassender Unterstützung für das Erstellen, Hinzufügen, Bearbeiten, Löschen, Extrahieren und Exportieren von Anmerkungen aus Bildern und verschiedenen anderen Dokumenten. Die vollständige Liste der unterstützten Dokumentformate finden Sie auf dieser [Seite](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Mit dieser Bibliothek können Sie nicht nur mit XLSM-Dokumenten arbeiten, sondern auch mit vielen anderen Dokumenttypen wie Word, Excel, PowerPoint, Outlook-E-Mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad und vielen anderen.
        Mit der GroupDocs.Annotation für Java-API können Sie neue Notizen erstellen und hinzufügen, Anmerkungen bearbeiten, Kommentare und Anmerkungen extrahieren und sie aus Dokumenten entfernen. Die Bibliothek unterstützt 13 verschiedene Anmerkungstypen, darunter Text, Polylinie, Fläche, Unterstreichung, Punkt, Wasserzeichen, Pfeil, Ellipse, Textersetzung, Abstand, Textfeld, Ressourcenschwärzung in PDF, HTML, Microsoft Word-Dokumenten, Tabellenkalkulationen, Diagrammen, Präsentationen, Zeichnungen, Bilder und viele andere Dateiformate.
        Das Beispiel (siehe unten) zeigt die Arbeit mit dem Dokument XLSM. In diesem Beispiel können Sie die Hauptschritte für die Arbeit mit GroupDocs.Annotation sehen: Richten Sie eine Lizenz ein, öffnen Sie ein Dokument, mit dem Sie arbeiten möchten, und erstellen Sie ein Annotation, Hinzufügen von Datenobjekten zum Festlegen von Annotationseigenschaften gemäß Ihren Anforderungen und Speichern des Ergebnisses am erforderlichen Ort. Außerdem können Sie einen detaillierteren Blick auf die unterstützten Funktionen auf unserer Github-[Seite](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) oder in unserer Produkt-[Dokumentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Schritte zum Hinzufügen von Anmerkungen zu XLSM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) erleichtert Java-Entwicklern das Hinzufügen verschiedener Annotationstypen zu XLSM-Dateien in jeder Java-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        *   Erstellen Sie Antwortobjekte mit Kommentar und Datum.
        *   Erstellen Sie ein AreaAnnotation-Objekt, legen Sie Bereichsoptionen fest und fügen Sie Antworten hinzu.
        *   Erstellen Sie ein Annotator-Objekt und fügen Sie eine Bereichsanmerkung hinzu.
        *   Ausgabedatei speichern.
    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Annotation für Java-APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.
        *   Betriebssysteme: Microsoft Windows, Linux, MacOS
        *   Entwicklungsumgebung: NetBeans, Intellij IDEA, Eclipse usw
        *   Java-Laufzeitumgebung: Java 7 (1.7) und höher
        *   Holen Sie sich die neueste Version von GroupDocs.Annotation für Java aus dem [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anmerkungsvorschau und Codebeispiel
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
    title_left: "Schritte zum Entfernen von Anmerkungen aus XLSM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) erleichtert Java-Entwicklern das Entfernen von Anmerkungsdetails aus XLSM-Dateien in jeder Java-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        *   Erstellen Sie Antwortobjekte mit Kommentar und Datum.
        *   Instanziieren Sie das SaveOptions-Objekt und legen Sie AnnotationTypes = AnnotationType.None fest.
        *   Rufen Sie die Speichermethode mit dem resultierenden Dokumentpfad oder -stream und dem SaveOptions-Objekt auf.

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
    title_left: "Schritte zum Bearbeiten von Anmerkungen aus XLSM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) erleichtert Java-Entwicklern das Aktualisieren verschiedener Annotationseigenschaften aus XLSM-Dateien in jeder Java-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        *   Instanziieren Sie das Annotator-Objekt mit dem Pfad oder Stream des Eingabedokuments mit instanziierten LoadOptions mit ImportAnnotations = true.
        *   Erstellen Sie eine AnnotationBase-Implementierung und legen Sie die ID der vorhandenen Anmerkung fest (wenn die Anmerkung mit dieser ID nicht gefunden wird, wird nichts geändert) oder die Pfadliste der Anmerkungen (alle vorhandenen Anmerkungen werden entfernt).
        *   Rufen Sie die Update-Methode des Annotator-Objekts mit übergebenen Annotationen auf.
        *   Rufen Sie die Speichermethode mit dem resultierenden Dokumentpfad oder -stream und dem SaveOptions-Objekt auf.

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
    title_left: "Schritte zum Extrahieren von Anmerkungen aus XLSM in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) macht es Java-Entwicklern durch die Implementierung einiger einfacher Schritte leicht, Dokumente mit Anmerkungen zu versehen und Anmerkungsinformationen aus XLSM-Dateien in jeder Java-basierten Anwendung zu extrahieren.
        *   Erstellen Sie Antwortobjekte mit Kommentar und Datum.
        *   Instanziieren Sie das LoadOptions-Objekt und rufen Sie SetImportAnnotations mit dem Argument true auf.
        *   Definieren Sie eine Variable vom Typ List.
        *   Rufen Sie die get-Methode auf und geben Sie das Ergebnis an die obige Variable zurück.

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
    title: "Live-Demos zum Hinzufügen, Entfernen, Bearbeiten und Extrahieren von Anmerkungen zu Dokumenten und Bildern"
    content: |
        Fügen Sie jetzt Anmerkungen zur Datei XLSM hinzu, entfernen Sie sie, bearbeiten Sie sie und extrahieren Sie sie, indem Sie die Website [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) besuchen. Die Live-Demo bietet folgende Vorteile

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsm"
          title: "Informationen zum Dateiformat XLSM"
          content: |
            Dateien mit der Erweiterung XLSM sind eine Art Tabellenkalkulationsdatei, die Makros unterstützt. Aus Anwendungssicht handelt es sich bei einem Makro um eine Reihe von Anweisungen, die zur Automatisierung von Prozessen verwendet werden. Ein Makro wird verwendet, um die Schritte aufzuzeichnen, die wiederholt ausgeführt werden, und erleichtert die Ausführung der Aktionen durch erneutes Ausführen des Makros. Makros werden mit Microsoft Visual Basic for Applications (VBA) aus der Excel-Arbeitsmappe heraus mit dem Visual Basic-Editor programmiert und können direkt von dort ausgeführt/debuggt werden.

          link: "https://docs.fileformat.com/image/xlsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbeiten mit anderen gängigen Dokumentformaten"
    content: |
        Aktualisieren Sie die Anmerkungseigenschaften einiger gängiger Dateiformate wie unten angegeben.
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