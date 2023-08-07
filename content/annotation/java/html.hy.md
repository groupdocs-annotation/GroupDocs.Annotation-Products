---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java HTML Annotation API Annotate in C#"
head_description: "Java API՝ HTML-ից հայտնի ծանոթագրությունների տեսակներ ստեղծելու և ծանոթագրելու համար, պատկերներ, գծագրեր և փաստաթղթերի ֆայլերի ձևաչափեր:"

############################# Header ############################
title: "Նշեք HTML Java-ից"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ներբեռնեք անվճար փորձաշրջան"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Annotation-ի մասին Java API-ի համար"
    content: |
        GroupDocs.Annotation-ը Java API-ի համար գրադարան է, որը թույլ է տալիս անոտացիաներ ավելացնել PDF, Word և այլ փաստաթղթեր Mac-ում, Windows-ում կամ Ubuntu-ում: [GroupDocs.Annotation for Java](/annotation/java) բնիկ Java API-ն է՝ ծանոթագրությունները կառավարելու համար՝ պատկերներից և տարբեր այլ փաստաթղթերից ծանոթագրություններ ստեղծելու, ավելացնելու, խմբագրելու, ջնջելու, հանելու և արտահանելու համապարփակ աջակցությամբ: Աջակցվող փաստաթղթերի ձևաչափերի ամբողջական ցանկը, որոնք կարող եք տեսնել այս [էջում] (https://docs.groupdocs.com/annotation/java/supported-document-formats/):
        Այս գրադարանը թույլ է տալիս աշխատել ոչ միայն HTML փաստաթղթի, այլ նաև բազմաթիվ այլ տեսակի փաստաթղթերի հետ, ինչպիսիք են Word, Excel, PowerPoint, Outlook էլ. նամակներ, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad և շատ այլ փաստաթղթեր:
        GroupDocs.Annotation-ը Java API-ի համար թույլ է տալիս ստեղծել և ավելացնել նոր նշումներ, խմբագրել ծանոթագրությունները, հանել մեկնաբանություններ, ծանոթագրություններ և հեռացնել դրանք փաստաթղթերից: Գրադարանը աջակցում է անոտացիայի 13 տարբեր տեսակների, այդ թվում՝ տեքստ, պոլիգիծ, տարածք, ընդգծում, կետ, ջրանիշ, սլաք, էլիպս, տեքստի փոխարինում, հեռավորություն, տեքստային դաշտ, ռեսուրսների խմբագրում PDF, HTML, Microsoft Word փաստաթղթերում, աղյուսակներ, դիագրամներ, ներկայացումներ, գծագրեր, պատկերներ և շատ այլ ֆայլերի ձևաչափեր:
        Օրինակը (տես ստորև) ցույց է տալիս աշխատանքը HTML փաստաթղթի հետ, այս օրինակում կարող եք տեսնել GroupDocs-ի հետ աշխատելու հիմնական քայլերը: Ծանոթագրություն. Կարգավորեք լիցենզիա, բացեք փաստաթուղթ, որի հետ ցանկանում եք աշխատել, ստեղծելով անոտացիա՝ ավելացնելով տվյալների օբյեկտներ՝ ձեր պահանջներին համապատասխան անոտացիոն հատկություններ սահմանելու համար և արդյունքը պահելով անհրաժեշտ տեղում: Նաև կարող եք ավելի մանրամասն ծանոթանալ մեր github-ի [էջի] աջակցվող գործառույթներին (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) կամ մեր արտադրանքի [փաստաթղթերում] (https: //docs.groupdocs.com/annotation/java/getting-started/):

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java-ում HTML-ին ծանոթագրություններ ավելացնելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java-ի մշակողների համար հեշտացնում է անոտացիայի զանազան տեսակներ ավելացնել HTML ֆայլերին Java-ի վրա հիմնված ցանկացած հավելվածի մեջ՝ մի քանի հեշտ քայլեր իրականացնելով:
        *   Ստեղծեք Reply օբյեկտներ՝ մեկնաբանությամբ և ամսաթվով:
        *   Ստեղծեք AreaAnnotation օբյեկտ, սահմանեք տարածքի ընտրանքները և ավելացրեք պատասխաններ:
        *   Ստեղծեք Annotator օբյեկտ և ավելացրեք տարածքի անոտացիա:
        *   Պահպանեք ելքային ֆայլը:
    title_right: "Համակարգի պահանջները"
    content_right: |
        GroupDocs.Annotation-ը Java API-ների համար աջակցվում է բոլոր հիմնական հարթակներում և օպերացիոն համակարգերում: Նախքան ստորև նշված կոդը գործարկելը, համոզվեք, որ ձեր համակարգում տեղադրված են հետևյալ նախադրյալները.
        *   Օպերացիոն համակարգեր՝ Microsoft Windows, Linux, MacOS
        *   Զարգացման միջավայր՝ NetBeans, Intellij IDEA, Eclipse և այլն
        *   Java Runtime Environment՝ Java 7 (1.7) և ավելի բարձր
        *   Ստացեք GroupDocs.Annotation-ի վերջին տարբերակը Java-ի համար [GroupDocs Artifact Repository]-ից (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Անոտացիայի նախադիտում և կոդի նմուշ
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
    title_left: "Java-ում ծանոթագրությունները HTML-ից հեռացնելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java-ի ծրագրավորողների համար հեշտացնում է անոտացիայի մանրամասները HTML ֆայլերից հեռացնելը Java-ի վրա հիմնված ցանկացած հավելվածի մեջ՝ մի քանի հեշտ քայլեր իրականացնելով:
        *   Ստեղծեք Reply օբյեկտներ՝ մեկնաբանությամբ և ամսաթվով:
        *   Տեղադրեք SaveOptions օբյեկտը և սահմանեք AnnotationTypes = AnnotationType.None:
        *   Զանգահարեք պահպանման մեթոդը՝ ստացված փաստաթղթի ճանապարհով կամ հոսքով և SaveOptions օբյեկտով:

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
    title_left: "Java-ում HTML-ի ծանոթագրությունները խմբագրելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java-ի մշակողների համար հեշտացնում է անոտացիայի տարբեր հատկություններ թարմացնել HTML ֆայլերից Java-ի վրա հիմնված ցանկացած հավելվածի մեջ՝ իրականացնելով մի քանի հեշտ քայլեր:
        *   Instantiate Annotator օբյեկտը մուտքագրված փաստաթղթի ուղով կամ հոսք՝ instantiated LoadOptions-ով ImportAnnotations-ով = true:
        *   Ստեղծեք AnnotationBase-ի ներդրում և սահմանեք գոյություն ունեցող անոտացիայի ID-ն (եթե այդ ID-ով ծանոթագրությունը չի գտնվել, ոչինչ չի փոխվի) կամ ծանոթագրությունների ուղու ցանկը (բոլոր գոյություն ունեցող ծանոթագրությունները կհեռացվեն):
        *   Annotator օբյեկտի զանգի թարմացման եղանակը՝ անցած ծանոթագրություններով:
        *   Զանգահարեք պահպանման մեթոդը՝ ստացված փաստաթղթի ճանապարհով կամ հոսքով և SaveOptions օբյեկտով:

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
    title_left: "Java-ում HTML-ից ծանոթագրություններ հանելու քայլեր"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java-ի մշակողների համար հեշտացնում է փաստաթղթերը ծանոթագրելը և HTML ֆայլերից անոտացիոն տեղեկություններ հանելը Java-ի վրա հիմնված ցանկացած հավելվածի մեջ՝ իրականացնելով մի քանի հեշտ քայլեր:
        *   Ստեղծեք Reply օբյեկտներ՝ մեկնաբանությամբ և ամսաթվով:
        *   Instantiate LoadOptions օբյեկտը և կանչեք SetImportAnnotations ճշմարիտ արգումենտով:
        *   Սահմանել փոփոխականը «List» տիպով:
        *   Զանգահարեք ստացման մեթոդը և վերադարձրեք արդյունքը վերը նշված փոփոխականին:

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
    title: "Կենդանի ցուցադրություններ՝ փաստաթղթերի և պատկերների վրա ավելացնելու, հեռացնելու, խմբագրելու, ծանոթագրություններ հանելու համար"
    content: |
        Ավելացրեք, հեռացրեք, խմբագրեք և հանեք ծանոթագրություններ HTML ֆայլում հենց հիմա՝ այցելելով [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) կայքը: Կենդանի ցուցադրությունն ունի հետևյալ առավելությունները

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-html"
          title: "HTML Ֆայլի ձևաչափի մասին"
          content: |
            HTML (Hyper Text Markup Language) ընդլայնումն է վեբ էջերի համար, որոնք ստեղծված են բրաուզերում ցուցադրելու համար: Հայտնի է որպես համացանցի լեզու, HTML-ը զարգացել է նոր տեղեկատվական պահանջների պահանջներով, որոնք պետք է ցուցադրվեն որպես վեբ էջերի մաս: Վերջին տարբերակը հայտնի է որպես HTML 5, որը մեծ ճկունություն է տալիս լեզվի հետ աշխատելու համար: HTML էջերը կամ ստացվում են սերվերից, որտեղ դրանք տեղակայված են, կամ կարող են բեռնվել նաև տեղական համակարգից: Յուրաքանչյուր HTML էջ կազմված է HTML տարրերից, ինչպիսիք են ձևերը, տեքստը, պատկերները, անիմացիաները, հղումները և այլն: Այս տարրերը ներկայացված են թեգերով, ինչպիսիք են img, a, p և մի քանի այլ պիտակներ, որտեղ յուրաքանչյուր պիտակ ունի սկիզբ և ավարտ: Այն կարող է նաև տեղադրել սկրիպտային լեզուներով գրված հավելվածներ, ինչպիսիք են JavaScript-ը և Style Sheets (CSS)՝ ընդհանուր դասավորության ներկայացման համար:

          link: "https://docs.fileformat.com/image/html/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Աշխատեք փաստաթղթի այլ հանրաճանաչ ձևաչափերի հետ"
    content: |
        Թարմացրեք ծանոթագրության հատկությունները որոշ հայտնի ֆայլերի ձևաչափերից, ինչպես նշված է ստորև:
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