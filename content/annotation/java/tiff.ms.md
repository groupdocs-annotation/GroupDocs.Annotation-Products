---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java TIFF Anotasi API Anotasi dalam C#"
head_description: "Java API untuk mencipta dan Menganotasi jenis anotasi popular daripada TIFF, imej, lukisan dan format fail dokumen."

############################# Header ############################
title: "Anotasi TIFF daripada Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Muat turun Percubaan Percuma"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Mengenai GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API ialah perpustakaan yang membolehkan anda menambah anotasi pada PDF, Word dan dokumen lain pada Mac, Windows atau Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) ialah API Java asli untuk mengurus anotasi dengan sokongan menyeluruh untuk mencipta, menambah, mengedit, memadam, mengekstrak dan mengeksport anotasi daripada imej dan pelbagai dokumen lain. Senarai penuh format dokumen yang disokong yang boleh anda lihat pada [halaman] ini (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Pustaka ini membolehkan anda bekerja bukan sahaja dengan dokumen TIFF tetapi juga dengan banyak jenis dokumen lain seperti Word, Excel, PowerPoint, e-mel Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad dan banyak lagi.
        API GroupDocs.Annotation untuk Java membolehkan anda membuat dan menambah nota baharu, mengedit anotasi, mengekstrak ulasan, anotasi dan mengalih keluarnya daripada dokumen. Pustaka menyokong 13 jenis anotasi yang berbeza, termasuk Teks, Poligaris, Kawasan, Garis bawah, Titik, Tera Air, Anak panah, Ellipse, Penggantian Teks, Jarak, Medan Teks, Redaksi Sumber dalam PDF, HTML, dokumen Microsoft Word, hamparan, rajah, pembentangan, lukisan, imej dan banyak lagi format fail.
        Contoh (sila lihat di bawah) menunjukkan bekerja dengan dokumen TIFF, dalam contoh ini anda boleh melihat langkah utama cara bekerja dengan GroupDocs. Anotasi: Sediakan lesen, buka dokumen yang anda ingin kerjakan, mencipta anotasi, menambah objek data untuk menetapkan sifat anotasi mengikut keperluan anda dan menyimpan hasilnya ke tempat yang diperlukan. Anda juga boleh melihat lebih terperinci tentang ciri yang disokong pada [halaman] github kami (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), atau dalam produk kami [dokumentasi](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Langkah untuk Menambah Anotasi pada TIFF dalam Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pembangun Java menambah pelbagai jenis anotasi pada fail TIFF dalam mana-mana aplikasi berasaskan Java dengan melaksanakan beberapa langkah mudah.
        *   Cipta objek Balas dengan ulasan dan tarikh.
        *   Buat objek AreaAnnotation, tetapkan pilihan kawasan dan tambah balasan.
        *   Cipta objek Annotator dan tambah anotasi kawasan.
        *   Simpan fail output.
    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Anotasi untuk API Java disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.
        *   Sistem Pengendalian: Microsoft Windows, Linux, MacOS
        *   Persekitaran Pembangunan: NetBeans, Intellij IDEA, Eclipse dll
        *   Java Runtime Environment: Java 7 (1.7) dan ke atas
        *   Dapatkan versi terkini GroupDocs.Annotation untuk Java daripada [Repositori Artifak GroupDocs](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Pratonton anotasi dan sampel kod
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
    title_left: "Langkah-langkah untuk Mengalih keluar Anotasi daripada TIFF dalam Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pembangun Java mengalih keluar butiran anotasi daripada fail TIFF dalam mana-mana aplikasi berasaskan Java dengan melaksanakan beberapa langkah mudah.
        *   Cipta objek Balas dengan ulasan dan tarikh.
        *   Semerta objek SaveOptions dan tetapkan AnnotationTypes = AnnotationType.None.
        *   Kaedah simpan panggilan dengan laluan atau strim dokumen terhasil dan objek SaveOptions.

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
    title_left: "Langkah-langkah untuk Mengedit Anotasi daripada TIFF dalam Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pembangun Java mengemas kini pelbagai sifat anotasi daripada fail TIFF dalam mana-mana aplikasi berasaskan Java dengan melaksanakan beberapa langkah mudah.
        *   Semerta objek Annotator dengan laluan dokumen input atau strim dengan LoadOptions dengan ImportAnnotations = benar.
        *   Cipta beberapa pelaksanaan AnnotationBase dan tetapkan Id bagi anotasi wujud (jika anotasi dengan Id itu tidak ditemui, tiada apa yang akan diubah) atau senarai laluan anotasi (semua anotasi wujud akan dialih keluar).
        *   Kaedah kemas kini panggilan objek Annotator dengan anotasi yang diluluskan.
        *   Kaedah simpan panggilan dengan laluan atau strim dokumen terhasil dan objek SaveOptions.

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
    title_left: "Langkah-langkah untuk Mengeluarkan Anotasi daripada TIFF dalam Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pembangun Java untuk menganotasi dokumen dan mengekstrak maklumat anotasi daripada fail TIFF dalam mana-mana aplikasi berasaskan Java dengan melaksanakan beberapa langkah mudah.
        *   Cipta objek Balas dengan ulasan dan tarikh.
        *   Segerakan objek LoadOptions dan panggil SetImportAnnotations dengan hujah yang benar.
        *   Tentukan pembolehubah dengan jenis Senarai.
        *   Panggil kaedah dapatkan dan kembalikan hasil kepada pembolehubah di atas.

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
    title: "Demo Langsung untuk Tambah, Alih Keluar, Edit, Ekstrak Anotasi pada Dokumen dan Imej"
    content: |
        Tambahkan, alih keluar, edit dan ekstrak anotasi pada fail TIFF sekarang dengan melawati tapak web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Demo langsung mempunyai faedah berikut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-tiff"
          title: "Mengenai Format Fail TIFF."
          content: |
            TIFF atau TIF, Format Fail Imej Teg, mewakili imej raster yang bertujuan untuk kegunaan pada pelbagai peranti yang mematuhi standard format fail ini. Ia mampu menerangkan data imej dwiparas, skala kelabu, warna palet dan warna penuh dalam beberapa ruang warna. Ia menyokong skim mampatan lossy serta lossless untuk memilih antara ruang dan masa untuk aplikasi menggunakan format. Format ini boleh diperluaskan dan telah menjalani beberapa semakan yang membenarkan kemasukan maklumat peribadi atau tujuan khas tanpa had. Format tidak bergantung pada mesin dan bebas daripada sempadan seperti pemproses, sistem pengendalian atau sistem fail.

          link: "https://docs.fileformat.com/image/tiff/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bekerja dengan Format Dokumen Popular Lain"
    content: |
        Kemas kini sifat anotasi daripada beberapa format fail popular seperti yang dinyatakan di bawah.
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