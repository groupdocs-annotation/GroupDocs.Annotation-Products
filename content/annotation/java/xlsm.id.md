---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API Anotasi XLSM Java Anotasi dalam C#"
head_description: "Java API untuk membuat dan Menganotasi jenis anotasi populer dari XLSM, gambar, gambar, dan format file dokumen."

############################# Header ############################
title: "Anotasi XLSM dari Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Unduh Uji Coba Gratis"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Annotation untuk Java API"
    content: |
        GroupDocs.Annotation for Java API adalah pustaka yang memungkinkan Anda menambahkan anotasi ke PDF, Word, dan dokumen lain di Mac, Windows, atau Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) adalah Java API asli untuk mengelola anotasi dengan dukungan komprehensif untuk membuat, menambahkan, mengedit, menghapus, mengekstrak, dan mengekspor anotasi dari gambar dan berbagai dokumen lainnya. Daftar lengkap format dokumen yang didukung dapat Anda lihat di [halaman](https://docs.groupdocs.com/annotation/java/supported-document-formats/) ini.
        Pustaka ini memungkinkan Anda untuk bekerja tidak hanya dengan dokumen XLSM tetapi juga dengan banyak jenis dokumen lainnya seperti Word, Excel, PowerPoint, email Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad, dan banyak lainnya.
        GroupDocs.Annotation for Java API memungkinkan Anda membuat dan menambahkan catatan baru, mengedit anotasi, mengekstrak komentar, anotasi, dan menghapusnya dari dokumen. Perpustakaan mendukung 13 jenis anotasi yang berbeda, termasuk Teks, Polyline, Area, Garis Bawah, Titik, Tanda Air, Panah, Ellipse, Penggantian Teks, Jarak, Bidang Teks, Redaksi Sumber Daya dalam PDF, HTML, dokumen Microsoft Word, spreadsheet, diagram, presentasi, gambar, gambar dan banyak format file lainnya.
        Contoh (silakan lihat di bawah) mendemonstrasikan bekerja dengan dokumen XLSM, dalam contoh ini Anda dapat melihat langkah-langkah utama tentang cara bekerja dengan GroupDocs. Anotasi: Menyiapkan lisensi, membuka dokumen yang ingin Anda kerjakan, membuat anotasi, menambahkan objek data untuk mengatur properti anotasi sesuai dengan kebutuhan Anda dan menyimpan hasilnya ke tempat yang diperlukan. Anda juga dapat melihat lebih mendetail tentang fitur yang didukung di [halaman] github kami (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), atau di [dokumentasi] produk kami (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Langkah-langkah untuk Menambahkan Anotasi ke XLSM di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Java untuk menambahkan berbagai jenis anotasi ke file XLSM dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.
        *   Buat objek Balas dengan komentar dan tanggal.
        *   Buat objek AreaAnnotation, setel opsi area, dan tambahkan balasan.
        *   Buat objek Annotator dan tambahkan anotasi area.
        *   Simpan file keluaran.
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Anotasi untuk Java API didukung di semua platform utama dan sistem operasi. Sebelum menjalankan kode di bawah ini, harap pastikan bahwa Anda telah menginstal prasyarat berikut di sistem Anda.
        *   Sistem Operasi: Microsoft Windows, Linux, MacOS
        *   Lingkungan Pengembangan: NetBeans, Intellij IDEA, Eclipse dll
        *   Java Runtime Environment: Java 7 (1.7) dan yang lebih baru
        *   Dapatkan versi terbaru GroupDocs.Annotation untuk Java dari [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Pratinjau anotasi dan contoh kode
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
    title_left: "Langkah-langkah untuk Menghapus Anotasi dari XLSM di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) mempermudah pengembang Java untuk menghapus detail anotasi dari file XLSM dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.
        *   Buat objek Balas dengan komentar dan tanggal.
        *   Instansiasi objek SaveOptions dan atur AnnotationTypes = AnnotationType.None.
        *   Panggil metode penyimpanan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.

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
    title_left: "Langkah-langkah untuk Mengedit Anotasi dari XLSM di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Java untuk memperbarui berbagai properti anotasi dari file XLSM dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.
        *   Instansiasi objek Annotator dengan jalur atau aliran dokumen masukan dengan LoadOptions yang dibuat instance dengan ImportAnnotations = true.
        *   Buat beberapa implementasi AnnotationBase dan tetapkan Id anotasi yang ada (jika anotasi dengan Id tersebut tidak ditemukan, tidak ada yang akan diubah) atau daftar jalur anotasi (semua anotasi yang ada akan dihapus).
        *   Panggil metode pembaruan objek Annotator dengan anotasi yang diteruskan.
        *   Panggil metode penyimpanan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.

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
    title_left: "Langkah-langkah untuk Mengekstrak Anotasi dari XLSM di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Java untuk membuat anotasi dokumen dan mengekstrak informasi anotasi dari file XLSM dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.
        *   Buat objek Balas dengan komentar dan tanggal.
        *   Instansiasi objek LoadOptions dan panggil SetImportAnnotations dengan argumen yang benar.
        *   Tentukan variabel dengan tipe Daftar.
        *   Panggil metode dapatkan dan kembalikan hasil ke variabel di atas.

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
    title: "Demo Langsung untuk Menambah, Menghapus, Mengedit, Mengekstrak Anotasi ke Dokumen dan Gambar"
    content: |
        Tambahkan, hapus, edit, dan ekstrak anotasi ke file XLSM sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Demo langsung memiliki manfaat berikut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsm"
          title: "Tentang XLSM Format File"
          content: |
            File dengan ekstensi XLSM adalah jenis file Spreadsheet yang mendukung Macro. Dari sudut pandang aplikasi, Makro adalah sekumpulan instruksi yang digunakan untuk mengotomatisasi proses. Makro digunakan untuk merekam langkah-langkah yang dilakukan berulang kali dan memfasilitasi melakukan tindakan dengan menjalankan makro lagi. Makro diprogram dengan Visual Basic for Applications (VBA) Microsoft dari dalam Buku Kerja Excel menggunakan Editor Visual Basic dan dapat dijalankan/di-debug langsung dari sana.

          link: "https://docs.fileformat.com/image/xlsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bekerja dengan Format Dokumen Populer Lainnya"
    content: |
        Perbarui properti anotasi dari beberapa format file populer seperti yang dinyatakan di bawah ini.
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