---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPSM Annotation API Annotate in C#"
head_description: "Java API om gewilde annotasietipes van PPSM, beelde, tekeninge en dokumentlêerformate te skep en te annoteer."

############################# Header ############################
title: "Annoteer PPSM vanaf Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Laai gratis proeflopie af"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Oor GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API is 'n biblioteek wat jou toelaat om aantekeninge by PDF, Word en ander dokumente op Mac, Windows of Ubuntu te voeg. [GroupDocs.Annotation for Java](/annotation/java) is 'n inheemse Java API vir die bestuur van aantekeninge met omvattende ondersteuning vir die skep, byvoeging, redigeer, uitvee, onttrek en uitvoer van aantekeninge van beelde en verskeie ander dokumente. Die volledige lys van ondersteunde dokumentformate wat jy op hierdie [bladsy] kan sien (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Hierdie biblioteek laat jou toe om nie net met PPSM dokument te werk nie, maar ook met baie ander tipe dokumente soos Word, Excel, PowerPoint, Outlook-e-posse, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad en vele ander.
        Die GroupDocs.Annotation for Java API laat jou toe om nuwe notas te skep en by te voeg, aantekeninge te wysig, opmerkings, annotasies te onttrek en dit uit dokumente te verwyder. Die biblioteek ondersteun 13 verskillende aantekeningtipes, insluitend teks, polilyn, area, onderstreep, punt, watermerk, pyl, ellips, teksvervanging, afstand, teksveld, hulpbronredaksie in PDF, HTML, Microsoft Word-dokumente, sigblaaie, diagramme, aanbiedings, tekeninge, beelde en baie ander lêerformate.
        Die voorbeeld (sien asseblief hieronder) demonstreer werk met PPSM dokument, in hierdie voorbeeld kan jy die hoofstappe sien van hoe om met GroupDocs te werk. Aantekening: Stel 'n lisensie op, maak 'n dokument oop waarmee jy wil werk, skep 'n annotasie, byvoeging van data-objekte om annotasie-eienskappe volgens u vereistes te stel en die resultaat op die nodige plek te stoor. U kan ook meer gedetailleerd kyk na die ondersteunde kenmerke op ons github [bladsy](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), of in ons produk [dokumentasie](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Stappe om aantekeninge by PPSM in Java te voeg"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maak dit maklik vir Java-ontwikkelaars om verskeie aantekeningtipes by PPSM-lêers binne enige Java-gebaseerde toepassing by te voeg deur 'n paar maklike stappe te implementeer.
        *   Skep Antwoord-objekte met kommentaar en datum.
        *   Skep AreaAnnotation-objek, stel area-opsies in en voeg antwoorde by.
        *   Skep Annotator-objek en voeg area-aantekening by.
        *   Stoor uitvoerlêer.
    title_right: "Stelselvereistes"
    content_right: |
        GroupDocs.Annotation vir Java API's word op alle groot platforms en bedryfstelsels ondersteun. Voordat u die kode hieronder uitvoer, maak asseblief seker dat u die volgende voorvereistes op u stelsel geïnstalleer het.
        *   Bedryfstelsels: Microsoft Windows, Linux, MacOS
        *   Ontwikkelingsomgewing: NetBeans, Intellij IDEA, Eclipse ens
        *   Java Runtime Environment: Java 7 (1.7) en hoër
        *   Kry die nuutste weergawe van GroupDocs.Annotation for Java vanaf [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Aantekeningvoorskou en kodevoorbeeld
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
    title_left: "Stappe om aantekeninge van PPSM in Java te verwyder"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maak dit makliker vir Java-ontwikkelaars om aantekeningbesonderhede van PPSM-lêers binne enige Java-gebaseerde toepassing te verwyder deur 'n paar maklike stappe te implementeer.
        *   Skep Antwoord-objekte met kommentaar en datum.
        *   Instantieer SaveOptions-objek en stel AnnotationTypes = AnnotationType.None.
        *   Oproep stoor metode met gevolglike dokument pad of stroom en SaveOptions voorwerp.

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
    title_left: "Stappe om aantekeninge van PPSM in Java te wysig"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maak dit makliker vir Java-ontwikkelaars om verskeie annotasie-eienskappe vanaf PPSM-lêers binne enige Java-gebaseerde toepassing op te dateer deur 'n paar maklike stappe te implementeer.
        *   Instansieer Annotator-objek met invoerdokumentpad of stroom met geïnstantieerde LoadOptions met ImportAnnotations = true.
        *   Skep 'n paar AnnotationBase-implementering en stel Id van bestaande aantekening (indien aantekening met daardie Id nie gevind word nie, sal niks verander word nie) of padlys van aantekeninge (alle bestaande aantekeninge sal verwyder word).
        *   Roep opdateringsmetode van Annotator-voorwerp met geslaagde aantekeninge op.
        *   Oproep stoor metode met gevolglike dokument pad of stroom en SaveOptions voorwerp.

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
    title_left: "Stappe om aantekeninge uit PPSM in Java te onttrek"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) maak dit maklik vir Java-ontwikkelaars om dokumente te annoteer en annotasie-inligting uit PPSM-lêers binne enige Java-gebaseerde toepassing te onttrek deur 'n paar maklike stappe te implementeer.
        *   Skep Antwoord-objekte met kommentaar en datum.
        *   Instansieer LoadOptions-voorwerp en noem SetImportAnnotations met ware argument.
        *   Definieer veranderlike met tipe Lys.
        *   Roep kry metode en gee resultaat terug na veranderlike hierbo.

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
    title: "Regstreekse demonstrasies om by te voeg, te verwyder, te wysig, aantekeninge by dokumente en prente te onttrek"
    content: |
        Voeg, verwyder, redigeer en onttrek aantekeninge by PPSM-lêer op die oomblik deur [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) webwerf te besoek. Die lewendige demo het die volgende voordele

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppsm"
          title: "Oor PPSM Lêerformaat"
          content: |
            Lêers met PPSM-uitbreiding verteenwoordig Makro-geaktiveerde skyfievertoning-lêerformaat geskep met Microsoft PowerPoint 2007 of hoër. Nog 'n soortgelyke lêerformaat is PPTM wat verskil in die opening met Microsoft PowerPoint in bewerkbare formaat in plaas daarvan om as skyfievertoning te loop. Wanneer dit as skyfievertoning uitgevoer word, wys die PPSM-lêer die aanbiedingskyfies met die inhoud ongeskonde in die skyfievertoning en is dit by verstek in leesalleenmodus. PPSM-lêers kan steeds in Microsoft PowerPoint geredigeer word deur dit in PowerPoint oop te maak.

          link: "https://docs.fileformat.com/image/ppsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Werk met ander gewilde dokumentformate"
    content: |
        Dateer annotasie-eienskappe op vanaf sommige van die gewilde lêerformate soos hieronder vermeld.
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