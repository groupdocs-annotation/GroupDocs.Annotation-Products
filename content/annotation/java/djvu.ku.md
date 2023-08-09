---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DJVU Annotation API Annotate in C#"
head_description: "Java API ku ji DJVU, wêne, xêzkirin û formatên pelên pelgeyê celebên annotasyonên populer çêbike û annot bike."

############################# Header ############################
title: "Ji Javayê DJVU şîrove bikin"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Daxistina Doza Belaş"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Der barê GroupDocs.Annotation ji bo Java API"
    content: |
        GroupDocs.Annotation ji bo Java API pirtûkxaneyek e ku dihêle hûn li ser Mac, Windows an Ubuntu şîroveyan li PDF, Word û belgeyên din zêde bikin. [GroupDocs.Annotation for Java](/annotation/java) API-ya Java ya xwecihî ye ji bo birêvebirina annotasyonên bi piştgirîya berfireh ji bo afirandin, zêdekirin, sererastkirin, jêbirin, derxistin û hinartina annotationan ji wêne û belgeyên din ên cihêreng. Navnîşa tevahî ya formên belgeyên piştgirî yên ku hûn dikarin li ser vê [rûpelê] bibînin (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ev pirtûkxane dihêle hûn ne tenê bi belgeya DJVU re lê her weha bi gelek celeb belgeyên din ên wekî Word, Excel, PowerPoint, e-nameyên Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad û gelekên din re bixebitin.
        GroupDocs.Annotation ji bo Java API destûrê dide te ku hûn notên nû biafirînin û lê zêde bikin, şîroveyan biguherînin, şîroveyan, şîroveyan derxînin û wan ji belgeyan derxin. Pirtûkxane 13 celebên annotasyonê yên cihêreng piştgirî dike, di nav de Nivîsar, Polyline, Herêm, Binxêz, Xal, Nîşan, Tîrek, Ellipse, Veguheztina Nivîsan, Dûrbûn, Qada Nivîsarê, Veguhastina Çavkaniyê di PDF, HTML, belgeyên Microsoft Word de, pelgeyên berbelav, diagram, pêşkêşî, xêzkirin, wêne û gelek formatên pelan ên din.
        Nimûne (ji kerema xwe li jêr binêre) nîşan dide ku bi belgeya DJVU re dixebite, di vê nimûneyê de hûn dikarin gavên sereke yên çawa bi GroupDocs re bixebitin bibînin.Annotation: Destûrnameyek saz bikin, belgeyek ku hûn dixwazin pê re bixebitin vekin, vekin annotation, lê zêdekirina tiştên daneyê da ku taybetmendiyên annotasyonê li gorî hewcedariyên we bicîh bikin û encamê li cîhê hewce hilînin. Di heman demê de hûn dikarin li ser taybetmendiyên piştgirîkirî yên li ser github me [rûpel](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), an jî di hilberê me de [belgekirin](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Gavên Zêdekirina Şîroveyan li DJVU di Java de"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Ji pêşdebirên Java re hêsan dike ku bi pêkanîna çend gavên hêsan ve cûrbecûr şîrovekirinê li pelên DJVU zêde bikin.
        *   Tiştên Bersiv bi şîrove û tarîxê biafirînin.
        *   Tişta AreaAnnotation biafirînin, vebijarkên deverê bicîh bikin û bersivan lê zêde bikin.
        *   Tişta Annotator biafirînin û şirovekirina deverê lê zêde bikin.
        *   Pelê derketinê tomar bike.
    title_right: "Pêdiviyên Sîstemê"
    content_right: |
        GroupDocs.Annotation ji bo API-ên Java-yê li ser hemî platformên sereke û pergalên xebitandinê têne piştgirî kirin. Berî ku hûn koda jêrîn bicîh bikin, ji kerema xwe pê ewle bibin ku we şertên jêrîn li ser pergala we hatine saz kirin.
        *   Pergalên Xebatê: Microsoft Windows, Linux, MacOS
        *   Jîngeha Pêşveçûnê: NetBeans, Intellij IDEA, Eclipse hwd
        *   Java Runtime Jîngeh: Java 7 (1.7) û jor
        *   Guhertoya herî dawî ya GroupDocs.Annotation ji bo Java-yê ji [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) bistînin

############################# Preview ############################
preview_Add:
    enable: true
    title: Pêşdîtina annotation û nimûneya kodê
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
    title_left: "Gavên Rakirina Şîroveyan ji DJVU li Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Ji pêşdebirên Java-yê re hêsantir dike ku hûrguliyên annotasyonê ji pelên DJVU di nav her serîlêdana Java-yê de bi cîbicîkirina çend gavên hêsan rakin.
        *   Tiştên Bersiv bi şîrove û tarîxê biafirînin.
        *   Tişta SaveOptions destnîşan bikin û AnnotationTypes = AnnotationType.None saz bikin.
        *   Rêbaza hilanînê bi rêça belgeya encam an tîrêjê û tiştê SaveOptions re bang bikin.

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
    title_left: "Gavên Guherandinên Şîrove ji DJVU di Java de"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Ji pêşdebirên Java-yê re hêsantir dike ku bi pêkanîna çend gavên hêsan ve taybetmendiyên cûrbecûr şîrovekirinê ji pelên DJVU di nav her serlêdanek Java-yê de nûve bikin.
        *   Tişta Annotatorê bi rêça belgeya têketinê ve bişopînin an bi Vebijarkên Loadê yên destnîşankirî bi ImportAnnotations re biherikînin = rast.
        *   Hin pêkanîna AnnotationBase biafirînin û Nasnameya annotationê ya heyî destnîşan bikin (heke şîroveya bi wê Nasnameyê re neyê dîtin, dê tiştek neyê guheztin) an navnîşa rêgezên şîroveyan (hemû şîroveyên heyî dê werin rakirin).
        *   Rêbaza nûvekirina tiştê Annotator bi şîroveyên derbasbûyî re bang bikin.
        *   Rêbaza hilanînê bi rêça belgeya encam an tîrêjê û tiştê SaveOptions re bang bikin.

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
    title_left: "Gavên Derxistina Şîroveyan ji DJVU di Java de"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Ji pêşdebirên Java-yê re hêsan dike ku bi pêkanîna çend gavên hêsan belgeyan binivîsin û agahdariya şîrovekirinê ji pelên DJVU derxînin.
        *   Tiştên Bersiv bi şîrove û tarîxê biafirînin.
        *   Objektîfên LoadOptions destnîşan bikin û bi argumana rast bangî SetImportAnnotations bikin.
        *   Guherbar bi tîpa Lîsteyê pênase bikin.
        *   Banga rêbaza wergirtinê bikin û encamê vegerînin guhêrbara jorîn.

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
    title: "Demoyên Zindî ku lê zêde bikin, jêbirin, biguherînin, şîroveyan ji belge û wêneyan derxin"
    content: |
        Bi seredana malpera [GroupDocs.Annotation Demos Zindî](https://products.groupdocs.app/annotation/family) niha li pelê DJVU şîroveyan zêde bikin, jêbikin, biguherînin û derxin. Demoya zindî xwedî feydeyên jêrîn e

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-djvu"
          title: "Derbarê DJVU Forma Pelê"
          content: |
            DjVu, wekî "déjà vu" tê bilêvkirin, pelgeyek pelê grafîkî ye ku ji bo belge û pirtûkên skankirî ye, nemaze yên ku têkeliya nivîs, xêzkirin, wêne û wêneyan dihewîne. Ew ji hêla AT&T Labs ve hatî pêşve xistin. Ew gelek teknolojiyên mîna veqetandina qata wêneyê ya wêneyên nivîs û paşîn, barkirina pêşkeftî, kodkirina jimareyî û berhevkirina windayî ji bo wêneyên bitonal bikar tîne. Ji ber ku pelê DJVU dikare wêneyên rengîn, wêne, nivîs, û xêzên pêçandî lê bi kalîte bilind vehewîne û dikare di cîhekî hindik de were hilanîn ji ber vê yekê, ew li ser malperê wekî eBook, destan, rojname, belgeyên kevnar, hwd tê bikar anîn.

          link: "https://docs.fileformat.com/image/djvu/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bi Formên Belgeya Din ên populer re dixebitin"
    content: |
        Taybetmendiyên annotasyonê ji hin formatên pelê yên populer ên ku li jêr têne destnîşan kirin nûve bikin.
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