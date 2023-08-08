---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DOCX Anótáil API Anótáil i C#"
head_description: "Java API chun cineálacha móréilimh anótála a chruthú agus a Anótáil ó DOCX, íomhánna, líníochtaí agus formáidí comhaid doiciméad."

############################# Header ############################
title: "Anótáil DOCX ó Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Íoslódáil Triail Saor in Aisce"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Maidir le GroupDocs.Annotation le haghaidh Java API"
    content: |
        Is leabharlann é GroupDocs.Annotation for Java API a ligeann duit nótaí a chur le PDF, Word agus doiciméid eile ar Mac, Windows nó Ubuntu. Is é [GroupDocs.Annotation for Java](/annotation/java) API dúchais Java chun nótaí a bhainistiú le tacaíocht chuimsitheach chun nótaí a chruthú, a chur leis, a chur in eagar, a scriosadh, a bhaint agus a easpórtáil ó íomhánna agus doiciméid éagsúla eile. An liosta iomlán de na formáidí doiciméad tacaithe a d’fhéadfá a fheiceáil ar an [leathanach] seo(https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ligeann an leabharlann seo duit oibriú ní hamháin le doiciméad DOCX ach freisin le go leor cineálacha doiciméad eile ar nós Word, Excel, PowerPoint, ríomhphoist Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad agus go leor eile.
        Ligeann an GroupDocs.Annotation for Java API duit nótaí nua a chruthú agus a chur leis, nótaí a chur in eagar, nótaí tráchta a bhaint as, agus iad a bhaint de dhoiciméid. Tacaíonn an leabharlann le 13 chineál nótaí éagsúla, lena n-áirítear Téacs, Polalíne, Achar, Líne Folaigh, Pointe, Comhartha Uisce, Arrow, Éilips, Athsholáthar Téacs, Fad, Réimse Téacs, Athchóiriú Acmhainní i bhformáid PDF, HTML, doiciméid Microsoft Word, scarbhileoga, léaráidí, cur i láthair, líníochtaí, íomhánna agus go leor formáidí comhaid eile.
        Léiríonn an sampla (féach thíos) oibriú le doiciméad DOCX, sa sampla seo d'fhéadfá na príomhchéimeanna a fheiceáil maidir le conas oibriú le GroupDocs.Annotation: Socraigh ceadúnas, oscail doiciméad a bhfuil tú ag iarraidh oibriú leis, cruthaigh doiciméad anótáil, rudaí sonraí a chur leis chun airíonna anótála a shocrú de réir do riachtanas agus an toradh a shábháil chuig an áit atá ag teastáil. Chomh maith leis sin d'fhéadfá breathnú níos mionsonraithe a bheith agat ar na gnéithe tacaithe ar ár leathanach github [] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), nó inár dtáirge [doiciméadúchán] (https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Céimeanna chun Anótálacha a Chur le DOCX i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) déanann sé éasca d’fhorbróirí Java cineálacha éagsúla nótaí a chur le comhaid DOCX laistigh d’fheidhmchlár Java-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cruthaigh oibiachtaí Freagra le trácht agus dáta.
        *   Cruthaigh réad AreaAnnotation, socraigh roghanna achair agus cuir freagraí leis.
        *   Cruthaigh réad Anótaire agus cuir anótáil achair leis.
        *   Sábháil an comhad aschuir.
    title_right: "Riachtanais Chórais"
    content_right: |
        Tacaítear le GroupDocs.Annotation le haghaidh Java API ar gach mór-ardán agus córas oibriúcháin. Sula ndéanann tú an cód thíos, déan cinnte go bhfuil na réamhriachtanais seo a leanas suiteáilte ar do chóras.
        *   Córais Oibriúcháin: Microsoft Windows, Linux, MacOS
        *   Timpeallacht Forbartha: NetBeans, Intellij IDEA, Eclipse etc
        *   Timpeallacht Java Runtime: Java 7 (1.7) agus os a chionn
        *   Faigh an leagan is déanaí de GroupDocs.Annotation for Java ó [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Réamhamharc anótála agus sampla cód
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
    title_left: "Céimeanna chun Anótálacha a Bhaint ó DOCX i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) déanann sé níos fusa d’fhorbróirí Java sonraí anóta a bhaint de chomhaid DOCX laistigh d’fheidhmchlár Java-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cruthaigh oibiachtaí Freagra le trácht agus dáta.
        *   Cuir réad SaveOptions ar bun agus socraigh AnnotationTypes = AnnotationType.None.
        *   Glaoigh ar an modh sábhála le cosán doiciméad nó sruth dá bharr agus réad SaveOptions.

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
    title_left: "Céimeanna chun Anótálacha ó DOCX a chur in eagar i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) déanann sé níos fusa d’fhorbróirí Java airíonna nótaí éagsúla ó chomhaid DOCX a nuashonrú laistigh d’fheidhmchlár Java-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cuir réad Anótaire ar an toirt le conair doiciméid ionchuir nó sruth le LoadOptions meandrach le ImportAnnotations = fíor.
        *   Cruthaigh roinnt cur i bhfeidhm AnnotationBase agus socraigh Aitheantas an anótála a bhí ann (mura bhfuarthas anótáil leis an Aitheantas sin, ní athrófar aon rud) nó liosta cosáin na nótaí (bainfear gach anótáil atá ann).
        *   Modh nuashonraithe an ghlao ar réad Anótaire le nótaí a ritheadh.
        *   Glaoigh ar an modh sábhála le cosán doiciméad nó sruth dá bharr agus réad SaveOptions.

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
    title_left: "Céimeanna chun Anótálacha a Bhaint as DOCX i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) déanann sé éasca d’fhorbróirí Java doiciméid a anótáil agus faisnéis anótála a bhaint as comhaid DOCX laistigh d’fheidhmchlár Java-bhunaithe ar bith trí roinnt céimeanna éasca a chur i bhfeidhm.
        *   Cruthaigh oibiachtaí Freagra le trácht agus dáta.
        *   Cuir oibiacht ar LoadOptions agus cuir glaoch ar SetImportAnnotations le fíorargóint.
        *   Sainmhínigh athróg le liosta cineáil.
        *   Modh faigh glao agus cuir an toradh ar ais chuig an athróg thuas.

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
    title: "Taispeántais Bheo le Cur Leis, Bain Amach, Cuir in Eagar, Anótálacha a Bhaint as Doiciméid agus Íomhánna"
    content: |
        Cuir nótaí le DOCX leis, bain, cuir in eagar agus bain amach iad faoi láthair trí chuairt a thabhairt ar [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Tá na buntáistí seo a leanas ag an taispeántas beo

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docx"
          title: "Maidir le DOCX Formáid Chomhaid"
          content: |
            Is formáid aitheanta é DOCX do dhoiciméid Microsoft Word. Arna thabhairt isteach ó 2007 le heisiúint Microsoft Office 2007, athraíodh struchtúr an fhormáid nua Doiciméid seo ó dhénárthach simplí go meascán de chomhaid XML agus dhénártha. Is féidir comhaid Docx a oscailt le Word 2007 agus le leaganacha cliathánach ach ní leis na leaganacha níos luaithe de MS Word a thacaíonn le síntí comhaid DOC.

          link: "https://docs.fileformat.com/image/docx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Ag Obair le Formáidí Doiciméad Coitianta Eile"
    content: |
        Nuashonraigh airíonna anótála ó chuid de na formáidí comhaid coitianta mar a luaitear thíos.
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