---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "جاوا DOC Annotation API Annotate در سی شارپ"
head_description: "Java API برای ایجاد و حاشیه نویسی انواع حاشیه نویسی محبوب از DOC، تصاویر، نقشه ها و فرمت های فایل سند."

############################# Header ############################
title: "حاشیه نویسی DOC از جاوا"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "دانلود نسخه آزمایشی رایگان"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Annotation برای Java API"
    content: |
        GroupDocs.Annotation برای Java API کتابخانه ای است که به شما امکان می دهد حاشیه نویسی را به PDF، Word و سایر اسناد در مک، ویندوز یا اوبونتو اضافه کنید. [GroupDocs.Annotation for Java](/annotation/java) یک API بومی جاوا برای مدیریت حاشیه نویسی با پشتیبانی جامع برای ایجاد، افزودن، ویرایش، حذف، استخراج و صادر کردن حاشیه نویسی از تصاویر و اسناد مختلف دیگر است. فهرست کامل قالب‌های سند پشتیبانی‌شده را می‌توانید در این [صفحه] ببینید (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        این کتابخانه به شما امکان می دهد نه تنها با سند DOC بلکه با بسیاری از اسناد دیگر مانند Word، Excel، PowerPoint، Outlook ایمیل ها، Visio، Adobe، OpenDocument، OpenOffice، Photoshop، AutoCad و بسیاری دیگر کار کنید.
        GroupDocs.Annotation for Java API به شما امکان می دهد یادداشت های جدید ایجاد و اضافه کنید، حاشیه نویسی ها را ویرایش کنید، نظرات، حاشیه نویسی را استخراج کنید و آنها را از اسناد حذف کنید. این کتابخانه از 13 نوع حاشیه نویسی مختلف پشتیبانی می کند، از جمله متن، چند خط، ناحیه، زیر خط، نقطه، واترمارک، پیکان، بیضی، جایگزینی متن، فاصله، فیلد متن، ویرایش منابع در PDF، HTML، اسناد Microsoft Word، صفحات گسترده، نمودارها، ارائه ها، نقشه ها، تصاویر و بسیاری از فرمت های فایل دیگر.
        مثال (لطفاً به زیر مراجعه کنید) کار با سند DOC را نشان می دهد، در این مثال می توانید مراحل اصلی نحوه کار با GroupDocs را مشاهده کنید. حاشیه نویسی: راه اندازی مجوز، باز کردن سندی که می خواهید با آن کار کنید، ایجاد یک حاشیه نویسی، اضافه کردن اشیاء داده برای تنظیم ویژگی های حاشیه نویسی با توجه به نیاز شما و ذخیره نتیجه در مکان مورد نیاز. همچنین می‌توانید جزئیات بیشتری از ویژگی‌های پشتیبانی‌شده در [صفحه] github ما (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java)، یا در محصول ما [اسناد] (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "مراحل افزودن حاشیه نویسی به DOC در جاوا"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) با اجرای چند مرحله آسان، افزودن انواع حاشیه نویسی به فایل های DOC در هر برنامه مبتنی بر جاوا را برای توسعه دهندگان جاوا آسان می کند.
        *   اشیاء Reply را با نظر و تاریخ ایجاد کنید.
        *   شی AreaAnnotation ایجاد کنید، گزینه های ناحیه را تنظیم کنید و پاسخ ها را اضافه کنید.
        *   شی Annotator ایجاد کنید و حاشیه نویسی ناحیه را اضافه کنید.
        *   ذخیره فایل خروجی
    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Annotation برای API های جاوا در همه سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.
        *   سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        *   محیط توسعه: NetBeans، Intellij IDEA، Eclipse و غیره
        *   محیط اجرای جاوا: جاوا 7 (1.7) و بالاتر
        *   آخرین نسخه GroupDocs.Annotation را برای جاوا از [GroupDocs Artifact Repository] دریافت کنید (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: پیش نمایش حاشیه نویسی و نمونه کد
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
    title_left: "مراحل حذف حاشیه نویسی از DOC در جاوا"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) با اجرای چند مرحله آسان، حذف جزئیات حاشیه نویسی از فایل های DOC در هر برنامه مبتنی بر جاوا را برای توسعه دهندگان جاوا آسان تر می کند.
        *   اشیاء Reply را با نظر و تاریخ ایجاد کنید.
        *   آبجکت SaveOptions را نمونه برداری کنید و AnnotationTypes = AnnotationType.None را تنظیم کنید.
        *   فراخوانی روش ذخیره با مسیر سند حاصل یا جریان و شی SaveOptions.

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
    title_left: "مراحل ویرایش حاشیه نویسی از DOC در جاوا"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) با اجرای چند مرحله آسان، به‌روزرسانی ویژگی‌های حاشیه‌نویسی مختلف از فایل‌های DOC در هر برنامه مبتنی بر جاوا را برای توسعه‌دهندگان جاوا آسان‌تر می‌کند.
        *   شی Annotator با مسیر سند ورودی یا جریان با LoadOptions نمونه با ImportAnnotations = درست است.
        *   مقداری پیاده سازی AnnotationBase ایجاد کنید و شناسه حاشیه نویسی موجود را تنظیم کنید (اگر حاشیه نویسی با آن شناسه یافت نشد، چیزی تغییر نخواهد کرد) یا لیست مسیر حاشیه نویسی ها (همه حاشیه نویسی های موجود حذف خواهند شد).
        *   فراخوانی روش به روز رسانی شی Annotator با حاشیه نویسی ارسال شده.
        *   فراخوانی روش ذخیره با مسیر سند حاصل یا جریان و شی SaveOptions.

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
    title_left: "مراحل استخراج حاشیه نویسی از DOC در جاوا"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) با اجرای چند مرحله آسان، حاشیه نویسی اسناد و استخراج اطلاعات حاشیه نویسی از فایل های DOC در هر برنامه مبتنی بر جاوا را برای توسعه دهندگان جاوا آسان می کند.
        *   اشیاء Reply را با نظر و تاریخ ایجاد کنید.
        *   شی LoadOptions را Instantiate کنید و SetImportAnnotations را با آرگومان واقعی فراخوانی کنید.
        *   متغیر را با نوع List تعریف کنید.
        *   روش دریافت را فراخوانی کنید و نتیجه را به متغیر بالا برگردانید.

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
    title: "دموهای زنده برای افزودن، حذف، ویرایش، استخراج حاشیه نویسی به اسناد و تصاویر"
    content: |
        همین حالا با مراجعه به وب سایت [GroupDocs.Annotation Live Demos] (https://products.groupdocs.app/annotation/family)، یادداشت ها را به فایل DOC اضافه، حذف، ویرایش و استخراج کنید. نسخه ی نمایشی زنده دارای مزایای زیر است

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-doc"
          title: "درباره فرمت فایل DOC"
          content: |
            فایل‌های با پسوند doc اسنادی را نشان می‌دهند که توسط Microsoft Word یا سایر اسناد پردازش کلمه در قالب فایل باینری تولید شده‌اند. این پسوند در ابتدا برای اسناد متنی ساده در چندین سیستم عامل مختلف استفاده شد. این می تواند شامل چندین نوع داده مختلف مانند تصاویر، قالب بندی شده و همچنین متن ساده، نمودارها، نمودارها، اشیاء جاسازی شده، پیوندها، صفحات، قالب بندی صفحه، تنظیمات چاپ و بسیاری موارد دیگر باشد. این قالب به دلیل گزینه‌های متنوعی که برای نوشتن راهنماها، پروپوزال‌ها، مشخصات، رزومه‌ها، مقالات یا هر سند مشابهی به کاربران ارائه می‌دهد، برای انواع اسناد محبوب بود. نسخه به روز شده DOC DOCX است که مبتنی بر Office OpenXML است که مشخصات آن آشکارا در دسترس است.

          link: "https://docs.fileformat.com/image/doc/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "کار با سایر فرمت های سند محبوب"
    content: |
        ویژگی های حاشیه نویسی را از برخی از فرمت های فایل محبوب همانطور که در زیر ذکر شده است به روز کنید.
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