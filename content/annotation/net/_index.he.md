---
############################# Static ############################
layout: "product"
date: 2022-02-23T12:00:00+02:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: "Net Document Annotation API | הצג והערת תמונות PDF Word Excel PPTX"
head_description: "Net Document Annotation API. הצג, תייג, הערה והערה PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAD ופורמטים של קבצי תמונה."

############################# Header ##########################
title: "הערת מסמך באמצעות Net API"
description: "בנה יישומי רשת עם יכולות הצגה והערה של PDF, HTML, MS Office ופורמטים אחרים של מסמכים מבלי להתקין תוכנה חיצונית כלשהי."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "הורד גרסת ניסיון בחינם"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu #########################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Net"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            # button loop
            - link: "#features"
              text: "מאפיינים"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "הדגמות חיות"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "תמחור"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Net API הוא מוצר המאפשר לך לעבוד עם הערות במסמכים בפלטפורמות ומערכות הפעלה שונות, כגון אנדרואיד, MacOS, Linux, Windows. GroupDocs.Annotation מספקת ספרייה עם API פשוט שנותן יתרונות רבים: למשל, אם אתה צריך לשמור על סודיות הנתונים או לבחור כמה כוח אתה צריך לעבוד עם הספרייה, או לשנות חלקית את העבודה עם הערות, הספרייה מאוד קל משקל וגמיש.

      GroupDocs.Annotation for Net API מאפשר לך לעבוד עם סוגים שונים של הערות, הכוללות: טקסט, פוליקו, שטח, קו תחתון, נקודה, סימן מים, חץ, אליפסה, החלפת טקסט, מרחק, שדה טקסט, עיבוד משאבים וכו'. ותומך ברוב פורמטים פופולריים של מסמכים כגון: PDF, HTML, Microsoft Office Word, גיליונות אלקטרוניים של Excel, מצגות PowerPoint, Visio, מיילים של Outlook, תמונות, מטא-קבצים, ציור CAD ועוד פורמטים שונים. ה-API מספק את היכולת לקבל תמונות ממוזערות של דפי מסמכים ותומך בייבוא ​​וייצוא הערות לקבצי PDF וממנה.

      באמצעות ספרייה, ניתן להוסיף, לערוך, לחלץ ולמחוק הערות ממסמכים, לסובב מסמכים, לשנות פתרון תמונות ממוזערות וזו אינה רשימה מלאה של כל האפשרויות. הוא גם מציע קבוצה מקיפה של אובייקטי נתונים כדי להתאים אישית את מאפייני ההערות בהתאם לדרישות שלך בכל פורמטי המסמכים הנתמכים.

      העבודה עם GroupDocs.Annotation for Net API היא פשוטה מאוד ומורכבת מכמה שלבים בסיסיים בלבד. בהתחלה אתה צריך להגדיר רישיון, ואז לבחור את הקובץ שאתה רוצה לעבוד איתו, ואז לעשות מניפולציה איכשהו עם הערות למסמך (מחק/ערוך/חילוץ/מחיקה) ולשמור את התוצאה. למידע נוסף, עיין בתיעוד המוצר או בערכת הדוגמאות שלנו.
      
      GroupDocs.Annotation מתעדכן באופן שוטף ומספק תמיכה ללקוחותיה, אתה תמיד מוזמן לשאול אותנו שאלות או לשלוח רעיונות או לספר לנו על הצרכים שלך למשהו חדש ואנו נשמח ליישם זאת בגרסאות החדשות שלנו.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          להלן סקירה כללית של GroupDocs.Annotation for Net:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title:  סקירה כללית
          content: |
            * הוסף הערות
            * ייצא הערות 
            * ייבוא ​​הערות
            * הערות מבוססות תשובות
            * תאימות הערות
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation for Net תומך בכל [פורמטי קובץ המסמכים] הפופולריים (https://docs.groupdocs.com/annotation/Net/supported-document-formats/) כולל: Microsoft Office, PDF, תמונות ועוד רבים אחרים.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: [DOC](/annotation/net/doc/), [DOCX](/annotation/net/docx/), [DOCM](/annotation/net/docm/), [DOT](/annotation/net/dot/), [DOTX](/annotation/net/dotx/), [RTF](/annotation/net/rtf/)
                * **Excel**: [XLS](/annotation/net/xls/), [XLSX](/annotation/net/xlsx/), [XLSB](/annotation/net/xlsb/), [XLSM](/annotation/net/xlsm/)
                * **PowerPoint**: [PPT](/annotation/net/ppt/), [PPTX](/annotation/net/pptx/), [PPS](/annotation/net/pps/), [PPSX](/annotation/net/ppsx/), [POTM](/annotation/net/potm/), [POTX](/annotation/net/potx/), [PPSM](/annotation/net/ppsm/), [PPTM](/annotation/net/pptm/), [WMF](/annotation/net/wmf/), [EMF](/annotation/net/emf/)
                * **Outlook**: [EML](/annotation/net/eml/), [EMLX](/annotation/net/emlx/), [MSG](/annotation/net/msg/)
                * **Visio**: [VSS](/annotation/net/vss/), [VST](/annotation/net/vst/), [VSD](/annotation/net/vsd/), [VSDX](/annotation/net/vsdx/), [VSX](/annotation/net/vsx/)

        right:
          enable: true
          table:
            # table loop
            - title: "Other Formats"
              content: |
                * **Portable**: [PDF](/annotation/net/pdf/) (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: [ODT](/annotation/net/odt/), [ODS](/annotation/net/ods/), [ODP](/annotation/net/odp/)
                * **Images**: [BMP](/annotation/net/bmp/), [JPG](/annotation/net/jpg/), [JPEG](/annotation/net/jpeg/), [TIFF](/annotation/net/tiff/), [TIF](/annotation/net/tif/), [PNG](/annotation/net/png/), [GIF](/annotation/net/gif/), [DCM](/annotation/net/dcm/), [DICOM](/annotation/net/dicom/)
                * **AutoCAD**: [DWG](/annotation/net/dwg/), [DXF](/annotation/net/dxf/), [CAD](/annotation/net/cad/)
                * **Other**: [HTM](/annotation/net/htm/), [HTML](/annotation/net/html/), [CSV](/annotation/net/csv/), [DJVU](/annotation/net/djvu/), [OTP](/annotation/net/otp/), [OTT](/annotation/net/ott/)

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Net תומך במנהלי מערכות הפעלה, מסגרות וחבילות הבאות:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title:  מערכות הפעלה
              content: |
                * Windows Desktop (x86 & x64)
                * Windows Server (x86 & x64)
                * Windows Azure
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title:  מסגרות נתמכות
              content: |
                * .NET Standard 2.0
                * .NET Framework 2.0 or higher
                * .NET Core 2.0 or higher
                * Mono Framework 1.2 or higher

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title:  מנהל אריזה
              content: |
                * NuGet
            
            # table loop
            - icon: "fas fa-tools"
              title:  סביבות פיתוח
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: GroupDocs.Annotation for Net Features

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: הוסף, ערוך והסר הערות ותשובות

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: ייצוא הערות למסמך

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/net/evaluation-limitations-and-licensing-of-groupdocs-annotation/"
        content: רישיון מדוד - חיוב מבוקר על ידי תשלום לפי שימוש ב-API
      
      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/net/extract-annotations-from-document/"
        content: קריאה עם פונקציה אחת לשליפה של כל ההערות של מסמך

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: הקצה ערך להערת נקודה או העבר ערך נקודה קיימת

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/net/add-link-annotation/"
        content: הוסף הערת קישור ל-PDF, Word ו-PowerPoint Slides

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: הגדר צבע רקע של הערה או הסר את כל ההערות מהמסמך

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: הערות קבצי PDF עם דיוק - קבל ייצוג תמונה של תצוגות מקדימות של מסמכי PDF ו-Cache

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/import-annotations/"
        content: קבל קואורדינטות טקסט של הערת טקסט בייצוג תמונה של מסמך

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: קשר הערות משתמש להערות אזור ותמיכה עבור הערות מקוונות

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/net/add-arrow-annotation/"
        content: השתמש בהערת חץ כדי להצביע על תוכן מסוים

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/net/add-distance-annotation/"
        content: השתמש בביאור מרחק כדי לצייר קו המייצג מרחק בין אובייקטים

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: הערה מבוססת נקודה שכאשר לוחצים עליה מקפיצה חלון כדי להוסיף הערות

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/net/add-polyline-annotation/"
        content: צור רצף מקושר של מקטעי קו שנוצרו כהערת פוליליין

      # feature loop
      - icon: "fas fa-lock"
        link: "https://docs.groupdocs.com/annotation/net/add-ellipse-annotation/"
        content: צור מקטעי קו ישר, מקטעי קשת או שילוב של שניהם

      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: סמן אזורי מסמכים המוצעים לעיבוד
      
      # feature loop
      - icon: "fas fa-fill-drip"
        link: "https://docs.groupdocs.com/annotation/net/add-image-annotation/"
        content: הוסף הערת תמונה ל-PDF, דיאגרמות, Word, Excel, מצגות ותמונות

      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: הוסף שדה טקסט וחותמת מבוססת טקסט או סימן מים במסמך

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: דחוף, קו תחתון או החלף טקסט מסוים במסמך

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/net/update-annotations/"
        content: שנה את גודל ההערה על ידי הקצאת פרמטרים חדשים של גובה ורוחב

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: קבל תמונות ממוזערות של דפי מסמכים. נהל מגוון של מסמכים מוערים עבור תמונות ודיאגרמות

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: ייצא הערות ועבוד עם קובצי TIFF מרובי עמודים
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-watermark-annotation/"
        content: התאם יישור אנכי ואופקי עבור הערת סימן מים
  
      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-text-field-annotation/"
        content: הוסף יישור אופקי של טקסט עבור שדה טקסט

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/document-text-info/"
        content: קבל מידע על שורות טקסט במסמך (טקסט, רוחב, גובה, כניסות)

    more_feature:
      # more_feature_loop
      - title: תמיכה במספר סוגים של הערות
        content: |
          GroupDocs.Annotation עבור .NET מאפשר לך לעבוד עם סוגים שונים של הערות. זה נותן חופש וקלות תקשורת תוך שיתוף פעולה עם הצוות שלך במשימות. אתה יכול להשתמש בהערות, כגון, הערת אזור (לסמן אזור כמלבן ולהוסיף לו הערות), הערת נקודה (להדביק הערות בכל נקודה במסמך), הערת טקסט (הוסף הערה לטקסט שנבחר), הערת מחיקה/קו תחתון ( מוחל על פסקה), ביאור פולילי (צייר צורות וקווים חופשיים), הערת חץ (מצביע חץ עם הערות מצורפות), ביאור אליפסה (הצגת טקסט בתוך האליפסה), הערת מרחק (צייר קו המייצג מרחק בין אובייקטים), קישור הערה (הוסף קישורי אינטרנט לפורמטים נתמכים של מסמכים), והערת סימן מים (ניתן להוסיף חותמת טקסט או סימן מים במסמך).

          ```cs
          // Initialize list of AnnotationInfo
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          // Initialize text annotation
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          // Add annotation to list
          annotations.Add(textAnnotation);
          // Get input file stream
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          // Export annotation and save output file
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: GroupDocs.Annotation מציע ממשקי API לצפייה במסמכים עבור סביבות פיתוח פופולריות אחרות

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---