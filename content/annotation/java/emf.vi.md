---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API chú thích Java EMF Chú thích trong C#"
head_description: "API Java để tạo và Chú thích các loại chú thích phổ biến từ EMF, hình ảnh, bản vẽ và định dạng tệp tài liệu."

############################# Header ############################
title: "Chú thích EMF từ Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Tải xuống bản dùng thử miễn phí"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Annotation cho Java API"
    content: |
        GroupDocs.Annotation for Java API là thư viện cho phép bạn thêm chú thích vào PDF, Word và các tài liệu khác trên Mac, Windows hoặc Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) là API Java gốc để quản lý chú thích với sự hỗ trợ toàn diện để tạo, thêm, chỉnh sửa, xóa, trích xuất và xuất chú thích từ hình ảnh và nhiều tài liệu khác. Bạn có thể xem danh sách đầy đủ các định dạng tài liệu được hỗ trợ trên [trang] này(https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Thư viện này cho phép bạn làm việc không chỉ với tài liệu EMF mà còn với nhiều loại tài liệu khác như Word, Excel, PowerPoint, email Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad và nhiều loại khác.
        API GroupDocs.Annotation cho Java cho phép bạn tạo và thêm ghi chú mới, chỉnh sửa chú thích, trích xuất nhận xét, chú thích và xóa chúng khỏi tài liệu. Thư viện hỗ trợ 13 loại chú thích khác nhau, bao gồm Văn bản, Đa tuyến, Vùng, Gạch chân, Điểm, Hình mờ, Mũi tên, Hình elip, Thay thế văn bản, Khoảng cách, Trường văn bản, Biên tập tài nguyên trong tài liệu PDF, HTML, Microsoft Word, bảng tính, sơ đồ, bản trình bày, bản vẽ, hình ảnh và nhiều định dạng tập tin khác.
        Ví dụ (vui lòng xem bên dưới) minh họa cách làm việc với tài liệu EMF, trong ví dụ này, bạn có thể thấy các bước chính về cách làm việc với GroupDocs. Chú thích: Thiết lập giấy phép, mở tài liệu bạn muốn làm việc, tạo một chú thích, thêm các đối tượng dữ liệu để đặt thuộc tính chú thích theo yêu cầu của bạn và lưu kết quả vào nơi cần thiết. Ngoài ra, bạn có thể xem chi tiết hơn về các tính năng được hỗ trợ trên [trang github của chúng tôi](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) hoặc trong sản phẩm của chúng tôi [tài liệu](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Các bước để thêm chú thích vào EMF trong Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) giúp các nhà phát triển Java dễ dàng thêm các loại chú thích khác nhau vào các tệp EMF trong bất kỳ ứng dụng dựa trên Java nào bằng cách triển khai một vài bước đơn giản.
        *   Tạo các đối tượng Trả lời với nhận xét và ngày tháng.
        *   Tạo đối tượng AreaAnnotation, đặt tùy chọn khu vực và thêm câu trả lời.
        *   Tạo đối tượng Annotator và thêm chú thích khu vực.
        *   Lưu tập tin đầu ra.
    title_right: "yêu cầu hệ thống"
    content_right: |
        API GroupDocs.Annotation cho Java được hỗ trợ trên tất cả các nền tảng và hệ điều hành chính. Trước khi thực thi mã bên dưới, vui lòng đảm bảo rằng bạn đã cài đặt các điều kiện tiên quyết sau trên hệ thống của mình.
        *   Hệ điều hành: Microsoft Windows, Linux, MacOS
        *   Môi trường phát triển: NetBeans, Intellij IDEA, Eclipse, v.v.
        *   Môi trường thời gian chạy Java: Java 7 (1.7) trở lên
        *   Tải phiên bản mới nhất của GroupDocs.Annotation cho Java từ [Kho lưu trữ tạo phẩm của GroupDocs](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Xem trước chú thích và mẫu mã
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Create an instance of Reply class and add comments
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Create an instance of AreaAnnotation class and set options
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
        
        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Add annotation
        annotator.add(area);
        
        // Save to file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Các bước để xóa chú thích khỏi EMF trong Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) giúp các nhà phát triển Java dễ dàng xóa các chi tiết chú thích khỏi các tệp EMF trong bất kỳ ứng dụng dựa trên Java nào bằng cách triển khai một vài bước đơn giản.
        *   Tạo các đối tượng Trả lời với nhận xét và ngày tháng.
        *   Khởi tạo đối tượng SaveOptions và đặt AnnotationTypes = AnnotationType.None.
        *   Gọi phương thức lưu với đường dẫn hoặc luồng tài liệu kết quả và đối tượng SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```java
        // Create an instance of Annotator class 
        Annotator annotator = new Annotator("C://input.bmp");

        // Remove annotation by set type None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Save annotation to output file
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Các bước để chỉnh sửa chú thích từ EMF trong Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) giúp các nhà phát triển Java dễ dàng cập nhật các thuộc tính chú thích khác nhau từ các tệp EMF trong bất kỳ ứng dụng dựa trên Java nào bằng cách triển khai một vài bước đơn giản.
        *   Khởi tạo đối tượng Chú thích với đường dẫn hoặc luồng tài liệu đầu vào với LoadOptions được khởi tạo với ImportAnnotations = true.
        *   Tạo một số triển khai AnnotationBase và đặt Id của chú thích đã tồn tại (nếu không tìm thấy chú thích với Id đó, sẽ không có gì thay đổi) hoặc danh sách đường dẫn của chú thích (tất cả chú thích hiện có sẽ bị xóa).
        *   Gọi phương thức cập nhật của đối tượng Annotator với các chú thích đã truyền.
        *   Gọi phương thức lưu với đường dẫn hoặc luồng tài liệu kết quả và đối tượng SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Create an instance of Reply class for first example and add comments
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Create an instance of Reply class for update first example
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Update and save annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Các bước để trích xuất chú thích từ EMF trong Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) giúp các nhà phát triển Java dễ dàng chú thích tài liệu và trích xuất thông tin chú thích từ các tệp EMF trong bất kỳ ứng dụng dựa trên Java nào bằng cách triển khai một vài bước đơn giản.
        *   Tạo các đối tượng Trả lời với nhận xét và ngày tháng.
        *   Khởi tạo đối tượng LoadOptions và gọi SetImportAnnotations với đối số đúng.
        *   Định nghĩa biến với kiểu List.
        *   Gọi phương thức get và trả về kết quả cho biến trên.

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```java
        // For using this example input file ("annotated.bmp") must be with annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Create an instance of Annotator class and get annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Bản demo trực tiếp để thêm, xóa, chỉnh sửa, trích xuất chú thích vào tài liệu và hình ảnh"
    content: |
        Thêm, xóa, chỉnh sửa và trích xuất chú thích vào tệp EMF ngay bây giờ bằng cách truy cập trang web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Bản demo trực tiếp có những lợi ích sau

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-emf"
          title: "Giới thiệu về định dạng tệp EMF"
          content: |
            Định dạng siêu tệp nâng cao (EMF) lưu trữ hình ảnh đồ họa độc lập với thiết bị. Siêu tệp của EMF bao gồm các bản ghi có độ dài thay đổi theo thứ tự thời gian có thể hiển thị hình ảnh được lưu trữ sau khi phân tích cú pháp trên bất kỳ thiết bị đầu ra nào. Các bản ghi có độ dài thay đổi này có thể là định nghĩa của các đối tượng kèm theo, các lệnh để vẽ và các thuộc tính đồ họa quan trọng để hiển thị hình ảnh một cách chính xác. Khi một thiết bị mở siêu tệp EMF bằng môi trường đồ họa của chính nó, tỷ lệ, kích thước, màu sắc và các thuộc tính đồ họa khác của hình ảnh gốc vẫn giữ nguyên bất kể nền tảng thiết bị mở là gì.

          link: "https://docs.fileformat.com/image/emf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Làm việc với các định dạng tài liệu phổ biến khác"
    content: |
        Cập nhật thuộc tính chú thích từ một số định dạng tệp phổ biến như được nêu bên dưới.
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/java/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/java/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/java/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/java/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/java/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/java/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/java/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/java/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/java/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/java/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/java/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/java/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/java/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/java/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/java/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/java/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/java/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/java/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/java/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/java/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/java/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/java/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/java/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/java/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/java/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/java/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/java/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/java/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/java/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/java/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/java/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/java/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/java/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/java/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/java/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---