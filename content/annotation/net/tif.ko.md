
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/tif"/>

############################# Head ############################
head_title: "Net TIF 주석 API C#으로 주석 달기"
head_description: "Net 생성 API 및 주석 달기 인기 있는 주석 유형 ~에서 TIF, 이미지, 도면 및 문서 파일 형식."

############################# Header ############################
title: "주석 TIF ~에서 {{플랫폼}}"
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
        img_alt: "Net에 대한 GroupDocs.Annotation"
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
    title: "Net API용 GroupDocs.Annotation 정보"
    content: |
        GroupDocs.Annotation for Net API는 Mac, Windows 또는 Ubuntu에서 PDF, Word 및 기타 문서에 주석을 추가할 수 있는 라이브러리입니다. [GroupDocs.Annotation for Net](/annotation/net)은 주석 생성, 추가, 편집, 삭제, 추출 및 내보내기를 포괄적으로 지원하는 주석 관리를 위한 기본 Net API입니다. 이미지 및 기타 다양한 문서. 이 [page](https://docs.groupdocs.com/annotation/net/supported-document-formats/)에서 볼 수 있는 지원되는 문서 형식의 전체 목록입니다.

        이 라이브러리를 사용하면 TIF 문서뿐만 아니라 Word, Excel, PowerPoint, Outlook 이메일, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad 및 기타 여러 유형의 문서와 함께 작업할 수 있습니다.

        Net API용 GroupDocs.Annotation을 사용하면 새 메모, edit 주석, extract 을 만들고 추가할 수 있습니다. 주석, 주석 및 문서에서 remove. 라이브러리는 텍스트, 다중선, 영역, 밑줄, 포인트, 워터마크, 화살표, 타원, 텍스트 대체, 거리, 텍스트 필드, PDF, HTML, Microsoft Word 문서, 스프레드시트, 다이어그램, 프레젠테이션, 도면, 이미지 및 기타 여러 파일 형식.

        예제(아래 참조)는 TIF 문서 작업을 보여줍니다. 이 예제에서는 GroupDocs 작업 방법의 주요 단계를 볼 수 있습니다. 주석: 라이선스 설정, 작업할 문서 열기, 주석, 데이터 개체를 추가하여 요구 사항에 따라 주석 속성을 설정하고 결과를 필요한 위치에 저장합니다. 또한 github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net) 또는 제품 문서]에서 지원되는 기능에 대해 자세히 살펴볼 수 있습니다 [documentation](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Net에서 ~에서 TIF 주석을 추가하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Net 개발자가 몇 가지 간단한 단계를 구현하여 모든 Net 기반 애플리케이션 내의 TIF 파일에 다양한 주석 유형을 쉽게 추가할 수 있습니다.
        * 댓글과 날짜가 포함된 회신 개체를 만듭니다.
        * AreaAnnotation 개체를 만들고 영역 옵션을 설정하고 답글을 추가합니다.
        * Annotator 개체를 만들고 영역 주석을 추가합니다.
        * 출력 파일을 저장합니다.
    title_right: "시스템 요구 사항"
    content_right: |
        Net API용 GroupDocs.Annotation은 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 필수 구성 요소가 설치되어 있는지 확인하십시오.
        * 운영 체제: Microsoft Windows, Linux, MacOS
        * 개발 환경: Visual Studio, Xamarin, MonoDevelop
        * 프레임워크: .NET Framework, .NET Standard, .NET Core, Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.annotation)에서 최신 버전의 .NET용 GroupDocs.Annotation을 다운로드합니다.

