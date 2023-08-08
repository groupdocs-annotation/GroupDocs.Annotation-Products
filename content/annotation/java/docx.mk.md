---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DOCX Annotation API Annotate во C#"
head_description: "Java API за создавање и забележување популарни типови прибелешки од DOCX, слики, цртежи и формати на датотеки на документи."

############################# Header ############################
title: "Прибелешка DOCX од Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Преземете бесплатен пробен период"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "За GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation за Java API е библиотека која ви овозможува да додавате прибелешки во PDF, Word и други документи на Mac, Windows или Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) е мајчин Java API за управување со прибелешки со сеопфатна поддршка за креирање, додавање, уредување, бришење, извлекување и извоз на прибелешки од слики и разни други документи. Целосната листа на поддржани формати на документи што може да ги видите на оваа [страница](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Оваа библиотека ви овозможува да работите не само со документи DOCX туку и со многу други видови документи како што се Word, Excel, PowerPoint, Outlook е-пошта, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad и многу други.
        АПИ на GroupDocs.Annotation за Java ви овозможува да креирате и додавате нови белешки, да уредувате прибелешки, да извлекувате коментари, прибелешки и да ги отстранувате од документите. Библиотеката поддржува 13 различни типови на прибелешки, вклучувајќи текст, полилинија, област, подвлечен, точка, воден печат, стрелка, елипса, замена на текст, растојание, поле за текст, редакција на ресурси во PDF, HTML, Microsoft Word документи, табеларни пресметки, дијаграми, презентации, цртежи, слики и многу други формати на датотеки.
        Примерот (видете подолу) покажува работа со документот DOCX, во овој пример можете да ги видите главните чекори како да работите со GroupDocs. Забелешка: Поставете лиценца, отворете документ со кој сакате да работите, креирајте прибелешка, додавање податочни објекти за поставување на својствата на прибелешка според вашите барања и зачувување на резултатот на потребното место. Исто така, можете да погледнете подетално за поддржаните функции на нашата github [страница](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) или во нашиот производ [документација](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Чекори за додавање прибелешки на DOCX во Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) им олеснува на развивачите на Java да додаваат различни типови на прибелешки на датотеките DOCX во која било апликација базирана на Java со спроведување на неколку лесни чекори.
        *   Креирајте објекти за одговор со коментар и датум.
        *   Креирајте објект AreaAnnotation, поставете опции за областа и додајте одговори.
        *   Креирајте објект Annotator и додајте прибелешка за областа.
        *   Зачувајте ја излезната датотека.
    title_right: "Системски барања"
    content_right: |
        GroupDocs.Annotation за Java API се поддржани на сите главни платформи и оперативни системи. Пред да го извршите кодот подолу, проверете дали ги имате инсталирано следните предуслови на вашиот систем.
        *   Оперативни системи: Microsoft Windows, Linux, MacOS
        *   Развојна средина: NetBeans, Intellij IDEA, Eclipse итн
        *   Java Runtime Environment: Java 7 (1.7) и погоре
        *   Добијте ја најновата верзија на GroupDocs.Annotation за Java од [Репозиториум на артефакти на ГрупДок](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Преглед на прибелешки и примерок на код
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
    title_left: "Чекори за отстранување на прибелешки од DOCX во Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) им олеснува на развивачите на Java да ги отстранат деталите за прибелешки од датотеките DOCX во која било апликација базирана на Java со спроведување на неколку лесни чекори.
        *   Креирајте објекти за одговор со коментар и датум.
        *   Инстантирајте го објектот SaveOptions и поставете AnnotationTypes = AnnotationType.None.
        *   Повикајте го методот за зачувување со резултат на патеката или преносот на документот и објектот SaveOptions.

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
    title_left: "Чекори за уредување прибелешки од DOCX во Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) им олеснува на развивачите на Java да ажурираат различни својства на прибелешки од датотеките DOCX во која било апликација базирана на Java со спроведување на неколку лесни чекори.
        *   Instantiate Annotator објект со патека на влезен документ или пренос со инстанцирани LoadOptions со ImportAnnotations = точно.
        *   Направете некоја имплементација на AnnotationBase и поставете ИД на постоечка прибелешка (ако прибелешката со таа ИД не е пронајдена, ништо нема да се смени) или листа на патеки со прибелешки (сите постојни прибелешки ќе бидат отстранети).
        *   Начин на ажурирање повик на објект Annotator со поминати прибелешки.
        *   Повикајте го методот за зачувување со резултат на патеката или преносот на документот и објектот SaveOptions.

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
    title_left: "Чекори за екстракција на прибелешки од DOCX во Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) им олеснува на програмерите на Java да ставаат прибелешки и да извлечат информации за прибелешки од датотеките DOCX во која било апликација базирана на Java со спроведување на неколку лесни чекори.
        *   Креирајте објекти за одговор со коментар и датум.
        *   Инстантирајте го објектот LoadOptions и повикајте SetImportAnnotations со вистински аргумент.
        *   Дефинирајте ја променливата со тип Листа.
        *   Повикајте го методот за добивање и вратете го резултатот на променливата погоре.

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
    title: "Живи демонстрации за додавање, отстранување, уредување, екстракција на прибелешки на документи и слики"
    content: |
        Додајте, отстранувајте, уредувајте и извлечете прибелешки во датотеката DOCX во моментов со посета на веб-локацијата [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Демото во живо ги има следните предности

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docx"
          title: "За форматот на датотеката DOCX"
          content: |
            DOCX е добро познат формат за документи на Microsoft Word. Воведен од 2007 година со објавувањето на Microsoft Office 2007, структурата на овој нов формат на документ беше променета од обичен бинарен во комбинација на XML и бинарни датотеки. Датотеките Docx може да се отворат со Word 2007 и страничните верзии, но не и со претходните верзии на MS Word кои поддржуваат екстензии на датотеки DOC.

          link: "https://docs.fileformat.com/image/docx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Работа со други популарни формати на документи"
    content: |
        Ажурирајте ги својствата на прибелешките од некои од популарните формати на датотеки како што е наведено подолу.
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