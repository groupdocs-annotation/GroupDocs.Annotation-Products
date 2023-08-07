---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net DOCM Annotation API Annotate in C #"
head_description: "Net API لإنشاء أنواع التعليقات التوضيحية الشائعة والتعليق عليها من DOCM وتنسيقات ملفات الصور والرسومات والمستندات."

############################# Header ############################
title: "علق DOCM من Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "تحميل النسخة التجريبية المجانية"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "حول GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API مكتبة تسمح لك بإضافة التعليقات التوضيحية إلى PDF و Word والمستندات الأخرى على Mac أو Windows أو Ubuntu. [GroupDocs.Annotation for Net] (/ حاشية / net) هي واجهة برمجة تطبيقات Net أصلية لإدارة التعليقات التوضيحية مع دعم شامل لإنشاء التعليقات التوضيحية وإضافتها وتحريرها وحذفها واستخراجها وتصديرها من الصور ومستندات أخرى متنوعة. القائمة الكاملة لتنسيقات المستندات المدعومة التي يمكن أن تراها في هذه [الصفحة] (https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        تتيح لك هذه المكتبة العمل ليس فقط مع مستند DOCM ولكن أيضًا مع العديد من أنواع المستندات الأخرى مثل Word و Excel و PowerPoint ورسائل البريد الإلكتروني في Outlook و Visio و Adobe و OpenDocument و OpenOffice و Photoshop و AutoCad وغيرها الكثير.
        تسمح لك GroupDocs.Annotation for Net API بإنشاء وإضافة ملاحظات جديدة وتعديل التعليقات التوضيحية واستخراج التعليقات والتعليقات التوضيحية وإزالتها من المستندات. تدعم المكتبة 13 نوعًا مختلفًا من التعليقات التوضيحية ، بما في ذلك Text و Polyline و Area و Underline و Point و Watermark و Arrow و Ellipse واستبدال النص والمسافة وحقل النص وتحرير الموارد في PDF و HTML ومستندات Microsoft Word وجداول البيانات والمخططات والعروض التقديمية ، الرسومات والصور والعديد من تنسيقات الملفات الأخرى.
        يوضح المثال (يرجى الاطلاع أدناه) العمل مع مستند DOCM ، في هذا المثال يمكنك رؤية الخطوات الرئيسية لكيفية العمل مع GroupDocs.Annotation: إعداد ترخيص ، افتح المستند الذي تريد العمل معه ، وإنشاء التعليق التوضيحي وإضافة كائنات البيانات لتعيين خصائص التعليقات التوضيحية وفقًا لمتطلباتك وحفظ النتيجة في المكان المطلوب. يمكنك أيضًا إلقاء نظرة أكثر تفصيلاً على الميزات المدعومة على github [صفحة] (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) ، أو في منتجنا [التوثيق] (https : //docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "خطوات إضافة التعليقات التوضيحية إلى DOCM في الشبكة"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) يسهل على مطوري الإنترنت إضافة أنواع مختلفة من التعليقات التوضيحية إلى ملفات DOCM داخل أي تطبيق قائم على الشبكة من خلال تنفيذ بضع خطوات سهلة.
        *   إنشاء كائنات الرد مع التعليق والتاريخ.
        *   إنشاء كائن AreaAnnotation ، وتعيين خيارات المنطقة وإضافة الردود.
        *   إنشاء كائن التعليق التوضيحي وإضافة تعليق توضيحي للمنطقة.
        *   حفظ ملف الإخراج.
    title_right: "متطلبات النظام"
    content_right: |
        GroupDocs.Annotation for Net APIs مدعومة على جميع الأنظمة الأساسية وأنظمة التشغيل الرئيسية. قبل تنفيذ الكود أدناه ، يرجى التأكد من تثبيت المتطلبات الأساسية التالية على نظامك.
        *   أنظمة التشغيل: مايكروسوفت ويندوز ، لينوكس ، ماك
        *   بيئات التطوير: Visual Studio و Xamarin و MonoDevelop
        *   الأطر: .NET Framework و .NET Standard و .NET Core و Mono
        *   قم بتنزيل أحدث إصدار من GroupDocs.Annotation for .NET من [NuGet] (https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: معاينة الشرح وعينة التعليمات البرمجية
    content: |
        ![Annotation preview image]https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png
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
    title_left: "خطوات إزالة التعليقات التوضيحية من DOCM في الشبكة"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) يسهل على مطوري الإنترنت إزالة تفاصيل التعليقات التوضيحية من ملفات DOCM داخل أي تطبيق قائم على الشبكة من خلال تنفيذ بضع خطوات سهلة.
        *   إنشاء كائنات الرد مع التعليق والتاريخ.
        *   إنشاء كائن SaveOptions وتعيين AnnotationTypes = AnnotationType.None.
        *   استدعاء طريقة حفظ مع مسار المستند الناتج أو دفق وكائن SaveOptions.

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
    title_left: "خطوات تحرير التعليقات التوضيحية من DOCM في الشبكة"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) يسهل على مطوري الإنترنت تحديث خصائص التعليقات التوضيحية المتنوعة من ملفات DOCM داخل أي تطبيق قائم على الشبكة من خلال تنفيذ بضع خطوات سهلة.
        *   إنشاء كائن Annotator مع مسار مستند الإدخال أو دفق مع LoadOptions تم إنشاء مثيل له مع ImportAnnotations = true.
        *   قم بإنشاء بعض تنفيذ AnnotationBase وقم بتعيين معرف التعليقات التوضيحية الموجودة (إذا لم يتم العثور على التعليق التوضيحي بهذا المعرف ، فلن يتم تغيير أي شيء) أو قائمة مسار التعليقات التوضيحية (ستتم إزالة جميع التعليقات التوضيحية الموجودة).
        *   طريقة تحديث المكالمة لكائن Annotator مع التعليقات التوضيحية التي تم تمريرها.
        *   استدعاء طريقة حفظ مع مسار المستند الناتج أو دفق وكائن SaveOptions.

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
    title_left: "خطوات استخراج التعليقات التوضيحية من DOCM في الشبكة"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) يُسهل على مطوري Net وضع تعليقات توضيحية على المستندات واستخراج معلومات التعليقات التوضيحية من ملفات DOCM داخل أي تطبيق مستند إلى Net عن طريق تنفيذ بضع خطوات سهلة.
        *   إنشاء كائنات الرد مع التعليق والتاريخ.
        *   إنشاء كائن LoadOptions واستدعاء SetImportAnnotations باستخدام وسيطة صحيحة.
        *   تحديد متغير مع نوع القائمة.
        *   استدعاء طريقة الحصول وإرجاع النتيجة إلى المتغير أعلاه.

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
    title: "العروض التوضيحية الحية لإضافة التعليقات التوضيحية إلى المستندات والصور وإزالتها وتحريرها واستخراجها"
    content: |
        قم بإضافة التعليقات التوضيحية وإزالتها وتعديلها واستخراجها إلى ملف DOCM الآن من خلال زيارة موقع ويب [GroupDocs.Annotation Live Demos] (https://products.groupdocs.app/annotation/family). يحتوي العرض التوضيحي المباشر على الفوائد التالية

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docm"
          title: "حول تنسيق الملف DOCM"
          content: |
            ملفات DOCM هي Microsoft Word 2007 أو مستندات تم إنشاؤها بأعلى مع إمكانية تشغيل وحدات الماكرو. إنه مشابه لتنسيق ملف DOCX ولكن القدرة على تشغيل وحدات الماكرو تجعله مختلفًا عن DOCX. مثل DOCX ، يمكن أن تخزن ملفات DOCM النصوص والصور والجداول والأشكال والمخططات والمحتويات الأخرى. تجعل القدرة على تشغيل وحدات الماكرو من السهل توفير الوقت عن طريق تنفيذ سلسلة الأوامر في شكل إجراءات مسجلة للإكمال التلقائي للمهمة . يمكن فتح ملفات DOCM وتحريرها في Microsoft Word 2007 وما فوق.

          link: "https://docs.fileformat.com/image/docm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "العمل مع تنسيقات المستندات الشائعة الأخرى"
    content: |
        قم بتحديث خصائص التعليقات التوضيحية من بعض تنسيقات الملفات الشائعة كما هو موضح أدناه.
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