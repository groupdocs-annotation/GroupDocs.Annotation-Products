---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "जावा PPSM एनोटेशन एपीआई सी# में एनोटेट"
head_description: "जावा एपीआई PPSM, छवियों, चित्रों और दस्तावेज़ फ़ाइल स्वरूपों से लोकप्रिय एनोटेशन प्रकार बनाने और एनोटेट करने के लिए।"

############################# Header ############################
title: "जावा से PPSM एनोटेट करें"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "नि: शुल्क परीक्षण डाउनलोड करें"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "जावा एपीआई के लिए GroupDocs.Annotation के बारे में"
    content: |
        जावा एपीआई के लिए GroupDocs.Annotation एक लाइब्रेरी है जो आपको मैक, विंडोज या उबंटू पर पीडीएफ, वर्ड और अन्य दस्तावेजों में एनोटेशन जोड़ने की अनुमति देती है। [GroupDocs.Annotation for Java](/annotation/java) छवियों और विभिन्न अन्य दस्तावेज़ों से एनोटेशन बनाने, जोड़ने, संपादित करने, हटाने, निकालने और निर्यात करने के लिए व्यापक समर्थन के साथ एनोटेशन प्रबंधित करने के लिए एक मूल जावा एपीआई है। समर्थित दस्तावेज़ प्रारूपों की पूरी सूची आप इस [पेज](https://docs.groupdocs.com/annotation/java/supported-document-formats/) पर देख सकते हैं।
        यह लाइब्रेरी आपको न केवल PPSM दस्तावेज़ के साथ बल्कि कई अन्य प्रकार के दस्तावेज़ों जैसे वर्ड, एक्सेल, पॉवरपॉइंट, आउटलुक ईमेल, विसिओ, एडोब, ओपनडॉक्यूमेंट, ओपनऑफिस, फ़ोटोशॉप, ऑटोकैड और कई अन्य के साथ भी काम करने की अनुमति देती है।
        जावा एपीआई के लिए GroupDocs.Annotation आपको नए नोट्स बनाने और जोड़ने, एनोटेशन संपादित करने, टिप्पणियाँ निकालने, एनोटेशन और उन्हें दस्तावेज़ों से हटाने की अनुमति देता है। लाइब्रेरी 13 अलग-अलग एनोटेशन प्रकारों का समर्थन करती है, जिनमें टेक्स्ट, पॉलीलाइन, एरिया, अंडरलाइन, पॉइंट, वॉटरमार्क, एरो, एलिप्स, टेक्स्ट रिप्लेसमेंट, डिस्टेंस, टेक्स्ट फील्ड, पीडीएफ में रिसोर्स रिडक्शन, HTML, माइक्रोसॉफ्ट वर्ड दस्तावेज़, स्प्रेडशीट, आरेख, प्रस्तुतियाँ शामिल हैं। चित्र, छवियाँ और कई अन्य फ़ाइल स्वरूप।
        उदाहरण (कृपया नीचे देखें) PPSM दस्तावेज़ के साथ काम करना दर्शाता है, इस उदाहरण में आप GroupDocs के साथ काम करने के मुख्य चरण देख सकते हैं। एनोटेशन: एक लाइसेंस सेटअप करें, एक दस्तावेज़ खोलें जिसके साथ आप काम करना चाहते हैं, एक दस्तावेज़ बनाना एनोटेशन, अपनी आवश्यकताओं के अनुसार एनोटेशन गुणों को सेट करने के लिए डेटा ऑब्जेक्ट जोड़ना और परिणाम को आवश्यक स्थान पर सहेजना। इसके अलावा आप हमारे github [पेज](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), या हमारे उत्पाद [दस्तावेज़ीकरण](https:) पर समर्थित सुविधाओं पर अधिक विस्तृत नज़र डाल सकते हैं। //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "जावा में PPSM में एनोटेशन जोड़ने के चरण"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) कुछ आसान चरणों को लागू करके जावा डेवलपर्स के लिए किसी भी जावा-आधारित एप्लिकेशन के भीतर PPSM फ़ाइलों में विभिन्न एनोटेशन प्रकार जोड़ना आसान हो जाता है।
        *   टिप्पणी और दिनांक के साथ उत्तर ऑब्जेक्ट बनाएं।
        *   एरियाएनोटेशन ऑब्जेक्ट बनाएं, एरिया विकल्प सेट करें और उत्तर जोड़ें।
        *   एनोटेटर ऑब्जेक्ट बनाएं और क्षेत्र एनोटेशन जोड़ें।
        *   आउटपुट फ़ाइल सहेजें.
    title_right: "सिस्टम आवश्यकताएं"
    content_right: |
        जावा एपीआई के लिए GroupDocs.Annotation सभी प्रमुख प्लेटफार्मों और ऑपरेटिंग सिस्टम पर समर्थित है। नीचे दिए गए कोड को निष्पादित करने से पहले, कृपया सुनिश्चित करें कि आपके सिस्टम पर निम्नलिखित आवश्यकताएँ स्थापित हैं।
        *   ऑपरेटिंग सिस्टम: माइक्रोसॉफ्ट विंडोज, लिनक्स, मैकओएस
        *   विकास पर्यावरण: नेटबीन्स, इंटेलीज आईडीईए, एक्लिप्स आदि
        *   जावा रनटाइम पर्यावरण: जावा 7 (1.7) और ऊपर
        *   जावा के लिए GroupDocs.Annotation का नवीनतम संस्करण [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/general/repo/com/groupdocs/groupdocs-annotation) से प्राप्त करें।

############################# Preview ############################
preview_Add:
    enable: true
    title: एनोटेशन पूर्वावलोकन और कोड नमूना
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
    title_left: "जावा में PPSM से एनोटेशन हटाने के चरण"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) कुछ आसान चरणों को लागू करके जावा डेवलपर्स के लिए किसी भी जावा-आधारित एप्लिकेशन के भीतर PPSM फ़ाइलों से एनोटेशन विवरण निकालना आसान हो जाता है।
        *   टिप्पणी और दिनांक के साथ उत्तर ऑब्जेक्ट बनाएं।
        *   SaveOptions ऑब्जेक्ट को इंस्टेंट करें और AnnotationTypes = AnnotationType.None सेट करें।
        *   परिणामी दस्तावेज़ पथ या स्ट्रीम और SaveOptions ऑब्जेक्ट के साथ सेव विधि को कॉल करें।

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
    title_left: "जावा में PPSM से एनोटेशन संपादित करने के चरण"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) कुछ आसान चरणों को लागू करके जावा डेवलपर्स के लिए किसी भी जावा-आधारित एप्लिकेशन के भीतर PPSM फ़ाइलों से विभिन्न एनोटेशन गुणों को अपडेट करना आसान हो जाता है।
        *   इनपुट दस्तावेज़ पथ या स्ट्रीम के साथ तत्काल एनोटेटर ऑब्जेक्ट को आयातएनोटेशन = सत्य के साथ तत्काल लोडऑप्शंस के साथ स्ट्रीम करें।
        *   कुछ एनोटेशनबेस कार्यान्वयन बनाएं और मौजूदा एनोटेशन की आईडी सेट करें (यदि उस आईडी के साथ एनोटेशन नहीं मिला, तो कुछ भी नहीं बदला जाएगा) या एनोटेशन की पथ सूची (सभी मौजूदा एनोटेशन हटा दिए जाएंगे)।
        *   पारित एनोटेशन के साथ एनोटेटर ऑब्जेक्ट की कॉल अपडेट विधि।
        *   परिणामी दस्तावेज़ पथ या स्ट्रीम और SaveOptions ऑब्जेक्ट के साथ सेव विधि को कॉल करें।

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
    title_left: "जावा में PPSM से एनोटेशन निकालने के चरण"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) जावा डेवलपर्स के लिए कुछ आसान चरणों को लागू करके किसी भी जावा-आधारित एप्लिकेशन के भीतर दस्तावेज़ों को एनोटेट करना और PPSM फ़ाइलों से एनोटेशन जानकारी निकालना आसान बनाता है।
        *   टिप्पणी और दिनांक के साथ उत्तर ऑब्जेक्ट बनाएं।
        *   LoadOptions ऑब्जेक्ट को इंस्टेंट करें और सही तर्क के साथ SetImportAnnotations को कॉल करें।
        *   प्रकार सूची के साथ वेरिएबल को परिभाषित करें।
        *   get विधि को कॉल करें और परिणाम को उपरोक्त वेरिएबल पर लौटाएँ।

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
    title: "दस्तावेज़ों और छवियों में एनोटेशन जोड़ने, हटाने, संपादित करने, निकालने के लिए लाइव डेमो"
    content: |
        अभी [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) वेबसाइट पर जाकर PPSM फ़ाइल में एनोटेशन जोड़ें, हटाएं, संपादित करें और निकालें। लाइव डेमो के निम्नलिखित लाभ हैं

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ppsm"
          title: "PPSM फ़ाइल स्वरूप के बारे में"
          content: |
            PPSM एक्सटेंशन वाली फ़ाइलें Microsoft PowerPoint 2007 या उच्चतर के साथ बनाई गई मैक्रो-सक्षम स्लाइड शो फ़ाइल स्वरूप का प्रतिनिधित्व करती हैं। एक अन्य समान फ़ाइल स्वरूप PPTM है जो स्लाइड शो के रूप में चलने के बजाय संपादन योग्य प्रारूप में Microsoft PowerPoint के साथ खुलने में भिन्न है। जब स्लाइड शो के रूप में चलाया जाता है, तो पीपीएसएम फ़ाइल प्रस्तुति स्लाइड को स्लाइड शो में बरकरार सामग्री के साथ दिखाती है और डिफ़ॉल्ट रूप से केवल-पढ़ने के लिए मोड में होती है। PPSM फ़ाइलों को अभी भी Microsoft PowerPoint में PowerPoint में खोलकर संपादित किया जा सकता है।

          link: "https://docs.fileformat.com/image/ppsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "अन्य लोकप्रिय दस्तावेज़ प्रारूपों के साथ कार्य करना"
    content: |
        जैसा कि नीचे बताया गया है, कुछ लोकप्रिय फ़ाइल स्वरूपों से एनोटेशन गुणों को अपडेट करें।
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