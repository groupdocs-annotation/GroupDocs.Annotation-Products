---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Bersih RTF Anotasi API Anotasi dalam C#"
head_description: "Net API untuk mencipta dan Menganotasi jenis anotasi popular daripada RTF, imej, lukisan dan format fail dokumen."

############################# Header ############################
title: "Anotasi RTF daripada Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Muat turun Percubaan Percuma"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Perihal GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API ialah perpustakaan yang membolehkan anda menambah anotasi pada PDF, Word dan dokumen lain pada Mac, Windows atau Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) ialah API Bersih asli untuk mengurus anotasi dengan sokongan menyeluruh untuk mencipta, menambah, mengedit, memadam, mengekstrak dan mengeksport anotasi daripada imej dan pelbagai dokumen lain. Senarai penuh format dokumen yang disokong yang boleh anda lihat pada [halaman] ini(https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Pustaka ini membolehkan anda bekerja bukan sahaja dengan dokumen RTF tetapi juga dengan banyak jenis dokumen lain seperti Word, Excel, PowerPoint, e-mel Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad dan banyak lagi.
        GroupDocs.Annotation for Net API membolehkan anda membuat dan menambah nota baharu, mengedit anotasi, mengekstrak ulasan, anotasi dan mengalih keluarnya daripada dokumen. Pustaka menyokong 13 jenis anotasi yang berbeza, termasuk Teks, Poligaris, Kawasan, Garis bawah, Titik, Tera Air, Anak panah, Ellipse, Penggantian Teks, Jarak, Medan Teks, Redaksi Sumber dalam PDF, HTML, dokumen Microsoft Word, hamparan, rajah, pembentangan, lukisan, imej dan banyak lagi format fail.
        Contoh (sila lihat di bawah) menunjukkan bekerja dengan dokumen RTF, dalam contoh ini anda boleh melihat langkah utama cara bekerja dengan GroupDocs. Anotasi: Sediakan lesen, buka dokumen yang anda ingin kerjakan, mencipta anotasi, menambah objek data untuk menetapkan sifat anotasi mengikut keperluan anda dan menyimpan hasilnya ke tempat yang diperlukan. Anda juga boleh melihat dengan lebih terperinci tentang ciri yang disokong pada [halaman] github kami (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), atau dalam produk kami [dokumentasi](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Langkah Menambah Anotasi pada RTF dalam Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) memudahkan pembangun Net menambah pelbagai jenis anotasi pada fail RTF dalam mana-mana aplikasi berasaskan Net dengan melaksanakan beberapa langkah mudah.
        *   Cipta objek Balas dengan ulasan dan tarikh.
        *   Buat objek AreaAnnotation, tetapkan pilihan kawasan dan tambah balasan.
        *   Cipta objek Annotator dan tambah anotasi kawasan.
        *   Simpan fail output.
    title_right: "Keperluan Sistem"
    content_right: |
        GroupDocs.Anotasi untuk API Bersih disokong pada semua platform dan sistem pengendalian utama. Sebelum melaksanakan kod di bawah, sila pastikan anda mempunyai prasyarat berikut dipasang pada sistem anda.
        *   Sistem Pengendalian: Microsoft Windows, Linux, MacOS
        *   Persekitaran Pembangunan: Visual Studio, Xamarin, MonoDevelop
        *   Rangka Kerja: Rangka Kerja .NET, Standard .NET, Teras .NET, Mono
        *   Muat turun versi terkini GroupDocs.Annotation untuk .NET daripada [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Pratonton anotasi dan sampel kod
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Add text field annotation to the document from local disk
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
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Langkah-langkah untuk Mengalih keluar Anotasi daripada RTF dalam Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) memudahkan pembangun Net mengalih keluar butiran anotasi daripada fail RTF dalam mana-mana aplikasi berasaskan Net dengan melaksanakan beberapa langkah mudah.
        *   Cipta objek Balas dengan ulasan dan tarikh.
        *   Semerta objek SaveOptions dan tetapkan AnnotationTypes = AnnotationType.None.
        *   Kaedah simpan panggilan dengan laluan atau strim dokumen terhasil dan objek SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```cs
        // 1- How to remove annotation from document using annotation index
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- How to remove annotation from document using annotation object
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- How to remove some annotations from document using list of ID’s
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- How to remove some annotations from document using list of annotations
        
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
    title_left: "Langkah-langkah untuk Mengedit Anotasi daripada RTF dalam Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) memudahkan pembangun Net mengemas kini pelbagai sifat anotasi daripada fail RTF dalam mana-mana aplikasi berasaskan Net dengan melaksanakan beberapa langkah mudah.
        *   Semerta objek Annotator dengan laluan dokumen input atau strim dengan LoadOptions dengan ImportAnnotations = benar.
        *   Cipta beberapa pelaksanaan AnnotationBase dan tetapkan Id bagi anotasi wujud (jika anotasi dengan Id itu tidak ditemui, tiada apa yang akan diubah) atau senarai laluan anotasi (semua anotasi wujud akan dialih keluar).
        *   Kaedah kemas kini panggilan objek Annotator dengan anotasi yang diluluskan.
        *   Kaedah simpan panggilan dengan laluan atau strim dokumen terhasil dan objek SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```cs
        // open annotated document
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //assuming we are going to change some properties of existing annotation
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // It's important to set existed annotation Id
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
                // update annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Langkah-langkah untuk Mengeluarkan Anotasi daripada RTF dalam Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) memudahkan pembangun Net untuk menganotasi dokumen dan mengekstrak maklumat anotasi daripada fail RTF dalam mana-mana aplikasi berasaskan Net dengan melaksanakan beberapa langkah mudah.
        *   Cipta objek Balas dengan ulasan dan tarikh.
        *   Segerakan objek LoadOptions dan panggil SetImportAnnotations dengan hujah yang benar.
        *   Tentukan pembolehubah dengan jenis Senarai.
        *   Panggil kaedah dapatkan dan kembalikan hasil kepada pembolehubah di atas.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```cs
        // for using this example input file ("annotated.bmp") must be with annotations
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
    title: "Demo Langsung untuk Tambah, Alih Keluar, Edit, Ekstrak Anotasi pada Dokumen dan Imej"
    content: |
        Tambahkan, alih keluar, edit dan ekstrak anotasi pada fail RTF sekarang dengan melawati tapak web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Demo langsung mempunyai faedah berikut

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-rtf"
          title: "Mengenai Format Fail RTF."
          content: |
            Diperkenalkan dan didokumenkan oleh Microsoft, Format Teks Kaya (RTF) mewakili kaedah pengekodan teks dan grafik berformat untuk digunakan dalam aplikasi. Format ini memudahkan pertukaran dokumen merentas platform dengan Produk Microsoft yang lain, dengan itu memenuhi tujuan kesalingoperasian. Keupayaan ini menjadikannya standard pemindahan data antara perisian pemprosesan perkataan dan, oleh itu, kandungan boleh dipindahkan dari satu sistem pengendalian ke sistem pengendalian yang lain tanpa kehilangan pemformatan dokumen. Spesifikasi format fail tersedia oleh Microsoft untuk muat turun awam dan boleh dirujuk dari perspektif pembangun.

          link: "https://docs.fileformat.com/image/rtf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Bekerja dengan Format Dokumen Popular Lain"
    content: |
        Kemas kini sifat anotasi daripada beberapa format fail popular seperti yang dinyatakan di bawah.
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