---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "C#의 Net PDF 주석 API 주석"
head_description: "PDF, 이미지, 그림 및 문서 파일 형식에서 인기 있는 주석 유형을 만들고 주석을 추가하는 Net API."

############################# Header ############################
title: "Net에서 PDF에 주석 달기"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "무료 평가판 다운로드"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Net API용 GroupDocs.Annotation 정보"
    content: |
        Net API용 GroupDocs.Annotation은 Mac, Windows 또는 Ubuntu에서 PDF, Word 및 기타 문서에 주석을 추가할 수 있는 라이브러리입니다. [GroupDocs.Annotation for Net](/annotation/net)은 이미지 및 기타 다양한 문서에서 주석 생성, 추가, 편집, 삭제, 추출 및 내보내기를 포괄적으로 지원하는 주석 관리를 위한 기본 Net API입니다. 이 [페이지](https://docs.groupdocs.com/annotation/net/supported-document-formats/)에서 볼 수 있는 지원되는 문서 형식의 전체 목록입니다.
        이 라이브러리를 사용하면 PDF 문서뿐만 아니라 Word, Excel, PowerPoint, Outlook 이메일, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad 및 기타 여러 유형의 문서와 함께 작업할 수 있습니다.
        Net API용 GroupDocs.Annotation을 사용하면 새 메모를 만들고 추가하고, 주석을 편집하고, 주석과 주석을 추출하고, 문서에서 제거할 수 있습니다. 라이브러리는 텍스트, 다중선, 영역, 밑줄, 포인트, 워터마크, 화살표, 타원, 텍스트 대체, 거리, 텍스트 필드, PDF, HTML, Microsoft Word 문서, 스프레드시트, 다이어그램, 프레젠테이션, 그림, 이미지 및 기타 여러 파일 형식.
        예제(아래 참조)는 PDF 문서 작업을 보여줍니다. 이 예제에서는 GroupDocs 작업 방법의 주요 단계를 볼 수 있습니다. 주석: 라이선스 설정, 작업할 문서 열기, 주석, 데이터 개체를 추가하여 요구 사항에 따라 주석 속성을 설정하고 결과를 필요한 위치에 저장합니다. 또한 github [페이지](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) 또는 제품 [문서](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Net에서 PDF에 주석을 추가하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net 개발자가 몇 가지 간단한 단계를 구현하여 Net 기반 응용 프로그램 내의 PDF 파일에 다양한 주석 유형을 쉽게 추가할 수 있습니다.
        *   댓글과 날짜가 포함된 Reply 객체를 생성합니다.
        *   AreaAnnotation 개체를 만들고 영역 옵션을 설정하고 답글을 추가합니다.
        *   Annotator 객체를 생성하고 영역 주석을 추가합니다.
        *   출력 파일을 저장합니다.
    title_right: "시스템 요구 사항"
    content_right: |
        Net API용 GroupDocs.Annotation은 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 아래 코드를 실행하기 전에 시스템에 다음 필수 구성 요소가 설치되어 있는지 확인하십시오.
        *   운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
        *   개발 환경: Visual Studio, Xamarin, MonoDevelop
        *   프레임워크: .NET Framework, .NET Standard, .NET Core, Mono
        *   [NuGet](https://www.nuget.org/packages/groupdocs.annotation)에서 최신 버전의 .NET용 GroupDocs.Annotation을 다운로드합니다.

############################# Preview ############################
preview_Add:
    enable: true
    title: 주석 미리보기 및 코드 샘플
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
    title_left: "Net의 PDF에서 주석을 제거하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net 개발자가 몇 가지 간단한 단계를 구현하여 Net 기반 응용 프로그램 내의 PDF 파일에서 주석 세부 정보를 쉽게 제거할 수 있습니다.
        *   댓글과 날짜가 포함된 Reply 객체를 생성합니다.
        *   SaveOptions 개체를 인스턴스화하고 AnnotationTypes = AnnotationType.None을 설정합니다.
        *   결과 문서 경로 또는 스트림과 SaveOptions 개체를 사용하여 저장 메서드를 호출합니다.

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
    title_left: "Net에서 PDF의 주석을 편집하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net 개발자가 몇 가지 간단한 단계를 구현하여 Net 기반 응용 프로그램 내의 PDF 파일에서 다양한 주석 속성을 쉽게 업데이트할 수 있습니다.
        *   ImportAnnotations = true로 인스턴스화된 LoadOptions가 있는 입력 문서 경로 또는 스트림으로 Annotator 개체를 인스턴스화합니다.
        *   일부 AnnotationBase 구현을 만들고 기존 주석의 ID(해당 ID를 가진 주석을 찾을 수 없는 경우 아무 것도 변경되지 않음) 또는 주석의 경로 목록(기존의 모든 주석이 제거됨)을 설정합니다.
        *   전달된 주석으로 Annotator 객체의 업데이트 메서드를 호출합니다.
        *   결과 문서 경로 또는 스트림과 SaveOptions 개체를 사용하여 저장 메서드를 호출합니다.

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
    title_left: "Net의 PDF에서 주석을 추출하는 단계"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) Net 개발자가 몇 가지 간단한 단계를 구현하여 Net 기반 응용 프로그램 내의 PDF 파일에서 문서에 쉽게 주석을 달고 주석 정보를 추출할 수 있습니다.
        *   댓글과 날짜가 포함된 Reply 객체를 생성합니다.
        *   LoadOptions 개체를 인스턴스화하고 true 인수를 사용하여 SetImportAnnotations를 호출합니다.
        *   목록 유형으로 변수를 정의하십시오.
        *   get 메서드를 호출하고 결과를 위의 변수에 반환합니다.

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
    title: "문서 및 이미지에 주석을 추가, 제거, 편집, 추출하는 라이브 데모"
    content: |
        지금 바로 [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) 웹사이트를 방문하여 주석을 PDF 파일에 추가, 제거, 편집 및 추출하세요. 라이브 데모에는 다음과 같은 이점이 있습니다.

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pdf"
          title: "PDF 파일 형식 정보"
          content: |
            PDF(Portable Document Format)는 Adobe에서 1990년대에 만든 문서 유형입니다. 이 파일 형식의 목적은 응용 프로그램 소프트웨어, 하드웨어 및 운영 체제와 독립적인 형식으로 문서 및 기타 참조 자료를 표현하기 위한 표준을 도입하는 것이었습니다. PDF 파일은 확장 프로그램/플러그인을 통해 Adobe Acrobat Reader/Writer는 물론 Chrome, Safari, Firefox와 같은 대부분의 최신 브라우저에서 열 수 있습니다. 대부분의 상용 소프트웨어 제품군은 추가 소프트웨어 구성 요소 없이도 문서를 PDF 파일 형식으로 변환할 수 있습니다. 따라서 PDF 파일 형식은 원본 문서의 일부가 될 수 있는 텍스트, 이미지, 하이퍼링크, 양식 필드, 리치 미디어, 디지털 서명, 첨부 파일, 메타데이터, 지형 공간 기능 및 3D 개체와 같은 정보를 포함할 수 있는 완전한 기능을 가지고 있습니다.

          link: "https://docs.fileformat.com/image/pdf/"

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