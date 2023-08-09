---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "הערות נטו של PPTM הערות API ב-C#"
head_description: "Net API ליצירה והערה של סוגי הערות פופולריים מ-PPTM, תמונות, שרטוטים ופורמטים של קבצי מסמכים."

############################# Header ############################
title: "הערה PPTM מ-Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "הורד גרסת ניסיון בחינם"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "אודות GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API היא ספרייה המאפשרת לך להוסיף הערות ל-PDF, Word ומסמכים אחרים ב-Mac, Windows או Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) הוא ממשק API מקורי של Net לניהול הערות עם תמיכה מקיפה ליצירה, הוספה, עריכה, מחיקה, חילוץ וייצוא הערות מתמונות ומסמכים שונים אחרים. הרשימה המלאה של פורמטי מסמכים נתמכים שתוכל לראות ב[דף] זה (https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        ספרייה זו מאפשרת לך לעבוד לא רק עם מסמך PPTM אלא גם עם סוגים רבים אחרים של מסמכים כגון Word, Excel, PowerPoint, מיילים של Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ועוד רבים אחרים.
        ה-GroupDocs.Annotation for Net API מאפשר לך ליצור ולהוסיף הערות חדשות, לערוך הערות, לחלץ הערות, הערות ולהסיר אותן ממסמכים. הספרייה תומכת ב-13 סוגי הערות שונים, כולל טקסט, קו פולי, שטח, קו תחתון, נקודה, סימן מים, חץ, אליפסה, החלפת טקסט, מרחק, שדה טקסט, עיבוד משאבים ב-PDF, HTML, מסמכי Microsoft Word, גיליונות אלקטרוניים, דיאגרמות, מצגות, ציורים, תמונות ופורמטים רבים אחרים של קבצים.
        הדוגמה (נא לראות להלן) מדגימה עבודה עם מסמך PPTM, בדוגמה זו תוכל לראות את השלבים העיקריים של איך לעבוד עם GroupDocs. הערה: הגדר רישיון, פתח מסמך שאתה רוצה לעבוד איתו, יצירת מסמך הערה, הוספת אובייקטי נתונים כדי להגדיר מאפייני הערה בהתאם לדרישות שלך ושמירת התוצאה במקום הדרוש. כמו כן, תוכל לעיין בפירוט רב יותר על התכונות הנתמכות ב-[github שלנו דף](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), [או במוצר שלנו תיעוד](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "שלבים להוספת הערות ל-PPTM ב-Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) מקל על מפתחי Net להוסיף סוגי הערות שונים לקבצי PPTM בתוך כל יישום מבוסס Net על ידי יישום כמה שלבים פשוטים.
        *   צור אובייקטי תגובה עם הערה ותאריך.
        *   צור אובייקט AreaAnnotation, הגדר אפשרויות אזור והוסף תשובות.
        *   צור אובייקט Annotator והוסף הערת אזור.
        *   שמור קובץ פלט.
    title_right: "דרישות מערכת"
    content_right: |
        GroupDocs.Annotation for Net APIs נתמכים בכל הפלטפורמות ומערכות ההפעלה העיקריות. לפני ביצוע הקוד שלהלן, אנא ודא שהדרישות המוקדמות הבאות מותקנים במערכת שלך.
        *   מערכות הפעלה: Microsoft Windows, Linux, MacOS
        *   סביבות פיתוח: Visual Studio, Xamarin, MonoDevelop
        *   מסגרות: .NET Framework, .NET Standard, .NET Core, Mono
        *   הורד את הגרסה העדכנית ביותר של GroupDocs.Annotation עבור .NET מ-[NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: תצוגה מקדימה של הערות ודגימת קוד
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
    title_left: "שלבים להסרת הערות מ-PPTM ב-Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) מקל על מפתחי Net להסיר פרטי הערות מקבצי PPTM בתוך כל יישום מבוסס Net על ידי יישום כמה שלבים פשוטים.
        *   צור אובייקטי תגובה עם הערה ותאריך.
        *   הצג אובייקט SaveOptions והגדר AnnotationTypes = AnnotationType.None.
        *   התקשר לשיטת השמירה עם נתיב המסמך או הזרם והאובייקט SaveOptions.

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
    title_left: "שלבים לעריכת הערות מ-PPTM ב-Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) מקל על מפתחי Net לעדכן מאפייני הערות שונים מקבצי PPTM בתוך כל יישום מבוסס Net על ידי יישום כמה שלבים פשוטים.
        *   יצירת אובייקט Annotator עם נתיב מסמך קלט או זרם עם LoadOptions מופע עם ImportAnnotations = true.
        *   צור יישום כלשהו של AnnotationBase והגדר את מזהה ההערה הקיימת (אם ההערה עם המזהה הזה לא נמצא, שום דבר לא ישתנה) או רשימת הנתיבים של ההערות (כל ההערות הקיימות יוסרו).
        *   התקשר לשיטת עדכון של אובייקט Annotator עם הערות שעברו.
        *   התקשר לשיטת השמירה עם נתיב המסמך או הזרם והאובייקט SaveOptions.

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
    title_left: "שלבים לחילוץ הערות מ-PPTM ב-Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) מקל על מפתחי Net להוסיף הערות למסמכים ולחלץ מידע הערות מקבצי PPTM בתוך כל יישום מבוסס Net על ידי יישום כמה שלבים פשוטים.
        *   צור אובייקטי תגובה עם הערה ותאריך.
        *   הצג אובייקט LoadOptions וקרא ל-SetImportAnnotations עם ארגומנט אמיתי.
        *   הגדר משתנה עם סוג רשימה.
        *   התקשר לשיטת get והחזר את התוצאה למשתנה למעלה.

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
    title: "הדגמות חיות להוספה, הסרה, עריכה, חילוץ הערות למסמכים ותמונות"
    content: |
        הוסף, הסר, ערוך וחלץ הערות לקובץ PPTM כעת על ידי ביקור באתר [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). להדגמה החיה יש את היתרונות הבאים

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pptm"
          title: "אודות פורמט הקובץ PPTM"
          content: |
            קבצים עם סיומת PPTM הם קובצי מצגת התומכים במאקרו שנוצרו עם Microsoft PowerPoint 2007 או גרסאות מתקדמות יותר. הם דומים לקבצי PPTX עם ההבדל שהצדדיים לא יכולים להפעיל פקודות מאקרו למרות שהם יכולים להכיל פקודות מאקרו. ניתן לערוך קבצי PPTM על ידי פתיחתם ב-Microsoft PowerPoint ועדכון התוכן. פורמט דומה נוסף הוא PPSM אך הוא קריאה בלבד כברירת מחדל ומתחיל את מצגת השקופיות כאשר היא נפתחת. PPTM, כמו PPTX, מכיל שקופיות עבור רכיבי מצגת שונים כמו טקסט, תמונות, סרטונים, גרפים וחומרים קשורים אחרים.

          link: "https://docs.fileformat.com/image/pptm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "עבודה עם פורמטים פופולריים אחרים של מסמכים"
    content: |
        עדכן את מאפייני ההערות מכמה מהפורמטים הפופולריים של הקבצים כפי שצוין להלן.
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