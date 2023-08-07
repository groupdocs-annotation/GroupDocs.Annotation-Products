---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java VSX Annotation API Annotate u C#"
head_description: "Java API za stvaranje i označavanje popularnih vrsta komentara iz VSX, slika, crteža i formata datoteka dokumenata."

############################# Header ############################
title: "Označite VSX iz Jave"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Preuzmite besplatnu probnu verziju"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API je biblioteka koja vam omogućuje dodavanje komentara u PDF, Word i druge dokumente na Macu, Windowsu ili Ubuntuu. [GroupDocs.Annotation for Java](/annotation/java) izvorni je Java API za upravljanje komentarima sa sveobuhvatnom podrškom za stvaranje, dodavanje, uređivanje, brisanje, izdvajanje i izvoz komentara iz slika i raznih drugih dokumenata. Potpuni popis podržanih formata dokumenata možete vidjeti na ovoj [stranici](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ova biblioteka vam omogućuje rad ne samo s dokumentom VSX već i s mnogim drugim vrstama dokumenata kao što su Word, Excel, PowerPoint, Outlook e-pošta, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad i mnogi drugi.
        GroupDocs.Annotation for Java API omogućuje stvaranje i dodavanje novih bilješki, uređivanje komentara, izdvajanje komentara, komentara i njihovo uklanjanje iz dokumenata. Knjižnica podržava 13 različitih vrsta komentara, uključujući tekst, poliliniju, područje, podcrtavanje, točku, vodeni žig, strelicu, elipsu, zamjenu teksta, udaljenost, tekstualno polje, redakciju resursa u PDF-u, HTML-u, Microsoft Word dokumentima, proračunskim tablicama, dijagramima, prezentacijama, crteži, slike i mnogi drugi formati datoteka.
        Primjer (pogledajte dolje) demonstrira rad s VSX dokumentom, u ovom primjeru možete vidjeti glavne korake rada s GroupDocs. Napomena: Postavite licencu, otvorite dokument s kojim želite raditi, kreirajte bilježenje, dodavanje podatkovnih objekata za postavljanje svojstava bilježaka prema vašim zahtjevima i spremanje rezultata na potrebno mjesto. Također možete detaljnije pogledati podržane značajke na našoj github [stranici](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), ili u našoj [dokumentaciji] proizvoda (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Koraci za dodavanje komentara u VSX u Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) olakšava Java programerima dodavanje različitih vrsta komentara VSX datotekama unutar bilo koje aplikacije temeljene na Javi implementacijom nekoliko jednostavnih koraka.
        *   Stvorite objekte odgovora s komentarom i datumom.
        *   Stvorite objekt AreaAnnotation, postavite opcije područja i dodajte odgovore.
        *   Stvorite objekt Annotator i dodajte oznaku područja.
        *   Spremi izlaznu datoteku.
    title_right: "Zahtjevi sustava"
    content_right: |
        API-ji GroupDocs.Annotation za Java podržani su na svim glavnim platformama i operativnim sustavima. Prije izvršavanja koda u nastavku, provjerite imate li sljedeće preduvjete instalirane na vašem sustavu.
        *   Operativni sustavi: Microsoft Windows, Linux, MacOS
        *   Razvojno okruženje: NetBeans, Intellij IDEA, Eclipse itd
        *   Java Runtime Environment: Java 7 (1.7) i novije verzije
        *   Preuzmite najnoviju verziju GroupDocs.Annotation za Javu iz [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Pregled komentara i uzorak koda
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
    title_left: "Koraci za uklanjanje komentara iz VSX u Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) olakšava Java programerima uklanjanje detalja komentara iz datoteka VSX unutar bilo koje aplikacije temeljene na Javi implementacijom nekoliko jednostavnih koraka.
        *   Stvorite objekte odgovora s komentarom i datumom.
        *   Instancirajte objekt SaveOptions i postavite AnnotationTypes = AnnotationType.None.
        *   Pozovite metodu spremanja s rezultirajućom putanjom dokumenta ili tokom i objektom SaveOptions.

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
    title_left: "Koraci za uređivanje komentara iz VSX u Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) olakšava Java programerima ažuriranje različitih svojstava komentara iz VSX datoteka unutar bilo koje aplikacije temeljene na Javi implementacijom nekoliko jednostavnih koraka.
        *   Instancirajte Annotator objekt s ulaznom putanjom dokumenta ili tok s instanciranim LoadOptions s ImportAnnotations = true.
        *   Napravite implementaciju AnnotationBase i postavite ID postojeće zabilješke (ako zabilješka s tim ID-om nije pronađena, ništa se neće promijeniti) ili popis puta zabilješki (sve postojeće zabilješke bit će uklonjene).
        *   Pozovite metodu ažuriranja objekta Annotator s proslijeđenim komentarima.
        *   Pozovite metodu spremanja s rezultirajućom putanjom dokumenta ili tokom i objektom SaveOptions.

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
    title_left: "Koraci za izdvajanje komentara iz VSX u Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java programerima olakšava označavanje dokumenata i izdvajanje informacija o komentarima iz datoteka VSX unutar bilo koje aplikacije temeljene na Javi implementacijom nekoliko jednostavnih koraka.
        *   Stvorite objekte odgovora s komentarom i datumom.
        *   Instancirajte objekt LoadOptions i pozovite SetImportAnnotations s argumentom true.
        *   Definirajte varijablu tipom List.
        *   Pozovi metodu get i vrati rezultat gornjoj varijabli.

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
    title: "Demonstracije uživo za dodavanje, uklanjanje, uređivanje, izdvajanje komentara na dokumente i slike"
    content: |
        Dodajte, uklonite, uredite i ekstrahirajte komentare u datoteku VSX odmah tako da posjetite [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) web mjesto.
Demo uživo ima sljedeće prednosti

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsx"
          title: "O formatu datoteke VSX"
          content: |
            Datoteke s ekstenzijom .VSX odnose se na šablone koje se sastoje od crteža i oblika koji se koriste za izradu dijagrama u programu Microsoft Visio. VSX datoteke spremaju se u XML formatu datoteke i bile su podržane do Visio 2013. Oni se razlikuju od primarnog VSDX formata datoteke koji je uveden s Microsoft Visio 2013. VSX datoteke mogu se otvoriti u bilo kojem uređivaču teksta za pregled sadržaja.

          link: "https://docs.fileformat.com/image/vsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Rad s drugim popularnim formatima dokumenata"
    content: |
        Ažurirajte svojstva zabilješki iz nekih od popularnih formata datoteka kao što je navedeno u nastavku.
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