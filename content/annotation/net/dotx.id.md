
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/dotx"/>

############################# Head ############################
head_title: "Net DOTX Anotasi API Anotasi dalam C#"
head_description: "Net API untuk membuat dan Menganotasi jenis anotasi populer dari DOTX, gambar, gambar, dan format file dokumen."

############################# Header ############################
title: "Beri anotasi DOTX dari Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Anotasi untuk Net"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Annotation untuk Net API"
    content: |
        GroupDocs.Annotation for Net API adalah pustaka yang memungkinkan Anda menambahkan anotasi ke PDF, Word, dan dokumen lain di Mac, Windows, atau Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) adalah API asli Net untuk mengelola anotasi dengan dukungan komprehensif untuk membuat, menambahkan, mengedit, menghapus, mengekstrak, dan mengekspor anotasi dari gambar dan berbagai dokumen lainnya. Daftar lengkap format dokumen yang didukung dapat Anda lihat di [halaman](https://docs.groupdocs.com/annotation/net/supported-document-formats/) ini.

        Pustaka ini memungkinkan Anda bekerja tidak hanya dengan dokumen DOTX tetapi juga dengan banyak jenis dokumen lainnya seperti Word, Excel, PowerPoint, email Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad, dan banyak lainnya.

        GroupDocs.Annotation untuk Net API memungkinkan Anda membuat dan menambahkan catatan baru, mengedit anotasi, mengekstrak komentar, anotasi, dan menghapusnya dari dokumen. Perpustakaan mendukung 13 jenis anotasi yang berbeda, termasuk Teks, Polyline, Area, Garis Bawah, Titik, Tanda Air, Panah, Ellipse, Penggantian Teks, Jarak, Bidang Teks, Redaksi Sumber Daya dalam PDF, HTML, dokumen Microsoft Word, spreadsheet, diagram, presentasi, gambar, gambar dan banyak format file lainnya.

        Contoh (silakan lihat di bawah) mendemonstrasikan bekerja dengan dokumen DOTX, dalam contoh ini Anda dapat melihat langkah-langkah utama tentang cara bekerja dengan GroupDocs. Anotasi: Menyiapkan lisensi, membuka dokumen yang ingin Anda kerjakan, membuat anotasi, menambahkan objek data untuk mengatur properti anotasi sesuai dengan kebutuhan Anda dan menyimpan hasilnya ke tempat yang diperlukan. Anda juga dapat melihat lebih detail tentang fitur yang didukung di [halaman] github kami (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), atau di [dokumentasi produk kami ](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Langkah-langkah untuk Menambahkan Anotasi dari DOTX di Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Net untuk menambahkan berbagai jenis anotasi ke file DOTX dalam aplikasi berbasis Net apa pun dengan menerapkan beberapa langkah mudah.
        * Buat objek Balas dengan komentar dan tanggal.
        * Buat objek AreaAnnotation, atur opsi area dan tambahkan balasan.
        * Buat objek Annotator dan tambahkan anotasi area.
        * Simpan file keluaran.
    title_right: "Persyaratan sistem"
    content_right: |
        GroupDocs.Annotation untuk Net API didukung di semua platform dan sistem operasi utama. Sebelum menjalankan kode di bawah ini, harap pastikan bahwa Anda telah menginstal prasyarat berikut di sistem Anda.
        * Sistem Operasi: Microsoft Windows, Linux, MacOS
        * Lingkungan Pengembangan: Visual Studio, Xamarin, MonoDevelop
        * Kerangka: .NET Framework, .NET Standard, .NET Core, Mono
        * Unduh versi terbaru GroupDocs.Annotation untuk .NET dari [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: "Pratinjau anotasi dan contoh kode"
    content: |
        ![Gambar pratinjau anotasi](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ``` cs
        //Tambahkan anotasi bidang teks ke dokumen dari disk lokal
        using (Annotator annotator = new Annotator("input.bmp"))
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "Ini adalah anotasi bidang teks",
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
                        Comment = "Komentar pertama",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Komentar kedua",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Langkah-langkah untuk Menghapus Anotasi dari DOTX di Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) mempermudah pengembang Net untuk menghapus detail anotasi dari file DOTX dalam aplikasi berbasis Net apa pun dengan menerapkan beberapa langkah mudah.
        * Buat objek Balas dengan komentar dan tanggal.
        * Instansiasi objek SaveOptions dan atur AnnotationTypes = AnnotationType.None.
        * Panggil metode penyimpanan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ``` cs
        // 1- Cara menghapus anotasi dari dokumen menggunakan indeks anotasi
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- Cara menghapus anotasi dari dokumen menggunakan objek anotasi
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- Cara menghapus beberapa anotasi dari dokumen menggunakan daftar ID
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- Cara menghapus beberapa anotasi dari dokumen menggunakan daftar anotasi
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp);
            annotator.Save("removed.bmp");
        }
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Langkah-langkah untuk Mengedit Anotasi dari DOTX di Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) mempermudah pengembang Net untuk memperbarui berbagai properti anotasi dari file DOTX dalam aplikasi berbasis Net apa pun dengan menerapkan beberapa langkah mudah.
        * Instansiasi objek Annotator dengan jalur atau aliran dokumen masukan dengan LoadOptions yang dibuat dengan ImportAnnotations = true.
        * Buat beberapa implementasi AnnotationBase dan tetapkan Id dari anotasi yang ada (jika anotasi dengan Id tersebut tidak ditemukan, tidak ada yang akan diubah) atau daftar jalur anotasi (semua anotasi yang ada akan dihapus).
        * Panggil metode pembaruan objek Annotator dengan anotasi yang diteruskan.
        * Panggil metode penyimpanan dengan jalur atau aliran dokumen yang dihasilkan dan objek SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ``` cs
        // buka dokumen beranotasi
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //dengan asumsi kita akan mengubah beberapa properti dari anotasi yang ada
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // Penting untuk menyetel ID anotasi yang ada
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Pesan = "Ini adalah anotasi yang diperbarui",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment "Komentar pertama diperbarui",
                                    Dibalas = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Komentar kedua diperbarui",
                                    Dibalas = DateTime.Now
                                }
                            }
                        };
                // perbarui anotasi
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Langkah-langkah untuk Mengekstrak Anotasi dari DOTX di Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) memudahkan pengembang Net untuk menganotasi dokumen dan mengekstrak informasi anotasi dari file DOTX dalam aplikasi berbasis Net apa pun dengan menerapkan beberapa langkah mudah.
        * Buat objek Balas dengan komentar dan tanggal.
        * Instansiasi objek LoadOptions dan panggil SetImportAnnotations dengan argumen yang benar.
        * Tentukan variabel dengan jenis Daftar.
        * Panggil metode dapatkan dan kembalikan hasilnya ke variabel di atas.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ``` cs
        // untuk menggunakan file input contoh ini ("annotated.bmp") harus dengan anotasi
        using (Annotator annotator = new Annotator("annotated.bmp"))
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

############################# Demos ############################
demos:
    enable: true
    title: "Demo Langsung untuk Menambah, Menghapus, Mengedit, Mengekstrak Anotasi ke Dokumen dan Gambar"
    content: |
        Tambahkan, hapus, edit, dan ekstrak anotasi ke file DOTX sekarang juga dengan mengunjungi situs web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        Demo langsung memiliki manfaat berikut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dotx"
          title: "Tentang DOTX Format Berkas"
          content: |
            File dengan ekstensi DOTX adalah file template yang dibuat oleh Microsoft Word untuk memiliki pengaturan pra-format untuk pembuatan file DOCX lebih lanjut. File template dibuat untuk memiliki pengaturan pengguna khusus yang harus diterapkan ke lalat berikutnya yang dibuat dari ini. Pengaturan ini mencakup margin halaman, batas, header, footer, dan pengaturan halaman lainnya. Templat semacam itu digunakan dalam dokumen resmi seperti kop surat perusahaan dan formulir standar. Format file DOTX diperkenalkan dengan rilis Microsoft Office 2007 untuk menggantikan format file DOT biner, tetapi juga didukung oleh versi yang lebih tinggi. Microsoft Word secara default membuka setiap dokumen baru berdasarkan file normal.dot. Jika dimodifikasi, semua file baru yang dibuat akan menghasilkan pengaturan yang sama seperti dari file template. Di Microsoft Word 2007, format file DOT telah diganti dengan format file DOTX berbasis Office OpenXML.
          link: "https://docs.fileformat.com/image/dotx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bekerja dengan Format Dokumen Populer Lainnya"
    content: |
        Perbarui properti anotasi dari beberapa format file populer seperti yang dinyatakan di bawah ini.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/net/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/net/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/net/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/net/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/net/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/net/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/net/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/net/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/net/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/net/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/net/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/net/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/net/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/net/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/net/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/net/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/net/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/net/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/net/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/net/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/net/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/net/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/net/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/net/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/net/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/net/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/net/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/net/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/net/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/net/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/net/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/net/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/net/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/net/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/net/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---