---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPTM Annotation API Annotate C#"
head_description: "Java API, lai izveidotu un anotētu populārus anotāciju veidus no PPTM, attēliem, zīmējumiem un dokumentu failu formātiem."

############################# Header ############################
title: "Anotējiet PPTM no Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Lejupielādēt bezmaksas izmēģinājuma versiju"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Par GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API ir bibliotēka, kas ļauj pievienot anotācijas PDF, Word un citiem dokumentiem operētājsistēmā Mac, Windows vai Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) ir vietējā Java API anotāciju pārvaldībai ar visaptverošu atbalstu attēlu un dažādu citu dokumentu anotāciju izveidei, pievienošanai, rediģēšanai, dzēšanai, izvilkšanai un eksportēšanai. Pilnu atbalstīto dokumentu formātu sarakstu varat skatīt šajā [lapā](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Šī bibliotēka ļauj strādāt ne tikai ar PPTM dokumentu, bet arī ar daudziem cita veida dokumentiem, piemēram, Word, Excel, PowerPoint, Outlook e-pastiem, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad un daudziem citiem.
        GroupDocs.Annotation for Java API ļauj izveidot un pievienot jaunas piezīmes, rediģēt anotācijas, iegūt komentārus, anotācijas un noņemt tos no dokumentiem. Bibliotēka atbalsta 13 dažādus anotāciju veidus, tostarp tekstu, daudzlīniju, apgabalu, pasvītrojumu, punktu, ūdenszīmi, bultiņu, elipsi, teksta aizstāšanu, attālumu, teksta lauku, resursu rediģēšanu PDF, HTML, Microsoft Word dokumentos, izklājlapās, diagrammās, prezentācijās, zīmējumi, attēli un daudzi citi failu formāti.
        Piemērā (lūdzu, skatiet tālāk) ir parādīts darbs ar PPTM dokumentu, šajā piemērā var redzēt galvenās darbības, kā strādāt ar GroupDocs. Anotācija: iestatiet licenci, atveriet dokumentu, ar kuru vēlaties strādāt, izveidojot anotācija, datu objektu pievienošana anotācijas rekvizītu iestatīšanai atbilstoši jūsu prasībām un rezultāta saglabāšana vajadzīgajā vietā. Varat arī skatīt sīkāku informāciju par atbalstītajām funkcijām mūsu github [lapā](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) vai mūsu produkta [dokumentācijā](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Darbības, lai pievienotu anotācijas failam PPTM Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Tas ļauj Java izstrādātājiem viegli pievienot dažādus anotāciju veidus PPTM failiem jebkurā Java lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidojiet atbildes objektus ar komentāru un datumu.
        *   Izveidojiet AreaAnnotation objektu, iestatiet apgabala opcijas un pievienojiet atbildes.
        *   Izveidojiet anotatora objektu un pievienojiet apgabala anotāciju.
        *   Saglabājiet izvades failu.
    title_right: "Sistēmas prasības"
    content_right: |
        GroupDocs.Annotation par Java API tiek atbalstītas visās lielākajās platformās un operētājsistēmās. Pirms tālāk norādītā koda izpildes, lūdzu, pārliecinieties, vai jūsu sistēmā ir instalēti šādi priekšnosacījumi.
        *   Operētājsistēmas: Microsoft Windows, Linux, MacOS
        *   Izstrādes vide: NetBeans, Intellij IDEA, Eclipse utt
        *   Java izpildlaika vide: Java 7 (1.7) un jaunāka versija
        *   Iegūstiet jaunāko GroupDocs.Annotation versiju Java no [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anotācijas priekšskatījums un koda paraugs
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
    title_left: "Darbības, lai noņemtu anotācijas no PPTM Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Tas ļauj Java izstrādātājiem vieglāk noņemt anotācijas informāciju no PPTM failiem jebkurā Java lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidojiet atbildes objektus ar komentāru un datumu.
        *   Izveidojiet objektu SaveOptions un iestatiet AnnotationTypes = AnnotationType.None.
        *   Izsauciet saglabāšanas metodi ar iegūto dokumenta ceļu vai straumi un SaveOptions objektu.

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
    title_left: "Darbības, lai rediģētu anotācijas no PPTM Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) atvieglo Java izstrādātājiem dažādu anotāciju rekvizītu atjaunināšanu no PPTM failiem jebkurā Java lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidot Annotatora objektu ar ievades dokumenta ceļu vai straumi ar instantierētām LoadOptions ar ImportAnnotations = true.
        *   Izveidojiet kādu AnnotationBase implementāciju un iestatiet esošās anotācijas ID (ja anotācija ar šo ID nav atrasta, nekas netiks mainīts) vai anotāciju ceļu sarakstu (visas esošās anotācijas tiks noņemtas).
        *   Izsaukt Annotator objekta atjaunināšanas metodi ar nodotām anotācijām.
        *   Izsauciet saglabāšanas metodi ar iegūto dokumenta ceļu vai straumi un SaveOptions objektu.

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
    title_left: "Darbības, lai izvilktu anotācijas no PPTM Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ļauj Java izstrādātājiem viegli anotēt dokumentus un izvilkt anotāciju informāciju no PPTM failiem jebkurā Java lietojumprogrammā, veicot dažas vienkāršas darbības.
        *   Izveidojiet atbildes objektus ar komentāru un datumu.
        *   Izveidojiet LoadOptions objektu un izsauciet SetImportAnnotations ar patiesu argumentu.
        *   Definējiet mainīgo ar tipu Saraksts.
        *   Izsauciet metodi get un atgrieziet rezultātu iepriekš norādītajam mainīgajam.

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
    title: "Tiešraides demonstrācijas, lai pievienotu, noņemtu, rediģētu un izvilktu anotācijas dokumentiem un attēliem"
    content: |
        Pievienojiet, noņemiet, rediģējiet un izvelciet anotācijas failam PPTM tūlīt, apmeklējot vietni [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Tiešraides demonstrācijai ir šādas priekšrocības

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pptm"
          title: "Par PPTM faila formātu"
          content: |
            Faili ar PPTM paplašinājumu ir makro iespējoti prezentāciju faili, kas izveidoti ar Microsoft PowerPoint 2007 vai jaunāku versiju. Tie ir līdzīgi PPTX failiem ar atšķirību, ka sānu malas nevar izpildīt makro, lai gan tajos var būt makro. PPTM failus var rediģēt, atverot tos programmā Microsoft PowerPoint un atjauninot saturu. Vēl viens līdzīgs formāts ir PPSM, taču pēc noklusējuma tas ir tikai lasāms un pēc atvēršanas sāk slaidrādi. PPTM, tāpat kā PPTX, satur slaidus dažādiem prezentācijas elementiem, piemēram, tekstam, attēliem, videoklipiem, grafikiem un citiem saistītiem materiāliem.

          link: "https://docs.fileformat.com/image/pptm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Darbs ar citiem populāriem dokumentu formātiem"
    content: |
        Atjauniniet anotācijas rekvizītus no dažiem populāriem failu formātiem, kā norādīts tālāk.
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