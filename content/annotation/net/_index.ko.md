---
############################# Static ############################
layout: "product"
date: 2022-07-05T12:44:18+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: "자바 문서 주석 API | PDF Word Excel PPTX 이미지 보기 및 주석 달기"
head_description: "자바 문서 주석 API. PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAD 및 이미지 파일 형식 보기, 태그 지정, 주석 달기 및 주석 달기."

############################# Header ############################
title: "Net API를 통한 문서 주석"
description: "외부 소프트웨어를 설치하지 않고도 PDF, HTML, MS Office 및 기타 문서 형식을 보고 주석을 달 수 있는 기능으로 Net 응용 프로그램 구축."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "무료 평가판 다운로드"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Net"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            - link: "#overview"
              text: "개요"

            - link: "#features"
              text: "특징"

            - link: "#support"
              text: "지원하다"

            - link: "https://products.groupdocs.app/annotation"
              text: "라이브 데모"

            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Net API는 Android, MacOS, Linux, Windows 등 다양한 플랫폼과 운영 체제에서 문서의 주석 작업을 할 수 있는 제품입니다. GroupDocs.Annotation은 많은 이점을 제공하는 간단한 API가 있는 라이브러리를 제공합니다. 예를 들어 데이터를 기밀로 유지해야 하거나 라이브러리 작업에 필요한 전력량을 선택하거나 주석 작업을 부분적으로 변경할 경우 라이브러리는 매우 유용합니다. 가볍고 유연합니다.

        {{플랫폼}} API용 GroupDocs.Annotation을 사용하면 텍스트, 폴리라인, 영역, 밑줄, 점, 워터마크, 화살표, 타원, 텍스트 대체, 거리, 텍스트 필드, 리소스 수정 등 다양한 유형의 주석으로 작업할 수 있습니다. PDF, HTML, Microsoft Office Word, Excel 스프레드시트, PowerPoint 프레젠테이션, Visio, Outlook 이메일, 이미지, 메타파일, CAD 도면 및 기타 다양한 형식과 같은 가장 널리 사용되는 문서 형식을 지원합니다. API는 문서 페이지의 축소판을 가져오는 기능을 제공하고 PDF 파일에서 주석 가져오기 및 내보내기를 지원합니다.

        라이브러리를 사용하여 [추가하다](/annotation/net/bmp/), [편집하다](/annotation/net/bmp/), [발췌](/annotation /net/bmp/) 및 [삭제](/annotation/net/bmp/) 문서에서 주석, 문서 회전, 축소판 솔루션 변경 및 이것은 전체 목록이 아닙니다. 가능성. 또한 지원되는 모든 문서 형식 내에서 요구 사항에 따라 주석 속성을 사용자 지정할 수 있는 포괄적인 데이터 개체 집합을 제공합니다.

        Net API용 GroupDocs.Annotation 작업은 매우 간단하며 몇 가지 기본 단계로 구성됩니다. 먼저 라이선스를 설정하고 작업할 파일을 선택한 다음 문서 주석으로 어떻게든 조작(삭제/편집/추출/삭제)하고 결과를 저장해야 합니다. 자세한 내용은 제품 [문서](https://docs.groupdocs.com/annotation/net/getting-started/) 또는 [예제](https://github.com/groupdocs-annotation)를 참조하세요. /GroupDocs.Annotation-for-.Net)이 설정되었습니다.

        GroupDocs.Annotation은 정기적으로 업데이트되며 고객을 지원합니다. 언제든지 질문을 하거나 아이디어를 보내거나 새로운 것에 대한 요구 사항을 알려주시면 새 버전에서 기꺼이 구현하겠습니다.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          다음은 Net용 GroupDocs.Annotation의 개요입니다.
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "개요"
          content: |
            * 주석 추가
            * 내보내기 주석
            * 주석 가져오기
            * 응답 기반 댓글
            * 주석 호환성
      
      ## TAB TWO ##
      tab_two:
        description: |
          Net용 GroupDocs.Annotation은 Microsoft Office, PDF, 이미지 및 기타 여러 가지를 포함하여 널리 사용되는 모든 [문서 파일 형식](https://docs.groupdocs.com/annotation/net/supported-document-formats/)을 지원합니다.
        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: [DOC](/annotation/net/doc/), [DOCX](/annotation/net/docx/), [DOCM](/annotation/net/docm/), [DOT](/annotation/net/dot/), [DOTX](/annotation/net/dotx/), [RTF](/annotation/net/rtf/)
                * **Excel**: [XLS](/annotation/net/xls/), [XLSX](/annotation/net/xlsx/), [XLSB](/annotation/net/xlsb/), [XLSM](/annotation/net/xlsm/)
                * **PowerPoint**: [PPT](/annotation/net/ppt/), [PPTX](/annotation/net/pptx/), [PPS](/annotation/net/pps/), [PPSX](/annotation/net/ppsx/), [POTM](/annotation/net/potm/), [POTX](/annotation/net/potx/), [PPSM](/annotation/net/ppsm/), [PPTM](/annotation/net/pptm/), [WMF](/annotation/net/wmf/), [EMF](/annotation/net/emf/)
                * **Outlook**: [EML](/annotation/net/eml/), [EMLX](/annotation/net/emlx/), [MSG](/annotation/net/msg/)
                * **Visio**: [VSS](/annotation/net/vss/), [VST](/annotation/net/vst/), [VSD](/annotation/net/vsd/), [VSDX](/annotation/net/vsdx/), [VSX](/annotation/net/vsx/)

        right:
          enable: true
          table:
            # table loop
            - title: "기타 형식"
              content: |
                * **Portable**: [PDF](/annotation/net/pdf/) (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: [ODT](/annotation/net/odt/), [ODS](/annotation/net/ods/), [ODP](/annotation/net/odp/)
                * **Images**: [BMP](/annotation/net/bmp/), [JPG](/annotation/net/jpg/), [JPEG](/annotation/net/jpeg/), [TIFF](/annotation/net/tiff/), [TIF](/annotation/net/tif/), [PNG](/annotation/net/png/), [GIF](/annotation/net/gif/), [DCM](/annotation/net/dcm/), [DICOM](/annotation/net/dicom/)
                * **AutoCAD**: [DWG](/annotation/net/dwg/), [DXF](/annotation/net/dxf/), [CAD](/annotation/net/cad/)
                * **Other**: [HTM](/annotation/net/htm/), [HTML](/annotation/net/html/), [CSV](/annotation/net/csv/), [DJVU](/annotation/net/djvu/), [OTP](/annotation/net/otp/), [OTT](/annotation/net/ott/)

      ## TAB THREE ##
      tab_three:
        description: |
          Net용 GroupDocs.Annotation은 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다.
      
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * Windows 데스크탑(x86 및 x64)
                * 윈도우 서버(x86 & x64)
                * 윈도우 애저
                * 리눅스
                * 맥 OS

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * .NET 표준 2.0
                * .NET 프레임워크 2.0 이상
                * .NET Core 2.0 이상
                * 모노 프레임워크 1.2 이상

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "패키지 관리자"
              content: |
                * 누겟
            
            - icon: "fas fa-tools"
              title: "개발 환경"
              content: |
                * 마이크로소프트 비주얼 스튜디오
                * 자마린.안드로이드
                * 자마린.IOS
                * 자마린.맥
                * 모노디벨롭

############################# Features ############################
features:
    enable: true
    title: "Net 기능에 대한 GroupDocs.Annotation"

    feature:
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: "주석 및 답장 추가, 편집 및 제거"

      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: "문서로 주석 내보내기"

      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/net/evaluation-limitations-and-licensing-of-groupdocs-annotation/"
        content: "계량 라이선스 – API 사용량에 따라 지불하여 제어된 청구"
      
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/net/extract-annotations-from-document/"
        content: "문서의 모든 주석을 가져오는 단일 함수 호출"

      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: "포인트 주석에 값 지정 또는 기존 포인트 값 이동"

      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/net/add-link-annotation/"
        content: "PDF, Word 및 PowerPoint 슬라이드에 링크 주석 추가"

      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: "주석의 배경색 설정 또는 문서에서 모든 주석 제거"

      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: "정확도로 PDF 파일에 주석 달기 – PDF 문서 및 캐시 페이지 미리보기의 이미지 표현 가져오기"

      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/import-annotations/"
        content: "문서의 이미지 표현에서 텍스트 주석의 텍스트 좌표 가져오기"

      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: "사용자 주석을 영역 주석에 연결 및 중첩 주석 지원"

      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/net/add-arrow-annotation/"
        content: "특정 콘텐츠를 가리키는 화살표 주석 사용"

      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/net/add-distance-annotation/"
        content: "거리 주석을 사용하여 객체 간의 거리를 나타내는 선 그리기"

      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: "클릭 시 주석을 추가하는 창이 팝업되는 포인트 기반 주석"

      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/net/add-polyline-annotation/"
        content: "폴리라인 주석으로 생성된 라인 세그먼트의 연결된 시퀀스 생성"

      - icon: "fas fa-lock"
        link: "https://docs.groupdocs.com/annotation/net/add-ellipse-annotation/"
        content: "직선 세그먼트, 호 세그먼트 또는 둘의 조합 생성"

      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: "교정을 위해 제안된 문서 영역 표시"
      
      - icon: "fas fa-fill-drip"
        link: "https://docs.groupdocs.com/annotation/net/add-image-annotation/"
        content: "PDF, 다이어그램, Word, Excel, 프레젠테이션 및 이미지에 이미지 주석 추가"

      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: "문서에 텍스트 필드 및 텍스트 기반 스탬프 또는 워터마크 추가"

      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: "문서의 특정 텍스트에 취소선, 밑줄 또는 바꾸기"

      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/net/update-annotations/"
        content: "새로운 높이 및 너비 매개변수를 할당하여 주석 크기 조정"

      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: "문서 페이지의 축소판을 가져옵니다. 이미지 및 다이어그램에 대해 주석이 달린 다양한 문서 관리"

      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: "다중 페이지 TIFF 파일로 주석 내보내기 및 작업"
  
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-watermark-annotation/"
        content: "워터마크 주석의 수직 및 수평 정렬 조정"
  
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-text-field-annotation/"
        content: "텍스트 필드에 텍스트 가로 맞춤 추가"

      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/document-text-info/"
        content: "문서 텍스트 줄(텍스트, 너비, 높이, 들여쓰기)에 대한 정보 가져오기"

    more_feature:
      - title: "여러 유형의 주석 지원"
        content: |
          .NET용 GroupDocs.Annotation을 사용하면 다양한 유형의 주석으로 작업할 수 있습니다. 이를 통해 작업에 대해 팀과 협업하는 동안 자유롭고 쉽게 의사 소통할 수 있습니다. 영역 주석(영역을 직사각형으로 표시하고 메모 추가), 포인트 주석(문서의 임의의 지점에 주석 붙이기), 텍스트 주석(선택한 텍스트에 주석 추가), 취소선/밑줄 주석( 단락에 적용), 폴리라인 주석(모양 및 자유형 선 그리기), 화살표 주석(주석이 첨부된 화살표 포인터), 타원 주석(타원 내부에 텍스트 표시), 거리 주석(객체 사이의 거리를 나타내는 선 그리기), 링크 주석(지원되는 문서 형식에 웹 링크 추가) 및 워터마크 주석(문서에 텍스트 스탬프 또는 워터마크를 추가할 수 있음).

          ```cs
          // AnnotationInfo 목록 초기화
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          // 텍스트 주석 초기화
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          // 목록에 주석 추가
          annotations.Add(textAnnotation);
          // 입력 파일 스트림 가져오기
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          // 주석 내보내기 및 출력 파일 저장
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation은 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---