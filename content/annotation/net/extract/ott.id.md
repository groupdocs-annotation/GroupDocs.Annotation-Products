---
layout: "auto-gen"
date: 2022-07-07T12:44:18+03:00
draft: false

head_title: "Ekstrak &amp; Ekspor Anotasi dari OTT File di C# .NET"
head_description: "C# .NET anotasi ekstraksiAPI untuk mengekstrak jenis anotasi populer dari file OTT, gambar, gambar, dan format file dokumen."

title: "Ekstrak Anotasi dari OTT di C#"
description: "Ekstrak anotasi dari Microsoft Office, gambar, HTML, gambar, dan format file dokumen lainnya dalam semua jenis aplikasi C# .NET."
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
        [GroupDocs.Annotation for .NET](/id/annotation/net/) adalah API manajemen anotasi .NET asli untuk membaca, menambah, mengedit, menghapus, mengekstrak, dan mengekspor anotasi dari gambar dan format file dokumen. Pengguna dapat dengan mudah mengekstrak komentar, catatan, komentar, dan berbagai jenis anotasi termasuk teks, grafik, dan tanda air dari PDF, HTML, dokumen Microsoft Word, spreadsheet Excel, diagram Visio, presentasi PowerPoint, gambar, gambar, dan banyak format file lainnya. Fitur pemrosesan anotasi dapat secara akurat membaca anotasi dari dokumen yang diimpor dan memungkinkan mengekspor kembali ke format file asli atau yang diinginkan setelah menerapkan penyesuaian anotasi.

steps:
    enable: true
    title_left: "Langkah-langkah Mengekstrak Anotasi dari OTT"
    content_left: |
        [GroupDocs.Annotation](/id/annotation/net/) memudahkan pengembang .NET untuk mengekstrak informasi anotasi dari file OTT dalam aplikasi mereka dengan menerapkan beberapa langkah mudah.

        * Buat instance objek Annotator dengan jalur atau aliran dokumen masukan.
        * Buat instance objek LoadOptions dan atur ImportAnnotation = true.
        * Tentukan variabel dengan tipe Daftar.
        * Metode Call Get dan kembalikan hasil ke variabel di atas.
        * Instansiasi objek XmlSerializer dengan tipe List.
        * Menggunakan FileStreamobject, buat anotasi bersambung ke file seperti pada contoh di bawah ini.
        
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk .NET API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, pastikan Anda telah menginstal prasyarat berikut di sistem Anda.

        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Annotation untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.annotation)
        
    code: |
        ```cs
        // untuk menggunakan contoh file input ini ("annotated.OTT") harus dengan anotasi
        using (Annotator annotator = new Annotator("annotated.ott"))
        {
        	List annotations = annotator.Get();
        	XmlSerializer formatter = new XmlSerializer(typeof(List));
        	using (FileStream fs = new FileStream("annotations.xml", FileMode.Create))
            {
            	fs.SetLength(0);
                formatter.Serialize(fs, annotations);
            }
        }
        ```
        
