---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPS Anotácia API Anotácia v C#"
head_description: "Java API na vytváranie a komentovanie populárnych typov anotácií z PPS, obrázkov, nákresov a formátov súborov dokumentov."

############################# Header ############################
title: "Anotujte súbor PPS z jazyka Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Stiahnite si bezplatnú skúšobnú verziu"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API je knižnica, ktorá vám umožňuje pridávať anotácie do PDF, Wordu a iných dokumentov na Mac, Windows alebo Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) je natívne Java API na správu anotácií s komplexnou podporou pre vytváranie, pridávanie, upravovanie, odstraňovanie, extrahovanie a exportovanie anotácií z obrázkov a rôznych iných dokumentov. Úplný zoznam podporovaných formátov dokumentov si môžete pozrieť na tejto [stránke](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Táto knižnica vám umožňuje pracovať nielen s dokumentom PPS, ale aj s mnohými ďalšími typmi dokumentov, ako sú Word, Excel, PowerPoint, Outlook e-maily, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad a mnoho ďalších.
        GroupDocs.Annotation for Java API vám umožňuje vytvárať a pridávať nové poznámky, upravovať anotácie, extrahovať komentáre, anotácie a odstraňovať ich z dokumentov. Knižnica podporuje 13 rôznych typov anotácií vrátane textu, polyline, oblasti, podčiarknutia, bodu, vodoznaku, šípky, elipsy, nahradenia textu, vzdialenosti, textového poľa, úpravy zdrojov v PDF, HTML, dokumentov Microsoft Word, tabuliek, diagramov, prezentácií, kresby, obrázky a mnoho ďalších formátov súborov.
        Príklad (pozri nižšie) ukazuje prácu s dokumentom PPS, v tomto príklade môžete vidieť hlavné kroky, ako pracovať s GroupDocs. Anotácia: Nastavte licenciu, otvorte dokument, s ktorým chcete pracovať, vytvorte anotáciu, pridanie dátových objektov na nastavenie vlastností anotácie podľa vašich požiadaviek a uloženie výsledku na potrebné miesto. Môžete si tiež pozrieť podrobnejšie informácie o podporovaných funkciách na našej [stránke github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) alebo v našom produkte [dokumentácia](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Kroky na pridanie anotácií do súboru PPS v jazyku Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) uľahčuje vývojárom jazyka Java pridávanie rôznych typov anotácií do súborov PPS v rámci akejkoľvek aplikácie založenej na jazyku Java implementáciou niekoľkých jednoduchých krokov.
        *   Vytvorte objekty odpovede s komentárom a dátumom.
        *   Vytvorte objekt AreaAnnotation, nastavte možnosti oblasti a pridajte odpovede.
        *   Vytvorte objekt anotátora a pridajte anotáciu oblasti.
        *   Uložiť výstupný súbor.
    title_right: "Požiadavky na systém"
    content_right: |
        GroupDocs.Annotation for Java API sú podporované na všetkých hlavných platformách a operačných systémoch. Pred spustením nižšie uvedeného kódu sa uistite, že máte vo svojom systéme nainštalované nasledujúce predpoklady.
        *   Operačné systémy: Microsoft Windows, Linux, MacOS
        *   Vývojové prostredie: NetBeans, Intellij IDEA, Eclipse atď
        *   Java Runtime Environment: Java 7 (1.7) a vyššie
        *   Získajte najnovšiu verziu GroupDocs.Annotation pre Java z [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Ukážka anotácie a ukážka kódu
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
    title_left: "Kroky na odstránenie anotácií zo súboru PPS v jazyku Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) uľahčuje vývojárom jazyka Java odstraňovanie podrobností anotácií zo súborov PPS v akejkoľvek aplikácii založenej na jazyku Java implementáciou niekoľkých jednoduchých krokov.
        *   Vytvorte objekty odpovede s komentárom a dátumom.
        *   Okamžite vytvorte objekt SaveOptions a nastavte AnnotationTypes = AnnotationType.None.
        *   Zavolajte metódu uloženia s výslednou cestou dokumentu alebo streamom a objektom SaveOptions.

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
    title_left: "Kroky na úpravu anotácií zo súboru PPS v jazyku Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) uľahčuje vývojárom Java aktualizovať rôzne vlastnosti anotácií zo súborov PPS v akejkoľvek aplikácii založenej na jazyku Java implementáciou niekoľkých jednoduchých krokov.
        *   Okamžitý objekt Annotator so vstupnou cestou dokumentu alebo stream s inštanciou LoadOptions s ImportAnnotations = true.
        *   Vytvorte nejakú implementáciu AnnotationBase a nastavte Id existujúcej anotácie (ak sa anotácia s týmto Id nenájde, nič sa nezmení) alebo zoznam ciest anotácií (všetky existujúce anotácie budú odstránené).
        *   Zavolajte metódu aktualizácie objektu Annotator s odovzdanými anotáciami.
        *   Zavolajte metódu uloženia s výslednou cestou dokumentu alebo streamom a objektom SaveOptions.

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
    title_left: "Kroky na extrahovanie anotácií zo súboru PPS v jazyku Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) uľahčuje vývojárom jazyka Java anotáciu dokumentov a extrahovanie informácií o anotáciách zo súborov PPS v akejkoľvek aplikácii založenej na jazyku Java implementáciou niekoľkých jednoduchých krokov.
        *   Vytvorte objekty odpovede s komentárom a dátumom.
        *   Vytvorte instanciu objektu LoadOptions a zavolajte SetImportAnnotations s argumentom true.
        *   Definujte premennú typom List.
        *   Zavolajte metódu get a vráťte výsledok do premennej vyššie.

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
    title: "Živé ukážky na pridanie, odstránenie, úpravu, extrahovanie anotácií do dokumentov a obrázkov"
    content: |
        Pridávajte, odstraňujte, upravujte a extrahujte anotácie do súboru PPS práve teraz na webovej lokalite [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Živá ukážka má nasledujúce výhody

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pps"
          title: "Informácie o formáte súboru PPS"
          content: |
            PPS, PowerPoint Slide Show, súbory sa vytvárajú pomocou programu Microsoft PowerPoint na účely prezentácie. Čítanie a vytváranie súborov PPS podporuje Microsoft PowerPoint 97-2003. Najnovšia verzia tohto formátu súboru je PPSX, ktorý je založený na štandardoch Office OpenXML. Súbory PPS možno stále čítať v najnovších verziách programu Microsoft PowerPoint, ale novovytvorené súbory je možné uložiť iba vo formáte súboru PPSX. Keď je súbor PPS zdieľaný s iným používateľom a otvorený, spustí sa ako Powerpoint show na rozdiel od súboru PPT, ktorý sa otvára v režime úprav.

          link: "https://docs.fileformat.com/image/pps/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Práca s inými populárnymi formátmi dokumentov"
    content: |
        Aktualizujte vlastnosti anotácií z niektorých populárnych formátov súborov, ako je uvedené nižšie.
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