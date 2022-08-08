---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Edit VST File Anotasi di Aplikasi Java"
head_description: "API editor anotasi Java untuk memperbarui jenis anotasi populer dari VST, gambar, gambar, dan format file dokumen."

title: "Edit Anotasi dalam File VST di Java"
description: "Editor anotasi Java untuk gambar, Microsoft Office, dan format file dokumen lainnya. Anotasi file VST menggunakan 13 jenis anotasi yang berbeda seperti; area, teks, catatan, tanda air, dll."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Unduh Uji Coba Gratis"
    link: "https://downloads.groupdocs.com/annotation/java"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "Referensi API"

            - link: "https://github.com/groupdocs-annotation"
              text: "Contoh Kode"

            - link: "https://products.groupdocs.app/annotation/family"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "Tentang GroupDocs.Annotation untuk Java API"
    content: |
        [GroupDocs.Annotation for Java](/id/annotation/java/) adalah solusi manipulasi anotasi Java asli untuk melihat, menambah, memperbarui, menghapus, dan mengekstrak anotasi dari gambar dan format file dokumen secara efisien. Pengguna dapat dengan mudah mengedit komentar, catatan, komentar, dan berbagai jenis anotasi termasuk teks, grafik, dan tanda air dalam PDF, HTML, Word, Excel, diagram Visio, presentasi, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara tepat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian.

