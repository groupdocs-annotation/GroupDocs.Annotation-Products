---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PDF Annotation API märkused C#-s"
head_description: "Java API populaarsete annotatsioonitüüpide PDF, piltide, jooniste ja dokumendifailivormingute loomiseks ja märkuste tegemiseks."

############################# Header ############################
title: "Märkige Java faili PDF"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Laadige alla tasuta prooviversioon"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Teave GroupDocs.Annotation kohta Java API jaoks"
    content: |
        GroupDocs.Annotation for Java API on teek, mis võimaldab teil lisada annotatsioone PDF-i, Wordi ja muudele Maci, Windowsi või Ubuntu dokumentidele. [GroupDocs.Annotation for Java](/annotation/java) on natiivne Java API märkuste haldamiseks, mis toetab igakülgset annotatsioonide loomist, lisamist, redigeerimist, kustutamist, ekstraktimist ja eksportimist piltidelt ja mitmesugustest muudest dokumentidest. Toetatud dokumendivormingute täielikku loendit näete sellel [lehel](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        See teek võimaldab teil töötada mitte ainult PDF dokumendiga, vaid ka palju muud tüüpi dokumentidega, nagu Word, Excel, PowerPoint, Outlooki meilid, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ja paljud teised.
        Java API GroupDocs.Annotation võimaldab teil luua ja lisada uusi märkmeid, redigeerida märkusi, ekstraktida kommentaare, märkusi ja neid dokumentidest eemaldada. Teek toetab 13 erinevat märkuste tüüpi, sealhulgas tekst, rida, ala, allajoon, punkt, vesimärk, nool, ellips, teksti asendamine, kaugus, tekstiväli, ressursi redigeerimine PDF-is, HTML-is, Microsoft Wordi dokumentides, arvutustabelites, diagrammides, esitlustes, joonised, pildid ja paljud muud failivormingud.
        Näide (vt allpool) demonstreerib töötamist dokumendiga PDF, selles näites näete GroupDocsiga töötamise peamisi samme. Annotatsioon: seadistage litsents, avage dokument, millega soovite töötada, luues annotatsioon, andmeobjektide lisamine annotatsiooni omaduste määramiseks vastavalt teie vajadustele ja tulemuse salvestamine vajalikku kohta. Samuti võite toetatud funktsioonide kohta üksikasjalikumalt tutvuda meie githubi [lehel](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) või meie toote [dokumentatsioonis](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Toimingud Java failile PDF märkuste lisamiseks"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) teeb Java-arendajatel lihtsaks lisada erinevaid märkuste tüüpe PDF-failidele mis tahes Java-põhises rakenduses, rakendades mõnda lihtsat sammu.
        *   Looge vastuseobjektid koos kommentaari ja kuupäevaga.
        *   Looge AreaAnnotation objekt, määrake ala valikud ja lisage vastuseid.
        *   Loo annotaatori objekt ja lisa ala märkus.
        *   Salvestage väljundfail.
    title_right: "Nõuded süsteemile"
    content_right: |
        GroupDocs.Annotation Java API-de jaoks on toetatud kõigil suurematel platvormidel ja operatsioonisüsteemidel. Enne alloleva koodi käivitamist veenduge, et teie süsteemi on installitud järgmised eeltingimused.
        *   Operatsioonisüsteemid: Microsoft Windows, Linux, MacOS
        *   Arenduskeskkond: NetBeans, Intellij IDEA, Eclipse jne
        *   Java käituskeskkond: Java 7 (1.7) ja uuemad
        *   Hankige Java jaoks mõeldud GroupDocs.Annotation uusim versioon saidilt [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Annotatsiooni eelvaade ja koodinäidis
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
    title_left: "Toimingud Java-failist PDF märkuste eemaldamiseks"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) muudab Java-arendajate jaoks lihtsamaks annotatsiooni üksikasjade eemaldamise mis tahes Java-põhises rakenduses olevast failist PDF, rakendades mõnda lihtsat sammu.
        *   Looge vastuseobjektid koos kommentaari ja kuupäevaga.
        *   Käivitage objekt SaveOptions ja määrake AnnotationTypes = AnnotationType.None.
        *   Helistage salvestamismeetodile tulemuseks oleva dokumendi tee või voo ja SaveOptions objektiga.

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
    title_left: "Toimingud faili PDF märkuste muutmiseks Javas"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) muudab Java-arendajate jaoks lihtsamaks erinevate annotatsioonide atribuutide värskendamise PDF-failidest mis tahes Java-põhises rakenduses, rakendades mõnda lihtsat sammu.
        *   Eksperimenteerige annotaatori objekt sisenddokumendi tee või vooga koos korduvate LoadOptionsiga koos ImportAnnotations = true.
        *   Looge AnnotationBase'i teostus ja määrake olemasoleva annotatsiooni ID (kui selle ID-ga annotatsiooni ei leitud, ei muudeta midagi) või märkuste teede loend (kõik olemasolevad annotatsioonid eemaldatakse).
        *   Kutsuge läbitud märkustega annotaatori objekti värskendusmeetodit.
        *   Helistage salvestamismeetodile tulemuseks oleva dokumendi tee või voo ja SaveOptions objektiga.

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
    title_left: "Toimingud Java-vormingus failist PDF märkuste ekstraheerimiseks"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) muudab Java-arendajate jaoks lihtsaks dokumentidele märkuste lisamise ja annotatsiooniteabe ekstraktimise mis tahes Java-põhises rakenduses olevatest failidest PDF, rakendades mõne lihtsa sammu.
        *   Looge vastuseobjektid koos kommentaari ja kuupäevaga.
        *   Esitage objekt LoadOptions ja kutsuge välja SetImportAnnotations tõese argumendiga.
        *   Määratle muutuja tüübiga List.
        *   Kutsuge meetod hankima ja tagastage tulemus ülaltoodud muutujale.

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
    title: "Reaalajas demod dokumentide ja piltide märkuste lisamiseks, eemaldamiseks, redigeerimiseks ja ekstraktimiseks"
    content: |
        Lisage, eemaldage, muutke ja ekstraktige faili PDF märkusi kohe, külastades veebisaiti [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Reaalajas demol on järgmised eelised

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pdf"
          title: "Teave failivormingu PDF kohta"
          content: |
            Portable Document Format (PDF) on teatud tüüpi dokument, mille Adobe lõi 1990ndatel. Selle failivormingu eesmärk oli kehtestada standard dokumentide ja muu võrdlusmaterjali esitamiseks vormingus, mis ei sõltu rakendustarkvarast, riistvarast ega ka operatsioonisüsteemist. PDF-faile saab avada nii Adobe Acrobat Readeris/Writeris kui ka enamikes kaasaegsetes brauserites, nagu Chrome, Safari, Firefox, laienduste/pistikprogrammide kaudu. Enamik kaubanduslikult saadaolevatest tarkvarakomplektidest pakuvad ka oma dokumentide teisendamist PDF-vormingusse ilma täiendava tarkvarakomponendita. Seega on PDF-failivormingus täielik võime sisaldada teavet, nagu tekst, pildid, hüperlingid, vormiväljad, rikasmeedia, digitaalallkirjad, manused, metaandmed, georuumilised funktsioonid ja 3D-objektid, mis võivad muutuda lähtedokumendi osaks.

          link: "https://docs.fileformat.com/image/pdf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Muude populaarsete dokumendivormingutega töötamine"
    content: |
        Värskendage mõne populaarse failivormingu annotatsiooni atribuute, nagu allpool kirjeldatud.
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