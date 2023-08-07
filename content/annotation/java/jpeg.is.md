---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java JPEG Annotation API Annotate í C#"
head_description: "Java API til að búa til og athugasemda við vinsælar athugasemdagerðir úr JPEG, myndum, teikningum og skjalaskráarsniðum."

############################# Header ############################
title: "Skýrðu JPEG frá Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Sækja ókeypis prufuáskrift"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Um GroupDocs.Annotation fyrir Java API"
    content: |
        GroupDocs.Annotation for Java API er bókasafn sem gerir þér kleift að bæta við athugasemdum við PDF, Word og önnur skjöl á Mac, Windows eða Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) er innbyggt Java API til að stjórna athugasemdum með alhliða stuðningi við að búa til, bæta við, breyta, eyða, draga út og flytja út athugasemdir úr myndum og ýmsum öðrum skjölum. Allur listi yfir studd skjalasnið sem þú gætir séð á þessari [síðu](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Þetta bókasafn gerir þér kleift að vinna ekki aðeins með JPEG skjölum heldur einnig með mörgum öðrum skjölum eins og Word, Excel, PowerPoint, Outlook tölvupósti, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad og mörgum öðrum.
        GroupDocs.Annotation for Java API gerir þér kleift að búa til og bæta við nýjum athugasemdum, breyta athugasemdum, draga út athugasemdir, athugasemdir og fjarlægja þær úr skjölum. Bókasafnið styður 13 mismunandi skýringargerðir, þar á meðal texta, fjöllínu, svæði, undirstrik, punkt, vatnsmerki, ör, sporbaug, textaskipti, fjarlægð, textareit, tilföng klippingu í PDF, HTML, Microsoft Word skjölum, töflureiknum, skýringarmyndum, kynningum, teikningar, myndir og mörg önnur skráarsnið.
        Dæmið (vinsamlegast sjáðu hér að neðan) sýnir að þú vinnur með JPEG skjal, í þessu dæmi gætirðu séð helstu skrefin í því hvernig á að vinna með GroupDocs.Athugasemd: Setja upp leyfi, opna skjal sem þú vilt vinna með, búa til athugasemd, bæta við gagnahlutum til að stilla athugasemdareiginleika í samræmi við kröfur þínar og vista niðurstöðuna á nauðsynlegum stað. Þú gætir líka skoðað studdu eiginleikana á github [síðu] okkar (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), eða í vörunni okkar [skjölum](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Skref til að bæta athugasemdum við JPEG í Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gerir það auðvelt fyrir Java forritara að bæta ýmsum athugasemdategundum við JPEG skrár innan hvaða Java-undirstaða forrits sem er með því að útfæra nokkur auðveld skref.
        *   Búðu til svarhluti með athugasemd og dagsetningu.
        *   Búðu til AreaAnnotation hlut, stilltu svæðisvalkosti og bættu við svörum.
        *   Búðu til Annotator hlut og bættu við svæðisskýringum.
        *   Vista úttaksskrá.
    title_right: "kerfis kröfur"
    content_right: |
        GroupDocs.Annotation fyrir Java API eru studd á öllum helstu kerfum og stýrikerfum. Áður en þú keyrir kóðann hér að neðan skaltu ganga úr skugga um að þú hafir eftirfarandi forsendur uppsettar á kerfinu þínu.
        *   Stýrikerfi: Microsoft Windows, Linux, MacOS
        *   Þróunarumhverfi: NetBeans, Intellij IDEA, Eclipse o.fl
        *   Java Runtime Environment: Java 7 (1.7) og nýrri
        *   Fáðu nýjustu útgáfuna af GroupDocs.Annotation fyrir Java frá [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Forskoðun athugasemda og kóðasýni
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
    title_left: "Skref til að fjarlægja athugasemdir úr JPEG í Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gerir það auðveldara fyrir Java forritara að fjarlægja athugasemdaupplýsingar úr JPEG skrám innan hvaða Java-undirstaða forrits sem er með því að útfæra nokkur einföld skref.
        *   Búðu til svarhluti með athugasemd og dagsetningu.
        *   Staðfestu SaveOptions hlutinn og stilltu AnnotationTypes = AnnotationType.None.
        *   Hringdu í vistunaraðferð með skjalaslóð eða straumi og SaveOptions hlut.

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
    title_left: "Skref til að breyta athugasemdum frá JPEG í Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gerir það auðveldara fyrir Java forritara að uppfæra ýmsa skýringaeiginleika úr JPEG skrám innan hvaða Java-undirstaða forrits sem er með því að útfæra nokkur einföld skref.
        *   Staðfestu Annotator hlut með innsláttarskjalsslóð eða straumi með instantiated LoadOptions með ImportAnnotations = true.
        *   Búðu til einhverja AnnotationBase útfærslu og stilltu auðkenni þeirra skýringa sem fyrir voru (ef athugasemd með því auðkenni finnst ekki verður engu breytt) eða slóðalista yfir athugasemdir (allar skýringar sem til eru verða fjarlægðar).
        *   Kalla uppfærsluaðferð á Annotator hlut með samþykktum athugasemdum.
        *   Hringdu í vistunaraðferð með skjalaslóð eða straumi og SaveOptions hlut.

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
    title_left: "Skref til að draga út athugasemdir úr JPEG í Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gerir það auðvelt fyrir Java forritara að skrifa athugasemdir við skjöl og draga út athugasemdaupplýsingar úr JPEG skrám í hvaða Java-undirstaða forriti sem er með því að útfæra nokkur einföld skref.
        *   Búðu til svarhluti með athugasemd og dagsetningu.
        *   Staðfestu LoadOptions hlut og hringdu í SetImportAnnotations með sannri röksemdafærslu.
        *   Skilgreindu breytu með gerð List.
        *   Hringdu í fá aðferð og skilaðu niðurstöðunni í breytuna hér að ofan.

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
    title: "Lifandi kynningar til að bæta við, fjarlægja, breyta, draga út athugasemdir við skjöl og myndir"
    content: |
        Bættu við, fjarlægðu, breyttu og dragðu út athugasemdir við JPEG skrána núna með því að fara á vefsíðu [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Lifandi kynningin hefur eftirfarandi kosti

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpeg"
          title: "Um JPEG skráarsnið"
          content: |
            JPEG er tegund myndsniðs sem er vistað með tapaða þjöppun. Úttaksmyndin, sem afleiðing af þjöppun, er skipting milli geymslustærðar og myndgæða. Notendur geta stillt þjöppunarstigið til að ná æskilegu gæðastigi en á sama tíma minnka geymslustærðina. Myndgæði hafa óveruleg áhrif ef 10:1 þjöppun er notuð á myndina. Því hærra sem þjöppunargildið er, því meiri skerðing á myndgæðum. JPEG myndskráarsnið var staðlað af Joint Photographic Experts Group og þar af leiðandi nafnið JPEG. Snið hefur verið val um að geyma og senda ljósmyndamyndir á vefnum. Næstum öll stýrikerfi hafa nú áhorfendur sem styðja sjónræningu á JPEG myndum, sem eru oft geymdar með JPG viðbótum líka. Jafnvel vefvöfrarnir styðja sjónræningu á JPEG myndum.

          link: "https://docs.fileformat.com/image/jpeg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Vinna með önnur vinsæl skjalasnið"
    content: |
        Uppfærðu athugasemdareiginleika frá sumum af vinsælustu skráarsniðunum eins og fram kemur hér að neðan.
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