demos:
    enable: true
    title: "Demo Langsung untuk Mengekstrak Anotasi"
    content: |
        Ekstrak anotasi dari file OTT sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demo](https://products.groupdocs.app/annotation/family).  
        Demo langsung memiliki manfaat sebagai berikut
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ott"
          title: "Tentang Format Berkas OTT"
          content: |
            File dengan ekstensi OTT mewakili dokumen template yang dihasilkan oleh aplikasi sesuai dengan format standar OpenDocument OASIS. Ini dibuat dengan aplikasi pengolah kata seperti OpenOffice Writer gratis dan dapat menyimpan pengaturan yang dapat digunakan untuk menghasilkan dokumen baru dari file template ini. Pengaturan ini termasuk margin halaman, batas, header, footer, dan pengaturan halaman lainnya. Template tersebut digunakan dalam dokumen resmi seperti kop surat perusahaan dan formulir standar.

          link: "https://docs.fileformat.com/word-processing/ott/"

more_formats:
    enable: false
    title: "Mengekstrak Anotasi Dari Format File Lain yang Didukung"
    content: |
        .NET anotasi ekstraksi API untuk dokumen dan gambar. Ekspor anotasi dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format: 
        - name: "Ekstrak Anotasi dari PDF"
          link: "https://products.groupdocs.com/annotation/net/extract/pdf/"
          description: "Format Dokumen Portabel Adobe"

        - name: "Ekstrak Anotasi dari DOC"
          link: "https://products.groupdocs.com/annotation/net/extract/doc/"
          description: "Dokumen Microsoft Word"

        - name: "Ekstrak Anotasi dari DOCM"
          link: "https://products.groupdocs.com/annotation/net/extract/docm/"
          description: "Dokumen Berkemampuan Makro Microsoft Word"

        - name: "Ekstrak Anotasi dari DOCX"
          link: "https://products.groupdocs.com/annotation/net/extract/docx/"
          description: "Microsoft Word Buka Dokumen XML"

        - name: "Ekstrak Anotasi dari DOT"
          link: "https://products.groupdocs.com/annotation/net/extract/dot/"
          description: "Templat Dokumen Microsoft Word"

        - name: "Ekstrak Anotasi dari DOTX"
          link: "https://products.groupdocs.com/annotation/net/extract/dotx/"
          description: "Templat Dokumen XML Word Terbuka"

        - name: "Ekstrak Anotasi dari DOTM"
          link: "https://products.groupdocs.com/annotation/net/extract/dotm/"
          description: "Templat Microsoft Word Macro-Enabled"

        - name: "Ekstrak Anotasi dari RTF"
          link: "https://products.groupdocs.com/annotation/net/extract/rtf/"
          description: "Dokumen Teks Kaya"

        - name: "Ekstrak Anotasi dari ODT"
          link: "https://products.groupdocs.com/annotation/net/extract/odt/"
          description: "Buka Teks Dokumen"

        - name: "Ekstrak Anotasi dari XLS"
          link: "https://products.groupdocs.com/annotation/net/extract/xls/"
          description: "Format File Biner Microsoft Excel"

        - name: "Ekstrak Anotasi dari XLSX"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsx/"
          description: "Microsoft Excel Buka XML Spreadsheet"

        - name: "Ekstrak Anotasi dari XLSM"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsm/"
          description: "Spreadsheet Berkemampuan Makro Microsoft Excel"

        - name: "Ekstrak Anotasi dari XLSB"
          link: "https://products.groupdocs.com/annotation/net/extract/xlsb/"
          description: "Lembar Kerja Biner Microsoft Excel"

        - name: "Ekstrak Anotasi dari ODS"
          link: "https://products.groupdocs.com/annotation/net/extract/ods/"
          description: "Buka Spreadsheet Dokumen"

        - name: "Ekstrak Anotasi dari PPT"
          link: "https://products.groupdocs.com/annotation/net/extract/ppt/"
          description: "Presentasi powerpoint"

        - name: "Ekstrak Anotasi dari PPTX"
          link: "https://products.groupdocs.com/annotation/net/extract/pptx/"
          description: "Presentasi PowerPoint Terbuka XML"

        - name: "Ekstrak Anotasi dari PPSX"
          link: "https://products.groupdocs.com/annotation/net/extract/ppsx/"
          description: "PowerPoint Terbuka XML Slide Show"

        - name: "Ekstrak Anotasi dari POTM"
          link: "https://products.groupdocs.com/annotation/net/extract/potm/"
          description: "Templat Microsoft PowerPoint"

        - name: "Ekstrak Anotasi dari PPTM"
          link: "https://products.groupdocs.com/annotation/net/extract/pptm/"
          description: "Presentasi Microsoft PowerPoint"

        - name: "Ekstrak Anotasi dari PPS"
          link: "https://products.groupdocs.com/annotation/net/extract/pps/"
          description: "Peragaan Slide Microsoft PowerPoint 97-2003"

        - name: "Ekstrak Anotasi dari ODP"
          link: "https://products.groupdocs.com/annotation/net/extract/odp/"
          description: "Presentasi OpenDocument"

        - name: "Ekstrak Anotasi dari HTML"
          link: "https://products.groupdocs.com/annotation/net/extract/html/"
          description: "Hyper Text Markup Language"

        - name: "Ekstrak Anotasi dari TIFF"
          link: "https://products.groupdocs.com/annotation/net/extract/tiff/"
          description: "Format File Gambar yang Ditandai"

        - name: "Ekstrak Anotasi dari JPEG"
          link: "https://products.groupdocs.com/annotation/net/extract/jpeg/"
          description: "Gambar JPEG"

        - name: "Ekstrak Anotasi dari PNG"
          link: "https://products.groupdocs.com/annotation/net/extract/png/"
          description: "Grafik Jaringan Portabel"

        - name: "Ekstrak Anotasi dari BMP"
          link: "https://products.groupdocs.com/annotation/net/extract/bmp/"
          description: "Format File Bitmap"

        - name: "Ekstrak Anotasi dari EML"
          link: "https://products.groupdocs.com/annotation/net/extract/eml/"
          description: "Pesan email"

        - name: "Ekstrak Anotasi dari MSG"
          link: "https://products.groupdocs.com/annotation/net/extract/msg/"
          description: "Pesan Email Microsoft Outlook"

        - name: "Ekstrak Anotasi dari VSD"
          link: "https://products.groupdocs.com/annotation/net/extract/vsd/"
          description: "Gambar Microsoft Visio 2003-2010"

        - name: "Ekstrak Anotasi dari VSDX"
          link: "https://products.groupdocs.com/annotation/net/extract/vsdx/"
          description: "Gambar Microsoft Visio"

        - name: "Ekstrak Anotasi dari VSS"
          link: "https://products.groupdocs.com/annotation/net/extract/vss/"
          description: "Microsoft Visio 2003-2010 Stensil"

        - name: "Ekstrak Anotasi dari VST"
          link: "https://products.groupdocs.com/annotation/net/extract/vst/"
          description: "Stensil Microsoft Visio 2013"

        - name: "Ekstrak Anotasi dari DWG"
          link: "https://products.groupdocs.com/annotation/net/extract/dwg/"
          description: "Format Data Desain Autodesk"

        - name: "Ekstrak Anotasi dari DXF"
          link: "https://products.groupdocs.com/annotation/net/extract/dxf/"
          description: "Pertukaran Gambar AutoCAD"

        - name: "Ekstrak Anotasi dari DCM"
          link: "https://products.groupdocs.com/annotation/net/extract/dcm/"
          description: "Pencitraan Digital dan Komunikasi dalam Kedokteran"

        - name: "Ekstrak Anotasi dari WMF"
          link: "https://products.groupdocs.com/annotation/net/extract/wmf/"
          description: "Metafile Windows"

        - name: "Ekstrak Anotasi dari EMF"
          link: "https://products.groupdocs.com/annotation/net/extract/emf/"
          description: "Format Metafile yang Ditingkatkan"


back_to_top:
    enable: true
---
