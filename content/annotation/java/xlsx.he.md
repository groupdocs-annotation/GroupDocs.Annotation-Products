---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java XLSX הערות API של הערות ב-C#"
head_description: "Java API ליצירה והערה של סוגי הערות פופולריים מ-XLSX, תמונות, שרטוטים ופורמטים של קבצי מסמכים."

############################# Header ############################
title: "הערה על XLSX מ-Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "הורד גרסת ניסיון בחינם"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "אודות GroupDocs.Annotation עבור Java API"
    content: |
        GroupDocs.Annotation for Java API היא ספרייה המאפשרת לך להוסיף הערות ל-PDF, Word ומסמכים אחרים ב-Mac, Windows או Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) הוא API מקורי של Java לניהול הערות עם תמיכה מקיפה ליצירה, הוספה, עריכה, מחיקה, חילוץ וייצוא הערות מתמונות ומסמכים שונים אחרים. הרשימה המלאה של פורמטי מסמכים נתמכים שתוכל לראות ב[דף] זה (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        ספרייה זו מאפשרת לך לעבוד לא רק עם מסמך XLSX אלא גם עם סוגים רבים אחרים של מסמכים כגון Word, Excel, PowerPoint, מיילים של Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ועוד רבים אחרים.
        ה-GroupDocs.Annotation for Java API מאפשר לך ליצור ולהוסיף הערות חדשות, לערוך הערות, לחלץ הערות, הערות ולהסיר אותן ממסמכים. הספרייה תומכת ב-13 סוגי הערות שונים, כולל טקסט, קו פולי, שטח, קו תחתון, נקודה, סימן מים, חץ, אליפסה, החלפת טקסט, מרחק, שדה טקסט, עיבוד משאבים ב-PDF, HTML, מסמכי Microsoft Word, גיליונות אלקטרוניים, דיאגרמות, מצגות, ציורים, תמונות ופורמטים רבים אחרים של קבצים.
        הדוגמה (נא לראות להלן) מדגימה עבודה עם מסמך XLSX, בדוגמה זו תוכל לראות את השלבים העיקריים של איך לעבוד עם GroupDocs. הערה: הגדר רישיון, פתח מסמך שאתה רוצה לעבוד איתו, יצירת מסמך הערה, הוספת אובייקטי נתונים כדי להגדיר מאפייני הערה בהתאם לדרישות שלך ושמירת התוצאה במקום הדרוש. כמו כן, תוכל לעיין בפירוט רב יותר על התכונות הנתמכות ב-github שלנו [דף](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), או במוצר שלנו [תיעוד](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "שלבים להוספת הערות ל-XLSX ב-Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) מקל על מפתחי Java להוסיף סוגי הערות שונים לקבצי XLSX בתוך כל יישום מבוסס Java על ידי יישום כמה שלבים פשוטים.
        *   צור אובייקטי תגובה עם הערה ותאריך.
        *   צור אובייקט AreaAnnotation, הגדר אפשרויות אזור והוסף תשובות.
        *   צור אובייקט Annotator והוסף הערת אזור.
        *   שמור קובץ פלט.
    title_right: "דרישות מערכת"
    content_right: |
        GroupDocs.Annotation עבור ממשקי API של Java נתמכים בכל הפלטפורמות ומערכות ההפעלה העיקריות. לפני ביצוע הקוד שלהלן, אנא ודא שהדרישות המוקדמות הבאות מותקנים במערכת שלך.
        *   מערכות הפעלה: Microsoft Windows, Linux, MacOS
        *   סביבת פיתוח: NetBeans, Intellij IDEA, Eclipse וכו'
        *   סביבת זמן ריצה של Java: Java 7 (1.7) ומעלה
        *   קבל את הגרסה העדכנית ביותר של GroupDocs.Annotation עבור Java מ-[GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: תצוגה מקדימה של הערות ודגימת קוד
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
    title_left: "שלבים להסרת הערות מ-XLSX ב-Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) מקל על מפתחי Java להסיר פרטי הערות מקבצי XLSX בתוך כל יישום מבוסס Java על ידי יישום כמה שלבים פשוטים.
        *   צור אובייקטי תגובה עם הערה ותאריך.
        *   הצג אובייקט SaveOptions והגדר AnnotationTypes = AnnotationType.None.
        *   התקשר לשיטת השמירה עם נתיב המסמך או הזרם והאובייקט SaveOptions.

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
    title_left: "שלבים לעריכת הערות מ-XLSX ב-Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) מקל על מפתחי Java לעדכן מאפייני הערות שונים מקבצי XLSX בתוך כל יישום מבוסס Java על ידי יישום כמה שלבים פשוטים.
        *   יצירת אובייקט Annotator עם נתיב מסמך קלט או זרם עם LoadOptions מופע עם ImportAnnotations = true.
        *   צור יישום כלשהו של AnnotationBase והגדר את מזהה ההערה הקיימת (אם ההערה עם המזהה הזה לא נמצא, שום דבר לא ישתנה) או רשימת הנתיבים של ההערות (כל ההערות הקיימות יוסרו).
        *   התקשר לשיטת עדכון של אובייקט Annotator עם הערות שעברו.
        *   התקשר לשיטת השמירה עם נתיב המסמך או הזרם והאובייקט SaveOptions.

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
    title_left: "שלבים לחילוץ הערות מ-XLSX ב-Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) מקל על מפתחי Java להוסיף הערות למסמכים ולחלץ מידע הערות מקבצי XLSX בתוך כל יישום מבוסס Java על ידי יישום כמה שלבים פשוטים.
        *   צור אובייקטי תגובה עם הערה ותאריך.
        *   הצג אובייקט LoadOptions וקרא ל-SetImportAnnotations עם ארגומנט אמיתי.
        *   הגדר משתנה עם סוג רשימה.
        *   התקשר לשיטת get והחזר את התוצאה למשתנה למעלה.

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
    title: "הדגמות חיות להוספה, הסרה, עריכה, חילוץ הערות למסמכים ותמונות"
    content: |
        הוסף, הסר, ערוך וחלץ הערות לקובץ XLSX כעת על ידי ביקור באתר [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
להדגמה החיה יש את היתרונות הבאים

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsx"
          title: "אודות פורמט הקובץ XLSX"
          content: |
            XLSX הוא פורמט ידוע עבור מסמכי Microsoft Excel שהוצג על ידי מיקרוסופט עם שחרורו של Microsoft Office 2007. מבוסס על מבנה המאורגן על פי אמנות האריזה הפתוחה כפי שמתואר בחלק 2 של תקן OOXML ECMA-376, הפורמט החדש הוא חבילת zip המכילה מספר קבצי XML. ניתן לבחון את המבנה והקבצים הבסיסיים על ידי פתיחת קובץ ה-.xlsx.

          link: "https://docs.fileformat.com/image/xlsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "עבודה עם פורמטים פופולריים אחרים של מסמכים"
    content: |
        עדכן את מאפייני ההערות מכמה מהפורמטים הפופולריים של הקבצים כפי שצוין להלן.
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