---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Tambahkan Anotasi ke BMP di Aplikasi Java"
head_description: "Java API untuk membuat dan menambahkan jenis anotasi populer ke BMP, gambar, gambar, dan format file dokumen."

title: "Anotasi BMP File di Java"
description: "Tambahkan anotasi ke BMP, dokumen Microsoft Office, gambar, HTML, gambar, dan format file lainnya di semua jenis aplikasi Java."
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
        [GroupDocs.Annotation for Java](/id/annotation/java/) adalah Java API asli untuk manajemen anotasi dengan dukungan komprehensif untuk membuat, menambah, mengedit, menghapus, mengekstrak, dan mengekspor anotasi dari gambar dan format file dokumen. Pengguna dapat dengan mudah mengekstrak komentar, catatan, komentar, dan 13 jenis anotasi yang berbeda termasuk teks, grafik, dan tanda air dalam PDF, HTML, dokumen Microsoft Word, spreadsheet Excel, diagram Visio, presentasi PowerPoint, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara akurat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian anotasi.

steps:
    enable: true
    title_left: "Langkah-langkah untuk Menambahkan Anotasi ke BMP di Java"
    content_left: |
        [GroupDocs.Annotation](/id/annotation/java/) memudahkan pengembang Java untuk menambahkan berbagai jenis anotasi ke file BMP dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.

        * Buat objek Balas dengan komentar dan tanggal.
        * Buat objek AreaAnnotation, atur opsi area dan tambahkan balasan.
        * Buat objek Annotator dan tambahkan anotasi area.
        * Simpan file keluaran.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, Intellij IDEA, Eclipse dll
        * Lingkungan Runtime Java: Java 7 (1.7) ke atas
        * Dapatkan versi terbaru GroupDocs.Annotation untuk Java dari [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)
        
    code: |
        ```java
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
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
        
        Annotator annotator = new Annotator("input.bmp");
        annotator.add(area);
        annotator.save("output.bmp");
        annotator.dispose();
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Menambahkan Anotasi ke Dokumen dan Gambar"
    content: |
        Buat dan tambahkan anotasi ke file BMP sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation](https://products.groupdocs.app/annotation/family). Demo langsung memiliki manfaat sebagai berikut.
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-bmp"
          title: "Tentang Format Berkas BMP"
          content: |
            File berekstensi .BMP merupakan file Gambar Bitmap yang digunakan untuk menyimpan gambar digital bitmap. Gambar-gambar ini tidak tergantung pada adaptor grafis dan juga disebut format file bitmap independen perangkat (DIB). Independensi ini bertujuan untuk membuka file di berbagai platform seperti Microsoft Windows dan Mac. Format file BMP dapat menyimpan data sebagai gambar digital dua dimensi baik dalam format monokrom maupun warna dengan kedalaman warna yang beragam.

          link: "https://docs.fileformat.com/image/bmp/"

more_formats:
    enable: false
    title: "Menganotasi Format File Populer Lainnya"
    content: |
        Pustaka manajemen anotasi Java untuk dokumen dan format gambar. Tambahkan properti anotasi ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan Anotasi ke PDF"
          link: "annotation/java/add/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan Anotasi ke DOC"
          link: "annotation/java/add/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan Anotasi ke DOCM"
          link: "annotation/java/add/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan Anotasi ke DOCX"
          link: "annotation/java/add/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan Anotasi ke DOT"
          link: "annotation/java/add/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan Anotasi ke DOTX"
          link: "annotation/java/add/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan Anotasi ke DOTM"
          link: "annotation/java/add/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan Anotasi ke RTF"
          link: "annotation/java/add/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan Anotasi ke ODT"
          link: "annotation/java/add/odt/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan Anotasi ke XLS"
          link: "annotation/java/add/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan Anotasi ke XLSX"
          link: "annotation/java/add/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan Anotasi ke XLSM"
          link: "annotation/java/add/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan Anotasi ke XLSB"
          link: "annotation/java/add/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan Anotasi ke ODS"
          link: "annotation/java/add/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan Anotasi ke PPT"
          link: "annotation/java/add/ppt/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan Anotasi ke PPTX"
          link: "annotation/java/add/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan Anotasi ke PPSX"
          link: "annotation/java/add/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan Anotasi ke POTM"
          link: "annotation/java/add/potm/"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan Anotasi ke PPTM"
          link: "annotation/java/add/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan Anotasi ke PPS"
          link: "annotation/java/add/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan Anotasi ke ODP"
          link: "annotation/java/add/odp/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan Anotasi ke HTML"
          link: "annotation/java/add/html/"
          description: "Hyper Text Markup Language"

        - name: "Tambahkan Anotasi ke TIFF"
          link: "annotation/java/add/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan Anotasi ke JPEG"
          link: "annotation/java/add/jpeg/"
          description: "Gambar JPEG"

        - name: "Tambahkan Anotasi ke PNG"
          link: "annotation/java/add/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan Anotasi ke EML"
          link: "annotation/java/add/eml/"
          description: "Pesan email"

        - name: "Tambahkan Anotasi ke MSG"
          link: "annotation/java/add/msg/"
          description: "Pesan Email Microsoft Outlook"

        - name: "Tambahkan Anotasi ke VSD"
          link: "annotation/java/add/vsd/"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Tambahkan Anotasi ke VSDX"
          link: "annotation/java/add/vsdx/"
          description: "Gambar Microsoft Visio"

        - name: "Tambahkan Anotasi ke VSS"
          link: "annotation/java/add/vss/"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Tambahkan Anotasi ke VST"
          link: "annotation/java/add/vst/"
          description: "Stensil Microsoft Visio 2013"

        - name: "Tambahkan Anotasi ke DWG"
          link: "annotation/java/add/dwg/"
          description: "Format Data Desain Autodesk"

        - name: "Tambahkan Anotasi ke DXF"
          link: "annotation/java/add/dxf/"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Tambahkan Anotasi ke DCM"
          link: "annotation/java/add/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Tambahkan Anotasi ke WMF"
          link: "annotation/java/add/wmf/"
          description: "Metafile Windows"

        - name: "Tambahkan Anotasi ke EMF"
          link: "annotation/java/add/emf/"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---
