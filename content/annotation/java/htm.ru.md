---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java HTM Annotation API Аннотации в C#"
head_description: "Java API для создания и аннотирования популярных типов аннотаций из HTM, изображений, рисунков и форматов файлов документов."

############################# Header ############################
title: "Аннотировать HTM из Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Скачать бесплатную пробную версию"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "О GroupDocs.Annotation для Java API"
    content: |
        GroupDocs.Annotation for Java API — это библиотека, позволяющая добавлять аннотации в PDF, Word и другие документы на Mac, Windows или Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) — это собственный Java API для управления аннотациями с комплексной поддержкой создания, добавления, редактирования, удаления, извлечения и экспорта аннотаций из изображений и различных других документов. Полный список поддерживаемых форматов документов вы можете увидеть на этой [странице](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Эта библиотека позволяет работать не только с документом HTM, но и со многими другими типами документов, такими как Word, Excel, PowerPoint, сообщения электронной почты Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad и многими другими.
        API GroupDocs.Annotation for Java позволяет создавать и добавлять новые заметки, редактировать аннотации, извлекать комментарии, аннотации и удалять их из документов. Библиотека поддерживает 13 различных типов аннотаций, включая текст, полилинию, область, подчеркивание, точку, водяной знак, стрелку, эллипс, замену текста, расстояние, текстовое поле, редактирование ресурсов в PDF, HTML, документах Microsoft Word, электронных таблицах, диаграммах, презентациях, чертежи, изображения и многие другие форматы файлов.
        Пример (см. ниже) демонстрирует работу с документом HTM, в этом примере вы можете увидеть основные шаги работы с GroupDocs. аннотацию, добавляя объекты данных для установки свойств аннотации в соответствии с вашими требованиями и сохраняя результат в нужном месте. Также вы можете более подробно ознакомиться с поддерживаемыми функциями на нашей [странице] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) или в [документации] нашего продукта (https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Шаги по добавлению аннотаций в HTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) позволяет разработчикам Java легко добавлять различные типы аннотаций к файлам HTM в любом приложении на основе Java, выполняя несколько простых шагов.
        *   Создайте объекты ответа с комментарием и датой.
        *   Создайте объект AreaAnnotation, установите параметры области и добавьте ответы.
        *   Создайте объект Annotator и добавьте аннотацию области.
        *   Сохраните выходной файл.
    title_right: "Системные Требования"
    content_right: |
        API GroupDocs.Annotation для Java поддерживаются на всех основных платформах и операционных системах. Перед выполнением приведенного ниже кода убедитесь, что в вашей системе установлены следующие предварительные компоненты.
        *   Операционные системы: Microsoft Windows, Linux, MacOS
        *   Среда разработки: NetBeans, Intellij IDEA, Eclipse и т. д.
        *   Среда выполнения Java: Java 7 (1.7) и выше
        *   Получите последнюю версию GroupDocs.Annotation для Java из [репозитория артефактов GroupDocs] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Предварительный просмотр аннотации и пример кода
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
    title_left: "Действия по удалению аннотаций из HTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) упрощает разработчикам Java удаление деталей аннотаций из файлов HTM в любом приложении на основе Java за счет выполнения нескольких простых шагов.
        *   Создайте объекты ответа с комментарием и датой.
        *   Создайте экземпляр объекта SaveOptions и установите AnnotationTypes = AnnotationType.None.
        *   Вызовите метод сохранения с результирующим путем или потоком документа и объектом SaveOptions.

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
    title_left: "Шаги по редактированию аннотаций из HTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) упрощает разработчикам Java обновление различных свойств аннотаций из файлов HTM в любом приложении на основе Java за счет выполнения нескольких простых шагов.
        *   Создайте экземпляр объекта Annotator с путем или потоком входного документа с созданным экземпляром LoadOptions с ImportAnnotations = true.
        *   Создайте некоторую реализацию AnnotationBase и установите идентификатор существующей аннотации (если аннотация с этим идентификатором не найдена, ничего не изменится) или список путей аннотаций (все существующие аннотации будут удалены).
        *   Вызвать метод обновления объекта Annotator с переданными аннотациями.
        *   Вызовите метод сохранения с результирующим путем или потоком документа и объектом SaveOptions.

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
    title_left: "Действия по извлечению аннотаций из HTM в Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) позволяет разработчикам Java легко аннотировать документы и извлекать аннотационную информацию из файлов HTM в любом приложении на основе Java, выполнив несколько простых шагов.
        *   Создайте объекты ответа с комментарием и датой.
        *   Создайте экземпляр объекта LoadOptions и вызовите SetImportAnnotations с аргументом true.
        *   Определите переменную с типом List.
        *   Вызовите метод get и верните результат в переменную выше.

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
    title: "Живые демонстрации для добавления, удаления, редактирования, извлечения аннотаций к документам и изображениям"
    content: |
        Добавляйте, удаляйте, редактируйте и извлекайте аннотации к файлу HTM прямо сейчас, посетив веб-сайт [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Живая демонстрация имеет следующие преимущества

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-htm"
          title: "О формате файла HTM"
          content: |
            Файлы с расширением HTM представляют собой язык гипертекстовой разметки для создания веб-страниц для отображения в веб-браузерах, таких как Google Chrome, Internet Explorer, Firefox и ряде других. Он определяет разметку для создания статических страниц, которые будут опубликованы во всемирной паутине (WWW) для доступа других лиц. Эти разметки сообщают браузерам, как отображать содержимое веб-страницы. Такие страницы могут содержать обычный текст, изображения, гиперссылки на другие страницы, видео и другую медиаинформацию. Когда веб-страница публикуется, вы можете взглянуть на код разметки, стоящий за ней, просмотрев исходный код страницы. Современные браузеры позволяют просматривать каждый раздел веб-страницы, где прорабатывается каждый подраздел или элемент разметки в исходном коде HTM.

          link: "https://docs.fileformat.com/image/htm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Работа с другими популярными форматами документов"
    content: |
        Обновите свойства аннотаций из некоторых популярных форматов файлов, как указано ниже.
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