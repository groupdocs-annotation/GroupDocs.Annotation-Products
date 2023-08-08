---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java OTP Annotation API ใส่คำอธิบายประกอบใน C#"
head_description: "Java API เพื่อสร้างและอธิบายประเภทคำอธิบายประกอบยอดนิยมจาก OTP รูปภาพ ภาพวาด และรูปแบบไฟล์เอกสาร"

############################# Header ############################
title: "ใส่คำอธิบายประกอบ OTP จาก Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "ดาวน์โหลดรุ่นทดลองใช้ฟรี"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับ GroupDocs.Annotation สำหรับ Java API"
    content: |
        GroupDocs.Annotation สำหรับ Java API เป็นไลบรารีที่ให้คุณเพิ่มคำอธิบายประกอบลงใน PDF, Word และเอกสารอื่นๆ บน Mac, Windows หรือ Ubuntu [GroupDocs.Annotation for Java](/annotation/java) เป็น Java API แบบเนทีฟสำหรับจัดการคำอธิบายประกอบด้วยการสนับสนุนที่ครอบคลุมสำหรับการสร้าง การเพิ่ม การแก้ไข การลบ การแยก และการส่งออกคำอธิบายประกอบจากรูปภาพและเอกสารอื่นๆ มากมาย รายการรูปแบบเอกสารที่รองรับทั้งหมดที่คุณสามารถดูได้ใน[หน้า](https://docs.groupdocs.com/annotation/java/supported-document-formats/)
        ไลบรารีนี้ช่วยให้คุณทำงานได้ไม่เฉพาะกับเอกสาร OTP เท่านั้น แต่ยังใช้กับเอกสารประเภทอื่นๆ ได้อีกมากมาย เช่น Word, Excel, PowerPoint, อีเมล Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad และอื่นๆ อีกมากมาย
        GroupDocs.Annotation สำหรับ Java API ช่วยให้คุณสร้างและเพิ่มบันทึกย่อใหม่ แก้ไขบันทึกย่อ แยกความคิดเห็น บันทึกย่อ และลบออกจากเอกสาร ไลบรารีรองรับคำอธิบายประกอบที่แตกต่างกัน 13 ประเภท ได้แก่ ข้อความ โพลีไลน์ พื้นที่ ขีดเส้นใต้ จุด ลายน้ำ ลูกศร วงรี การแทนที่ข้อความ ระยะทาง ช่องข้อความ การแก้ไขทรัพยากรในรูปแบบ PDF, HTML, เอกสาร Microsoft Word, สเปรดชีต, ไดอะแกรม, งานนำเสนอ, ภาพวาด รูปภาพ และรูปแบบไฟล์อื่นๆ อีกมากมาย
        ตัวอย่าง (โปรดดูด้านล่าง) สาธิตการทำงานกับเอกสาร OTP ในตัวอย่างนี้ คุณสามารถดูขั้นตอนหลักของวิธีการทำงานกับ GroupDocs คำอธิบายประกอบ: ตั้งค่าใบอนุญาต เปิดเอกสารที่คุณต้องการใช้งาน การสร้าง คำอธิบายประกอบ เพิ่มวัตถุข้อมูลเพื่อตั้งค่าคุณสมบัติคำอธิบายประกอบตามความต้องการของคุณ และบันทึกผลลัพธ์ไปยังตำแหน่งที่ต้องการ นอกจากนี้ คุณยังสามารถดูรายละเอียดเพิ่มเติมเกี่ยวกับคุณสมบัติที่รองรับบน Github [หน้า](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) หรือในผลิตภัณฑ์ของเรา [เอกสาร](https://docs.groupdocs.com/annotation/java/getting-started/)

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "ขั้นตอนในการเพิ่มคำอธิบายประกอบใน OTP ใน Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ทำให้นักพัฒนา Java สามารถเพิ่มประเภทคำอธิบายประกอบต่างๆ ลงในไฟล์ OTP ได้อย่างง่ายดายภายในแอปพลิเคชันที่ใช้ Java โดยดำเนินการตามขั้นตอนง่ายๆ ไม่กี่ขั้นตอน
        *   สร้างวัตถุตอบกลับพร้อมความคิดเห็นและวันที่
        *   สร้างวัตถุ AreaAnnotation ตั้งค่าตัวเลือกพื้นที่ และเพิ่มการตอบกลับ
        *   สร้างวัตถุ Annotator และเพิ่มคำอธิบายประกอบพื้นที่
        *   บันทึกไฟล์เอาต์พุต
    title_right: "ความต้องการของระบบ"
    content_right: |
        GroupDocs คำอธิบายประกอบสำหรับ Java API ได้รับการสนับสนุนบนแพลตฟอร์มและระบบปฏิบัติการหลักทั้งหมด ก่อนดำเนินการโค้ดด้านล่าง โปรดตรวจสอบว่าคุณได้ติดตั้งข้อกำหนดเบื้องต้นต่อไปนี้ในระบบของคุณแล้ว
        *   ระบบปฏิบัติการ: Microsoft Windows, Linux, MacOS
        *   สภาพแวดล้อมการพัฒนา: NetBeans, Intellij IDEA, Eclipse เป็นต้น
        *   Java Runtime Environment: Java 7 (1.7) ขึ้นไป
        *   รับ GroupDocs.Annotation เวอร์ชันล่าสุดสำหรับ Java จาก [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: ตัวอย่างคำอธิบายประกอบและตัวอย่างโค้ด
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
    title_left: "ขั้นตอนในการลบคำอธิบายประกอบจาก OTP ใน Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ช่วยให้นักพัฒนา Java ลบรายละเอียดคำอธิบายประกอบออกจากไฟล์ OTP ภายในแอปพลิเคชันที่ใช้ Java ได้ง่ายขึ้น โดยใช้ขั้นตอนง่ายๆ ไม่กี่ขั้นตอน
        *   สร้างวัตถุตอบกลับพร้อมความคิดเห็นและวันที่
        *   ยกตัวอย่างวัตถุ SaveOptions และตั้งค่า AnnotationTypes = AnnotationType.None
        *   วิธีการบันทึกการโทรพร้อมเส้นทางเอกสารผลลัพธ์หรือสตรีมและวัตถุ SaveOptions

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
    title_left: "ขั้นตอนในการแก้ไขคำอธิบายประกอบจาก OTP ใน Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ช่วยให้นักพัฒนา Java อัปเดตคุณสมบัติคำอธิบายประกอบต่างๆ จากไฟล์ OTP ได้ง่ายขึ้นภายในแอปพลิเคชันที่ใช้ Java โดยดำเนินการตามขั้นตอนง่ายๆ ไม่กี่ขั้นตอน
        *   ยกตัวอย่างวัตถุ Annotator ด้วยเส้นทางเอกสารอินพุตหรือสตรีมด้วย LoadOptions ที่สร้างอินสแตนซ์ด้วย ImportAnnotations = จริง
        *   สร้างการใช้งาน AnnotationBase และตั้งค่า Id ของคำอธิบายประกอบที่มีอยู่ (หากไม่พบคำอธิบายประกอบที่มีรหัสนั้น จะไม่มีอะไรเปลี่ยนแปลง) หรือรายการพาธของคำอธิบายประกอบ (คำอธิบายประกอบที่มีอยู่ทั้งหมดจะถูกลบออก)
        *   เรียกใช้เมธอดการอัปเดตของออบเจกต์ Annotator พร้อมคำอธิบายประกอบที่ส่งผ่าน
        *   วิธีการบันทึกการโทรพร้อมเส้นทางเอกสารผลลัพธ์หรือสตรีมและวัตถุ SaveOptions

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
    title_left: "ขั้นตอนในการแยกคำอธิบายประกอบจาก OTP ใน Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) ทำให้นักพัฒนา Java สามารถใส่คำอธิบายประกอบเอกสารและดึงข้อมูลคำอธิบายประกอบจากไฟล์ OTP ได้อย่างง่ายดายภายในแอปพลิเคชันที่ใช้ Java โดยใช้ขั้นตอนง่ายๆ ไม่กี่ขั้นตอน
        *   สร้างวัตถุตอบกลับพร้อมความคิดเห็นและวันที่
        *   ยกตัวอย่างวัตถุ LoadOptions และเรียก SetImportAnnotations ด้วยอาร์กิวเมนต์จริง
        *   กำหนดตัวแปรด้วยประเภท List
        *   เรียกใช้เมธอด get และส่งคืนผลลัพธ์ไปยังตัวแปรด้านบน

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
    title: "การสาธิตสดเพื่อเพิ่ม ลบ แก้ไข แยกคำอธิบายประกอบในเอกสารและรูปภาพ"
    content: |
        เพิ่ม ลบ แก้ไข และแยกคำอธิบายประกอบลงในไฟล์ OTP ทันทีโดยไปที่เว็บไซต์ [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) การสาธิตสดมีประโยชน์ดังต่อไปนี้

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-otp"
          title: "เกี่ยวกับรูปแบบไฟล์ OTP"
          content: |
            ไฟล์ที่มีนามสกุล .OTP แสดงถึงไฟล์เทมเพลตการนำเสนอที่สร้างโดยแอปพลิเคชันในรูปแบบมาตรฐาน OASIS OpenDocument เนื้อหาของไฟล์ดังกล่าวประกอบด้วยข้อมูลการนำเสนอในรูปแบบของสไลด์ที่มีข้อความ รูปภาพ รูปร่าง เนื้อหามัลติมีเดีย เอฟเฟกต์การเปลี่ยนภาพ และองค์ประกอบสไลด์อื่นๆ ไฟล์เทมเพลตเหล่านี้ใช้สำหรับสร้างงานนำเสนอใหม่อย่างรวดเร็วตามข้อมูลการจัดรูปแบบที่จัดเก็บไว้ในเทมเพลต ไฟล์ OTP สามารถสร้างและบันทึกได้ด้วยแอพพลิเคชั่นต่างๆ เช่น Impress ที่มาพร้อมกับชุด OpenOffice และ Microsoft PowerPoint รูปแบบไฟล์ OTP คล้ายกับไฟล์เทมเพลต Microsoft PowerPoint .POT และ .POTX

          link: "https://docs.fileformat.com/image/otp/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "การทำงานกับรูปแบบเอกสารยอดนิยมอื่นๆ"
    content: |
        อัปเดตคุณสมบัติคำอธิบายประกอบจากรูปแบบไฟล์ยอดนิยมบางรูปแบบตามที่ระบุไว้ด้านล่าง
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