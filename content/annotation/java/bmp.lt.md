---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java BMP Annotation API komentaras C#"
head_description: "Java API, skirta kurti ir komentuoti populiarius komentarų tipus iš BMP, vaizdų, brėžinių ir dokumentų failų formatų."

############################# Header ############################
title: "Komentuoti BMP iš „Java“."
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Atsisiųskite nemokamą bandomąją versiją"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Apie GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API yra biblioteka, leidžianti pridėti komentarų į PDF, Word ir kitus dokumentus Mac, Windows ar Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) yra savoji Java API, skirta komentarams tvarkyti su visapusišku palaikymu kuriant, įtraukiant, redaguojant, ištrinant, ištraukiant ir eksportuojant komentarus iš vaizdų ir įvairių kitų dokumentų. Visą palaikomų dokumentų formatų sąrašą galite pamatyti šiame [puslapyje](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ši biblioteka leidžia dirbti ne tik su BMP dokumentu, bet ir su daugelio kitų tipų dokumentais, tokiais kaip Word, Excel, PowerPoint, Outlook el. laiškai, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ir daugelis kitų.
        „Java“ API „GroupDocs.Annotation“ leidžia kurti ir pridėti naujų pastabų, redaguoti komentarus, išgauti komentarus, anotacijas ir pašalinti juos iš dokumentų. Biblioteka palaiko 13 skirtingų anotacijų tipų, įskaitant tekstą, poliliniją, sritį, pabraukimą, tašką, vandens ženklą, rodyklę, elipsę, teksto pakeitimą, atstumą, teksto lauką, išteklių redagavimą PDF, HTML, Microsoft Word dokumentuose, skaičiuokles, diagramas, pristatymus, brėžiniai, vaizdai ir daugelis kitų failų formatų.
        Pavyzdyje (žr. toliau) parodytas darbas su BMP dokumentu. Šiame pavyzdyje galite pamatyti pagrindinius darbo su GroupDocs veiksmus. Anotacija: nustatykite licenciją, atidarykite dokumentą, su kuriuo norite dirbti, ir sukurkite anotacija, pridedant duomenų objektus, kad nustatytumėte anotacijos ypatybes pagal jūsų poreikius ir išsaugant rezultatą reikiamoje vietoje. Taip pat galite sužinoti daugiau apie palaikomas funkcijas mūsų „github“ [puslapyje] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) arba mūsų produkto [dokumentacijoje] (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Veiksmai, kaip pridėti komentarų prie BMP Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) „Java“ kūrėjai gali lengvai pridėti įvairių tipų komentarų prie BMP failų bet kurioje „Java“ programoje, atlikdami kelis paprastus veiksmus.
        *   Sukurkite atsakymo objektus su komentaru ir data.
        *   Sukurkite AreaAnnotation objektą, nustatykite srities parinktis ir pridėkite atsakymus.
        *   Sukurkite komentatoriaus objektą ir pridėkite srities anotaciją.
        *   Išsaugoti išvesties failą.
    title_right: "Sistemos reikalavimai"
    content_right: |
        GroupDocs.Annotation Java API palaiko visose pagrindinėse platformose ir operacinėse sistemose. Prieš vykdydami toliau pateiktą kodą, įsitikinkite, kad jūsų sistemoje yra įdiegtos šios būtinos sąlygos.
        *   Operacinės sistemos: Microsoft Windows, Linux, MacOS
        *   Kūrimo aplinka: NetBeans, Intellij IDEA, Eclipse ir kt
        *   Java Runtime Environment: Java 7 (1.7) ir naujesnės versijos
        *   Gaukite naujausią GroupDocs.Annotation for Java versiją iš [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Anotacijos peržiūra ir kodo pavyzdys
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
    title_left: "Veiksmai, kaip pašalinti komentarus iš BMP „Java“."
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) leidžia „Java“ kūrėjams lengviau pašalinti komentarų informaciją iš BMP failų bet kurioje „Java“ pagrįstoje programoje, atlikus kelis paprastus veiksmus.
        *   Sukurkite atsakymo objektus su komentaru ir data.
        *   Sukurkite objektą SaveOptions ir nustatykite AnnotationTypes = AnnotationType.None.
        *   Iškvieskite išsaugojimo metodą su gautu dokumento keliu arba srautu ir objektu „SaveOptions“.

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
    title_left: "Veiksmai, kaip redaguoti komentarus iš BMP Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) „Java“ kūrėjams leidžia lengviau atnaujinti įvairias komentarų ypatybes iš BMP failų bet kurioje „Java“ pagrįstoje programoje, įgyvendinant kelis paprastus veiksmus.
        *   Sukurkite komentatoriaus objektą su įvesties dokumento keliu arba srautu su momentinėmis LoadOptions su ImportAnnotations = true.
        *   Sukurkite kokį nors AnnotationBase diegimą ir nustatykite esamo komentaro ID (jei komentaras su tuo ID nerastas, niekas nebus pakeistas) arba komentarų kelių sąrašą (visi esami komentarai bus pašalinti).
        *   Iškvieskite komentatoriaus objekto atnaujinimo metodą su priimtais komentarais.
        *   Iškvieskite išsaugojimo metodą su gautu dokumento keliu arba srautu ir objektu „SaveOptions“.

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
    title_left: "Veiksmai, kaip išgauti komentarus iš BMP „Java“."
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) leidžia „Java“ kūrėjams lengvai komentuoti dokumentus ir išgauti komentarų informaciją iš BMP failų bet kurioje „Java“ pagrįstoje programoje, atlikus kelis paprastus veiksmus.
        *   Sukurkite atsakymo objektus su komentaru ir data.
        *   Sukurkite LoadOptions objektą ir iškvieskite SetImportAnnotations su tikru argumentu.
        *   Apibrėžkite kintamąjį naudodami tipą Sąrašas.
        *   Iškvieskite metodą gauti ir grąžinkite rezultatą į aukščiau esantį kintamąjį.

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
    title: "Tiesioginės demonstracinės versijos, skirtos dokumentų ir vaizdų komentarams pridėti, pašalinti, redaguoti, išgauti"
    content: |
        Pridėkite, pašalinkite, redaguokite ir išskleiskite komentarus prie BMP failo dabar, apsilankę [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) svetainėje.
Tiesioginė demonstracinė versija turi šiuos privalumus

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-bmp"
          title: "Apie BMP failo formatą"
          content: |
            Failai, kurių plėtinys yra .BMP, yra taškinio vaizdo failai, naudojami taškinių skaitmeninių vaizdų saugojimui. Šie vaizdai nepriklauso nuo grafikos adapterio ir dar vadinami nuo įrenginio nepriklausomo bitmap (DIB) failo formatu. Ši nepriklausomybė skirta atidaryti failą keliose platformose, pvz., „Microsoft Windows“ ir „Mac“. BMP failo formatas gali saugoti duomenis kaip dvimačius skaitmeninius vaizdus tiek nespalvotu, tiek spalvotu formatu su įvairiu spalvų gyliu.

          link: "https://docs.fileformat.com/image/bmp/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Darbas su kitais populiariais dokumentų formatais"
    content: |
        Atnaujinkite komentarų ypatybes iš kai kurių populiarių failų formatų, kaip nurodyta toliau.
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