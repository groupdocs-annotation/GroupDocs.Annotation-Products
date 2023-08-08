---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java VSD Annotation API C# тіліндегі аннотация"
head_description: "VSD, кескіндер, сызбалар және құжат файл пішімінен танымал аннотация түрлерін жасауға және аннотациялауға арналған Java API."

############################# Header ############################
title: "Java тіліндегі VSD файлына түсініктеме беріңіз"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Тегін сынақ нұсқасын жүктеп алыңыз"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "GroupDocs туралы. Java API үшін аннотация"
    content: |
        GroupDocs.Annotation for Java API — бұл PDF, Word және Mac, Windows немесе Ubuntu жүйелеріндегі басқа құжаттарға аннотациялар қосуға мүмкіндік беретін кітапхана. [GroupDocs.Annotation for Java](/annotation/java) — кескіндер мен басқа да әртүрлі құжаттардан аннотацияларды жасауға, қосуға, өңдеуге, жоюға, шығарып алуға және экспорттауға арналған жан-жақты қолдауы бар аннотацияларды басқаруға арналған Java API интерфейсі. Қолдау көрсетілетін құжат пішімдерінің толық тізімін осы [бетте](https://docs.groupdocs.com/annotation/java/supported-document-formats/) көруге болады.
        Бұл кітапхана тек VSD құжатымен ғана емес, Word, Excel, PowerPoint, Outlook электрондық пошталары, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad және т.б. сияқты көптеген құжаттар түрлерімен жұмыс істеуге мүмкіндік береді.
        GroupDocs.Annotation for Java API жаңа ескертпелер жасауға және қосуға, аннотацияларды өңдеуге, түсініктемелерді, аннотацияларды шығарып алуға және оларды құжаттардан жоюға мүмкіндік береді. Кітапхана 13 түрлі аннотация түрлерін қолдайды, соның ішінде мәтін, полисызық, аймақ, астын сызу, нүкте, су таңбасы, көрсеткі, эллипс, мәтінді ауыстыру, қашықтық, мәтін өрісі, PDF, HTML, Microsoft Word құжаттарындағы ресурстарды өңдеу, электрондық кестелер, диаграммалар, презентациялар, сызбалар, кескіндер және басқа да көптеген файл пішімдері.
        Мысал (төменде қараңыз) VSD құжатымен жұмыс істеуді көрсетеді, бұл мысалда GroupDocs бағдарламасымен жұмыс істеудің негізгі қадамдарын көруге болады. Аннотация: Лицензияны орнату, жұмыс істегіңіз келетін құжатты ашу, файл жасау аннотация, талаптарыңызға сәйкес аннотация сипаттарын орнату үшін деректер нысандарын қосу және нәтижені қажетті орынға сақтау. Сондай-ақ, github [бетте](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) немесе өнімімізде [documentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java тіліндегі VSD файлына аннотацияларды қосу қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген Java негізіндегі қолданбадағы VSD файлдарына әртүрлі аннотация түрлерін қосуды жеңілдетеді.
        *   Түсініктеме мен күні бар Жауап нысандарын жасаңыз.
        *   AreaAnnotation нысанын жасаңыз, аймақ опцияларын орнатыңыз және жауаптарды қосыңыз.
        *   Аннотатор нысанын жасаңыз және аймаққа аннотация қосыңыз.
        *   Шығару файлын сақтаңыз.
    title_right: "Жүйе талаптары"
    content_right: |
        Java API интерфейстеріне арналған GroupDocs.Аннотацияға барлық негізгі платформалар мен операциялық жүйелерде қолдау көрсетіледі. Төмендегі кодты орындамас бұрын, жүйеде келесі алғышарттар орнатылғанына көз жеткізіңіз.
        *   Операциялық жүйелер: Microsoft Windows, Linux, MacOS
        *   Даму ортасы: NetBeans, Intellij IDEA, Eclipse т.б
        *   Java Runtime Environment: Java 7 (1.7) және одан жоғары
        *   Java үшін GroupDocs.Annotation бағдарламасының соңғы нұсқасын [GroupDocs Artifact Repository] сайтынан алыңыз (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Аннотацияны алдын ала қарау және код үлгісі
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
    title_left: "Java тіліндегі VSD файлынан аннотацияларды жою қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген Java негізіндегі қолданбадағы VSD файлдарынан аннотация мәліметтерін жоюды жеңілдетеді.
        *   Түсініктеме мен күні бар Жауап нысандарын жасаңыз.
        *   SaveOptions нысанын жасаңыз және AnnotationTypes = AnnotationType.None орнатыңыз.
        *   Нәтижелік құжат жолы немесе ағыны және SaveOptions нысаны бар қоңырауды сақтау әдісі.

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
    title_left: "Java тіліндегі VSD аннотацияларын өңдеу қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген Java негізіндегі қолданбадағы VSD файлдарының әртүрлі аннотация сипаттарын жаңартуды жеңілдетеді.
        *   Кіріс құжат жолы бар аннотатор нысанын құру немесе ImportAnnotations көмегімен даналық LoadOptions ағыны = шын.
        *   Кейбір AnnotationBase енгізуін жасаңыз және бар аннотацияның идентификаторын орнатыңыз (егер бұл идентификаторы бар аннотация табылмаса, ештеңе өзгертілмейді) немесе аннотациялардың жол тізімін (барлық аннотациялар жойылады).
        *   Өткізілген аннотациялары бар Annotator нысанының қоңырауды жаңарту әдісі.
        *   Нәтижелік құжат жолы немесе ағыны және SaveOptions нысаны бар қоңырауды сақтау әдісі.

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
    title_left: "Java тіліндегі VSD файлынан аннотацияларды шығару қадамдары"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java әзірлеушілеріне бірнеше оңай қадамдарды орындау арқылы кез келген Java негізіндегі қолданбадағы VSD файлдарынан құжаттарға аннотация жасауды және аннотация ақпаратын шығаруды жеңілдетеді.
        *   Түсініктеме мен күні бар Жауап нысандарын жасаңыз.
        *   LoadOptions нысанын іске қосыңыз және шынайы аргументпен SetImportAnnotations шақырыңыз.
        *   Тізім түрімен айнымалыны анықтаңыз.
        *   Get әдісіне қоңырау шалыңыз және нәтижені жоғарыдағы айнымалыға қайтарыңыз.

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
    title: "Құжаттар мен кескіндерге аннотацияларды қосу, жою, өңдеу, шығару үшін тікелей көрсетілімдер"
    content: |
        Дәл қазір [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) веб-сайтына кіру арқылы VSD файлына аннотацияларды қосу, жою, өңдеу және шығару. Тікелей демонстрацияның келесі артықшылықтары бар

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsd"
          title: "VSD Файл пішімі туралы"
          content: |
            VSD файлдары әртүрлі графикалық нысандарды және олардың арасындағы өзара байланысты көрсету үшін Microsoft Visio қолданбасымен жасалған сызбалар. Мұндай сызбаларда көрнекі нысандар, ағын диаграммалары, UML диаграммасы, ақпарат ағыны, ұйымдық диаграммалар, бағдарламалық қамтамасыз ету диаграммалары, желі орналасуы, деректер базасының үлгілері, объектілерді салыстыру және басқа ұқсас ақпараттар сияқты көрнекі нысандар болуы мүмкін. Microsoft Visio Visio файлдарын PNG, BMP, PDF және т.б. қоса алғанда, бірнеше түрлі файл пішіміне түрлендіру мүмкіндігін ұсынады.

          link: "https://docs.fileformat.com/image/vsd/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Басқа танымал құжат пішімдерімен жұмыс істеу"
    content: |
        Төменде көрсетілгендей кейбір танымал файл пішімдерінің аннотация сипаттарын жаңартыңыз.
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