---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java XLSM API анотації Анотація в C#"
head_description: "Java API для створення та анотування популярних типів анотацій із XLSM, зображень, малюнків і форматів файлів документів."

############################# Header ############################
title: "Анотація XLSM з Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Завантажте безкоштовну пробну версію"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Про GroupDocs.Annotation для Java API"
    content: |
        GroupDocs.Annotation for Java API — це бібліотека, яка дозволяє додавати анотації до PDF, Word та інших документів на Mac, Windows або Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) — це нативний Java API для керування анотаціями з повною підтримкою створення, додавання, редагування, видалення, вилучення й експорту анотацій із зображень та різних інших документів. Повний список підтримуваних форматів документів можна переглянути на цій [сторінці](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Ця бібліотека дозволяє вам працювати не лише з документом XLSM, а й з багатьма іншими типами документів, такими як Word, Excel, PowerPoint, електронні листи Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad та багато інших.
        API GroupDocs.Annotation для Java дозволяє створювати та додавати нові нотатки, редагувати анотації, вилучати коментарі, анотації та видаляти їх із документів. Бібліотека підтримує 13 різних типів анотацій, зокрема текст, ламана лінія, область, підкреслення, точка, водяний знак, стрілка, еліпс, заміна тексту, відстань, текстове поле, редакція ресурсу в документах PDF, HTML, Microsoft Word, електронних таблицях, діаграмах, презентаціях, малюнки, зображення та багато інших форматів файлів.
        Приклад (див. нижче) демонструє роботу з документом XLSM, у цьому прикладі ви можете побачити основні кроки роботи з GroupDocs. Анотація: налаштуйте ліцензію, відкрийте документ, з яким хочете працювати, створіть анотація, додавання об’єктів даних для встановлення властивостей анотації відповідно до ваших вимог і збереження результату в потрібному місці. Також ви можете детальніше ознайомитися з підтримуваними функціями на нашій [сторінці github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) або в [документації нашого продукту](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Кроки для додавання анотацій до XLSM у Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) дозволяє розробникам Java легко додавати різні типи анотацій до файлів XLSM у будь-якій програмі на основі Java, виконавши кілька простих кроків.
        *   Створення об’єктів відповіді з коментарем і датою.
        *   Створіть об’єкт AreaAnnotation, установіть параметри області та додайте відповіді.
        *   Створіть об’єкт Annotator і додайте анотацію області.
        *   Зберегти вихідний файл.
    title_right: "Системні вимоги"
    content_right: |
        API GroupDocs.Annotation для Java підтримуються на всіх основних платформах і операційних системах. Перш ніж виконувати наведений нижче код, переконайтеся, що у вашій системі встановлено такі передумови.
        *   Операційні системи: Microsoft Windows, Linux, MacOS
        *   Середовище розробки: NetBeans, Intellij IDEA, Eclipse тощо
        *   Java Runtime Environment: Java 7 (1.7) і вище
        *   Отримайте останню версію GroupDocs.Annotation для Java із [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Попередній перегляд анотації та приклад коду
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
    title_left: "Кроки для видалення анотацій із XLSM у Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) полегшує розробникам Java видалення деталей анотації з файлів XLSM у будь-якій програмі на основі Java, реалізувавши кілька простих кроків.
        *   Створення об’єктів відповіді з коментарем і датою.
        *   Створіть об’єкт SaveOptions і встановіть AnnotationTypes = AnnotationType.None.
        *   Виклик методу збереження з кінцевим шляхом або потоком документа та об’єктом SaveOptions.

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
    title_left: "Кроки для редагування анотацій із XLSM у Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) полегшує розробникам Java оновлення різноманітних властивостей анотацій із файлів XLSM у будь-якій програмі на основі Java за допомогою кількох простих кроків.
        *   Створення екземпляра об’єкта Annotator із вхідним шляхом документа або потоку з екземпляром LoadOptions із ImportAnnotations = true.
        *   Створіть деяку реалізацію AnnotationBase та встановіть ідентифікатор наявної анотації (якщо анотація з таким ідентифікатором не знайдена, нічого не буде змінено) або список шляхів анотацій (усі існуючі анотації буде видалено).
        *   Виклик методу оновлення об’єкта Annotator із переданими анотаціями.
        *   Виклик методу збереження з кінцевим шляхом або потоком документа та об’єктом SaveOptions.

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
    title_left: "Кроки для вилучення анотацій із XLSM у Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) спрощує розробникам Java коментувати документи та отримувати анотаційну інформацію з файлів XLSM у будь-якій програмі на основі Java, виконавши кілька простих кроків.
        *   Створення об’єктів відповіді з коментарем і датою.
        *   Створення екземпляра об’єкта LoadOptions і виклику SetImportAnnotations з аргументом true.
        *   Визначте змінну з типом List.
        *   Виклик методу get і повернення результату до змінної вище.

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
    title: "Живі демонстрації для додавання, видалення, редагування та вилучення анотацій до документів і зображень"
    content: |
        Додавайте, видаляйте, редагуйте та витягуйте анотації до файлу XLSM прямо зараз, відвідавши веб-сайт [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Жива демонстрація має такі переваги

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsm"
          title: "Про формат файлу XLSM"
          content: |
            Файли з розширенням XLSM – це тип файлів електронних таблиць, які підтримують макроси. З прикладної точки зору макрос — це набір інструкцій, які використовуються для автоматизації процесів. Макрос використовується для запису кроків, які виконуються неодноразово, і полегшує виконання дій шляхом повторного запуску макросу. Макроси програмуються за допомогою Microsoft Visual Basic for Applications (VBA) із робочої книги Excel за допомогою редактора Visual Basic, і їх можна запускати/налагоджувати безпосередньо звідти.

          link: "https://docs.fileformat.com/image/xlsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Робота з іншими популярними форматами документів"
    content: |
        Оновіть властивості анотації з деяких популярних форматів файлів, як зазначено нижче.
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