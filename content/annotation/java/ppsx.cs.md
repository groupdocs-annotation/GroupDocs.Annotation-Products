---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPSX Anotace API Anotace v C#"
head_description: "Java API pro vytváření a komentování oblíbených typů anotací z PPSX, obrázků, nákresů a formátů souborů dokumentů."

############################# Header ############################
title: "Anotace PPSX z Javy"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Stáhněte si zkušební verzi zdarma"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API je knihovna, která umožňuje přidávat anotace do PDF, Wordu a dalších dokumentů na Mac, Windows nebo Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) je nativní Java API pro správu anotací s komplexní podporou pro vytváření, přidávání, úpravy, mazání, extrahování a export anotací z obrázků a různých dalších dokumentů. Úplný seznam podporovaných formátů dokumentů můžete vidět na této [stránce](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Tato knihovna vám umožňuje pracovat nejen s dokumentem PPSX, ale také s mnoha dalšími typy dokumentů, jako jsou Word, Excel, PowerPoint, Outlook e-maily, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad a mnoho dalších.
        GroupDocs.Annotation for Java API umožňuje vytvářet a přidávat nové poznámky, upravovat anotace, extrahovat komentáře, anotace a odstraňovat je z dokumentů. Knihovna podporuje 13 různých typů anotací, včetně textu, křivky, plochy, podtržení, bodu, vodoznaku, šipky, elipsy, nahrazení textu, vzdálenosti, textového pole, úpravy zdrojů v PDF, HTML, dokumentů Microsoft Word, tabulek, diagramů, prezentací, výkresy, obrázky a mnoho dalších formátů souborů.
        Příklad (viz níže) ukazuje práci s dokumentem PPSX, v tomto příkladu můžete vidět hlavní kroky, jak pracovat s GroupDocs. Anotace: Nastavte licenci, otevřete dokument, se kterým chcete pracovat, vytvořte anotace, přidání datových objektů pro nastavení vlastností anotace podle vašich požadavků a uložení výsledku na potřebné místo. Také se můžete podrobněji podívat na podporované funkce na naší github [stránce](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) nebo v našem produktu [dokumentace](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Postup přidání anotací do souboru PPSX v jazyce Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) usnadňuje vývojářům jazyka Java přidávat různé typy anotací do souborů PPSX v jakékoli aplikaci založené na jazyce Java implementací několika snadných kroků.
        *   Vytvořte objekty odpovědi s komentářem a datem.
        *   Vytvořte objekt AreaAnnotation, nastavte možnosti oblasti a přidejte odpovědi.
        *   Vytvořte objekt Annotator a přidejte popis oblasti.
        *   Uložit výstupní soubor.
    title_right: "Požadavky na systém"
    content_right: |
        GroupDocs.Annotation for Java API jsou podporovány na všech hlavních platformách a operačních systémech. Před spuštěním níže uvedeného kódu se prosím ujistěte, že máte na svém systému nainstalovány následující předpoklady.
        *   Operační systémy: Microsoft Windows, Linux, MacOS
        *   Vývojové prostředí: NetBeans, Intellij IDEA, Eclipse atd
        *   Java Runtime Environment: Java 7 (1.7) a vyšší
        *   Získejte nejnovější verzi GroupDocs.Annotation pro Java z [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Náhled anotace a ukázka kódu
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
    title_left: "Kroky k odstranění anotací z PPSX v Javě"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) usnadňuje vývojářům jazyka Java odstranění podrobností anotací ze souborů PPSX v jakékoli aplikaci založené na jazyce Java implementací několika snadných kroků.
        *   Vytvořte objekty odpovědi s komentářem a datem.
        *   Vytvořte instanci objektu SaveOptions a nastavte AnnotationTypes = AnnotationType.None.
        *   Volejte metodu uložení s výslednou cestou dokumentu nebo streamem a objektem SaveOptions.

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
    title_left: "Kroky k úpravě anotací z PPSX v Javě"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) usnadňuje vývojářům jazyka Java aktualizaci různých vlastností anotací ze souborů PPSX v jakékoli aplikaci založené na jazyce Java implementací několika snadných kroků.
        *   Vytvořte instanci objektu Annotator se vstupní cestou dokumentu nebo streamu s instancí LoadOptions s ImportAnnotations = true.
        *   Vytvořte nějakou implementaci AnnotationBase a nastavte Id existující anotace (pokud anotace s tímto Id nebude nalezena, nic se nezmění) nebo seznam cest anotací (všechny existující anotace budou odstraněny).
        *   Zavolejte metodu aktualizace objektu Annotator s předanými anotacemi.
        *   Volejte metodu uložení s výslednou cestou dokumentu nebo streamem a objektem SaveOptions.

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
    title_left: "Kroky k extrahování anotací z PPSX v Javě"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) usnadňuje vývojářům jazyka Java anotaci dokumentů a extrahování anotačních informací ze souborů PPSX v jakékoli aplikaci založené na Java implementací několika snadných kroků.
        *   Vytvořte objekty odpovědi s komentářem a datem.
        *   Vytvořte instanci objektu LoadOptions a zavolejte SetImportAnnotations s argumentem true.
        *   Definujte proměnnou typem List.
        *   Zavolejte metodu get a vraťte výsledek do proměnné výše.

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
    title: "Živé ukázky pro přidání, odebrání, úpravu, extrahování anotací do dokumentů a obrázků"
    content: |
        Přidávejte, odebírejte, upravujte a extrahujte anotace do souboru PPSX právě teď na webu [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Živé demo má následující výhody

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppsx"
          title: "O formátu souboru PPSX"
          content: |
            Soubor PPSX, Power Point Slide Show, je vytvořen pomocí aplikace Microsoft PowerPoint 2007 a vyšší pro účely prezentace. Jedná se o aktualizaci formátu souboru PPS, který byl podporován verzemi Microsoft PowerPoint 97-2003. Když je soubor PPSX sdílen s jiným uživatelem a otevřen, spustí se jako PowerPoint show na rozdíl od souboru PPTX, který se otevře v upravitelném režimu. Pořadí prezentace je stejné jako v původní prezentaci. Všechny snímky doprovázejí obrázky, zvuky a další vložená média doprovázejí snímky prezentace do PPSX během prezentace.

          link: "https://docs.fileformat.com/image/ppsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Práce s jinými oblíbenými formáty dokumentů"
    content: |
        Aktualizujte vlastnosti anotace z některých oblíbených formátů souborů, jak je uvedeno níže.
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