---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPT Anodi API Anodi yn C#"
head_description: "Java API i greu ac Anodi mathau o anodiadau poblogaidd o PPT, delweddau, lluniadau a fformatau ffeil dogfen."

############################# Header ############################
title: "Anodwch PPT o Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Treial Am Ddim"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Ynglŷn â GroupDocs.Annotation ar gyfer Java API"
    content: |
        Mae GroupDocs.Annotation for Java API yn llyfrgell sy'n eich galluogi i ychwanegu anodiadau i PDF, Word a dogfennau eraill ar Mac, Windows neu Ubuntu. Mae [GroupDocs.Annotation ar gyfer Java] (/anodiad/java) yn API Java brodorol ar gyfer rheoli anodiadau gyda chefnogaeth gynhwysfawr ar gyfer creu, ychwanegu, golygu, dileu, echdynnu ac allforio anodiadau o ddelweddau a dogfennau amrywiol eraill. Y rhestr lawn o fformatau dogfennau â chymorth y gallech eu gweld ar y [dudalen] hon(https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Mae'r llyfrgell hon yn eich galluogi i weithio nid yn unig gyda PPT dogfen ond hefyd gyda llawer o fathau eraill o ddogfennau megis Word, Excel, PowerPoint, e-byst Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad a llawer o rai eraill.
        Mae'r GroupDocs.Annotation for Java API yn eich galluogi i greu ac ychwanegu nodiadau newydd, golygu anodiadau, tynnu sylwadau, anodiadau, a'u tynnu o ddogfennau. Mae'r llyfrgell yn cefnogi 13 o wahanol fathau o anodi, gan gynnwys Testun, Polyline, Arwynebedd, Tanlinellu, Pwynt, Dyfrnod, Saeth, Ellipse, Amnewid Testun, Pellter, Maes Testun, Golygu Adnoddau mewn PDF, HTML, dogfennau Microsoft Word, taenlenni, diagramau, cyflwyniadau, lluniadau, delweddau a llawer o fformatau ffeil eraill.
        Mae'r enghraifft (gweler isod) yn dangos gweithio gyda dogfen PPT, yn yr enghraifft hon gallech weld y prif gamau o sut i weithio gyda GroupDocs.Annotation: Gosod trwydded, agor dogfen rydych am weithio gyda hi, creu a anodi, ychwanegu gwrthrychau data i osod priodweddau anodi yn unol â'ch gofynion ac arbed y canlyniad i'r lle sydd ei angen. Hefyd fe allech chi gael golwg fanylach ar y nodweddion a gefnogir ar ein tudalen github [] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), neu yn ein cynnyrch [dogfennaeth] ( https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Camau i Ychwanegu Anodiadau i PPT yn Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) yn ei gwneud yn hawdd i ddatblygwyr Java ychwanegu gwahanol fathau o anodiadau at ffeiliau PPT o fewn unrhyw raglen sy'n seiliedig ar Java trwy roi ychydig o gamau hawdd ar waith.
        *   Creu gwrthrychau Ateb gyda sylw a dyddiad.
        *   Creu gwrthrych AreaAnnotation, gosod opsiynau ardal ac ychwanegu atebion.
        *   Creu gwrthrych Annotator ac ychwanegu anodiad ardal.
        *   Arbed ffeil allbwn.
    title_right: "Gofynion y System"
    content_right: |
        Cefnogir GroupDocs.Annotation ar gyfer API Java ar bob prif lwyfan a system weithredu. Cyn gweithredu'r cod isod, gwnewch yn siŵr bod gennych y rhagofynion canlynol wedi'u gosod ar eich system.
        *   Systemau Gweithredu: Microsoft Windows, Linux, MacOS
        *   Amgylchedd Datblygu: NetBeans, Intellij IDEA, Eclipse ac ati
        *   Amgylchedd Amser Rhedeg Java: Java 7 (1.7) ac uwch
        *   Sicrhewch y fersiwn diweddaraf o GroupDocs.Annotation ar gyfer Java o [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Rhagolwg anodi a sampl cod
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
    title_left: "Camau i Dynnu Anodiadau o PPT yn Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) yn ei gwneud yn haws i ddatblygwyr Java dynnu manylion anodiad o PPT o ffeiliau o fewn unrhyw raglen sy'n seiliedig ar Java drwy roi ychydig o gamau hawdd ar waith.
        *   Creu gwrthrychau Ateb gyda sylw a dyddiad.
        *   Instantiate SaveOptions object a gosod AnnotationTypes = AnnotationType.None.
        *   Dull arbed galwadau gyda llwybr dogfen canlyniadol neu ffrwd a gwrthrych SaveOptions.

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
    title_left: "Camau i Olygu Anodiadau o PPT yn Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) yn ei gwneud yn haws i ddatblygwyr Java ddiweddaru priodweddau anodi amrywiol o PPT o ffeiliau o fewn unrhyw raglen sy'n seiliedig ar Java trwy roi ychydig o gamau hawdd ar waith.
        *   Instantiate Annotator gwrthrych gyda llwybr dogfen mewnbwn neu ffrwd gyda LoadOptions instantiated gyda ImportAnnotations = gwir.
        *   Creu rhywfaint o weithrediad AnnotationBase a gosod ID o'r anodiadau sy'n bodoli (os na chanfuwyd yr anodiad gyda'r Id hwnnw, ni fydd unrhyw beth yn cael ei newid) neu restr llwybr o anodiadau (bydd yr holl anodiadau sy'n bodoli yn cael eu dileu).
        *   Dull diweddaru galwadau o wrthrych Annotator gydag anodiadau wedi'u pasio.
        *   Dull arbed galwadau gyda llwybr dogfen canlyniadol neu ffrwd a gwrthrych SaveOptions.

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
    title_left: "Camau i Echdynnu Anodiadau o PPT yn Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) yn ei gwneud hi'n hawdd i ddatblygwyr Java anodi dogfennau a thynnu gwybodaeth anodiad o PPT ffeil o fewn unrhyw raglen sy'n seiliedig ar Java trwy roi ychydig o gamau hawdd ar waith.
        *   Creu gwrthrychau Ateb gyda sylw a dyddiad.
        *   Cychwynnwch wrthrych LoadOptions a ffoniwch SetImportAnnotations gyda dadl wir.
        *   Diffinio newidyn gyda math Rhestr.
        *   Dull cael galwad a dychwelyd y canlyniad i'r newidyn uchod.

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
    title: "Demos Byw i'w Ychwanegu, Tynnu, Golygu, Tynnu Anodiadau i Ddogfennau a Delweddau"
    content: |
        Ychwanegu, dileu, golygu a thynnu anodiadau i ffeil PPT ar hyn o bryd drwy ymweld â gwefan [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
Mae gan y demo byw y buddion canlynol

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppt"
          title: "Ynglŷn â PPT Fformat Ffeil"
          content: |
            Mae ffeil gydag estyniad PPT yn cynrychioli ffeil PowerPoint sy'n cynnwys casgliad o sleidiau i'w harddangos fel Sioe Sleidiau. Mae'n nodi'r Fformat Ffeil Deuaidd a ddefnyddir gan Microsoft PowerPoint 97-2003. Gall ffeil PPT gynnwys sawl math gwahanol o wybodaeth megis testun, pwyntiau bwled, delweddau, amlgyfrwng a gwrthrychau OLE eraill sydd wedi'u mewnosod. Lluniodd Microsoft fformat ffeil mwy newydd ar gyfer PowerPoint, a elwir yn PPTX, o 2007 ymlaen sy'n seiliedig ar Office OpenXML ac sy'n wahanol i'r fformat ffeil deuaidd hwn. Gall sawl rhaglen gais arall fel OpenOffice Impress ac Apple Keynote hefyd greu ffeiliau PPT.

          link: "https://docs.fileformat.com/image/ppt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Gweithio gyda Fformatau Dogfennau Poblogaidd Eraill"
    content: |
        Diweddaru priodweddau anodi o rai o'r fformatau ffeil poblogaidd fel y nodir isod.
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