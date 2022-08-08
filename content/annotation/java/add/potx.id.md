---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Tambahkan Anotasi ke POTX di Aplikasi Java"
head_description: "Java API untuk membuat dan menambahkan jenis anotasi populer ke POTX, gambar, gambar, dan format file dokumen."

title: "Anotasi POTX File di Java"
description: "Tambahkan anotasi ke POTX, dokumen Microsoft Office, gambar, HTML, gambar, dan format file lainnya di semua jenis aplikasi Java."
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
        [GroupDocs.Annotation for Java](https://products.groupdocs.com/{{$1}/java) adalah Java API asli untuk manajemen anotasi dengan dukungan komprehensif untuk membuat, menambah, mengedit, menghapus, mengekstrak, dan mengekspor anotasi dari gambar dan format file dokumen. Pengguna dapat dengan mudah mengekstrak komentar, catatan, komentar, dan 13 jenis anotasi yang berbeda termasuk teks, grafik, dan tanda air dalam PDF, HTML, dokumen Microsoft Word, spreadsheet Excel, diagram Visio, presentasi PowerPoint, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara akurat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian anotasi.

steps:
    enable: true
    title_left: "Langkah-langkah untuk Menambahkan Anotasi ke POTX di Java"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/java) memudahkan pengembang Java untuk menambahkan berbagai jenis anotasi ke file POTX dalam aplikasi berbasis Java dengan menerapkan beberapa langkah mudah.

        * Buat instance objek Annotator dengan jalur atau aliran dokumen masukan.
        * Buat instance objek TextFieldAnnotation dengan properti yang diinginkan (posisi, nomor halaman, dll).
        * Panggil metode tambah dan lewati objek TextFieldAnnotation.
        * Panggil metode simpan dengan jalur atau aliran dokumen yang dihasilkan.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk Java API didukung di semua platform dan sistem operasi utama. Sebelum mengeksekusi kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: NetBeans, Intellij IDEA, Eclipse dll
        * Lingkungan Runtime Java: J2SE 6.0 dan yang lebih baru
        * Dapatkan versi terbaru GroupDocs.Annotation untuk Java dari [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-conversion)
        
    code: |
        ```java
        String outputPath = Constants.getOutputFilePath("AddTextStrikeoutAnnotation", FilenameUtils.getExtension(input.potx));
                    final Annotator annotator = new Annotator(input.potx);
                    try {
                        Reply reply1 = new Reply();
                        reply1.setComment("First comment");
                        reply1.setRepliedOn(Calendar.getInstance().getTime());
                        Reply reply2 = new Reply();
                        reply2.setComment("Second comment");
                        reply2.setRepliedOn(Calendar.getInstance().getTime());
                        java.util.List replies =  new ArrayList();
                        replies.add(reply1);
                        replies.add(reply2);
                        Point point1 = new Point(80, 730);
                        Point point2 = new Point(240, 730);
                        Point point3 = new Point(80, 650);
                        Point point4 = new Point(240, 650);
                        List points = new ArrayList();
                        points.add(point1);
                        points.add(point2);
                        points.add(point3);
                        points.add(point4);
                        StrikeoutAnnotation strikeout = new StrikeoutAnnotation();
                        strikeout.setCreatedOn(Calendar.getInstance().getTime());
                        strikeout.setFontColor(65535);
                        strikeout.setMessage("This is strikeout annotation");
                        strikeout.setOpacity(0.7);
                        strikeout.setPageNumber(0);
                        strikeout.setPoints(points);
                        strikeout.setReplies(replies);
                        annotator.add(strikeout);
                        annotator.save(output.potx);
                    } finally {
                        if (annotator != null) {
                            annotator.dispose();
                        }
                    }
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Menambahkan Anotasi ke Dokumen dan Gambar"
    content: |
        Buat dan tambahkan anotasi ke file POTX sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demo](https://products.groupdocs.app/annotation/family).  
        Demo langsung memiliki manfaat sebagai berikut
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-potx"
          title: "Tentang Format Berkas POTX"
          content: |
            File dengan ekstensi .POTX mewakili presentasi template Microsoft PowerPoint yang dibuat dengan Microsoft PowerPoint 2007 dan yang lebih baru. Format ini dibuat untuk menggantikan format file POT yang didasarkan pada format file biner dan didukung dengan PowerPoint 97-2003. File yang dihasilkan dapat digunakan untuk membuat presentasi yang memiliki tata letak yang sama dan pengaturan lain yang diperlukan untuk diterapkan ke file baru. Pengaturan ini dapat mencakup gaya, latar belakang, palet warna, font, dan default. File tersebut dibuat untuk membuat file template siap pakai untuk penggunaan resmi.

          link: "https://docs.fileformat.com/presentation/potx/"

more_formats:
    enable: false
    title: "Menganotasi Format File Populer Lainnya"
    content: |
        Pustaka manajemen anotasi Java untuk dokumen dan format gambar. Tambahkan properti anotasi ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan Anotasi ke PDF"
          link: "https://products.groupdocs.com/annotation/java/add/pdf"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan Anotasi ke DOC"
          link: "https://products.groupdocs.com/annotation/java/add/doc"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan Anotasi ke DOCM"
          link: "https://products.groupdocs.com/annotation/java/add/docm"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Tambahkan Anotasi ke DOCX"
          link: "https://products.groupdocs.com/annotation/java/add/docx"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan Anotasi ke DOT"
          link: "https://products.groupdocs.com/annotation/java/add/dot"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan Anotasi ke DOTX"
          link: "https://products.groupdocs.com/annotation/java/add/dotx"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan Anotasi ke DOTM"
          link: "https://products.groupdocs.com/annotation/java/add/dotm"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan Anotasi ke RTF"
          link: "https://products.groupdocs.com/annotation/java/add/rtf"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan Anotasi ke ODT"
          link: "https://products.groupdocs.com/annotation/java/add/odt"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan Anotasi ke XLS"
          link: "https://products.groupdocs.com/annotation/java/add/xls"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan Anotasi ke XLSX"
          link: "https://products.groupdocs.com/annotation/java/add/xlsx"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan Anotasi ke XLSM"
          link: "https://products.groupdocs.com/annotation/java/add/xlsm"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan Anotasi ke XLSB"
          link: "https://products.groupdocs.com/annotation/java/add/xlsb"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan Anotasi ke ODS"
          link: "https://products.groupdocs.com/annotation/java/add/ods"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan Anotasi ke PPT"
          link: "https://products.groupdocs.com/annotation/java/add/ppt"
          description: "Presentasi powerpoint"

        - name: "Tambahkan Anotasi ke PPTX"
          link: "https://products.groupdocs.com/annotation/java/add/pptx"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan Anotasi ke PPSX"
          link: "https://products.groupdocs.com/annotation/java/add/ppsx"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan Anotasi ke POTM"
          link: "https://products.groupdocs.com/annotation/java/add/potm"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan Anotasi ke PPTM"
          link: "https://products.groupdocs.com/annotation/java/add/pptm"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan Anotasi ke PPS"
          link: "https://products.groupdocs.com/annotation/java/add/pps"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan Anotasi ke ODP"
          link: "https://products.groupdocs.com/annotation/java/add/odp"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan Anotasi ke HTML"
          link: "https://products.groupdocs.com/annotation/java/add/html"
          description: "Hyper Text Markup Language"

        - name: "Tambahkan Anotasi ke TIFF"
          link: "https://products.groupdocs.com/annotation/java/add/tiff"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan Anotasi ke JPEG"
          link: "https://products.groupdocs.com/annotation/java/add/jpeg"
          description: "Gambar JPEG"

        - name: "Tambahkan Anotasi ke PNG"
          link: "https://products.groupdocs.com/annotation/java/add/png"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan Anotasi ke BMP"
          link: "https://products.groupdocs.com/annotation/java/add/bmp"
          description: "Format File Bitmap"

        - name: "Tambahkan Anotasi ke EML"
          link: "https://products.groupdocs.com/annotation/java/add/eml"
          description: "Pesan email"

        - name: "Tambahkan Anotasi ke MSG"
          link: "https://products.groupdocs.com/annotation/java/add/msg"
          description: "Pesan Email Microsoft Outlook"

        - name: "Tambahkan Anotasi ke VSD"
          link: "https://products.groupdocs.com/annotation/java/add/vsd"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Tambahkan Anotasi ke VSDX"
          link: "https://products.groupdocs.com/annotation/java/add/vsdx"
          description: "Gambar Microsoft Visio"

        - name: "Tambahkan Anotasi ke VSS"
          link: "https://products.groupdocs.com/annotation/java/add/vss"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Tambahkan Anotasi ke VST"
          link: "https://products.groupdocs.com/annotation/java/add/vst"
          description: "Stensil Microsoft Visio 2013"

        - name: "Tambahkan Anotasi ke DWG"
          link: "https://products.groupdocs.com/annotation/java/add/dwg"
          description: "Format Data Desain Autodesk"

        - name: "Tambahkan Anotasi ke DXF"
          link: "https://products.groupdocs.com/annotation/java/add/dxf"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Tambahkan Anotasi ke DCM"
          link: "https://products.groupdocs.com/annotation/java/add/dcm"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Tambahkan Anotasi ke WMF"
          link: "https://products.groupdocs.com/annotation/java/add/wmf"
          description: "Metafile Windows"

        - name: "Tambahkan Anotasi ke EMF"
          link: "https://products.groupdocs.com/annotation/java/add/emf"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---
