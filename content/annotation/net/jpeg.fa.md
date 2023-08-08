---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net JPEG Annotation API Annotate در سی شارپ"
head_description: "Net API برای ایجاد و حاشیه نویسی انواع حاشیه نویسی محبوب از JPEG، تصاویر، نقشه ها و فرمت های فایل سند."

############################# Header ############################
title: "حاشیه نویسی JPEG از Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "دانلود نسخه آزمایشی رایگان"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "درباره GroupDocs.Annotation برای Net API"
    content: |
        GroupDocs.Annotation برای Net API کتابخانه ای است که به شما امکان می دهد حاشیه نویسی را به PDF، Word و سایر اسناد در مک، ویندوز یا اوبونتو اضافه کنید. [GroupDocs.Annotation for Net](/annotation/net) یک Net API بومی برای مدیریت حاشیه نویسی با پشتیبانی جامع برای ایجاد، افزودن، ویرایش، حذف، استخراج و صادر کردن حاشیه نویسی از تصاویر و اسناد مختلف دیگر است. فهرست کامل قالب‌های سند پشتیبانی‌شده را می‌توانید در این [صفحه] ببینید (https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        این کتابخانه به شما امکان می دهد نه تنها با سند JPEG بلکه با بسیاری از اسناد دیگر مانند Word، Excel، PowerPoint، Outlook ایمیل ها، Visio، Adobe، OpenDocument، OpenOffice، Photoshop، AutoCad و بسیاری دیگر کار کنید.
        GroupDocs.Annotation for Net API به شما امکان می دهد یادداشت های جدید ایجاد و اضافه کنید، حاشیه نویسی ها را ویرایش کنید، نظرات، حاشیه نویسی را استخراج کنید و آنها را از اسناد حذف کنید. این کتابخانه از 13 نوع حاشیه نویسی مختلف پشتیبانی می کند، از جمله متن، چند خط، ناحیه، زیر خط، نقطه، واترمارک، پیکان، بیضی، جایگزینی متن، فاصله، فیلد متن، ویرایش منابع در PDF، HTML، اسناد Microsoft Word، صفحات گسترده، نمودارها، ارائه ها، نقشه ها، تصاویر و بسیاری از فرمت های فایل دیگر.
        مثال (لطفاً به زیر مراجعه کنید) کار با سند JPEG را نشان می دهد، در این مثال می توانید مراحل اصلی نحوه کار با GroupDocs را مشاهده کنید. حاشیه نویسی: راه اندازی مجوز، باز کردن سندی که می خواهید با آن کار کنید، ایجاد یک حاشیه نویسی، اضافه کردن اشیاء داده برای تنظیم ویژگی های حاشیه نویسی با توجه به نیاز شما و ذخیره نتیجه در مکان مورد نیاز. همچنین می‌توانید جزئیات بیشتری از ویژگی‌های پشتیبانی‌شده در [صفحه] github ما (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) یا در محصول ما [اسناد] (https) داشته باشید. ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "مراحل افزودن حاشیه نویسی به JPEG در Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) با اجرای چند مرحله آسان، افزودن انواع حاشیه نویسی به فایل های JPEG در هر برنامه مبتنی بر شبکه را برای توسعه دهندگان Net آسان می کند.
        *   اشیاء Reply را با نظر و تاریخ ایجاد کنید.
        *   شی AreaAnnotation ایجاد کنید، گزینه های ناحیه را تنظیم کنید و پاسخ ها را اضافه کنید.
        *   شی Annotator ایجاد کنید و حاشیه نویسی ناحیه را اضافه کنید.
        *   ذخیره فایل خروجی
    title_right: "سیستم مورد نیاز"
    content_right: |
        GroupDocs.Annotation برای API های Net در همه سیستم عامل ها و سیستم عامل های اصلی پشتیبانی می شود. لطفا قبل از اجرای کد زیر، از نصب پیش نیازهای زیر بر روی سیستم خود اطمینان حاصل کنید.
        *   سیستم عامل: مایکروسافت ویندوز، لینوکس، MacOS
        *   محیط های توسعه: Visual Studio، Xamarin، MonoDevelop
        *   فریم‌ورک‌ها: NET Framework، NET Standard، NET Core، Mono
        *   آخرین نسخه GroupDocs.Annotation را برای NET از [NuGet] دانلود کنید (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: پیش نمایش حاشیه نویسی و نمونه کد
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
        using (Annotator annotator = new Annotator("input.bmp"))
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "This is text field annotation",
                Opacity = 0.7,
                PageNumber = 0,
                PenStyle = PenStyle.Dot,
                PenWidth = 3,
                FontFamily = "Arial",
                TextHorizontalAlignment = HorizontalAlignment.Center,
                Replies = new List
                {
                    new Reply
                    {
                        Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "مراحل حذف حاشیه نویسی از JPEG در Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) با اجرای چند مرحله آسان، حذف جزئیات حاشیه نویسی از فایل های JPEG در هر برنامه مبتنی بر شبکه را برای توسعه دهندگان Net آسان تر می کند.
        *   اشیاء Reply را با نظر و تاریخ ایجاد کنید.
        *   آبجکت SaveOptions را نمونه برداری کنید و AnnotationTypes = AnnotationType.None را تنظیم کنید.
        *   فراخوانی روش ذخیره با مسیر سند حاصل یا جریان و شی SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "مراحل ویرایش حاشیه نویسی از JPEG در Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) با اجرای چند مرحله آسان، به‌روزرسانی ویژگی‌های حاشیه‌نویسی مختلف از فایل‌های JPEG در هر برنامه مبتنی بر شبکه را برای توسعه‌دهندگان Net آسان‌تر می‌کند.
        *   شی Annotator با مسیر سند ورودی یا جریان با LoadOptions نمونه با ImportAnnotations = درست است.
        *   مقداری پیاده سازی AnnotationBase ایجاد کنید و شناسه حاشیه نویسی موجود را تنظیم کنید (اگر حاشیه نویسی با آن شناسه یافت نشد، چیزی تغییر نخواهد کرد) یا لیست مسیر حاشیه نویسی ها (همه حاشیه نویسی های موجود حذف خواهند شد).
        *   فراخوانی روش به روز رسانی شی Annotator با حاشیه نویسی ارسال شده.
        *   فراخوانی روش ذخیره با مسیر سند حاصل یا جریان و شی SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```cs
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Updated first comment",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Updated second comment",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "مراحل استخراج حاشیه نویسی از JPEG در Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) با اجرای چند مرحله آسان، حاشیه نویسی اسناد و استخراج اطلاعات حاشیه نویسی از فایل های JPEG را برای توسعه دهندگان Net آسان می کند.
        *   اشیاء Reply را با نظر و تاریخ ایجاد کنید.
        *   شی LoadOptions را Instantiate کنید و SetImportAnnotations را با آرگومان واقعی فراخوانی کنید.
        *   متغیر را با نوع List تعریف کنید.
        *   روش دریافت را فراخوانی کنید و نتیجه را به متغیر بالا برگردانید.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```cs
        // for using this example input file ("annotated.bmp") must be with annotations
        using (Annotator annotator = new Annotator("annotated.bmp"))
        {
            List annotations = annotator.Get();
            XmlSerializer formatter = new XmlSerializer(typeof(List));
            using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
                fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```

############################# Demos ############################
demos:
    enable: true
    title: "دموهای زنده برای افزودن، حذف، ویرایش، استخراج حاشیه نویسی به اسناد و تصاویر"
    content: |
        همین حالا با مراجعه به وب سایت [GroupDocs.Annotation Live Demos] (https://products.groupdocs.app/annotation/family)، یادداشت ها را به فایل JPEG اضافه، حذف، ویرایش و استخراج کنید. نسخه ی نمایشی زنده دارای مزایای زیر است

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpeg"
          title: "درباره فرمت فایل JPEG"
          content: |
            JPEG نوعی فرمت تصویر است که با استفاده از روش فشرده سازی با اتلاف ذخیره می شود. تصویر خروجی، در نتیجه فشرده سازی، تعادلی بین اندازه ذخیره سازی و کیفیت تصویر است. کاربران می توانند سطح فشرده سازی را برای رسیدن به سطح کیفی مورد نظر تنظیم کنند و در عین حال اندازه ذخیره سازی را کاهش دهند. اگر فشرده سازی 10:1 روی تصویر اعمال شود، کیفیت تصویر به میزان قابل توجهی تحت تأثیر قرار می گیرد. هرچه مقدار فشرده سازی بیشتر باشد، کیفیت تصویر کاهش می یابد. فرمت فایل تصویر JPEG توسط Joint Photographic Experts Group استاندارد شد و از این رو JPEG نام گرفت. فرمت انتخاب ذخیره و انتقال تصاویر عکاسی در وب بوده است. تقریباً تمام سیستم‌های عامل اکنون بیننده‌هایی دارند که از تجسم تصاویر JPEG پشتیبانی می‌کنند، که اغلب با پسوند JPG نیز ذخیره می‌شوند. حتی مرورگرهای وب از تجسم تصاویر JPEG پشتیبانی می کنند.

          link: "https://docs.fileformat.com/image/jpeg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "کار با سایر فرمت های سند محبوب"
    content: |
        ویژگی های حاشیه نویسی را از برخی از فرمت های فایل محبوب همانطور که در زیر ذکر شده است به روز کنید.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/net/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/net/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/net/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/net/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/net/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/net/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/net/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/net/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/net/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/net/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/net/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/net/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/net/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/net/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/net/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/net/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/net/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/net/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/net/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/net/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/net/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/net/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/net/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/net/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/net/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/net/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/net/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/net/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/net/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/net/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/net/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/net/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/net/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/net/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/net/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---