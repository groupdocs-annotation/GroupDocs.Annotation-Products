---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DWG Annotation API Annotate v C#"
head_description: "Java API za ustvarjanje in označevanje priljubljenih vrst opomb iz DWG, slik, risb in oblik datotek dokumentov."

############################# Header ############################
title: "Označite DWG iz Jave"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Prenesite brezplačno preskusno različico"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "O GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API je knjižnica, ki vam omogoča dodajanje opomb v PDF, Word in druge dokumente v sistemu Mac, Windows ali Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) je izvorni Java API za upravljanje opomb s celovito podporo za ustvarjanje, dodajanje, urejanje, brisanje, ekstrahiranje in izvoz komentarjev iz slik in različnih drugih dokumentov. Celoten seznam podprtih formatov dokumentov si lahko ogledate na tej [strani](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ta knjižnica vam omogoča delo ne samo z dokumentom DWG, ampak tudi z mnogimi drugimi vrstami dokumentov, kot so Word, Excel, PowerPoint, Outlookova e-pošta, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad in mnogi drugi.
        GroupDocs.Annotation for Java API vam omogoča ustvarjanje in dodajanje novih opomb, urejanje opomb, ekstrahiranje komentarjev, opomb in njihovo odstranjevanje iz dokumentov. Knjižnica podpira 13 različnih vrst opomb, vključno z besedilom, poličrtijo, območjem, podčrtajem, točko, vodnim žigom, puščico, elipso, zamenjavo besedila, razdaljo, besedilnim poljem, redakcijo virov v dokumentih PDF, HTML, Microsoft Word, preglednicah, diagramih, predstavitvah, risbe, slike in številne druge oblike datotek.
        Primer (glejte spodaj) prikazuje delo z dokumentom DWG, v tem primeru si lahko ogledate glavne korake dela z GroupDocs. Opomba: nastavite licenco, odprite dokument, s katerim želite delati, ustvarite opombo, dodajanje podatkovnih objektov za nastavitev lastnosti opombe glede na vaše zahteve in shranjevanje rezultata na potrebno mesto. Prav tako si lahko podrobneje ogledate podprte funkcije na naši [strani github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) ali v [dokumentaciji našega izdelka](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Koraki za dodajanje opomb k DWG v Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) razvijalcem Java olajša dodajanje različnih vrst opomb datotekam DWG znotraj katere koli aplikacije, ki temelji na Javi, z implementacijo nekaj preprostih korakov.
        *   Ustvarite objekte odgovora s komentarjem in datumom.
        *   Ustvarite predmet AreaAnnotation, nastavite možnosti območja in dodajte odgovore.
        *   Ustvarite objekt Annotator in dodajte opombo območja.
        *   Shrani izhodno datoteko.
    title_right: "Sistemske zahteve"
    content_right: |
        API-ji GroupDocs.Annotation za Java so podprti na vseh večjih platformah in operacijskih sistemih. Preden izvedete spodnjo kodo, se prepričajte, da imate v sistemu nameščene naslednje predpogoje.
        *   Operacijski sistemi: Microsoft Windows, Linux, MacOS
        *   Razvojno okolje: NetBeans, Intellij IDEA, Eclipse itd
        *   Java Runtime Environment: Java 7 (1.7) in novejši
        *   Prenesite najnovejšo različico GroupDocs.Annotation za Javo iz [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Predogled pripisov in vzorec kode
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
    title_left: "Koraki za odstranitev opomb iz DWG v Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) razvijalcem Java olajša odstranjevanje podrobnosti opombe iz datotek DWG znotraj katere koli aplikacije, ki temelji na Javi, z implementacijo nekaj preprostih korakov.
        *   Ustvarite objekte odgovora s komentarjem in datumom.
        *   Instanciirajte objekt SaveOptions in nastavite AnnotationTypes = AnnotationType.None.
        *   Pokličite metodo shranjevanja z nastalo potjo dokumenta ali tokom in objektom SaveOptions.

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
    title_left: "Koraki za urejanje opomb iz DWG v Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) razvijalcem Java olajša posodabljanje različnih lastnosti opomb iz datotek DWG znotraj katere koli aplikacije, ki temelji na Javi, z implementacijo nekaj preprostih korakov.
        *   Instanciirajte objekt Annotator s potjo vhodnega dokumenta ali tok z instanciranimi LoadOptions z ImportAnnotations = true.
        *   Ustvarite implementacijo AnnotationBase in nastavite ID obstoječe opombe (če opomba s tem ID-jem ni najdena, ne bo nič spremenjeno) ali seznam poti opomb (vse obstoječe opombe bodo odstranjene).
        *   Pokličite metodo posodobitve objekta Annotator s posredovanimi opombami.
        *   Pokličite metodo shranjevanja z nastalo potjo dokumenta ali tokom in objektom SaveOptions.

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
    title_left: "Koraki za ekstrahiranje opomb iz DWG v Javi"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) razvijalcem Java olajša dodajanje opomb dokumentom in pridobivanje informacij o opombah iz datotek DWG znotraj katere koli aplikacije, ki temelji na Javi, z implementacijo nekaj preprostih korakov.
        *   Ustvarite objekte odgovora s komentarjem in datumom.
        *   Instanciirajte objekt LoadOptions in pokličite SetImportAnnotations z argumentom true.
        *   Definirajte spremenljivko s tipom List.
        *   Pokličite metodo get in vrnite rezultat zgornji spremenljivki.

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
    title: "Predstavitve v živo za dodajanje, odstranjevanje, urejanje, ekstrahiranje opomb v dokumente in slike"
    content: |
        Takoj dodajte, odstranite, uredite in izvlecite opombe v datoteko DWG tako, da obiščete spletno mesto [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Predstavitev v živo ima naslednje prednosti

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dwg"
          title: "O formatu datoteke DWG"
          content: |
            Datoteke s pripono DWG predstavljajo lastniške binarne datoteke, ki se uporabljajo za shranjevanje 2D in 3D načrtovalnih podatkov. Tako kot DXF, ki so datoteke ASCII, DWG predstavlja binarno obliko datoteke za risbe CAD (računalniško podprto načrtovanje). Vsebuje vektorsko sliko in metapodatke za predstavitev vsebine datotek CAD. Na voljo so brezplačni pregledovalniki za ogled datotek DWG v operacijskem sistemu Windows, kot je brezplačni Autodeskov DWG TrueView. Obstajajo tudi druge aplikacije tretjih oseb, ki podpirajo dostop do datotek DWG.

          link: "https://docs.fileformat.com/image/dwg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Delo z drugimi priljubljenimi formati dokumentov"
    content: |
        Posodobite lastnosti pripisov iz nekaterih priljubljenih formatov datotek, kot je navedeno spodaj.
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