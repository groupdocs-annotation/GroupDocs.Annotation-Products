---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Hapus Anotasi dari File MSG di Aplikasi C# .NET"
head_description: "C# .NET annotation API untuk menghapus jenis anotasi populer ke file MSG, gambar, gambar, dan format file dokumen."

title: "Hapus Anotasi dari MSG di C#"
description: "Hapus semua anotasi yang ditambahkan sebelumnya dari Microsoft Office, gambar, web, gambar, dan format file dokumen lainnya dalam semua jenis aplikasi .NET."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Unduh Uji Coba Gratis"
    link: "https://downloads.groupdocs.com/annotation/net"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Annotation for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: ".NET"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "Referensi API"

            - link: "https://github.com/groupdocs-annotation"
              text: "Contoh Kode"

            - link: "https://products.groupdocs.app/annotation/family"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "Tentang GroupDocs.Annotation untuk .NET API"
    content: |
        [GroupDocs.Annotation for .NET](/id/annotation/net/) adalah API pemrosesan anotasi .NET asli untuk melihat, menambah, memodifikasi, menghapus, dan mengekstrak anotasi dari gambar dan format file dokumen. Pengguna dapat dengan mudah menghapus komentar, catatan, komentar, dan berbagai jenis anotasi termasuk teks, grafik, dan tanda air dalam PDF, HTML, Word, Excel, diagram Visio, presentasi, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara tepat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian.

