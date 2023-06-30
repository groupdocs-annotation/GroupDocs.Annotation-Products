
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/jpg"/>

############################# Head ############################
head_title: "Java JPG 주석 API C#으로 주석 달기"
head_description: "Java 생성 API 및 주석 달기 인기 있는 주석 유형 ~에서 JPG, 이미지, 도면 및 문서 파일 형식."

############################# Header ############################
title: "주석 JPG ~에서 {{플랫폼}}"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "Java에 대한 GroupDocs.Annotation"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Java API용 GroupDocs.Annotation 정보"
    content: |
        GroupDocs.Annotation for Java API는 Mac, Windows 또는 Ubuntu에서 PDF, Word 및 기타 문서에 주석을 추가할 수 있는 라이브러리입니다. [GroupDocs.Annotation for Java](/annotation/java)은 주석 생성, 추가, 편집, 삭제, 추출 및 내보내기를 포괄적으로 지원하는 주석 관리를 위한 기본 Java API입니다. 이미지 및 기타 다양한 문서. 이 [page](https://docs.groupdocs.com/annotation/java/supported-document-formats/)에서 볼 수 있는 지원되는 문서 형식의 전체 목록입니다.

        이 라이브러리를 사용하면 JPG 문서뿐만 아니라 Word, Excel, PowerPoint, Outlook 이메일, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad 및 기타 여러 유형의 문서와 함께 작업할 수 있습니다.

        Java API용 GroupDocs.Annotation을 사용하면 새 메모, edit 주석, extract 을 만들고 추가할 수 있습니다. 주석, 주석 및 문서에서 remove. 라이브러리는 텍스트, 다중선, 영역, 밑줄, 포인트, 워터마크, 화살표, 타원, 텍스트 대체, 거리, 텍스트 필드, PDF, HTML, Microsoft Word 문서, 스프레드시트, 다이어그램, 프레젠테이션, 도면, 이미지 및 기타 여러 파일 형식.

        예제(아래 참조)는 JPG 문서 작업을 보여줍니다. 이 예제에서는 GroupDocs 작업 방법의 주요 단계를 볼 수 있습니다. 주석: 라이선스 설정, 작업할 문서 열기, 주석, 데이터 개체를 추가하여 요구 사항에 따라 주석 속성을 설정하고 결과를 필요한 위치에 저장합니다. 또한 github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) 또는 제품 문서]에서 지원되는 기능에 대해 자세히 살펴볼 수 있습니다 [documentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java에서 ~에서 JPG 주석을 추가하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 모든 Java 기반 애플리케이션 내의 JPG 파일에 다양한 주석 유형을 쉽게 추가할 수 있습니다.
        * 댓글과 날짜가 포함된 회신 개체를 만듭니다.
        * AreaAnnotation 개체를 만들고 영역 옵션을 설정하고 답글을 추가합니다.
        * Annotator 개체를 만들고 영역 주석을 추가합니다.
        * 출력 파일을 저장합니다.
    title_right: "시스템 요구 사항"
    content_right: |
        Java API용 GroupDocs.Annotation은 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 필수 구성 요소가 설치되어 있는지 확인하십시오.
        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: NetBeans, Intellij IDEA, Eclipse 등
        * Java 런타임 환경: Java 7(1.7) 이상
        * [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)에서 최신 버전의 Java용 GroupDocs.Annotation을 다운로드하세요.

############################# Preview ############################
preview_Add:
    enable: true
    title: "주석 미리보기 및 코드 샘플"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```자바
        // Reply 클래스 인스턴스 생성 및 주석 추가
        Reply firstReply = new Reply();
        firstReply.setComment("첫 댓글");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("두 번째 댓글");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // AreaAnnotation 클래스의 인스턴스 생성 및 옵션 설정
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("영역 주석입니다.");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Annotator 클래스의 인스턴스 생성
        Annotator annotator = new Annotator("input.bmp");
        
        // 주석 추가
        annotator.add(area);
        
        // 파일에 저장
        annotator.save("출력.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Java에서 ~에서 JPG 주석을 제거하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 모든 Java 기반 애플리케이션 내의 JPG 파일에서 주석 세부 정보를 쉽게 제거할 수 있습니다.
        * 댓글과 날짜가 포함된 회신 개체를 만듭니다.
        * SaveOptions 개체를 인스턴스화하고 AnnotationTypes = AnnotationType.None을 설정합니다.
        * 결과 문서 경로 또는 스트림 및 SaveOptions 개체와 함께 저장 메서드를 호출합니다.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```자바
        // Annotator 클래스의 인스턴스 생성
        Annotator annotator = new Annotator("C://input.bmp");

        // 세트 유형으로 주석 제거 없음
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // 출력 파일에 주석 저장
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Java에서 주석 ~에서 JPG을 편집하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 모든 Java 기반 애플리케이션 내의 JPG 파일에서 다양한 주석 속성을 쉽게 업데이트할 수 있습니다.
        * ImportAnnotations = true로 인스턴스화된 LoadOptions가 있는 입력 문서 경로 또는 스트림으로 Annotator 개체를 인스턴스화합니다.
        * 일부 AnnotationBase 구현을 만들고 기존 주석의 ID(해당 ID를 가진 주석을 찾을 수 없는 경우 아무 것도 변경되지 않음) 또는 주석의 경로 목록(기존의 모든 주석이 제거됨)을 설정합니다.
        * 전달된 주석이 있는 Annotator 개체의 업데이트 메서드를 호출합니다.
        * 결과 문서 경로 또는 스트림 및 SaveOptions 개체와 함께 저장 메서드를 호출합니다.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```자바
        String outputPath = "UpdateAnnotation.bmp";

        // Annotator 클래스의 인스턴스 생성
        Annotator annotator = new Annotator("input.bmp");
        
        // 첫 번째 예제에 대한 Reply 클래스의 인스턴스를 생성하고 주석을 추가합니다.
        Reply reply1 = new Reply();
        reply1.setComment("원래 첫 댓글");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("원래 두 번째 댓글");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // AreaAnnotation 클래스의 인스턴스 생성 및 옵션 설정
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("원본 주석입니다.");
        original.setReplies(replies);
        
        // 원래 주석 추가
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // 주석이 달린 문서 열기
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // 첫 번째 업데이트 예를 위한 Reply 클래스의 인스턴스 생성
        Reply reply3 = new Reply();
        reply3.setComment("첫 댓글 업데이트");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("두 번째 댓글 업데이트");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // 기존 주석의 일부 속성을 변경할 것을 제안합니다.
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("업데이트된 주석입니다.");
        updated.setReplies(replies1);
        
        // 주석 업데이트 및 저장
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Java에서 ~에서 JPG 주석을 추출하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 개발자가 몇 가지 간단한 단계를 구현하여 Java 기반 애플리케이션 내의 JPG 파일에서 문서에 주석을 추가하고 주석 정보를 쉽게 추출할 수 있습니다.
        * 댓글과 날짜가 포함된 회신 개체를 만듭니다.
        * LoadOptions 개체를 인스턴스화하고 true 인수로 SetImportAnnotations를 호출합니다.
        * 목록 유형으로 변수를 정의하십시오.
        * get 메서드를 호출하고 결과를 위의 변수에 반환합니다.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```자바
        // 이 예제를 사용하려면 입력 파일("annotated.bmp")에 주석이 있어야 합니다.
        LoadOptions loadOptions = new LoadOptions();
        
        // Annotator 클래스의 인스턴스 생성 및 주석 가져오기
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "문서 및 이미지에 주석을 추가, 제거, 편집, 추출하는 라이브 데모"
    content: |
        지금 바로 [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) 웹사이트를 방문하여 JPG 파일에 주석을 추가, 제거, 편집 및 추출하세요.
        라이브 데모에는 다음과 같은 이점이 있습니다

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpg"
          title: "JPG 파일 형식 정보"
          content: |
            JPG는 손실 압축 방법을 사용하여 저장되는 이미지 형식의 한 유형입니다. 압축 결과 출력 이미지는 스토리지 크기와 이미지 품질 간의 절충안입니다. 사용자는 압축 수준을 조정하여 원하는 품질 수준을 달성하는 동시에 스토리지 크기를 줄일 수 있습니다. 10:1 압축이 이미지에 적용되는 경우 이미지 품질에 미치는 영향은 미미합니다. 압축 값이 높을수록 이미지 품질 저하가 커집니다.
          link: "https://docs.fileformat.com/image/jpg/"

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