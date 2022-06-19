---
layout: "auto-gen"
date: 2021-05-13T12:44:25+03:00
draft: false

head_title: "JavaアプリケーションのPPSXに注釈を追加する"
head_description: "一般的な注釈タイプを作成してPPSX、画像、図面、ドキュメントファイル形式に追加するJava API."

title: "JavaでPPSXファイルに注釈を付ける"
description: "あらゆるタイプのJavaアプリケーションで、PPSX、Microsoft Officeドキュメント、画像、HTML、図面、およびその他のファイル形式に注釈を追加します."
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
        [GroupDocs.Annotation for Java](/annotation/java/)は、画像やドキュメントファイル形式から注釈を作成、追加、編集、削除、抽出、エクスポートするための包括的なサポートを備えた、注釈管理用のネイティブJavaAPIです。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Microsoft Word文書、Excelスプレッドシート、Visioダイアグラム、PowerPointプレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしを含む13種類の注釈を簡単に抽出できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、注釈のカスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "JavaでPPSXに注釈を追加する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、Javaベースのアプリケーション内のPPSXファイルにさまざまな注釈タイプを簡単に追加できます。

        *コメントと日付を使用して返信オブジェクトを作成します。
        * AreaAnnotationオブジェクトを作成し、エリアオプションを設定し、返信を追加します。
        * Annotatorオブジェクトを作成し、領域の注釈を追加します。
        *出力ファイルを保存します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：NetBeans、Intellij IDEA、Eclipseなど
        * Javaランタイム環境：Java 7（1.7）以降
        * [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)から最新バージョンのGroupDocs.AnnotationforJavaを入手してください。
        
    code: |
        ```java
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
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
        
        Annotator annotator = new Annotator("input.ppsx");
        annotator.add(area);
        annotator.save("output.pptx");
        annotator.dispose();
        ```
        
demos:
    enable: true
    title: "ドキュメントや画像に注釈を追加するライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、今すぐPPSXファイルに注釈を作成して追加します。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ppsx"
          title: "PPSXファイル形式について"
          content: |
            PPSX、パワーポイントスライドショー、ファイルは、スライドショーの目的でMicrosoftPowerPoint2007以降を使用して作成されます。これは、MicrosoftPowerPoint97-2003バージョンでサポートされていたPPSファイル形式の更新です。 PPSXファイルを別のユーザーと共有して開くと、編集可能モードで開くPPTXファイルとは異なり、PowerPointの表示として起動します。スライドショーの順序は、元のプレゼンテーションと同じです。スライドショー中のPPSXへのプレゼンテーションスライドには、すべてのスライドに画像、音声、その他の埋め込みメディアが付属しています。

          link: "https://docs.fileformat.com/presentation/ppsx/"

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