steps:
    enable: true
    title_left: "Langkah-langkah untuk Mengedit Anotasi dari VST di Java"
    content_left: |
        [GroupDocs.Annotation](/id/annotation/java/) memudahkan pengembang Java untuk memperbarui berbagai properti anotasi dari file VST dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.

        * Instansiasi objek Annotator dengan jalur atau aliran dokumen masukan dengan LoadOptions yang diinstansiasi dengan ImportAnnotations = true.
        * Buat beberapa implementasi AnnotationBase dan atur Id dari anotasi yang ada (jika anotasi dengan Id itu tidak ditemukan, tidak ada yang akan diubah) atau daftar jalur anotasi (semua anotasi yang ada akan dihapus).
        * Memanggil metode pembaruan objek Annotator dengan anotasi yang diteruskan.
        * Panggil metode simpan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, Intellij IDEA, Eclipse dll
        * Lingkungan Runtime Java: Java 7 (1.7) ke atas
        * Dapatkan versi terbaru GroupDocs.Annotation untuk Java dari [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)
        
    code: |
        ```java
        String outputPath = "UpdateAnnotation.vst";
        Annotator annotator = new Annotator("input.vst");
        
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // tambahkan anotasi asli
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        loadOptions.setImportAnnotations(true);
        
        // buka dokumen beranotasi
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);
        
        // sarankan kami ingin mengubah beberapa properti dari anotasi yang ada
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // perbarui anotasi
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Memodifikasi Anotasi dari Dokumen dan Gambar"
    content: |
        Baca dan edit anotasi dari file VST sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demo](https://products.groupdocs.app/annotation/family).  
        Demo langsung memiliki manfaat sebagai berikut
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-vst"
          title: "Tentang Format Berkas VST"
          content: |
            File dengan ekstensi VST adalah file gambar vektor yang dibuat dengan Microsoft Visio dan bertindak sebagai template untuk membuat file lebih lanjut. File templat ini dalam format file biner dan berisi tata letak dan pengaturan default yang digunakan untuk pembuatan gambar Visio baru. Saat file VST dibuka di Microsoft Visio, file tersebut berisi pengaturan yang ada untuk terus bekerja dengan dokumen. Secara umum, file Visio digunakan untuk membuat gambar yang berisi objek visual, diagram alir, diagram UML, aliran informasi, bagan organisasi, diagram perangkat lunak, tata letak jaringan, model basis data, pemetaan objek, dan informasi serupa lainnya. File yang dihasilkan menggunakan Visio juga dapat diekspor ke berbagai format file seperti PNG, BMP, PDF, dan lainnya.

          link: "https://docs.fileformat.com/image/vst/"

more_formats:
    enable: false
    title: "Mengedit Anotasi Dari Format File Populer Lainnya"
    content: |
        API editor anotasi Java untuk dokumen dan format gambar. Perbarui properti anotasi dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Edit Anotasi dari PDF"
          link: "https://products.groupdocs.com/annotation/java/edit/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Edit Anotasi dari DOC"
          link: "https://products.groupdocs.com/annotation/java/edit/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Edit Anotasi dari DOCM"
          link: "https://products.groupdocs.com/annotation/java/edit/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Edit Anotasi dari DOCX"
          link: "https://products.groupdocs.com/annotation/java/edit/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Edit Anotasi dari DOT"
          link: "https://products.groupdocs.com/annotation/java/edit/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Edit Anotasi dari DOTX"
          link: "https://products.groupdocs.com/annotation/java/edit/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Edit Anotasi dari DOTM"
          link: "https://products.groupdocs.com/annotation/java/edit/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Edit Anotasi dari RTF"
          link: "https://products.groupdocs.com/annotation/java/edit/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Edit Anotasi dari ODT"
          link: "https://products.groupdocs.com/annotation/java/edit/odt/"
          description: "Buka Teks Dokumen"

        - name: "Edit Anotasi dari XLS"
          link: "https://products.groupdocs.com/annotation/java/edit/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Edit Anotasi dari XLSX"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Edit Anotasi dari XLSM"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Edit Anotasi dari XLSB"
          link: "https://products.groupdocs.com/annotation/java/edit/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Edit Anotasi dari ODS"
          link: "https://products.groupdocs.com/annotation/java/edit/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Edit Anotasi dari PPT"
          link: "https://products.groupdocs.com/annotation/java/edit/ppt/"
          description: "Presentasi powerpoint"

        - name: "Edit Anotasi dari PPTX"
          link: "https://products.groupdocs.com/annotation/java/edit/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Edit Anotasi dari PPSX"
          link: "https://products.groupdocs.com/annotation/java/edit/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Edit Anotasi dari POTM"
          link: "https://products.groupdocs.com/annotation/java/edit/potm/"
          description: "Templat Microsoft PowerPoint"

        - name: "Edit Anotasi dari PPTM"
          link: "https://products.groupdocs.com/annotation/java/edit/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Edit Anotasi dari PPS"
          link: "https://products.groupdocs.com/annotation/java/edit/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Edit Anotasi dari ODP"
          link: "https://products.groupdocs.com/annotation/java/edit/odp/"
          description: "Presentasi OpenDocument"

        - name: "Edit Anotasi dari HTML"
          link: "https://products.groupdocs.com/annotation/java/edit/html/"
          description: "Hyper Text Markup Language"

        - name: "Edit Anotasi dari TIFF"
          link: "https://products.groupdocs.com/annotation/java/edit/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Edit Anotasi dari JPEG"
          link: "https://products.groupdocs.com/annotation/java/edit/jpeg/"
          description: "Gambar JPEG"

        - name: "Edit Anotasi dari PNG"
          link: "https://products.groupdocs.com/annotation/java/edit/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Edit Anotasi dari BMP"
          link: "https://products.groupdocs.com/annotation/java/edit/bmp/"
          description: "Format File Bitmap"

        - name: "Edit Anotasi dari EML"
          link: "https://products.groupdocs.com/annotation/java/edit/eml/"
          description: "Pesan email"

        - name: "Edit Anotasi dari MSG"
          link: "https://products.groupdocs.com/annotation/java/edit/msg/"
          description: "Pesan Email Microsoft Outlook"

        - name: "Edit Anotasi dari VSD"
          link: "https://products.groupdocs.com/annotation/java/edit/vsd/"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Edit Anotasi dari VSDX"
          link: "https://products.groupdocs.com/annotation/java/edit/vsdx/"
          description: "Gambar Microsoft Visio"

        - name: "Edit Anotasi dari VSS"
          link: "https://products.groupdocs.com/annotation/java/edit/vss/"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Edit Anotasi dari DWG"
          link: "https://products.groupdocs.com/annotation/java/edit/dwg/"
          description: "Format Data Desain Autodesk"

        - name: "Edit Anotasi dari DXF"
          link: "https://products.groupdocs.com/annotation/java/edit/dxf/"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Edit Anotasi dari DCM"
          link: "https://products.groupdocs.com/annotation/java/edit/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Edit Anotasi dari WMF"
          link: "https://products.groupdocs.com/annotation/java/edit/wmf/"
          description: "Metafile Windows"

        - name: "Edit Anotasi dari EMF"
          link: "https://products.groupdocs.com/annotation/java/edit/emf/"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---
