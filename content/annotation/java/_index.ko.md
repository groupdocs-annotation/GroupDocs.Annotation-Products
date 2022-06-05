---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

head_title: "자바 문서 주석 API | PDF Word Excel PPTX 이미지 보기 및 주석 달기"
head_description: "자바 문서 주석 API. PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAD 및 이미지 파일 형식 보기, 태그 지정, 주석 달기 및 주석 달기."

title: "Java API를 통한 문서 주석"
description: "외부 소프트웨어를 설치하지 않고도 PDF, HTML, MS Office 및 기타 문서 형식을 보고 주석을 달 수 있는 기능으로 Java 응용 프로그램 구축."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "무료 평가판 다운로드"
    link: "https://downloads.groupdocs.com/annotation/java"

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

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

            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Annotation for Java API는 Java 기반 비즈니스 애플리케이션에서 사용하기 쉬운 문서, 주석 관리 및 조작 기능을 제공합니다. Java 주석 라이브러리를 사용하면 텍스트, 폴리라인, 영역, 밑줄, 포인트, 워터마크, 화살표, 타원, 텍스트 대체, 거리, 텍스트 필드, 리소스 수정 등을 포함한 다양한 유형의 주석으로 작업할 수 있습니다. 또한 포괄적인 세트도 제공합니다. PDF, HTML, Microsoft Office Word, Excel 스프레드시트, PowerPoint 프레젠테이션, Visio, Outlook 이메일, 이미지, 메타파일, CAD 도면 및 기타 다양한 형식을 포함하여 지원되는 모든 문서 형식 내에서 요구 사항에 따라 주석 속성을 사용자 정의하는 데이터 개체의.  
        
      API는 문서 페이지의 축소판을 가져오는 기능을 제공하고 PDF 파일에서 주석 가져오기 및 내보내기를 지원합니다.
    tabs:
      enable: true
      
      tab_one:
        description: |
          다음은 Java용 GroupDocs.Annotation의 개요입니다.
      
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
      
      tab_two:
        description: |
          Java용 GroupDocs.Annotation은 Microsoft Office, PDF, 이미지 및 기타 여러 가지를 포함하여 널리 사용되는 모든 [문서 파일 형식](https://docs.groupdocs.com/annotation/java/supported-document-formats/)을 지원합니다.

        left:
          enable: true
          table:
            - title: "마이크로소프트 오피스 형식"
              content: |
                * **단어**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **엑셀**: XLS, XLSX, XLSB, XLSM
                * **파워포인트**: PPT, PPTX, PPS, PPSX
                * **전망**: EML, EMLX
                * **Visio**: VSS, VST, VSD, VSDX

        right:
          enable: true
          table:
            - title: "기타 형식"
              content: |
                * **휴대용**: PDF(PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: ODT, ODS, ODP
                * **이미지**: BMP, JPG, TIFF, TIF, PNG
                * **오토캐드**: DWG, DXF
                * **기타**: HTML

      tab_three:
        description: |
          Java용 GroupDocs.Annotation은 다음 운영 체제, 프레임워크 및 패키지 관리자를 지원합니다.
      
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * 마이크로소프트 윈도우 데스크탑
                * 마이크로소프트 윈도우 서버
                * 리눅스
                * 맥 OS

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * 자바 7(1.7) 이상

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "개발 환경"
              content: |
                * 넷빈
                * IntelliJ 아이디어
                * 이클립스
            - icon: "fas fa-tools"
              title: "빌드 자동화 도구"
              content: |
                * 메이븐

features:
    enable: true
    title: "Java 기능에 대한 GroupDocs.Annotation"

    feature:
      - icon: "fas fa-copy"
        content: "문서에 영역 주석 추가 및 단순 및 중첩 주석 연결"

      - icon: "fas fa-eye"
        content: "화살표 주석을 사용하여 특정 콘텐츠 가리킴"

      - icon: "fas fa-bolt"
        content: "각진 위치에서 텍스트 워터마크를 PDF, 슬라이드, Excel 워크시트, 이미지 및 다이어그램으로 설정"
      
      - icon: "fas fa-file-powerpoint"
        content: "포인트 주석을 사용하여 문서의 모든 위치에 팝업 주석 추가"

      - icon: "fas fa-code"
        content: "폴리라인 주석을 사용하여 라인 세그먼트, 호 세그먼트 또는 둘 다의 시퀀스 연결"

      - icon: "fas fa-cloud"
        content: "PDF, Word 문서, 스프레드시트, 프레젠테이션, 다이어그램 및 이미지에 타원 주석 추가"

      - icon: "fas fa-remove-format"
        content: "PDF, PowerPoint, Excel, 이미지 및 다이어그램에 대한 각진 워터마크 추가"

      - icon: "fas fa-comment-slash"
        content: "문서의 이미지 표현에서 텍스트 주석의 좌표 가져오기"

      - icon: "fas fa-location-arrow"
        content: "문서의 특정 텍스트에 밑줄, 취소선 또는 수정"

      - icon: "fas fa-border-all"
        content: "문서에 텍스트 스탬프 또는 워터마크 및 텍스트 필드 추가"

      - icon: "fas fa-wrench"
        content: "Word 문서 및 PowerPoint 프레젠테이션 간에 주석 가져오기 및 내보내기"

      - icon: "fas fa-columns"
        content: "텍스트, TextReplacement, 워터마크 및 리소스 수정 주석 유형으로 Excel 스프레드시트에 주석 달기"

      - icon: "fas fa-file-word"
        content: "PowerPoint 프레젠테이션 및 슬라이드에 폴리라인, 취소선, 밑줄 또는 텍스트 주석 추가"

      - icon: "fas fa-envelope"
        content: "X, Y 좌표를 사용하여 프레젠테이션에서 포인트 주석 표시"

      - icon: "fas fa-print"
        content: "이미지에 취소선, 텍스트, 밑줄 또는 폴리라인 주석 추가"

      - icon: "fas fa-file-archive"
        content: "VSS 및 VSD와 같은 Visio 다이어그램에 대한 문서 정보 및 이미지 가져오기"

      - icon: "fas fa-file-code"
        content: "문서 페이지의 축소판 가져오기 및 다중 페이지 TIFF 파일 작업"
      
      - icon: "fas fa-file-excel"
        content: "단일 함수 호출로 문서의 모든 주석 가져오기"

      - icon: "fas fa-heading"
        content: "PDF, Word 및 PowerPoint 프레젠테이션에 링크 주석 추가"

      - icon: "fas fa-project-diagram"
        content: "PDF, Word, 다이어그램, 슬라이드 및 기타 주요 문서 형식에 대한 SVG 경로 구문 분석 지원"

      - icon: "fas fa-cube"
        content: "Word 문서에 워터마크 주석 추가 및 텍스트 교체를 위한 정리 지원"

      - icon: "fab fa-uncharted"
        content: "텍스트 주석에 대한 다이어그램의 모양 처리 지원"

      - icon: "fab fa-uncharted"
        content: "더 빠른 처리를 위해 문서의 페이지 미리보기를 캐싱하여 시간 절약"

      - icon: "fab fa-uncharted"
        content: "이전 형식에서도 Word, Excel 및 PowerPoint 문서에 쉽게 주석 달기"

      - icon: "fab fa-uncharted"
        content: "Excel, PowerPoint 및 다이어그램에 대한 거리 주석 캡션 표시"

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Annotation은 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        - img_alt: "GroupDocs.Annotation for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

back_to_top:
  enable: true
---
