
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/emf"/>

############################# Head ############################
head_title: "Java EMF Anotasi API Anotasi dalam C#"
head_description: "Java API untuk membuat dan Menganotasi jenis anotasi populer dari EMF, gambar, gambar, dan format file dokumen."

############################# Header ############################
title: "Beri anotasi EMF dari Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Anotasi untuk Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Annotation untuk Java API"
    content: |
        GroupDocs.Annotation for Java API adalah pustaka yang memungkinkan Anda menambahkan anotasi ke PDF, Word, dan dokumen lain di Mac, Windows, atau Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) adalah API asli Java untuk mengelola anotasi dengan dukungan komprehensif untuk membuat, menambahkan, mengedit, menghapus, mengekstrak, dan mengekspor anotasi dari gambar dan berbagai dokumen lainnya. Daftar lengkap format dokumen yang didukung dapat Anda lihat di [halaman](https://docs.groupdocs.com/annotation/java/supported-document-formats/) ini.

        Pustaka ini memungkinkan Anda bekerja tidak hanya dengan dokumen EMF tetapi juga dengan banyak jenis dokumen lainnya seperti Word, Excel, PowerPoint, email Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad, dan banyak lainnya.

        GroupDocs.Annotation untuk Java API memungkinkan Anda membuat dan menambahkan catatan baru, mengedit anotasi, mengekstrak komentar, anotasi, dan menghapusnya dari dokumen. Perpustakaan mendukung 13 jenis anotasi yang berbeda, termasuk Teks, Polyline, Area, Garis Bawah, Titik, Tanda Air, Panah, Ellipse, Penggantian Teks, Jarak, Bidang Teks, Redaksi Sumber Daya dalam PDF, HTML, dokumen Microsoft Word, spreadsheet, diagram, presentasi, gambar, gambar dan banyak format file lainnya.

        Contoh (silakan lihat di bawah) mendemonstrasikan bekerja dengan dokumen EMF, dalam contoh ini Anda dapat melihat langkah-langkah utama tentang cara bekerja dengan GroupDocs. Anotasi: Menyiapkan lisensi, membuka dokumen yang ingin Anda kerjakan, membuat anotasi, menambahkan objek data untuk mengatur properti anotasi sesuai dengan kebutuhan Anda dan menyimpan hasilnya ke tempat yang diperlukan. Anda juga dapat melihat lebih detail tentang fitur yang didukung di github kami [halaman](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), atau di [dokumentasi produk kami ](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Langkah-langkah untuk Menambahkan Anotasi dari EMF di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Java untuk menambahkan berbagai jenis anotasi ke file EMF dalam aplikasi berbasis Java apa pun dengan menerapkan beberapa langkah mudah.
        * Buat objek Balas dengan komentar dan tanggal.
        * Buat objek AreaAnnotation, atur opsi area dan tambahkan balasan.
        * Buat objek Annotator dan tambahkan anotasi area.
        * Simpan file keluaran.
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, harap pastikan bahwa Anda telah menginstal prasyarat berikut di sistem Anda.
        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, Intellij IDEA, Eclipse dll
        * Java Runtime Environment: Java 7 (1.7) dan yang lebih baru
        * Dapatkan versi terbaru GroupDocs.Annotation untuk Java dari [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: "Pratinjau anotasi dan contoh kode"
    content: |
        ![Gambar pratinjau anotasi](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ``` jawa
        // Buat instance kelas Balas dan tambahkan komentar
        Reply firstReply = new Reply();
        firstReply.setComment("Komentar pertama");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Komentar kedua");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Buat instance kelas AreaAnnotation dan setel opsi
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle baru(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("Ini adalah anotasi area");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Buat instance kelas Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Tambahkan anotasi
        anotator.add(area);
        
        // Simpan ke file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Langkah-langkah untuk Menghapus Anotasi dari EMF di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) mempermudah pengembang Java untuk menghapus detail anotasi dari file EMF dalam aplikasi berbasis Java apa pun dengan menerapkan beberapa langkah mudah.
        * Buat objek Balas dengan komentar dan tanggal.
        * Instansiasi objek SaveOptions dan atur AnnotationTypes = AnnotationType.None.
        * Panggil metode penyimpanan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ``` jawa
        // Buat instance kelas Annotator
        Annotator annotator = new Annotator("C://input.bmp");

        // Hapus anotasi berdasarkan tipe yang ditetapkan Tidak ada
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Simpan anotasi ke file keluaran
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Langkah-langkah untuk Mengedit Anotasi dari EMF di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) mempermudah pengembang Java untuk memperbarui berbagai properti anotasi dari file EMF dalam aplikasi berbasis Java apa pun dengan menerapkan beberapa langkah mudah.
        * Instansiasi objek Annotator dengan jalur atau aliran dokumen masukan dengan LoadOptions yang dibuat dengan ImportAnnotations = true.
        * Buat beberapa implementasi AnnotationBase dan tetapkan Id dari anotasi yang ada (jika anotasi dengan Id tersebut tidak ditemukan, tidak ada yang akan diubah) atau daftar jalur anotasi (semua anotasi yang ada akan dihapus).
        * Panggil metode pembaruan objek Annotator dengan anotasi yang diteruskan.
        * Panggil metode penyimpanan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ``` jawa
        String outputPath = "UpdateAnnotation.bmp";

        // Buat instance kelas Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Buat instance kelas Balas untuk contoh pertama dan tambahkan komentar
        Reply reply1 = new Reply();
        reply1.setComment("Komentar pertama asli");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Komentar kedua asli");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Buat instance kelas AreaAnnotation dan setel opsi
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("Ini adalah anotasi asli");
        original.setReplies(replies);
        
        // Tambahkan anotasi asli
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = LoadOptions baru();
        
        // Buka dokumen beranotasi
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Buat instance kelas Balas untuk memperbarui contoh pertama
        Reply reply3 = new Reply();
        reply3.setComment("Komentar pertama diperbarui");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Komentar kedua diperbarui");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Sarankan kami ingin mengubah beberapa properti dari anotasi yang ada
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle baru(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("Ini adalah anotasi yang diperbarui");
        updated.setReplies(replies1);
        
        // Perbarui dan simpan anotasi
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Langkah-langkah untuk Mengekstrak Anotasi dari EMF di Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Java untuk menganotasi dokumen dan mengekstrak informasi anotasi dari file EMF dalam aplikasi berbasis Java apa pun dengan menerapkan beberapa langkah mudah.
        * Buat objek Balas dengan komentar dan tanggal.
        * Instansiasi objek LoadOptions dan panggil SetImportAnnotations dengan argumen yang benar.
        * Tentukan variabel dengan jenis Daftar.
        * Panggil metode dapatkan dan kembalikan hasilnya ke variabel di atas.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ``` jawa
        // Untuk menggunakan file input contoh ini ("annotated.bmp") harus dengan anotasi
        LoadOptions loadOptions = LoadOptions baru();
        
        // Buat instance kelas Annotator dan dapatkan anotasi
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Demo Langsung untuk Menambah, Menghapus, Mengedit, Mengekstrak Anotasi ke Dokumen dan Gambar"
    content: |
        Tambahkan, hapus, edit, dan ekstrak anotasi ke file EMF sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        Demo langsung memiliki manfaat berikut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-emf"
          title: "Tentang EMF Format Berkas"
          content: |
            Enhanced metafile format (EMF) menyimpan gambar grafis secara mandiri. Metafiles EMF terdiri dari catatan panjang variabel dalam urutan kronologis yang dapat merender gambar yang disimpan setelah diuraikan pada perangkat keluaran apa pun. Rekaman dengan panjang variabel ini dapat berupa definisi objek terlampir, perintah untuk menggambar, dan properti grafik yang penting untuk merender gambar secara akurat. Saat perangkat membuka metafile EMF menggunakan lingkungan grafisnya sendiri, proporsi, dimensi, warna, dan properti grafis lainnya dari gambar asli tetap sama terlepas dari platform perangkat pembuka.
          link: "https://docs.fileformat.com/image/emf/"

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