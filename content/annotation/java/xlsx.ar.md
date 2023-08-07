---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java XLSX Annotation API Annotate in C #"
head_description: "Java API لإنشاء أنواع التعليقات التوضيحية الشائعة والتعليق عليها من XLSX وتنسيقات ملفات الصور والرسومات والمستندات."

############################# Header ############################
title: "علق XLSX من جافا"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "تحميل النسخة التجريبية المجانية"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "حول GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API هي مكتبة تسمح لك بإضافة التعليقات التوضيحية إلى PDF و Word والمستندات الأخرى على Mac أو Windows أو Ubuntu. [GroupDocs.Annotation for Java] (/ annotation / java) هي واجهة برمجة تطبيقات Java أصلية لإدارة التعليقات التوضيحية مع دعم شامل لإنشاء التعليقات التوضيحية وإضافتها وتحريرها وحذفها واستخراجها وتصديرها من الصور ومستندات أخرى متنوعة. القائمة الكاملة لتنسيقات المستندات المدعومة التي يمكن أن تراها في هذه [الصفحة] (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        تتيح لك هذه المكتبة العمل ليس فقط مع مستند XLSX ولكن أيضًا مع العديد من أنواع المستندات الأخرى مثل Word و Excel و PowerPoint ورسائل البريد الإلكتروني في Outlook و Visio و Adobe و OpenDocument و OpenOffice و Photoshop و AutoCad وغيرها الكثير.
        تسمح لك GroupDocs.Annotation for Java API بإنشاء وإضافة ملاحظات جديدة وتحرير التعليقات التوضيحية واستخراج التعليقات والتعليقات التوضيحية وإزالتها من المستندات. تدعم المكتبة 13 نوعًا مختلفًا من التعليقات التوضيحية ، بما في ذلك Text و Polyline و Area و Underline و Point و Watermark و Arrow و Ellipse واستبدال النص والمسافة وحقل النص وتحرير الموارد في PDF و HTML ومستندات Microsoft Word وجداول البيانات والمخططات والعروض التقديمية ، الرسومات والصور والعديد من تنسيقات الملفات الأخرى.
        يوضح المثال (يرجى الاطلاع أدناه) العمل مع مستند XLSX ، في هذا المثال يمكنك رؤية الخطوات الرئيسية لكيفية العمل مع GroupDocs.Annotation: إعداد ترخيص ، افتح المستند الذي تريد العمل معه ، وإنشاء التعليق التوضيحي وإضافة كائنات البيانات لتعيين خصائص التعليقات التوضيحية وفقًا لمتطلباتك وحفظ النتيجة في المكان المطلوب. يمكنك أيضًا إلقاء نظرة أكثر تفصيلاً على الميزات المدعومة على github [صفحة] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) ، أو في منتجنا [التوثيق] (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "خطوات إضافة التعليقات التوضيحية إلى XLSX في Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) يُسهل على مطوري Java إضافة أنواع مختلفة من التعليقات التوضيحية إلى ملفات XLSX داخل أي تطبيق قائم على Java عن طريق تنفيذ بضع خطوات سهلة.
        *   إنشاء كائنات الرد مع التعليق والتاريخ.
        *   إنشاء كائن AreaAnnotation ، وتعيين خيارات المنطقة وإضافة الردود.
        *   إنشاء كائن التعليق التوضيحي وإضافة تعليق توضيحي للمنطقة.
        *   حفظ ملف الإخراج.
    title_right: "متطلبات النظام"
    content_right: |
        GroupDocs.Annotation for Java APIs مدعومة على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.
        *   أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        *   بيئة التطوير: NetBeans ، Intellij IDEA ، Eclipse إلخ
        *   Java Runtime Environment: Java 7 (1.7) وما فوق
        *   احصل على أحدث إصدار من GroupDocs.Annotation for Java من [GroupDocs Artifact Repository] (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: معاينة الشرح وعينة التعليمات البرمجية
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
    title_left: "خطوات إزالة التعليقات التوضيحية من XLSX في Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) يسهل على مطوري Java إزالة تفاصيل التعليقات التوضيحية من ملفات XLSX داخل أي تطبيق مستند إلى Java عن طريق تنفيذ بضع خطوات سهلة.
        *   إنشاء كائنات الرد مع التعليق والتاريخ.
        *   إنشاء كائن SaveOptions وتعيين AnnotationTypes = AnnotationType.None.
        *   استدعاء طريقة حفظ مع مسار المستند الناتج أو دفق وكائن SaveOptions.

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
    title_left: "خطوات تحرير التعليقات التوضيحية من XLSX في Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) يسهل على مطوري Java تحديث خصائص التعليقات التوضيحية المتنوعة من ملفات XLSX داخل أي تطبيق قائم على Java عن طريق تنفيذ بضع خطوات سهلة.
        *   إنشاء كائن Annotator مع مسار مستند الإدخال أو دفق مع LoadOptions تم إنشاء مثيل له مع ImportAnnotations = true.
        *   قم بإنشاء بعض تنفيذ AnnotationBase وقم بتعيين معرف التعليقات التوضيحية الموجودة (إذا لم يتم العثور على التعليق التوضيحي بهذا المعرف ، فلن يتم تغيير أي شيء) أو قائمة مسار التعليقات التوضيحية (ستتم إزالة جميع التعليقات التوضيحية الموجودة).
        *   طريقة تحديث المكالمة لكائن Annotator مع التعليقات التوضيحية التي تم تمريرها.
        *   استدعاء طريقة حفظ مع مسار المستند الناتج أو دفق وكائن SaveOptions.

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
    title_left: "خطوات استخراج التعليقات التوضيحية من XLSX في Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) يُسهل على مطوري Java كتابة التعليقات التوضيحية على المستندات واستخراج معلومات التعليقات التوضيحية من ملفات XLSX داخل أي تطبيق مستند إلى Java عن طريق تنفيذ بضع خطوات سهلة.
        *   إنشاء كائنات الرد مع التعليق والتاريخ.
        *   إنشاء كائن LoadOptions واستدعاء SetImportAnnotations باستخدام وسيطة صحيحة.
        *   تحديد متغير مع نوع القائمة.
        *   استدعاء طريقة الحصول وإرجاع النتيجة إلى المتغير أعلاه.

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
    title: "العروض التوضيحية الحية لإضافة التعليقات التوضيحية إلى المستندات والصور وإزالتها وتحريرها واستخراجها"
    content: |
        قم بإضافة التعليقات التوضيحية وإزالتها وتعديلها واستخراجها إلى ملف XLSX الآن من خلال زيارة موقع ويب [GroupDocs.Annotation Live Demos] (https://products.groupdocs.app/annotation/family). يحتوي العرض التوضيحي المباشر على الفوائد التالية

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsx"
          title: "حول تنسيق الملف XLSX"
          content: |
            XLSX هو تنسيق معروف لمستندات Microsoft Excel تم تقديمه بواسطة Microsoft مع إصدار Microsoft Office 2007. استنادًا إلى الهيكل المنظم وفقًا لاتفاقيات التغليف المفتوح كما هو موضح في الجزء 2 من معيار OOXML ECMA-376 ، فإن التنسيق الجديد هو حزمة مضغوطة تحتوي على عدد من ملفات XML. يمكن فحص البنية والملفات الأساسية ببساطة عن طريق فك ضغط ملف .xlsx.

          link: "https://docs.fileformat.com/image/xlsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "العمل مع تنسيقات المستندات الشائعة الأخرى"
    content: |
        قم بتحديث خصائص التعليقات التوضيحية من بعض تنسيقات الملفات الشائعة كما هو موضح أدناه.
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