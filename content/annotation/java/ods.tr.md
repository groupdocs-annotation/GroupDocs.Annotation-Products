---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java ODS Ek Açıklama API'si C#'ta Ek Açıklama"
head_description: "ODS, resimler, çizimler ve belge dosyası biçimlerinden popüler açıklama türleri oluşturmak ve Açıklama eklemek için Java API."

############################# Header ############################
title: "Java'dan ODS notunu ekleyin"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ücretsiz deneme sürümünü indirin"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Annotation for Java API hakkında"
    content: |
        GroupDocs.Annotation for Java API, PDF, Word ve Mac, Windows veya Ubuntu'daki diğer belgelere ek açıklamalar eklemenizi sağlayan bir kitaplıktır. [GroupDocs.Annotation for Java](/annotation/java), resimlerden ve diğer çeşitli belgelerden açıklamaları oluşturmaya, eklemeye, düzenlemeye, silmeye, ayıklamaya ve dışa aktarmaya yönelik kapsamlı destekle açıklamaları yönetmeye yönelik yerel bir Java API'sidir. Bu [sayfada](https://docs.groupdocs.com/annotation/java/supported-document-formats/) görebileceğiniz desteklenen belge biçimlerinin tam listesi.
        Bu kitaplık, yalnızca ODS belgesiyle değil, Word, Excel, PowerPoint, Outlook e-postaları, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ve diğerleri gibi diğer birçok belge türüyle çalışmanıza olanak tanır.
        GroupDocs.Annotation for Java API, yeni notlar oluşturmanıza ve eklemenize, ek açıklamaları düzenlemenize, yorumları, açıklamaları ayıklamanıza ve bunları belgelerden kaldırmanıza olanak tanır. Kitaplık, Metin, Çoklu Çizgi, Alan, Altı Çizili, Nokta, Filigran, Ok, Elips, Metin Değiştirme, Mesafe, Metin Alanı, PDF'de Kaynak Redaksiyonu, HTML, Microsoft Word belgeleri, elektronik tablolar, diyagramlar, sunumlar dahil olmak üzere 13 farklı açıklama türünü destekler. çizimler, resimler ve diğer birçok dosya formatı.
        Örnek (lütfen aşağıya bakın) ODS belgesiyle çalışmayı gösterir, bu örnekte GroupDocs ile çalışmanın ana adımlarını görebilirsiniz. Ek Açıklama: Bir lisans ayarlayın, çalışmak istediğiniz bir belgeyi açın, bir ek açıklama, açıklama özelliklerini ihtiyaçlarınıza göre ayarlamak için veri nesneleri ekleme ve sonucu gereken yere kaydetme. Ayrıca github [sayfa](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) veya ürün [documentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java'da ODS Dosyasına Ek Açıklama Ekleme Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java geliştiricilerinin, birkaç kolay adımı uygulayarak herhangi bir Java tabanlı uygulama içindeki ODS dosyalarına çeşitli ek açıklama türleri eklemesini kolaylaştırır.
        *   Yorum ve tarih içeren Yanıt nesneleri oluşturun.
        *   AreaAnnotation nesnesi oluşturun, alan seçeneklerini ayarlayın ve yanıtlar ekleyin.
        *   Annotator nesnesi oluşturun ve alan açıklaması ekleyin.
        *   Çıktı dosyasını kaydedin.
    title_right: "sistem gereksinimleri"
    content_right: |
        GroupDocs.Annotation for Java API'leri tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen sisteminizde aşağıdaki önkoşulların yüklü olduğundan emin olun.
        *   İşletim Sistemleri: Microsoft Windows, Linux, MacOS
        *   Geliştirme Ortamı: NetBeans, Intellij IDEA, Eclipse vb.
        *   Java Çalışma Zamanı Ortamı: Java 7 (1.7) ve üzeri
        *   GroupDocs.Annotation for Java'nın en son sürümünü [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) adresinden edinin.

############################# Preview ############################
preview_Add:
    enable: true
    title: Ek açıklama önizlemesi ve kod örneği
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
    title_left: "Java'da ODS Ek Açıklamalarını Kaldırma Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java geliştiricilerinin, birkaç kolay adımı uygulayarak herhangi bir Java tabanlı uygulamadaki ODS dosyalarından ek açıklama ayrıntılarını kaldırmasını kolaylaştırır.
        *   Yorum ve tarih içeren Yanıt nesneleri oluşturun.
        *   SaveOptions nesnesini oluşturun ve AnnotationTypes = AnnotationType.None olarak ayarlayın.
        *   Ortaya çıkan belge yolu veya akışı ve SaveOptions nesnesi ile kaydetme yöntemini çağırın.

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
    title_left: "Java'da ODS Ek Açıklamalarını Düzenleme Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java geliştiricilerinin, birkaç kolay adımı uygulayarak herhangi bir Java tabanlı uygulama içindeki ODS dosyalarından çeşitli ek açıklama özelliklerini güncellemesini kolaylaştırır.
        *   ImportAnnotations = true ile örneklenmiş LoadOptions ile giriş belgesi yolu veya akış ile Annotator nesnesini örnekleyin.
        *   Bazı AnnotationBase uygulamaları oluşturun ve varolan ek açıklamanın kimliğini ayarlayın (bu kimliğe sahip ek açıklama bulunmazsa, hiçbir şey değiştirilmeyecektir) veya ek açıklamaların yol listesi (mevcut tüm ek açıklamalar kaldırılacaktır).
        *   Geçirilen ek açıklamalarla Annotator nesnesinin güncelleme yöntemini çağırın.
        *   Ortaya çıkan belge yolu veya akışı ve SaveOptions nesnesi ile kaydetme yöntemini çağırın.

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
    title_left: "Java'da ODS Dosyasından Ek Açıklamaları Çıkarma Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java geliştiricilerinin belgelere açıklama eklemesini ve birkaç kolay adımı uygulayarak Java tabanlı herhangi bir uygulamadaki ODS dosyalarından açıklama bilgilerini çıkarmasını kolaylaştırır.
        *   Yorum ve tarih içeren Yanıt nesneleri oluşturun.
        *   LoadOptions nesnesini oluşturun ve SetImportAnnotations'ı gerçek bağımsız değişkenle çağırın.
        *   List tipinde değişken tanımlayın.
        *   Get yöntemini çağırın ve sonucu yukarıdaki değişkene döndürün.

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
    title: "Belgelere ve Görüntülere Ek Açıklamalar Eklemek, Kaldırmak, Düzenlemek, Çıkarmak için Canlı Demolar"
    content: |
        Hemen şimdi [GroupDocs.Annotation Canlı Demolar](https://products.groupdocs.app/annotation/family) web sitesini ziyaret ederek ODS dosyasına ek açıklama ekleyin, kaldırın, düzenleyin ve çıkarın. Canlı demo aşağıdaki avantajlara sahiptir

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ods"
          title: "ODS Dosya Biçimi Hakkında"
          content: |
            ODS uzantılı dosyalar, kullanıcı tarafından düzenlenebilen OpenDocument Elektronik Tablo Belge biçimini ifade eder. Veriler, ODF dosyasında satırlar ve sütunlar halinde saklanır. XML tabanlı bir formattır ve Açık Belge Formatları (ODF) ailesindeki çeşitli alt tiplerden biridir. Biçim, OASIS tarafından yayınlanan ve sürdürülen ODF 1.2 belirtimlerinin bir parçası olarak belirtilir. Windows ve diğer işletim sistemlerindeki bir dizi uygulama, Microsoft Excel, NeoOffice ve LibreOffice dahil olmak üzere ODS dosyalarını düzenleme ve işleme için açabilir. ODS dosyaları, farklı uygulamalar tarafından XLS, XLSX ve diğerleri gibi diğer elektronik tablo biçimlerine de dönüştürülebilir.

          link: "https://docs.fileformat.com/image/ods/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Diğer Popüler Belge Biçimleriyle Çalışma"
    content: |
        Bazı popüler dosya biçimlerinden ek açıklama özelliklerini aşağıda belirtildiği gibi güncelleyin.
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