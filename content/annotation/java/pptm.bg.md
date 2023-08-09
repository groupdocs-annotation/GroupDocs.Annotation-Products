---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPTM Анотация на API за анотация в C#"
head_description: "Java API за създаване и анотиране на популярни типове анотации от PPTM, изображения, чертежи и файлови формати на документи."

############################# Header ############################
title: "Анотирайте PPTM от Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Изтеглете безплатна пробна версия"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Относно GroupDocs.Annotation за Java API"
    content: |
        GroupDocs.Annotation for Java API е библиотека, която ви позволява да добавяте анотации към PDF, Word и други документи на Mac, Windows или Ubuntu. [GroupDocs.Annotation за Java](/annotation/java) е оригинален Java API за управление на анотации с цялостна поддръжка за създаване, добавяне, редактиране, изтриване, извличане и експортиране на анотации от изображения и различни други документи. Пълният списък на поддържаните формати на документи можете да видите на тази [страница](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Тази библиотека ви позволява да работите не само с документ PPTM, но и с много други типове документи като Word, Excel, PowerPoint, Outlook имейли, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad и много други.
        GroupDocs.Annotation за Java API ви позволява да създавате и добавяте нови бележки, да редактирате анотации, да извличате коментари, анотации и да ги премахвате от документи. Библиотеката поддържа 13 различни типа анотации, включително текст, полилиния, област, подчертаване, точка, воден знак, стрелка, елипса, замяна на текст, разстояние, текстово поле, редакция на ресурси в PDF, HTML, документи на Microsoft Word, електронни таблици, диаграми, презентации, чертежи, изображения и много други файлови формати.
        Примерът (моля, вижте по-долу) демонстрира работа с документ PPTM, в този пример можете да видите основните стъпки за това как да работите с GroupDocs. Анотация: Настройте лиценз, отворете документ, с който искате да работите, създаване на анотация, добавяне на обекти с данни, за да зададете свойства на анотация според вашите изисквания и запазване на резултата на необходимото място. Също така бихте могли да разгледате по-подробно поддържаните функции на нашата [страница в github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) или в [документацията на нашия продукт](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Стъпки за добавяне на анотации към PPTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) улеснява разработчиците на Java да добавят различни типове анотации към PPTM файлове във всяко приложение, базирано на Java, чрез прилагане на няколко лесни стъпки.
        *   Създайте обекти за отговор с коментар и дата.
        *   Създайте обект AreaAnnotation, задайте опции за областта и добавете отговори.
        *   Създайте обект Annotator и добавете анотация на областта.
        *   Запазете изходния файл.
    title_right: "Системни изисквания"
    content_right: |
        GroupDocs.Annotation за Java API се поддържат на всички основни платформи и операционни системи. Преди да изпълните кода по-долу, моля, уверете се, че имате следните предпоставки, инсталирани на вашата система.
        *   Операционни системи: Microsoft Windows, Linux, MacOS
        *   Среда за разработка: NetBeans, Intellij IDEA, Eclipse и др
        *   Java Runtime Environment: Java 7 (1.7) и по-нова версия
        *   Вземете най-новата версия на GroupDocs.Annotation за Java от [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Визуализация на анотация и примерен код
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
    title_left: "Стъпки за премахване на анотации от PPTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) улеснява разработчиците на Java да премахнат подробности за анотация от PPTM файлове в рамките на всяко Java-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте обекти за отговор с коментар и дата.
        *   Създайте обект SaveOptions и задайте AnnotationTypes = AnnotationType.None.
        *   Извикване на метод за запазване с резултатен път на документ или поток и обект SaveOptions.

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
    title_left: "Стъпки за редактиране на анотации от PPTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) улеснява разработчиците на Java да актуализират различни свойства на анотации от PPTM файлове в рамките на всяко Java-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте екземпляр на обект Annotator с входен път на документа или поток с инстанцирани LoadOptions с ImportAnnotations = true.
        *   Създайте реализация на AnnotationBase и задайте идентификатор на съществуваща анотация (ако анотация с този идентификатор не бъде намерена, нищо няма да бъде променено) или списък с пътеки на анотации (всички съществуващи анотации ще бъдат премахнати).
        *   Извикване на метод за актуализиране на обект Annotator с предадени анотации.
        *   Извикване на метод за запазване с резултатен път на документ или поток и обект SaveOptions.

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
    title_left: "Стъпки за извличане на анотации от PPTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) улеснява Java разработчиците да анотират документи и да извличат анотационна информация от PPTM файлове във всяко Java-базирано приложение чрез прилагане на няколко лесни стъпки.
        *   Създайте обекти за отговор с коментар и дата.
        *   Създайте обект LoadOptions и извикайте SetImportAnnotations с аргумент true.
        *   Дефинирайте променлива с тип List.
        *   Извикайте метода get и върнете резултата към променливата по-горе.

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
    title: "Демонстрации на живо за добавяне, премахване, редактиране, извличане на анотации към документи и изображения"
    content: |
        Добавяйте, премахвайте, редактирайте и извличайте анотации към файла PPTM точно сега, като посетите уебсайта [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Демото на живо има следните предимства

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pptm"
          title: "Относно файловия формат PPTM"
          content: |
            Файловете с разширение PPTM са презентационни файлове с активиран макрос, които са създадени с Microsoft PowerPoint 2007 или по-нови версии. Те са подобни на PPTX файловете с тази разлика, че страничните не могат да изпълняват макроси, въпреки че могат да съдържат макроси. PPTM файловете могат да се редактират, като ги отворите в Microsoft PowerPoint и актуализирате съдържанието. Друг подобен формат е PPSM, но той е само за четене по подразбиране и стартира слайдшоуто, когато се отвори. PPTM, подобно на PPTX, съдържа слайдове за различни презентационни елементи като текст, изображения, видеоклипове, графики и други свързани материали.

          link: "https://docs.fileformat.com/image/pptm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Работа с други популярни формати на документи"
    content: |
        Актуализирайте свойствата на анотацията от някои от популярните файлови формати, както е посочено по-долу.
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