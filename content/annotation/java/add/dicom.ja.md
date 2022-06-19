---
layout: "auto-gen"
date: 2021-05-13T12:44:20+03:00
draft: false

head_title: "JavaアプリケーションのDICOMに注釈を追加する"
head_description: "人気のある注釈タイプを作成してDICOM、画像、図面、ドキュメントファイル形式に追加するJava API."

title: "JavaでDICOMファイルに注釈を付ける"
description: "あらゆるタイプのJavaアプリケーションで、DICOM、Microsoft Officeドキュメント、画像、HTML、図面、およびその他のファイル形式に注釈を追加します."
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/annotation/java"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "APIリファレンス"

            - link: "https://github.com/groupdocs-annotation"
              text: "コード例"

            - link: "https://products.groupdocs.app/annotation/family"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "GroupDocs.Annotation for Java APIについて"
    content: |
        [GroupDocs.Annotation for Java](https://products.groupdocs.com/{{$1}/java)は、注釈の作成、追加、編集、削除、抽出、およびエクスポートを包括的にサポートする、注釈管理用のネイティブJavaAPIです。画像およびドキュメントファイル形式から。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Microsoft Word文書、Excelスプレッドシート、Visioダイアグラム、PowerPointプレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしを含む13種類の注釈を簡単に抽出できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、注釈のカスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "JavaでDICOMに注釈を追加する手順"
    content_left: |
        [GroupDocs.Annotation](https://products.groupdocs.com/annotation/java)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、Javaベースのアプリケーション内のDICOMファイルにさまざまな注釈タイプを簡単に追加できます。

        *入力ドキュメントパスまたはストリームを使用してAnnotatorオブジェクトをインスタンス化します。
        *必要なプロパティ（位置、ページ番号など）を使用してTextFieldAnnotationオブジェクトをインスタンス化します。
        * addメソッドを呼び出し、TextFieldAnnotationオブジェクトを渡します。
        *結果のドキュメントパスまたはストリームを使用してsaveメソッドを呼び出します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：NetBeans、Intellij IDEA、Eclipseなど
        * Javaランタイム環境：J2SE6.0以降
        * [Maven](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-conversion)から最新バージョンのGroupDocs.AnnotationforJavaを入手してください。
        
    code: |
        ```java
        String outputPath = Constants.getOutputFilePath("AddTextStrikeoutAnnotation", FilenameUtils.getExtension(input.dicom));
                    final Annotator annotator = new Annotator(input.dicom);
                    try {
                        Reply reply1 = new Reply();
                        reply1.setComment("First comment");
                        reply1.setRepliedOn(Calendar.getInstance().getTime());
                        Reply reply2 = new Reply();
                        reply2.setComment("Second comment");
                        reply2.setRepliedOn(Calendar.getInstance().getTime());
                        java.util.List replies =  new ArrayList();
                        replies.add(reply1);
                        replies.add(reply2);
                        Point point1 = new Point(80, 730);
                        Point point2 = new Point(240, 730);
                        Point point3 = new Point(80, 650);
                        Point point4 = new Point(240, 650);
                        List points = new ArrayList();
                        points.add(point1);
                        points.add(point2);
                        points.add(point3);
                        points.add(point4);
                        StrikeoutAnnotation strikeout = new StrikeoutAnnotation();
                        strikeout.setCreatedOn(Calendar.getInstance().getTime());
                        strikeout.setFontColor(65535);
                        strikeout.setMessage("This is strikeout annotation");
                        strikeout.setOpacity(0.7);
                        strikeout.setPageNumber(0);
                        strikeout.setPoints(points);
                        strikeout.setReplies(replies);
                        annotator.add(strikeout);
                        annotator.save(output.dicom);
                    } finally {
                        if (annotator != null) {
                            annotator.dispose();
                        }
                    }
        ```
        
demos:
    enable: true
    title: "ドキュメントや画像に注釈を追加するライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、今すぐDICOMファイルに注釈を作成して追加します。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-dicom"
          title: "DICOMファイル形式について"
          content: |
            DICOMは、Medical Imaging and Communications in Medicineの頭字語であり、医療情報学の分野に関係しています。 DICOMは、ファイル形式の定義とネットワーク通信プロトコルを組み合わせたものです。 DICOMは.DCM拡張子を使用します。 .DCMは、フォーマット1.xとフォーマット2.xの2つの異なるフォーマットで存在します。 DCMフォーマット1.xは、通常と拡張の2つのバージョンでさらに利用できます。 DICOMは、さまざまなベンダーのプリンター、サーバー、スキャナーなどの医用画像装置の統合に使用され、一意性のために各患者の識別データも含まれています。 DICOMファイルは、DICOM形式の画像データを受信できる場合、2者間で共有できます。 DICOMの通信部分はアプリケーション層プロトコルであり、TCP/IPを使用してエンティティ間で通信します。 HTTPおよびHTTPSプロトコルは、DICOMのWebサービスに使用されます。 Webサービスでサポートされているバージョンは、1.0、1.1、2以降です。

          link: "https://docs.fileformat.com/image/dicom/"

more_formats:
    enable: false
    title: "他の一般的なファイル形式に注釈を付ける"
    content: |
        ドキュメントおよび画像形式用のJava注釈管理ライブラリ。以下に説明するように、一般的なファイル形式のいくつかに注釈プロパティを追加します。
    format: 
          link: "https://products.groupdocs.com/annotation/java/add/pdf"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/java/add/doc"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/java/add/docm"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/java/add/docx"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/java/add/dot"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/java/add/dotx"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "https://products.groupdocs.com/annotation/java/add/dotm"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "https://products.groupdocs.com/annotation/java/add/rtf"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/java/add/odt"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/java/add/xls"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/java/add/xlsx"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/add/xlsm"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/add/xlsb"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/java/add/ods"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/java/add/ppt"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/add/pptx"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/add/ppsx"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/java/add/potm"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/java/add/pptm"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/add/pps"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/java/add/odp"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/add/html"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/java/add/tiff"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/java/add/jpeg"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/java/add/png"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/java/add/bmp"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/java/add/eml"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/add/msg"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/add/vsd"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/java/add/vsdx"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/java/add/vss"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/java/add/vst"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/java/add/dwg"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/java/add/dxf"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/java/add/dcm"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/java/add/wmf"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/java/add/emf"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
