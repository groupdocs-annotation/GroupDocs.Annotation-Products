---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DOCM 주석 API C# 주석"
head_description: "DOCM, 이미지, 그림 및 문서 파일 형식에서 인기 있는 주석 유형을 만들고 주석을 추가하는 Java API."

############################# Header ############################
title: "자바에서 DOCM에 주석 달기"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "무료 평가판 다운로드"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Java API용 GroupDocs.Annotation 정보"
    content: |
        GroupDocs.Annotation for Java API는 Mac, Windows 또는 Ubuntu에서 PDF, Word 및 기타 문서에 주석을 추가할 수 있는 라이브러리입니다. [GroupDocs.Annotation for Java](/annotation/java)는 이미지 및 기타 다양한 문서에서 주석 생성, 추가, 편집, 삭제, 추출 및 내보내기를 포괄적으로 지원하는 주석 관리를 위한 기본 Java API입니다. 이 [페이지](https://docs.groupdocs.com/annotation/java/supported-document-formats/)에서 볼 수 있는 지원되는 문서 형식의 전체 목록입니다.
        이 라이브러리를 사용하면 DOCM 문서뿐만 아니라 Word, Excel, PowerPoint, Outlook 이메일, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad 및 기타 여러 유형의 문서와 함께 작업할 수 있습니다.
        GroupDocs.Annotation for Java API를 사용하면 새 메모를 만들고 추가하고, 주석을 편집하고, 주석과 주석을 추출하고, 문서에서 제거할 수 있습니다. 라이브러리는 텍스트, 다중선, 영역, 밑줄, 포인트, 워터마크, 화살표, 타원, 텍스트 대체, 거리, 텍스트 필드, PDF, HTML, Microsoft Word 문서, 스프레드시트, 다이어그램, 프레젠테이션, 그림, 이미지 및 기타 여러 파일 형식.
        예제(아래 참조)는 DOCM 문서 작업을 보여줍니다. 이 예제에서는 GroupDocs 작업 방법의 주요 단계를 볼 수 있습니다. 주석: 라이선스 설정, 작업할 문서 열기, 주석, 데이터 개체를 추가하여 요구 사항에 따라 주석 속성을 설정하고 결과를 필요한 위치에 저장합니다. 또한 github [페이지](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) 또는 제품 [문서](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java에서 DOCM에 주석을 추가하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 Java 기반 응용 프로그램 내의 DOCM 파일에 다양한 주석 유형을 쉽게 추가할 수 있습니다.
        *   댓글과 날짜가 포함된 Reply 객체를 생성합니다.
        *   AreaAnnotation 개체를 만들고 영역 옵션을 설정하고 답글을 추가합니다.
        *   Annotator 객체를 생성하고 영역 주석을 추가합니다.
        *   출력 파일을 저장합니다.
    title_right: "시스템 요구 사항"
    content_right: |
        GroupDocs.Annotation for Java API는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 필수 구성 요소가 설치되어 있는지 확인하십시오.
        *   운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
        *   개발 환경: NetBeans, Intellij IDEA, Eclipse 등
        *   Java 런타임 환경: Java 7(1.7) 이상
        *   [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)에서 최신 버전의 Java용 GroupDocs.Annotation을 다운로드하세요.

############################# Preview ############################
preview_Add:
    enable: true
    title: 주석 미리보기 및 코드 샘플
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
    title_left: "Java의 DOCM에서 주석을 제거하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 Java 기반 응용 프로그램 내의 DOCM 파일에서 주석 세부 정보를 쉽게 제거할 수 있습니다.
        *   댓글과 날짜가 포함된 Reply 객체를 생성합니다.
        *   SaveOptions 개체를 인스턴스화하고 AnnotationTypes = AnnotationType.None을 설정합니다.
        *   결과 문서 경로 또는 스트림과 SaveOptions 개체를 사용하여 저장 메서드를 호출합니다.

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
    title_left: "Java에서 DOCM의 주석을 편집하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 Java 기반 응용 프로그램 내의 DOCM 파일에서 다양한 주석 속성을 쉽게 업데이트할 수 있습니다.
        *   ImportAnnotations = true로 인스턴스화된 LoadOptions가 있는 입력 문서 경로 또는 스트림으로 Annotator 개체를 인스턴스화합니다.
        *   일부 AnnotationBase 구현을 만들고 기존 주석의 ID(해당 ID를 가진 주석을 찾을 수 없는 경우 아무 것도 변경되지 않음) 또는 주석의 경로 목록(기존의 모든 주석이 제거됨)을 설정합니다.
        *   전달된 주석으로 Annotator 객체의 업데이트 메서드를 호출합니다.
        *   결과 문서 경로 또는 스트림과 SaveOptions 개체를 사용하여 저장 메서드를 호출합니다.

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
    title_left: "Java의 DOCM에서 주석을 추출하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 Java 기반 애플리케이션 내의 DOCM 파일에서 쉽게 문서에 주석을 달고 주석 정보를 추출할 수 있습니다.
        *   댓글과 날짜가 포함된 Reply 객체를 생성합니다.
        *   LoadOptions 개체를 인스턴스화하고 true 인수를 사용하여 SetImportAnnotations를 호출합니다.
        *   목록 유형으로 변수를 정의하십시오.
        *   get 메서드를 호출하고 결과를 위의 변수에 반환합니다.

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
    title: "문서 및 이미지에 주석을 추가, 제거, 편집, 추출하는 라이브 데모"
    content: |
        지금 바로 [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) 웹사이트를 방문하여 주석을 DOCM 파일에 추가, 제거, 편집 및 추출하세요.
라이브 데모에는 다음과 같은 이점이 있습니다.

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-docm"
          title: "DOCM 파일 형식 정보"
          content: |
            DOCM 파일은 매크로 실행 기능이 있는 Microsoft Word 2007 이상에서 생성된 문서입니다. DOCX 파일 형식과 비슷하지만 매크로 실행 기능이 DOCX와 다릅니다. DOCX와 마찬가지로 DOCM 파일은 텍스트, 이미지, 테이블, 도형, 차트 및 기타 콘텐츠를 저장할 수 있습니다. 매크로 실행 기능을 통해 일련의 명령을 기록된 동작 형태로 실행하여 작업을 자동으로 완료함으로써 시간을 쉽게 절약할 수 있습니다. . DOCM 파일은 Microsoft Word 2007 이상에서 열고 편집할 수 있습니다.

          link: "https://docs.fileformat.com/image/docm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "기타 널리 사용되는 문서 형식 작업"
    content: |
        아래에 설명된 대로 널리 사용되는 일부 파일 형식에서 주석 속성을 업데이트합니다.
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