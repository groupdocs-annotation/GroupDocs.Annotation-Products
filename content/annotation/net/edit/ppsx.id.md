---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Baca &amp; Edit Anotasi dalam File PPSX di Aplikasi C# .NET"
head_description: "C# .NET annotation editor API untuk memperbarui jenis anotasi populer ke file PPSX, gambar, gambar, dan format file dokumen."

title: "Edit Anotasi dalam File PPSX di .NET"
description: ".Editor anotasi .NET untuk gambar, Microsoft Office, dan format file dokumen lainnya. Anotasi dokumen menggunakan 13 jenis anotasi yang berbeda seperti; area, teks, catatan, tanda air, dll."
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
        [GroupDocs.Annotation for .NET](/id/annotation/net/) adalah API manajemen & editor anotasi asli .NET yang membaca, menambah, memperbarui, menghapus, dan mengekstrak anotasi dari gambar dan format file dokumen. Pengguna dapat dengan mudah memperbarui komentar, catatan, komentar, dan berbagai jenis anotasi termasuk teks, grafik, dan tanda air dalam PDF, HTML, Word, Excel, diagram Visio, presentasi, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara tepat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian.

steps:
    enable: true
    title_left: "Langkah-langkah untuk Mengedit Anotasi dari PPSX di C#"
    content_left: |
        [GroupDocs.Annotation](/id/annotation/net/) memudahkan pengembang .NET untuk mengedit detail anotasi dari file PPSX dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance objek Annotator dengan jalur atau aliran dokumen masukan.
        * Buat beberapa implementasi AnnotationBase dan atur Id dari anotasi yang ada (jika anotasi dengan Id itu tidak ditemukan, tidak ada yang akan diubah) atau daftar jalur anotasi (semua anotasi yang ada akan dihapus).
        * Metode Pembaruan Panggilan objek Annotator dengan anotasi yang diteruskan.
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
        // buka dokumen beranotasi
        using (Annotator annotator = new Annotator("result.ppsx"))
        {
        	// dengan asumsi kita akan mengubah beberapa properti dari anotasi yang ada
                AreaAnnotation updated = new AreaAnnotation
                	{
                            // Penting untuk mengatur Id anotasi yang ada
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "This is updated annotation",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Updated first comment",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Updated second comment",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // perbarui anotasi
                annotator.Update(updated);
                annotator.Save("result.ppsx");
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Memperbarui Anotasi"
    content: |
        Edit anotasi dalam file PPSX sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demo](https://products.groupdocs.app/annotation/family).  
        Demo langsung memiliki manfaat sebagai berikut
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ppsx"
          title: "Tentang Format Berkas PPSX"
          content: |
            PPSX, Power Point Slide Show, file dibuat menggunakan Microsoft PowerPoint 2007 dan di atasnya untuk tujuan Slide Show. Ini adalah pembaruan untuk format file PPS yang didukung oleh versi Microsoft PowerPoint 97-2003. Saat file PPSX dibagikan dengan pengguna lain dan dibuka, itu dimulai sebagai PowerPoint yang ditampilkan tidak seperti file PPTX yang terbuka dalam mode yang dapat diedit. Urutan tayangan slide sama seperti pada presentasi aslinya. Semua slide menyertai gambar, suara, dan media tertanam lainnya menyertai slide presentasi ke PPSX selama pertunjukan slide.

          link: "https://docs.fileformat.com/presentation/ppsx/"

more_formats:
    enable: false
    title: "Mengedit Anotasi Dalam Format File Lain"
    content: |
        API editor anotasi dokumen dan gambar multi format untuk .NET. Perbarui anotasi dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Edit Anotasi dalam PDF"
          link: "https://products.groupdocs.com/annotation/net/edit/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Edit Anotasi di DOC"
          link: "https://products.groupdocs.com/annotation/net/edit/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Edit Anotasi di DOCM"
          link: "https://products.groupdocs.com/annotation/net/edit/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Edit Anotasi di DOCX"
          link: "https://products.groupdocs.com/annotation/net/edit/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Edit Anotasi di DOT"
          link: "https://products.groupdocs.com/annotation/net/edit/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Edit Anotasi di DOTX"
          link: "https://products.groupdocs.com/annotation/net/edit/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Edit Anotasi di DOTM"
          link: "https://products.groupdocs.com/annotation/net/edit/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Edit Anotasi di RTF"
          link: "https://products.groupdocs.com/annotation/net/edit/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Edit Anotasi di ODT"
          link: "https://products.groupdocs.com/annotation/net/edit/odt/"
          description: "Buka Teks Dokumen"

        - name: "Edit Anotasi di XLS"
          link: "https://products.groupdocs.com/annotation/net/edit/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Edit Anotasi di XLSX"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Edit Anotasi di XLSM"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Edit Anotasi di XLSB"
          link: "https://products.groupdocs.com/annotation/net/edit/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Edit Anotasi di ODS"
          link: "https://products.groupdocs.com/annotation/net/edit/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Edit Anotasi di PPT"
          link: "https://products.groupdocs.com/annotation/net/edit/ppt/"
          description: "Presentasi powerpoint"

        - name: "Edit Anotasi di PPTX"
          link: "https://products.groupdocs.com/annotation/net/edit/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Edit Anotasi di POTM"
          link: "https://products.groupdocs.com/annotation/net/edit/potm/"
          description: "Templat Microsoft PowerPoint"

        - name: "Edit Anotasi di PPTM"
          link: "https://products.groupdocs.com/annotation/net/edit/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Edit Anotasi di PPS"
          link: "https://products.groupdocs.com/annotation/net/edit/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Edit Anotasi di ODP"
          link: "https://products.groupdocs.com/annotation/net/edit/odp/"
          description: "Presentasi OpenDocument"

        - name: "Edit Anotasi dalam HTML"
          link: "https://products.groupdocs.com/annotation/net/edit/html/"
          description: "Hyper Text Markup Language"

        - name: "Edit Anotasi di TIFF"
          link: "https://products.groupdocs.com/annotation/net/edit/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Edit Anotasi dalam JPEG"
          link: "https://products.groupdocs.com/annotation/net/edit/jpeg/"
          description: "Gambar JPEG"

        - name: "Edit Anotasi dalam PNG"
          link: "https://products.groupdocs.com/annotation/net/edit/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Edit Anotasi di BMP"
          link: "https://products.groupdocs.com/annotation/net/edit/bmp/"
          description: "Format File Bitmap"

        - name: "Edit Anotasi di EML"
          link: "https://products.groupdocs.com/annotation/net/edit/eml/"
          description: "Pesan email"

        - name: "Edit Anotasi di MSG"
          link: "https://products.groupdocs.com/annotation/net/edit/msg/"
          description: "Pesan Email Microsoft Outlook"

        - name: "Edit Anotasi di VSD"
          link: "https://products.groupdocs.com/annotation/net/edit/vsd/"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Edit Anotasi di VSDX"
          link: "https://products.groupdocs.com/annotation/net/edit/vsdx/"
          description: "Gambar Microsoft Visio"

        - name: "Edit Anotasi di VSS"
          link: "https://products.groupdocs.com/annotation/net/edit/vss/"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Edit Anotasi di VST"
          link: "https://products.groupdocs.com/annotation/net/edit/vst/"
          description: "Stensil Microsoft Visio 2013"

        - name: "Edit Anotasi di DWG"
          link: "https://products.groupdocs.com/annotation/net/edit/dwg/"
          description: "Format Data Desain Autodesk"

        - name: "Edit Anotasi di DXF"
          link: "https://products.groupdocs.com/annotation/net/edit/dxf/"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Edit Anotasi di DCM"
          link: "https://products.groupdocs.com/annotation/net/edit/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Edit Anotasi di WMF"
          link: "https://products.groupdocs.com/annotation/net/edit/wmf/"
          description: "Metafile Windows"

        - name: "Edit Anotasi di EMF"
          link: "https://products.groupdocs.com/annotation/net/edit/emf/"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---