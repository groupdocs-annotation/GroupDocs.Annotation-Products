---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net VSD Chú thích API Chú thích trong C#"
head_description: "Net API để tạo và Chú thích các loại chú thích phổ biến từ VSD, hình ảnh, bản vẽ và định dạng tệp tài liệu."

############################# Header ############################
title: "Chú thích VSD từ Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Tải xuống bản dùng thử miễn phí"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Annotation cho Net API"
    content: |
        GroupDocs.Annotation for Net API là thư viện cho phép bạn thêm chú thích vào PDF, Word và các tài liệu khác trên Mac, Windows hoặc Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) là API Net gốc để quản lý chú thích với sự hỗ trợ toàn diện để tạo, thêm, chỉnh sửa, xóa, trích xuất và xuất chú thích từ hình ảnh và nhiều tài liệu khác. Bạn có thể xem danh sách đầy đủ các định dạng tài liệu được hỗ trợ trên [trang] này(https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Thư viện này cho phép bạn làm việc không chỉ với tài liệu VSD mà còn với nhiều loại tài liệu khác như Word, Excel, PowerPoint, email Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad và nhiều loại khác.
        API GroupDocs.Annotation cho Net cho phép bạn tạo và thêm ghi chú mới, chỉnh sửa chú thích, trích xuất nhận xét, chú thích và xóa chúng khỏi tài liệu. Thư viện hỗ trợ 13 loại chú thích khác nhau, bao gồm Văn bản, Đa tuyến, Vùng, Gạch chân, Điểm, Hình mờ, Mũi tên, Hình elip, Thay thế văn bản, Khoảng cách, Trường văn bản, Biên tập tài nguyên trong tài liệu PDF, HTML, Microsoft Word, bảng tính, sơ đồ, bản trình bày, bản vẽ, hình ảnh và nhiều định dạng tập tin khác.
        Ví dụ (vui lòng xem bên dưới) minh họa cách làm việc với tài liệu VSD, trong ví dụ này, bạn có thể thấy các bước chính về cách làm việc với GroupDocs. Chú thích: Thiết lập giấy phép, mở tài liệu bạn muốn làm việc, tạo một chú thích, thêm các đối tượng dữ liệu để đặt thuộc tính chú thích theo yêu cầu của bạn và lưu kết quả vào nơi cần thiết. Ngoài ra, bạn có thể xem chi tiết hơn về các tính năng được hỗ trợ trên [trang] github của chúng tôi (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) hoặc trong sản phẩm của chúng tôi [tài liệu](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Các bước để thêm chú thích vào VSD trong Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) giúp các nhà phát triển Net dễ dàng thêm nhiều loại chú thích khác nhau vào các tệp VSD trong bất kỳ ứng dụng dựa trên Net nào bằng cách triển khai một vài bước đơn giản.
        *   Tạo các đối tượng Trả lời với nhận xét và ngày tháng.
        *   Tạo đối tượng AreaAnnotation, đặt tùy chọn khu vực và thêm câu trả lời.
        *   Tạo đối tượng Annotator và thêm chú thích khu vực.
        *   Lưu tập tin đầu ra.
    title_right: "yêu cầu hệ thống"
    content_right: |
        GroupDocs.Annotation cho Net API được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực thi mã bên dưới, vui lòng đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.
        *   Hệ điều hành: Microsoft Windows, Linux, MacOS
        *   Môi trường phát triển: Visual Studio, Xamarin, MonoDevelop
        *   Khung: .NET Framework, .NET Standard, .NET Core, Mono
        *   Tải xuống phiên bản mới nhất của GroupDocs.Annotation cho .NET từ [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Xem trước chú thích và mẫu mã
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
    title_left: "Các bước để xóa chú thích khỏi VSD trong Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) giúp các nhà phát triển Net dễ dàng xóa các chi tiết chú thích khỏi các tệp VSD trong bất kỳ ứng dụng dựa trên Net nào bằng cách triển khai một vài bước đơn giản.
        *   Tạo các đối tượng Trả lời với nhận xét và ngày tháng.
        *   Khởi tạo đối tượng SaveOptions và đặt AnnotationTypes = AnnotationType.None.
        *   Gọi phương thức lưu với đường dẫn hoặc luồng tài liệu kết quả và đối tượng SaveOptions.

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
    title_left: "Các bước để chỉnh sửa chú thích từ VSD trong Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) giúp các nhà phát triển Net dễ dàng cập nhật các thuộc tính chú thích khác nhau từ các tệp VSD trong bất kỳ ứng dụng dựa trên Net nào bằng cách triển khai một vài bước đơn giản.
        *   Khởi tạo đối tượng Chú thích với đường dẫn hoặc luồng tài liệu đầu vào với LoadOptions được khởi tạo với ImportAnnotations = true.
        *   Tạo một số triển khai AnnotationBase và đặt Id của chú thích đã tồn tại (nếu không tìm thấy chú thích với Id đó, sẽ không có gì thay đổi) hoặc danh sách đường dẫn của chú thích (tất cả chú thích hiện có sẽ bị xóa).
        *   Gọi phương thức cập nhật của đối tượng Annotator với các chú thích đã truyền.
        *   Gọi phương thức lưu với đường dẫn hoặc luồng tài liệu kết quả và đối tượng SaveOptions.

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
    title_left: "Các bước để trích xuất chú thích từ VSD trong Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) giúp các nhà phát triển Net dễ dàng chú thích tài liệu và trích xuất thông tin chú thích từ các tệp VSD trong bất kỳ ứng dụng dựa trên Net nào bằng cách triển khai một vài bước đơn giản.
        *   Tạo các đối tượng Trả lời với nhận xét và ngày tháng.
        *   Khởi tạo đối tượng LoadOptions và gọi SetImportAnnotations với đối số đúng.
        *   Định nghĩa biến với kiểu List.
        *   Gọi phương thức get và trả về kết quả cho biến trên.

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
    title: "Bản demo trực tiếp để thêm, xóa, chỉnh sửa, trích xuất chú thích vào tài liệu và hình ảnh"
    content: |
        Thêm, xóa, chỉnh sửa và trích xuất chú thích vào tệp VSD ngay bây giờ bằng cách truy cập trang web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Bản demo trực tiếp có những lợi ích sau

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsd"
          title: "Giới thiệu về định dạng tệp VSD"
          content: |
            Các tệp VSD là các bản vẽ được tạo bằng ứng dụng Microsoft Visio để thể hiện nhiều đối tượng đồ họa và sự kết nối giữa các đối tượng này. Các bản vẽ như vậy có thể chứa các đối tượng trực quan như đối tượng trực quan, biểu đồ luồng, sơ đồ UML, luồng thông tin, sơ đồ tổ chức, sơ đồ phần mềm, bố cục mạng, mô hình cơ sở dữ liệu, ánh xạ đối tượng và các thông tin tương tự khác. Microsoft Visio cung cấp khả năng chuyển đổi các tệp Visio sang một số định dạng tệp khác nhau bao gồm PNG, BMP, PDF và các định dạng khác.

          link: "https://docs.fileformat.com/image/vsd/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Làm việc với các định dạng tài liệu phổ biến khác"
    content: |
        Cập nhật thuộc tính chú thích từ một số định dạng tệp phổ biến như được nêu bên dưới.
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