############################# Preview ############################
preview_Add:
    enable: true
    title: "주석 미리보기 및 코드 샘플"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //로컬 디스크에서 문서에 텍스트 필드 주석 추가
        (Annotator annotator = new Annotator("input.bmp")) 사용
        {
            TextFieldAnnotation textField = new TextFieldAnnotation
            {
                BackgroundColor = 65535,
                Box = new Rectangle(100, 100, 100, 100),
                CreatedOn = DateTime.Now,
                Text = "Some text",
                FontColor = 65535,
                FontSize = 12,
                Message = "텍스트 필드 주석입니다",
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
                        Comment = "첫 번째 댓글",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "두 번째 댓글",
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
    title_left: "Net에서 ~에서 TIF 주석을 제거하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Net 개발자가 몇 가지 간단한 단계를 구현하여 모든 Net 기반 애플리케이션 내의 TIF 파일에서 주석 세부 정보를 쉽게 제거할 수 있습니다.
        * 댓글과 날짜가 포함된 회신 개체를 만듭니다.
        * SaveOptions 개체를 인스턴스화하고 AnnotationTypes = AnnotationType.None을 설정합니다.
        * 결과 문서 경로 또는 스트림 및 SaveOptions 개체와 함께 저장 메서드를 호출합니다.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```cs
        // 1- 주석 색인을 사용하여 문서에서 주석을 제거하는 방법
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- 주석 개체를 사용하여 문서에서 주석을 제거하는 방법
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- ID 목록을 사용하여 문서에서 일부 주석을 제거하는 방법
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- 주석 목록을 사용하여 문서에서 일부 주석을 제거하는 방법
        
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
    title_left: "Net에서 주석 ~에서 TIF을 편집하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Net 개발자가 몇 가지 간단한 단계를 구현하여 모든 Net 기반 애플리케이션 내의 TIF 파일에서 다양한 주석 속성을 쉽게 업데이트할 수 있습니다.
        * ImportAnnotations = true로 인스턴스화된 LoadOptions가 있는 입력 문서 경로 또는 스트림으로 Annotator 개체를 인스턴스화합니다.
        * 일부 AnnotationBase 구현을 만들고 기존 주석의 ID(해당 ID를 가진 주석을 찾을 수 없는 경우 아무 것도 변경되지 않음) 또는 주석의 경로 목록(기존의 모든 주석이 제거됨)을 설정합니다.
        * 전달된 주석이 있는 Annotator 개체의 업데이트 메서드를 호출합니다.
        * 결과 문서 경로 또는 스트림 및 SaveOptions 개체와 함께 저장 메서드를 호출합니다.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```cs
        // 주석이 달린 문서 열기
        (Annotator annotator = new Annotator("result.bmp")) 사용
        {
            // 기존 주석의 일부 속성을 변경한다고 가정합니다.
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // 존재하는 주석 ID를 설정하는 것이 중요합니다.
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "이것은 업데이트된 주석입니다",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "업데이트된 첫 번째 댓글",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "두 번째 댓글 업데이트됨",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // 업데이트 주석
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Net에서 ~에서 TIF 주석을 추출하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Net 개발자가 몇 가지 간단한 단계를 구현하여 Net 기반 애플리케이션 내의 TIF 파일에서 문서에 주석을 추가하고 주석 정보를 쉽게 추출할 수 있습니다.
        * 댓글과 날짜가 포함된 회신 개체를 만듭니다.
        * LoadOptions 개체를 인스턴스화하고 true 인수로 SetImportAnnotations를 호출합니다.
        * 목록 유형으로 변수를 정의하십시오.
        * get 메서드를 호출하고 결과를 위의 변수에 반환합니다.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```cs
        // 이 예제 입력 파일("annotated.bmp")을 사용하려면 주석이 있어야 합니다.
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
    title: "문서 및 이미지에 주석을 추가, 제거, 편집, 추출하는 라이브 데모"
    content: |
        지금 바로 [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) 웹사이트를 방문하여 TIF 파일에 주석을 추가, 제거, 편집 및 추출하세요.
        라이브 데모에는 다음과 같은 이점이 있습니다

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-tif"
          title: "TIF 파일 형식 정보"
          content: |
            TIFF 또는 TIF(Tagged Image File Format)는 이 파일 형식 표준을 준수하는 다양한 장치에서 사용하기 위한 래스터 이미지를 나타냅니다. 여러 색 공간에서 이중 수준, 회색조, 팔레트 색상 및 풀 컬러 이미지 데이터를 설명할 수 있습니다. 형식을 사용하는 응용 프로그램의 공간과 시간 중에서 선택할 수 있도록 손실 및 무손실 압축 체계를 지원합니다. 형식은 기계에 의존하지 않으며 프로세서, 운영 체제 또는 파일 시스템과 같은 범위에서 자유롭습니다.
          link: "https://docs.fileformat.com/image/tif/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "기타 널리 사용되는 문서 형식 작업"
    content: |
        아래에 설명된 대로 널리 사용되는 일부 파일 형식에서 주석 속성을 업데이트합니다.
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