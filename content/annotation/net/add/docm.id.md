---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Tambahkan Anotasi ke File DOCM di Aplikasi C# .NET"
head_description: "Pemrosesan anotasi C# .NET &amp; API manajemen untuk menambahkan jenis anotasi populer ke file DOCM, gambar, gambar, dan format file dokumen."

title: "Tambahkan Anotasi ke DOCM di .NET"
description: "Anotasi gambar, Microsoft Office, dan format file dokumen lainnya menggunakan 13 jenis anotasi berbeda termasuk teks, komentar, catatan, dll."
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
        [GroupDocs.Annotation for .NET](/id/annotation/net/) adalah .NET API asli yang memungkinkan pengguna untuk menambah, mengedit, dan menghapus anotasi dari gambar dan format file dokumen. Anda dapat dengan mudah menggunakan komentar, catatan, komentar, dan berbagai jenis anotasi termasuk teks, grafik, dan tanda air ke PDF, HTML, Word, Excel, diagram Visio, presentasi, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara tepat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian.

steps:
    enable: true
    title_left: "Langkah-langkah untuk Menambahkan Anotasi ke DOCM di C#"
    content_left: |
        [GroupDocs.Annotation](/id/annotation/net/) memudahkan pengembang .NET untuk menambahkan properti anotasi ke file DOCM dari dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance objek Annotator dengan jalur atau aliran dokumen masukan.
        * Buat instance objek TextFieldAnnotation dengan properti yang diinginkan (posisi, nomor halaman, dll).
        * Panggil metode Add dan berikan objek TextFieldAnnotation.
        * Metode Panggil Simpan dengan jalur atau aliran dokumen yang dihasilkan.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Annotation untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.annotation)
        
    code: |
        ```cs
        //Tambahkan anotasi bidang teks ke dokumen dari disk lokal
        using (Annotator annotator = new Annotator("input.docm"))
        {
        	TextFieldAnnotation textField = new TextFieldAnnotation
            {
            	BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "This is text field annotation",
                Opacity = 0.7,
                PageNumber = 0,
                PenStyle = PenStyle.Dot,
                PenWidth = 3,
                FontFamily = "Arial",
                TextHorizontalAlignment = HorizontalAlignment.Center,
                Replies = new List
                {
                	new Reply
                    {
                    	Comment = "First comment",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                    	Comment = "Second comment",
                        RepliedOn = DateTime.Now
                    }
                }
        	};
            annotator.Add(textField);
            annotator.Save("result.docm");
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Menambahkan Anotasi"
    content: |
        Tambahkan anotasi ke file DOCM sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demo](https://products.groupdocs.app/annotation/family).  
        Demo langsung memiliki manfaat sebagai berikut
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-docm"
          title: "Tentang Format Berkas DOCM"
          content: |
            File DOCM adalah dokumen yang dihasilkan Microsoft Word 2007 atau lebih tinggi dengan kemampuan untuk menjalankan makro. Ini mirip dengan format file DOCX tetapi kemampuan untuk menjalankan makro membuatnya berbeda dari DOCX. Seperti DOCX, file DOCM dapat menyimpan teks, gambar, tabel, bentuk, bagan, dan konten lainnya. Kemampuan menjalankan makro memudahkan untuk menghemat waktu dengan menjalankan serangkaian perintah dalam bentuk tindakan yang direkam untuk penyelesaian tugas secara otomatis . File DOCM dapat dibuka dan diedit di Microsoft Word 2007 ke atas.

          link: "https://docs.fileformat.com/word-processing/docm/"

more_formats:
    enable: false
    title: "Menambahkan Anotasi Ke Format File Lain"
    content: |
        Dokumen multi format dan API pemrosesan anotasi gambar untuk .NET. Tambahkan anotasi ke beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Tambahkan Anotasi ke PDF"
          link: "https://products.groupdocs.com/annotation/net/add/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Tambahkan Anotasi ke DOC"
          link: "https://products.groupdocs.com/annotation/net/add/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Tambahkan Anotasi ke DOCX"
          link: "https://products.groupdocs.com/annotation/net/add/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Tambahkan Anotasi ke DOT"
          link: "https://products.groupdocs.com/annotation/net/add/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Tambahkan Anotasi ke DOTX"
          link: "https://products.groupdocs.com/annotation/net/add/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Tambahkan Anotasi ke DOTM"
          link: "https://products.groupdocs.com/annotation/net/add/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Tambahkan Anotasi ke RTF"
          link: "https://products.groupdocs.com/annotation/net/add/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Tambahkan Anotasi ke ODT"
          link: "https://products.groupdocs.com/annotation/net/add/odt/"
          description: "Buka Teks Dokumen"

        - name: "Tambahkan Anotasi ke XLS"
          link: "https://products.groupdocs.com/annotation/net/add/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Tambahkan Anotasi ke XLSX"
          link: "https://products.groupdocs.com/annotation/net/add/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Tambahkan Anotasi ke XLSM"
          link: "https://products.groupdocs.com/annotation/net/add/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Tambahkan Anotasi ke XLSB"
          link: "https://products.groupdocs.com/annotation/net/add/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Tambahkan Anotasi ke ODS"
          link: "https://products.groupdocs.com/annotation/net/add/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Tambahkan Anotasi ke PPT"
          link: "https://products.groupdocs.com/annotation/net/add/ppt/"
          description: "Presentasi powerpoint"

        - name: "Tambahkan Anotasi ke PPTX"
          link: "https://products.groupdocs.com/annotation/net/add/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Tambahkan Anotasi ke PPSX"
          link: "https://products.groupdocs.com/annotation/net/add/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Tambahkan Anotasi ke POTM"
          link: "https://products.groupdocs.com/annotation/net/add/potm/"
          description: "Templat Microsoft PowerPoint"

        - name: "Tambahkan Anotasi ke PPTM"
          link: "https://products.groupdocs.com/annotation/net/add/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Tambahkan Anotasi ke PPS"
          link: "https://products.groupdocs.com/annotation/net/add/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Tambahkan Anotasi ke ODP"
          link: "https://products.groupdocs.com/annotation/net/add/odp/"
          description: "Presentasi OpenDocument"

        - name: "Tambahkan Anotasi ke HTML"
          link: "https://products.groupdocs.com/annotation/net/add/html/"
          description: "Hyper Text Markup Language"

        - name: "Tambahkan Anotasi ke TIFF"
          link: "https://products.groupdocs.com/annotation/net/add/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Tambahkan Anotasi ke JPEG"
          link: "https://products.groupdocs.com/annotation/net/add/jpeg/"
          description: "Gambar JPEG"

        - name: "Tambahkan Anotasi ke PNG"
          link: "https://products.groupdocs.com/annotation/net/add/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Tambahkan Anotasi ke BMP"
          link: "https://products.groupdocs.com/annotation/net/add/bmp/"
          description: "Format File Bitmap"

        - name: "Tambahkan Anotasi ke EML"
          link: "https://products.groupdocs.com/annotation/net/add/eml/"
          description: "Pesan email"

        - name: "Tambahkan Anotasi ke MSG"
          link: "https://products.groupdocs.com/annotation/net/add/msg/"
          description: "Pesan Email Microsoft Outlook"

        - name: "Tambahkan Anotasi ke VSD"
          link: "https://products.groupdocs.com/annotation/net/add/vsd/"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Tambahkan Anotasi ke VSDX"
          link: "https://products.groupdocs.com/annotation/net/add/vsdx/"
          description: "Gambar Microsoft Visio"

        - name: "Tambahkan Anotasi ke VSS"
          link: "https://products.groupdocs.com/annotation/net/add/vss/"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Tambahkan Anotasi ke VST"
          link: "https://products.groupdocs.com/annotation/net/add/vst/"
          description: "Stensil Microsoft Visio 2013"

        - name: "Tambahkan Anotasi ke DWG"
          link: "https://products.groupdocs.com/annotation/net/add/dwg/"
          description: "Format Data Desain Autodesk"

        - name: "Tambahkan Anotasi ke DXF"
          link: "https://products.groupdocs.com/annotation/net/add/dxf/"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Tambahkan Anotasi ke DCM"
          link: "https://products.groupdocs.com/annotation/net/add/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Tambahkan Anotasi ke WMF"
          link: "https://products.groupdocs.com/annotation/net/add/wmf/"
          description: "Metafile Windows"

        - name: "Tambahkan Anotasi ke EMF"
          link: "https://products.groupdocs.com/annotation/net/add/emf/"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---