steps:
    enable: true
    title_left: "Langkah-langkah untuk Menghapus Anotasi dari MSG"
    content_left: |
        [GroupDocs.Annotation](/id/annotation/net/) memudahkan pengembang .NET untuk menghapus detail anotasi dari file MSG dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance objek Annotator dengan jalur atau aliran dokumen masukan.
        * Buat instance objek SaveOptions dan atur AnnotationTypes = AnnotationType.None.
        * Metode Panggil Simpan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Annotation untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.annotation)
        
    code: |
        ```cs
        // 1- Cara menghapus anotasi dari dokumen menggunakan indeks anotasi
        
        using (Annotator annotator = new Annotator("result.msg"))
        {
        	annotator.Remove(0);
        	annotator.Save("removed.msg");
        }
        
        // 2- Cara menghapus anotasi dari dokumen menggunakan objek anotasi
        
        using (Annotator annotator = new Annotator("result.msg"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp[0]);
        	annotator.Save("removed.msg");
        }
        
        // 3- Cara menghapus beberapa anotasi dari dokumen menggunakan daftar ID
        
        using (Annotator annotator = new Annotator("result.msg"))
        {
        	var idList = new List{1, 2, 3};
        	annotator.Remove(idList);
        	annotator.Save("removed.msg");
        }
        
        // 4- Cara menghapus beberapa anotasi dari dokumen menggunakan daftar anotasi
        
        using (Annotator annotator = new Annotator("result.msg"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp);
        	annotator.Save("removed.msg");
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Menghapus Anotasi"
    content: |
        Hapus anotasi dari file MSG sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation](https://products.groupdocs.app/annotation/family).  
        Demo langsung memiliki manfaat sebagai berikut
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-msg"
          title: "Tentang Format Berkas MSG"
          content: |
            MSG adalah format file yang digunakan oleh Microsoft Outlook dan Exchange untuk menyimpan pesan email, kontak, janji temu, atau tugas lainnya. Pesan tersebut mungkin berisi satu atau beberapa bidang email, dengan pengirim, penerima, subjek, tanggal, dan isi pesan, atau informasi kontak, rincian janji temu, dan satu atau lebih spesifikasi tugas. Properti yang membentuk objek Pesan, termasuk juga merupakan bagian dari file MSG. File MSG memiliki header, isi pesan utama, dan hyperlink sebagai teks ASCII biasa. File MSG juga cocok dengan program yang membutuhkan Antarmuka Pemrograman Aplikasi Pesan Microsoft (MAPI).

          link: "https://docs.fileformat.com/email/msg/"

more_formats:
    enable: false
    title: "Menghapus Anotasi Dari Format File Lain yang Didukung"
    content: |
        Dokumen multi format dan anotasi gambar menghapus API untuk .NET. Hapus anotasi dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Hapus Anotasi dari PDF"
          link: "https://products.groupdocs.com/annotation/net/remove/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Hapus Anotasi dari DOC"
          link: "https://products.groupdocs.com/annotation/net/remove/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Hapus Anotasi dari DOCM"
          link: "https://products.groupdocs.com/annotation/net/remove/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Hapus Anotasi dari DOCX"
          link: "https://products.groupdocs.com/annotation/net/remove/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Hapus Anotasi dari DOT"
          link: "https://products.groupdocs.com/annotation/net/remove/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Hapus Anotasi dari DOTX"
          link: "https://products.groupdocs.com/annotation/net/remove/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Hapus Anotasi dari DOTM"
          link: "https://products.groupdocs.com/annotation/net/remove/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Hapus Anotasi dari RTF"
          link: "https://products.groupdocs.com/annotation/net/remove/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Hapus Anotasi dari ODT"
          link: "https://products.groupdocs.com/annotation/net/remove/odt/"
          description: "Buka Teks Dokumen"

        - name: "Hapus Anotasi dari XLS"
          link: "https://products.groupdocs.com/annotation/net/remove/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Hapus Anotasi dari XLSX"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Hapus Anotasi dari XLSM"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Hapus Anotasi dari XLSB"
          link: "https://products.groupdocs.com/annotation/net/remove/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Hapus Anotasi dari ODS"
          link: "https://products.groupdocs.com/annotation/net/remove/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Hapus Anotasi dari PPT"
          link: "https://products.groupdocs.com/annotation/net/remove/ppt/"
          description: "Presentasi powerpoint"

        - name: "Hapus Anotasi dari PPTX"
          link: "https://products.groupdocs.com/annotation/net/remove/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Hapus Anotasi dari PPSX"
          link: "https://products.groupdocs.com/annotation/net/remove/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Hapus Anotasi dari POTM"
          link: "https://products.groupdocs.com/annotation/net/remove/potm/"
          description: "Templat Microsoft PowerPoint"

        - name: "Hapus Anotasi dari PPTM"
          link: "https://products.groupdocs.com/annotation/net/remove/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Hapus Anotasi dari PPS"
          link: "https://products.groupdocs.com/annotation/net/remove/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Hapus Anotasi dari ODP"
          link: "https://products.groupdocs.com/annotation/net/remove/odp/"
          description: "Presentasi OpenDocument"

        - name: "Hapus Anotasi dari HTML"
          link: "https://products.groupdocs.com/annotation/net/remove/html/"
          description: "Hyper Text Markup Language"

        - name: "Hapus Anotasi dari TIFF"
          link: "https://products.groupdocs.com/annotation/net/remove/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Hapus Anotasi dari JPEG"
          link: "https://products.groupdocs.com/annotation/net/remove/jpeg/"
          description: "Gambar JPEG"

        - name: "Hapus Anotasi dari PNG"
          link: "https://products.groupdocs.com/annotation/net/remove/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Hapus Anotasi dari BMP"
          link: "https://products.groupdocs.com/annotation/net/remove/bmp/"
          description: "Format File Bitmap"

        - name: "Hapus Anotasi dari EML"
          link: "https://products.groupdocs.com/annotation/net/remove/eml/"
          description: "Pesan email"

        - name: "Hapus Anotasi dari VSD"
          link: "https://products.groupdocs.com/annotation/net/remove/vsd/"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Hapus Anotasi dari VSDX"
          link: "https://products.groupdocs.com/annotation/net/remove/vsdx/"
          description: "Gambar Microsoft Visio"

        - name: "Hapus Anotasi dari VSS"
          link: "https://products.groupdocs.com/annotation/net/remove/vss/"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Hapus Anotasi dari VST"
          link: "https://products.groupdocs.com/annotation/net/remove/vst/"
          description: "Stensil Microsoft Visio 2013"

        - name: "Hapus Anotasi dari DWG"
          link: "https://products.groupdocs.com/annotation/net/remove/dwg/"
          description: "Format Data Desain Autodesk"

        - name: "Hapus Anotasi dari DXF"
          link: "https://products.groupdocs.com/annotation/net/remove/dxf/"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Hapus Anotasi dari DCM"
          link: "https://products.groupdocs.com/annotation/net/remove/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Hapus Anotasi dari WMF"
          link: "https://products.groupdocs.com/annotation/net/remove/wmf/"
          description: "Metafile Windows"

        - name: "Hapus Anotasi dari EMF"
          link: "https://products.groupdocs.com/annotation/net/remove/emf/"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---
