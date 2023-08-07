---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java PPTX Annotation API Annotate in C#"
head_description: "Java API პოპულარული ანოტაციის ტიპების შესაქმნელად და ანოტაციისთვის PPTX-დან, სურათებიდან, ნახატებიდან და დოკუმენტის ფაილის ფორმატებიდან."

############################# Header ############################
title: "ანოტაცია PPTX Java-დან"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "ჩამოტვირთეთ უფასო საცდელი"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Annotation-ის შესახებ Java API-სთვის"
    content: |
        GroupDocs.Annotation for Java API არის ბიბლიოთეკა, რომელიც საშუალებას გაძლევთ დაამატოთ ანოტაციები PDF, Word და სხვა დოკუმენტებში Mac, Windows ან Ubuntu-ზე. [GroupDocs.Annotation for Java](/annotation/java) არის მშობლიური Java API ანოტაციების მართვისთვის ყოვლისმომცველი მხარდაჭერით სურათებიდან ან სხვა დოკუმენტებიდან ანოტაციების შექმნის, დამატების, რედაქტირების, წაშლის, ამოღებისა და ექსპორტისთვის. მხარდაჭერილი დოკუმენტების ფორმატების სრული სია, რომელიც შეგიძლიათ იხილოთ ამ [გვერდზე] (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        ეს ბიბლიოთეკა საშუალებას გაძლევთ იმუშაოთ არა მხოლოდ PPTX დოკუმენტთან, არამედ მრავალი სხვა ტიპის დოკუმენტთან, როგორიცაა Word, Excel, PowerPoint, Outlook ელფოსტა, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad და მრავალი სხვა.
        GroupDocs.Annotation for Java API გაძლევთ საშუალებას შექმნათ და დაამატოთ ახალი შენიშვნები, დაარედაქტიროთ ანოტაციები, ამოიღოთ კომენტარები, ანოტაციები და წაშალოთ ისინი დოკუმენტებიდან. ბიბლიოთეკა მხარს უჭერს 13 სხვადასხვა ტიპის ანოტაციას, მათ შორის ტექსტს, პოლიხაზს, ფართობს, ხაზს, წერტილს, ჭვირნიშანს, ისარს, ელიფსს, ტექსტის ჩანაცვლებას, მანძილს, ტექსტის ველს, რესურსების რედაქციას PDF, HTML, Microsoft Word დოკუმენტებში, ცხრილებში, დიაგრამებში, პრეზენტაციებში, ნახატები, სურათები და მრავალი სხვა ფაილის ფორმატი.
        მაგალითი (იხილეთ ქვემოთ) ასახავს PPTX დოკუმენტთან მუშაობას, ამ მაგალითში შეგიძლიათ იხილოთ GroupDocs-თან მუშაობის ძირითადი ნაბიჯები. ანოტაცია: დააყენეთ ლიცენზია, გახსენით დოკუმენტი, რომელთანაც გსურთ მუშაობა, შექმნათ ანოტაცია, მონაცემთა ობიექტების დამატება ანოტაციის თვისებების დასაყენებლად თქვენი მოთხოვნების შესაბამისად და შედეგის შესანახად საჭირო ადგილას. ასევე შეგიძლიათ უფრო დეტალურად გაეცნოთ მხარდაჭერილ ფუნქციებს ჩვენს github-ზე [გვერდზე](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), ან ჩვენს პროდუქტში [დოკუმენტაცია](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "ნაბიჯები ანოტაციების დასამატებლად PPTX Java-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ჯავის დეველოპერებს უადვილებს ანოტაციის სხვადასხვა ტიპების დამატებას PPTX ფაილებზე Java-ზე დაფუძნებულ ნებისმიერ აპლიკაციაში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   შექმენით პასუხის ობიექტები კომენტარებით და თარიღით.
        *   შექმენით AreaAnnotation ობიექტი, დააყენეთ არეალის პარამეტრები და დაამატეთ პასუხები.
        *   შექმენით Annotator ობიექტი და დაამატეთ არეალის ანოტაცია.
        *   შეინახეთ გამომავალი ფაილი.
    title_right: "სისტემის მოთხოვნები"
    content_right: |
        GroupDocs.Annotation Java API-ებისთვის მხარდაჭერილია ყველა ძირითად პლატფორმაზე და ოპერაციულ სისტემაზე. ქვემოთ მოცემული კოდის შესრულებამდე, დარწმუნდით, რომ თქვენს სისტემაში დაინსტალირებული გაქვთ შემდეგი წინაპირობები.
        *   ოპერაციული სისტემები: Microsoft Windows, Linux, MacOS
        *   განვითარების გარემო: NetBeans, Intellij IDEA, Eclipse და ა.შ
        *   Java Runtime Environment: Java 7 (1.7) და ზემოთ
        *   მიიღეთ GroupDocs.Annotation-ის უახლესი ვერსია Java-სთვის [GroupDocs Artifact Repository]-დან (https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: ანოტაციის გადახედვა და კოდის ნიმუში
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
    title_left: "ნაბიჯები ანოტაციების წასაშლელად PPTX Java-დან"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ჯავის დეველოპერებს უადვილებს ანოტაციის დეტალების წაშლას PPTX ფაილებიდან Java-ზე დაფუძნებულ ნებისმიერ აპლიკაციაში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   შექმენით პასუხის ობიექტები კომენტარებით და თარიღით.
        *   შექმენით SaveOptions ობიექტი და დააყენეთ AnnotationTypes = AnnotationType.None.
        *   ზარის შენახვის მეთოდის შედეგი დოკუმენტის გზა ან ნაკადი და SaveOptions ობიექტი.

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
    title_left: "ნაბიჯები ანოტაციების რედაქტირებისთვის PPTX Java-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) უადვილებს Java დეველოპერებს განაახლონ სხვადასხვა ანოტაციის თვისებები PPTX ფაილებიდან Java-ზე დაფუძნებული აპლიკაციის ფარგლებში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   Instantiate Annotator ობიექტის შეყვანის დოკუმენტის გზა ან ნაკადი instantiated LoadOptions ერთად ImportAnnotations = true.
        *   შექმენით AnnotationBase იმპლემენტაცია და დააყენეთ არსებული ანოტაციის ID (თუ ანოტაცია ამ Id-ით ვერ მოიძებნა, არაფერი შეიცვლება) ან ანოტაციების ბილიკის სია (ყველა არსებული ანოტაცია წაიშლება).
        *   Annotator ობიექტის ზარის განახლების მეთოდი გადაცემული ანოტაციებით.
        *   ზარის შენახვის მეთოდის შედეგი დოკუმენტის გზა ან ნაკადი და SaveOptions ობიექტი.

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
    title_left: "ნაბიჯები ანოტაციების ამოღების მიზნით PPTX-დან Java-ში"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ჯავის დეველოპერებს უადვილებს დოკუმენტების ანოტაციას და ანოტაციის ინფორმაციის ამოღებას PPTX ფაილებიდან Java-ზე დაფუძნებული ნებისმიერი აპლიკაციის ფარგლებში რამდენიმე მარტივი ნაბიჯის განხორციელებით.
        *   შექმენით პასუხის ობიექტები კომენტარებით და თარიღით.
        *   Instantate LoadOptions ობიექტი და გამოიძახეთ SetImportAnnotations ჭეშმარიტი არგუმენტით.
        *   განსაზღვრეთ ცვლადი სია ტიპის მიხედვით.
        *   გამოიძახეთ get მეთოდი და დააბრუნეთ შედეგი ზემოთ ცვლადში.

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
    title: "ცოცხალი დემოები დოკუმენტებსა და სურათებზე ანოტაციების დასამატებლად, ამოსაღებად, რედაქტირებისთვის"
    content: |
        დაამატეთ, წაშალეთ, დაარედაქტირეთ და ამოიღეთ ანოტაციები PPTX ფაილში ახლავე, ეწვიეთ [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) ვებსაიტს.
ცოცხალი დემოს აქვს შემდეგი უპირატესობები

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pptx"
          title: "PPTX ფაილის ფორმატის შესახებ"
          content: |
            ფაილები PPTX გაფართოებით არის საპრეზენტაციო ფაილები, რომლებიც შექმნილია პოპულარული Microsoft PowerPoint აპლიკაციით. პრეზენტაციის ფაილის ფორმატის PPT წინა ვერსიისგან განსხვავებით, რომელიც ორობითი იყო, PPTX ფორმატი ეფუძნება Microsoft PowerPoint-ის ღია XML პრეზენტაციის ფაილის ფორმატს. პრეზენტაციის ფაილი არის სლაიდების კოლექცია, სადაც თითოეული სლაიდი შეიძლება შეიცავდეს ტექსტს, სურათებს, ფორმატირებას, ანიმაციებს და სხვა მედიას. ეს სლაიდები აუდიტორიას წარუდგენს სლაიდების ჩვენების სახით, მორგებული პრეზენტაციის პარამეტრებით.

          link: "https://docs.fileformat.com/image/pptx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "მუშაობა სხვა პოპულარულ დოკუმენტის ფორმატებთან"
    content: |
        განაახლეთ ანოტაციის თვისებები ზოგიერთი პოპულარული ფაილის ფორმატიდან, როგორც ეს მოცემულია ქვემოთ.
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