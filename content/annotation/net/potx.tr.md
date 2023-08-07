---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net POTX Ek Açıklama API'si C#'ta Ek Açıklama"
head_description: "POTX, resimler, çizimler ve belge dosyası biçimlerinden popüler ek açıklama türleri oluşturmak ve Ek Açıklama eklemek için Net API."

############################# Header ############################
title: "Net'ten POTX not ekleyin"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ücretsiz deneme sürümünü indirin"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "GroupDocs.Annotation for Net API hakkında"
    content: |
        GroupDocs.Annotation for Net API, PDF, Word ve Mac, Windows veya Ubuntu'daki diğer belgelere ek açıklamalar eklemenizi sağlayan bir kitaplıktır. [GroupDocs.Annotation for Net](/annotation/net), resimlerden ve diğer çeşitli belgelerden açıklama oluşturma, ekleme, düzenleme, silme, ayıklama ve dışa aktarma için kapsamlı destekle açıklamaları yönetmeye yönelik yerel bir Net API'sidir. Bu [sayfada](https://docs.groupdocs.com/annotation/net/supported-document-formats/) görebileceğiniz desteklenen belge biçimlerinin tam listesi.
        Bu kitaplık, yalnızca POTX belgesiyle değil, Word, Excel, PowerPoint, Outlook e-postaları, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad ve diğerleri gibi diğer birçok belge türüyle çalışmanıza olanak tanır.
        GroupDocs.Annotation for Net API, yeni notlar oluşturmanıza ve eklemenize, açıklamaları düzenlemenize, yorumları, ek açıklamaları ayıklamanıza ve bunları belgelerden kaldırmanıza olanak tanır. Kitaplık, Metin, Çoklu Çizgi, Alan, Altı Çizili, Nokta, Filigran, Ok, Elips, Metin Değiştirme, Mesafe, Metin Alanı, PDF'de Kaynak Redaksiyonu, HTML, Microsoft Word belgeleri, elektronik tablolar, diyagramlar, sunumlar dahil olmak üzere 13 farklı açıklama türünü destekler. çizimler, resimler ve diğer birçok dosya formatı.
        Örnek (lütfen aşağıya bakın) POTX belgesiyle çalışmayı gösterir, bu örnekte GroupDocs ile çalışmanın ana adımlarını görebilirsiniz. Ek Açıklama: Bir lisans ayarlayın, çalışmak istediğiniz bir belgeyi açın, bir ek açıklama, açıklama özelliklerini ihtiyaçlarınıza göre ayarlamak için veri nesneleri ekleme ve sonucu gereken yere kaydetme. Ayrıca github [sayfa](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) veya ürün [documentation](https) sayfamızda desteklenen özellikler hakkında daha ayrıntılı bir göz atabilirsiniz. ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Net'te POTX Dosyasına Ek Açıklama Ekleme Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net geliştiricilerinin, birkaç basit adımı uygulayarak herhangi bir Net tabanlı uygulama içindeki POTX dosyalarına çeşitli ek açıklama türleri eklemesini kolaylaştırır.
        *   Yorum ve tarih içeren Yanıt nesneleri oluşturun.
        *   AreaAnnotation nesnesi oluşturun, alan seçeneklerini ayarlayın ve yanıtlar ekleyin.
        *   Annotator nesnesi oluşturun ve alan açıklaması ekleyin.
        *   Çıktı dosyasını kaydedin.
    title_right: "sistem gereksinimleri"
    content_right: |
        Net API'leri için GroupDocs.Annotation, tüm büyük platformlarda ve işletim sistemlerinde desteklenir. Aşağıdaki kodu çalıştırmadan önce lütfen sisteminizde aşağıdaki önkoşulların yüklü olduğundan emin olun.
        *   İşletim Sistemleri: Microsoft Windows, Linux, MacOS
        *   Geliştirme Ortamları: Visual Studio, Xamarin, MonoDevelop
        *   Çerçeveler: .NET Framework, .NET Standard, .NET Core, Mono
        *   GroupDocs.Annotation for .NET'in en son sürümünü [NuGet](https://www.nuget.org/packages/groupdocs.annotation) adresinden indirin.

############################# Preview ############################
preview_Add:
    enable: true
    title: Ek açıklama önizlemesi ve kod örneği
    content: |
        ![Annotation preview image]https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png
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
    title_left: "Net'teki POTX Ek Açıklamalarını Kaldırma Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net geliştiricilerinin, birkaç basit adımı uygulayarak herhangi bir Net tabanlı uygulama içindeki POTX dosyalarından ek açıklama ayrıntılarını kaldırmasını kolaylaştırır.
        *   Yorum ve tarih içeren Yanıt nesneleri oluşturun.
        *   SaveOptions nesnesini oluşturun ve AnnotationTypes = AnnotationType.None olarak ayarlayın.
        *   Ortaya çıkan belge yolu veya akışı ve SaveOptions nesnesi ile kaydetme yöntemini çağırın.

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
    title_left: "Net'te POTX Ek Açıklamalarını Düzenleme Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net geliştiricilerinin, birkaç kolay adımı uygulayarak herhangi bir Net tabanlı uygulama içindeki POTX dosyalarından çeşitli ek açıklama özelliklerini güncellemelerini kolaylaştırır.
        *   ImportAnnotations = true ile örneklenmiş LoadOptions ile giriş belgesi yolu veya akış ile Annotator nesnesini örnekleyin.
        *   Bazı AnnotationBase uygulamaları oluşturun ve varolan ek açıklamanın kimliğini ayarlayın (bu kimliğe sahip ek açıklama bulunmazsa, hiçbir şey değiştirilmeyecektir) veya ek açıklamaların yol listesi (mevcut tüm ek açıklamalar kaldırılacaktır).
        *   Geçirilen ek açıklamalarla Annotator nesnesinin güncelleme yöntemini çağırın.
        *   Ortaya çıkan belge yolu veya akışı ve SaveOptions nesnesi ile kaydetme yöntemini çağırın.

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
    title_left: "Net'teki POTX Dosyasından Ek Açıklamaları Çıkarma Adımları"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net geliştiricilerinin belgelere açıklama eklemesini ve birkaç kolay adımı uygulayarak herhangi bir Net tabanlı uygulama içindeki POTX dosyalarından açıklama bilgilerini çıkarmasını kolaylaştırır.
        *   Yorum ve tarih içeren Yanıt nesneleri oluşturun.
        *   LoadOptions nesnesini oluşturun ve SetImportAnnotations'ı gerçek bağımsız değişkenle çağırın.
        *   List tipinde değişken tanımlayın.
        *   Get yöntemini çağırın ve sonucu yukarıdaki değişkene döndürün.

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
    title: "Belgelere ve Görüntülere Ek Açıklamalar Eklemek, Kaldırmak, Düzenlemek, Çıkarmak için Canlı Demolar"
    content: |
        Hemen şimdi [GroupDocs.Annotation Canlı Demolar](https://products.groupdocs.app/annotation/family) web sitesini ziyaret ederek POTX dosyasına ek açıklama ekleyin, kaldırın, düzenleyin ve çıkarın. Canlı demo aşağıdaki avantajlara sahiptir

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-potx"
          title: "POTX Dosya Biçimi Hakkında"
          content: |
            .POTX uzantılı dosyalar, Microsoft PowerPoint 2007 ve üzeri ile oluşturulan Microsoft PowerPoint şablon sunumlarını temsil eder. Bu biçim, ikili dosya biçimini temel alan ve PowerPoint 97-2003 tarafından desteklenen POT dosya biçimini değiştirmek için oluşturulmuştur. Oluşturulan dosyalar, aynı düzene ve yeni dosyalara uygulanması gereken diğer ayarlara sahip sunumlar oluşturmak için kullanılabilir. Bu ayarlar stilleri, arka planları, renk paletini, yazı tiplerini ve varsayılanları içerebilir. Bu tür dosyalar, resmi kullanım için kullanıma hazır şablon dosyaları oluşturmak için oluşturulur.

          link: "https://docs.fileformat.com/image/potx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Diğer Popüler Belge Biçimleriyle Çalışma"
    content: |
        Bazı popüler dosya biçimlerinden ek açıklama özelliklerini aşağıda belirtildiği gibi güncelleyin.
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