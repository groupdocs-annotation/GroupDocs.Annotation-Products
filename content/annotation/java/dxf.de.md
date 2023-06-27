
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/dxf"/>

############################# Head ############################
head_title: "Entfernen Anmerkungen aus DXF in der Java-Anwendung"
head_description: "Java API zum Erstellen und Entfernen beliebter Anmerkungstypen aus DXF, Bilder, Zeichnungen und Dokumentdateiformate."

############################# Header ############################
title: "Kommentieren Sie DXF aus Java"
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
        img_alt: "GroupDocs.Annotation für Java"
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
    title: "Über GroupDocs.Annotation für die Java-API"
    content: |
        GroupDocs.Annotation for Java API ist eine Bibliothek, mit der Sie Anmerkungen zu PDF-, Word- und anderen Dokumenten auf Mac, Windows oder Ubuntu hinzufügen können. [GroupDocs.Annotation für Java](/annotation/java) ist eine native Java-API zum Verwalten von Anmerkungen mit umfassender Unterstützung für das Erstellen, Hinzufügen, Bearbeiten, Löschen, Extrahieren und Exportieren von Anmerkungen Bilder und verschiedene andere Dokumente. Die vollständige Liste der unterstützten Dokumentformate finden Sie auf dieser [Seite](https://docs.groupdocs.com/annotation/java/supported-document-formats/).

        Mit dieser Bibliothek können Sie nicht nur mit DXF-Dokumenten arbeiten, sondern auch mit vielen anderen Dokumenttypen wie Word, Excel, PowerPoint, Outlook-E-Mails, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad und vielen anderen.

        Mit der GroupDocs.Annotation for Java-API können Sie neue Notizen erstellen und hinzufügen, edit Annotationen, extract Kommentare und Anmerkungen und entfernen sie aus Dokumenten. Die Bibliothek unterstützt 13 verschiedene Anmerkungstypen, darunter Text, Polylinie, Fläche, Unterstreichung, Punkt, Wasserzeichen, Pfeil, Ellipse, Textersetzung, Abstand, Textfeld, Ressourcenschwärzung in PDF, HTML, Microsoft Word-Dokumenten, Tabellenkalkulationen, Diagrammen, Präsentationen, Zeichnungen, Bilder und viele andere Dateiformate.

        Das Beispiel (siehe unten) zeigt die Arbeit mit einem DXF-Dokument. In diesem Beispiel können Sie die Hauptschritte für die Arbeit mit GroupDocs sehen. Anmerkung: Richten Sie eine Lizenz ein, öffnen Sie ein Dokument, mit dem Sie arbeiten möchten, und erstellen Sie ein Annotation, Hinzufügen von Datenobjekten zum Festlegen von Annotationseigenschaften gemäß Ihren Anforderungen und Speichern des Ergebnisses am erforderlichen Ort. Außerdem können Sie einen detaillierteren Blick auf die unterstützten Funktionen auf unserer Github-[Seite](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) oder in unserer Produkt [dokumentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Schritte zum Hinzufügen von Anmerkungen aus DXF in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) erleichtert Java-Entwicklern das Hinzufügen verschiedener Anmerkungstypen zu DXF-Dateien in jeder Java-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        * Antwortobjekte mit Kommentar und Datum erstellen.
        * Erstellen Sie ein AreaAnnotation-Objekt, legen Sie Bereichsoptionen fest und fügen Sie Antworten hinzu.
        * Erstellen Sie ein Annotator-Objekt und fügen Sie eine Bereichsanmerkung hinzu.
        * Ausgabedatei speichern.
    title_right: "System Anforderungen"
    content_right: |
        GroupDocs.Annotation für Java-APIs werden auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Bevor Sie den folgenden Code ausführen, stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem System installiert sind.
        * Betriebssysteme: Microsoft Windows, Linux, MacOS
        * Entwicklungsumgebung: NetBeans, Intellij IDEA, Eclipse usw
        * Java Runtime Environment: Java 7 (1.7) und höher
        * Holen Sie sich die neueste Version von GroupDocs.Annotation für Java aus dem [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    Titel: „Anmerkungsvorschau und Codebeispiel“
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        „Java
        // Eine Instanz der Reply-Klasse erstellen und Kommentare hinzufügen
        Reply firstReply = new Reply();
        firstReply.setComment("Erster Kommentar");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Zweiter Kommentar");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Eine Instanz der AreaAnnotation-Klasse erstellen und Optionen festlegen
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("Dies ist eine Bereichsanmerkung");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Eine Instanz der Annotator-Klasse erstellen
        Annotator annotator = new Annotator("input.bmp");
        
        // Anmerkung hinzufügen
        annotator.add(area);
        
        // Speichern unter
        annotator.save("output.bmp");
        annotator.dispose();
        „

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Schritte zum Entfernen von Anmerkungen aus DXF in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) erleichtert Java-Entwicklern das Entfernen von Anmerkungsdetails aus DXF-Dateien in jeder Java-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        * Antwortobjekte mit Kommentar und Datum erstellen.
        * Instanziieren Sie das SaveOptions-Objekt und legen Sie AnnotationTypes = AnnotationType.None fest.
        * Rufen Sie die Speichermethode mit dem resultierenden Dokumentpfad oder -stream und dem SaveOptions-Objekt auf.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        „Java
        // Eine Instanz der Annotator-Klasse erstellen
        Annotator annotator = new Annotator("C://input.bmp");

        // Annotation nach Set-Typ entfernen None
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Anmerkung in Ausgabedatei speichern
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        „

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Schritte zum Bearbeiten von Anmerkungen aus DXF in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) erleichtert Java-Entwicklern das Aktualisieren verschiedener Anmerkungseigenschaften aus DXF-Dateien in jeder Java-basierten Anwendung durch die Implementierung einiger einfacher Schritte.
        * Instanziieren Sie das Annotator-Objekt mit dem Pfad oder Stream des Eingabedokuments mit instanziierten LoadOptions mit ImportAnnotations = true.
        * Erstellen Sie eine AnnotationBase-Implementierung und legen Sie die ID der vorhandenen Anmerkung fest (wenn die Anmerkung mit dieser ID nicht gefunden wird, wird nichts geändert) oder die Pfadliste der Anmerkungen (alle vorhandenen Anmerkungen werden entfernt).
        * Rufen Sie die Update-Methode des Annotator-Objekts mit übergebenen Annotationen auf.
        * Rufen Sie die Speichermethode mit dem resultierenden Dokumentpfad oder -stream und dem SaveOptions-Objekt auf.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        „Java
        String OutputPath = "UpdateAnnotation.bmp";

        // Eine Instanz der Annotator-Klasse erstellen
        Annotator annotator = new Annotator("input.bmp");
        
        // Erstellen Sie eine Instanz der Reply-Klasse für das erste Beispiel und fügen Sie Kommentare hinzu
        Reply reply1 = new Reply();
        reply1.setComment("Ursprünglicher erster Kommentar");
        Reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Ursprünglicher zweiter Kommentar");
        Reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Eine Instanz der AreaAnnotation-Klasse erstellen und Optionen festlegen
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(neues Rechteck(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("Dies ist die Originalanmerkung");
        original.setReplies(replies);
        
        // Originalanmerkung hinzufügen
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Kommentiertes Dokument öffnen
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Erstellen Sie eine Instanz der Reply-Klasse für das erste Update-Beispiel
        Reply reply3 = new Reply();
        reply3.setComment("Erster Kommentar aktualisiert");
        Reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Zweiter Kommentar aktualisiert");
        Reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Schlagen Sie vor, dass wir einige Eigenschaften der vorhandenen Anmerkung ändern möchten
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(neues Rechteck(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("Dies ist eine aktualisierte Anmerkung");
        updated.setReplies(replies1);
        
        // Anmerkung aktualisieren und speichern
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        „

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Schritte zum Extrahieren von Anmerkungen aus DXF in Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) macht es Java-Entwicklern einfach, Dokumente mit Anmerkungen zu versehen und Anmerkungsinformationen aus DXF-Dateien in jeder Java-basierten Anwendung zu extrahieren, indem sie ein paar einfache Schritte implementieren.
        * Antwortobjekte mit Kommentar und Datum erstellen.
        * Instanziieren Sie das LoadOptions-Objekt und rufen Sie SetImportAnnotations mit dem Argument true auf.
        * Definieren Sie eine Variable vom Typ Liste.
        * Rufen Sie die get-Methode auf und geben Sie das Ergebnis an die obige Variable zurück.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        „Java
        // Zur Verwendung dieses Beispiels muss die Eingabedatei („annotated.bmp“) Anmerkungen enthalten
        LoadOptions loadOptions = new LoadOptions();
        
        // Eine Instanz der Annotator-Klasse erstellen und Anmerkungen abrufen
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        „

############################# Demos ############################
demos:
    enable: true
    title: "Live-Demos zum Extrahieren von Anmerkungen"
    content: |
        Sehen Sie sich jetzt Anmerkungen aus der Datei DXF an und entfernen Sie sie, indem Sie die Website [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) besuchen.
        Die Live-Demo bietet folgende Vorteile

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dxf"
          title: "Informationen zum DXF-Dateiformat"
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