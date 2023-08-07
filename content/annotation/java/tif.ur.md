---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "C# میں Java TIF تشریح API تشریح"
head_description: "جاوا API TIF، تصاویر، ڈرائنگ اور دستاویز کی فائل فارمیٹس سے مشہور تشریحی اقسام بنانے اور تشریح کرنے کے لیے۔"

############################# Header ############################
title: "جاوا سے TIF تشریح کریں۔"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "مفت ٹرائل ڈاؤن لوڈ کریں۔"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "جاوا API کے لیے GroupDocs.Annotation کے بارے میں"
    content: |
        GroupDocs.Annotation for Java API ایک لائبریری ہے جو آپ کو PDF، Word اور Mac، Windows یا Ubuntu پر دیگر دستاویزات میں تشریحات شامل کرنے کی اجازت دیتی ہے۔ [GroupDocs.Annotation for Java](/annotation/java) تصاویر اور دیگر دستاویزات سے تشریحات بنانے، شامل کرنے، ترمیم کرنے، حذف کرنے، نکالنے اور برآمد کرنے کے لیے جامع تعاون کے ساتھ تشریحات کے انتظام کے لیے ایک مقامی Java API ہے۔ معاون دستاویز کے فارمیٹس کی مکمل فہرست جو آپ اس [صفحہ] (https://docs.groupdocs.com/annotation/java/supported-document-formats/) پر دیکھ سکتے ہیں۔
        یہ لائبریری آپ کو نہ صرف TIF دستاویز کے ساتھ کام کرنے کی اجازت دیتی ہے بلکہ بہت سی دوسری قسم کی دستاویزات جیسے Word, Excel, PowerPoint, Outlook ای میلز, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad اور بہت سے دوسرے کے ساتھ بھی کام کرنے کی اجازت دیتی ہے۔
        جاوا API کے لیے GroupDocs.Annotation آپ کو نئے نوٹ بنانے اور شامل کرنے، تشریحات میں ترمیم کرنے، تبصرے، تشریحات نکالنے اور انہیں دستاویزات سے ہٹانے کی اجازت دیتا ہے۔ لائبریری 13 مختلف تشریحی اقسام کو سپورٹ کرتی ہے، بشمول ٹیکسٹ، پولی لائن، ایریا، انڈر لائن، پوائنٹ، واٹر مارک، ایرو، ایلیپس، ٹیکسٹ ریپلیسمنٹ، فاصلہ، ٹیکسٹ فیلڈ، پی ڈی ایف میں ریسورس ریڈیکشن، ایچ ٹی ایم ایل، مائیکروسافٹ ورڈ دستاویزات، اسپریڈ شیٹس، ڈایاگرام، پریزنٹیشنز، ڈرائنگ، تصاویر اور بہت سے دوسرے فائل فارمیٹس۔
        مثال (براہ کرم نیچے دیکھیں) TIF دستاویز کے ساتھ کام کرنے کو ظاہر کرتی ہے، اس مثال میں آپ گروپ ڈاکس کے ساتھ کام کرنے کے اہم مراحل دیکھ سکتے ہیں۔ تشریح: ایک لائسنس ترتیب دیں، وہ دستاویز کھولیں جس کے ساتھ آپ کام کرنا چاہتے ہیں، ایک تخلیق تشریح، آپ کی ضروریات کے مطابق تشریحی خصوصیات کو سیٹ کرنے کے لیے ڈیٹا آبجیکٹ کو شامل کرنا اور نتیجہ کو مطلوبہ جگہ پر محفوظ کرنا۔ اس کے علاوہ آپ ہمارے گیتھب [صفحہ](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) پر یا ہماری پروڈکٹ [دستاویزات](https: //docs.groupdocs.com/annotation/java/getting-started/)۔

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "جاوا میں TIF میں تشریحات شامل کرنے کے اقدامات"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) جاوا ڈویلپرز کے لیے کسی بھی جاوا پر مبنی ایپلی کیشن میں TIF فائلوں میں مختلف تشریحی اقسام کو شامل کرنا آسان بناتا ہے چند آسان مراحل کو لاگو کرکے۔
        *   تبصرہ اور تاریخ کے ساتھ جوابی اشیاء بنائیں۔
        *   ایریا اینوٹیشن آبجیکٹ بنائیں، ایریا کے آپشن سیٹ کریں اور جوابات شامل کریں۔
        *   Annotator آبجیکٹ بنائیں اور علاقے کی تشریح شامل کریں۔
        *   آؤٹ پٹ فائل کو محفوظ کریں۔
    title_right: "سسٹم کے تقاضے"
    content_right: |
        GroupDocs.Annotation for Java APIs تمام بڑے پلیٹ فارمز اور آپریٹنگ سسٹمز پر تعاون یافتہ ہیں۔ ذیل کے کوڈ پر عمل کرنے سے پہلے، براہ کرم یقینی بنائیں کہ آپ کے سسٹم پر درج ذیل شرائط انسٹال ہیں۔
        *   آپریٹنگ سسٹمز: مائیکروسافٹ ونڈوز، لینکس، میک او ایس
        *   ترقیاتی ماحول: نیٹ بینز، انٹیلیج آئیڈیا، ایکلیپس وغیرہ
        *   Java Runtime Environment: Java 7 (1.7) اور اس سے اوپر
        *   جاوا کے لیے GroupDocs.Annotation کا تازہ ترین ورژن [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) سے حاصل کریں۔

############################# Preview ############################
preview_Add:
    enable: true
    title: تشریح کا پیش نظارہ اور کوڈ کا نمونہ
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
    title_left: "جاوا میں TIF سے تشریحات کو ہٹانے کے اقدامات"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) جاوا ڈویلپرز کے لیے کسی بھی جاوا پر مبنی ایپلیکیشن کے اندر سے TIF فائلوں سے تشریحی تفصیلات کو ہٹانا آسان بناتا ہے چند آسان اقدامات کو لاگو کرکے۔
        *   تبصرہ اور تاریخ کے ساتھ جوابی اشیاء بنائیں۔
        *   SaveOptions آبجیکٹ کو فوری بنائیں اور AnnotationTypes = AnnotationType.None سیٹ کریں۔
        *   نتیجہ خیز دستاویز کے راستے یا ندی اور SaveOptions آبجیکٹ کے ساتھ سیو میتھڈ کو کال کریں۔

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
    title_left: "جاوا میں TIF سے تشریحات میں ترمیم کرنے کے مراحل"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) جاوا ڈویلپرز کے لیے کسی بھی جاوا پر مبنی ایپلیکیشن کے اندر TIF فائلوں سے مختلف تشریحی خصوصیات کو اپ ڈیٹ کرنا آسان بناتا ہے چند آسان اقدامات کو لاگو کرکے۔
        *   Instantiate Annotator آبجیکٹ ان پٹ دستاویز کے راستے کے ساتھ یا سٹریم کے ساتھ Instantiated LoadOptions کے ساتھ ImportAnnotations = true۔
        *   کچھ AnnotationBase نفاذ بنائیں اور موجود تشریح کی Id سیٹ کریں (اگر اس Id کے ساتھ تشریح نہیں ملی تو کچھ بھی تبدیل نہیں کیا جائے گا) یا تشریحات کی پاتھ لسٹ (تمام موجود تشریحات کو ہٹا دیا جائے گا)۔
        *   منظور شدہ تشریحات کے ساتھ Annotator آبجیکٹ کے اپ ڈیٹ کا طریقہ۔
        *   نتیجہ خیز دستاویز کے راستے یا ندی اور SaveOptions آبجیکٹ کے ساتھ سیو میتھڈ کو کال کریں۔

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
    title_left: "جاوا میں TIF سے تشریحات نکالنے کے مراحل"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) جاوا ڈویلپرز کے لیے کچھ آسان اقدامات کو لاگو کرکے کسی بھی جاوا پر مبنی ایپلیکیشن کے اندر دستاویزات کی تشریح اور TIF فائلوں سے تشریحی معلومات نکالنا آسان بناتا ہے۔
        *   تبصرہ اور تاریخ کے ساتھ جوابی اشیاء بنائیں۔
        *   Instantiate LoadOptions آبجیکٹ اور SetImportAnnotations کو حقیقی دلیل کے ساتھ کال کریں۔
        *   قسم کی فہرست کے ساتھ متغیر کی وضاحت کریں۔
        *   حاصل کرنے کا طریقہ کال کریں اور نتیجہ اوپر متغیر پر لوٹائیں۔

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
    title: "دستاویزات اور تصاویر میں تشریحات شامل کرنے، ہٹانے، ترمیم کرنے، نکالنے کے لیے لائیو ڈیمو"
    content: |
        ابھی [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) ویب سائٹ پر جا کر TIF فائل میں تشریحات شامل کریں، ہٹائیں، ترمیم کریں اور نکالیں۔ لائیو ڈیمو کے درج ذیل فوائد ہیں۔

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-tif"
          title: "TIF فائل فارمیٹ کے بارے میں"
          content: |
            TIFF یا TIF، ٹیگ شدہ امیج فائل فارمیٹ، راسٹر امیجز کی نمائندگی کرتا ہے جو اس فائل فارمیٹ کے معیار کے مطابق مختلف آلات پر استعمال کے لیے ہیں۔ یہ متعدد رنگوں کی جگہوں پر بائل لیول، گرے اسکیل، پیلیٹ کلر اور فل کلر امیج ڈیٹا کو بیان کرنے کی صلاحیت رکھتا ہے۔ یہ فارمیٹ کا استعمال کرتے ہوئے ایپلی کیشنز کے لیے جگہ اور وقت کے درمیان انتخاب کرنے کے لیے نقصان دہ اور نقصان کے بغیر کمپریشن اسکیموں کی حمایت کرتا ہے۔ فارمیٹ مشین پر منحصر نہیں ہے اور یہ پروسیسر، آپریٹنگ سسٹم، یا فائل سسٹم جیسی حدود سے آزاد ہے۔

          link: "https://docs.fileformat.com/image/tif/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "دوسرے مشہور دستاویزی فارمیٹس کے ساتھ کام کرنا"
    content: |
        ذیل میں بیان کردہ کچھ مشہور فائل فارمیٹس سے تشریحی خصوصیات کو اپ ڈیٹ کریں۔
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