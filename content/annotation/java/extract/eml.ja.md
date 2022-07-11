---
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:37+03:00
draft: false

head_title: "JavaでEMLから注釈を抽出する-注釈抽出API"
head_description: "EML、画像、図面、ドキュメントファイル形式から一般的な注釈タイプを抽出するJava注釈抽出API."

title: "EML用のJavaアノテーション抽出API"
description: "あらゆるタイプのJavaアプリケーションで、Microsoft Officeドキュメント、画像、HTML、図面、およびその他のファイル形式から注釈を抽出します."
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
        [GroupDocs.Annotation for Java](/annotation/java/)は、高度な注釈管理ソリューションであり、開発者が画像やドキュメントファイル形式から注釈を表示、[追加](/annotation/java/add/eml/)、[更新](/annotation/java/edit/eml/)、[削除](/annotation/java/remove/eml/)、抽出、およびエクスポートできるようにします。ユーザーは、コメント、メモ、コメント、およびテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを、PDF、HTML、Microsoft Word文書、Excelスプレッドシート、Visioダイアグラム、PowerPointプレゼンテーション、図面、画像、およびその他の多くのファイル形式から簡単に抽出できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、注釈のカスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "Javaで注釈を抽出するための手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、Javaベースのアプリケーション内のEMLファイルからドキュメントに注釈を付けたり注釈情報を抽出したりできます。

        *コメントと日付を使用して返信オブジェクトを作成します。
        * LoadOptionsオブジェクトをインスタンス化し、true引数を指定してSetImportAnnotationsを呼び出します。
        *タイプリストで変数を定義します。
        * getメソッドを呼び出し、結果を上記の変数に返します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：NetBeans、Intellij IDEA、Eclipseなど
        * Javaランタイム環境：Java 7（1.7）以降
        * [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)から最新バージョンのGroupDocs.AnnotationforJavaを入手してください。
        
    code: |
        ```java
        //この例を使用するには、入力ファイル（ "annotated.eml"）に注釈を付ける必要があります
         
        LoadOptions loadOptions = new LoadOptions();
        loadOptions.setImportAnnotations(true);
        
        final Annotator annotator = new Annotator("annotated.eml", loadOptions);
        List annotations = annotator.get();
        ```
        
demos:
    enable: true
    title: "ドキュメントと画像に注釈を付けるためのライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、EMLファイルから注釈情報を今すぐ抽出します。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-eml"
          title: "EMLファイル形式について"
          content: |
            EMLファイル形式は、Outlookおよびその他の関連アプリケーションを使用して保存された電子メールメッセージを表します。ほとんどすべての電子メールクライアントは、RFC-822インターネットメッセージ形式標準に準拠するためにこのファイル形式をサポートしています。 Microsoft Outlookは、EMLメッセージタイプを開くためのデフォルトのソフトウェアです。 EMLファイルは、ディスクへの保存や、通信プロトコルを使用した受信者への送信に使用できます。

          link: "https://docs.fileformat.com/email/eml/"

more_formats:
    enable: false
    title: "サポートされている他のファイル形式からの注釈の抽出"
    content: |
        ドキュメントおよび画像形式用のJava注釈抽出ライブラリ。以下に示すように、いくつかの一般的なファイル形式の注釈の詳細を取得します。
    format: 
          link: "https://products.groupdocs.com/annotation/java/extract/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/java/extract/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/java/extract/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/java/extract/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/java/extract/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/java/extract/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "https://products.groupdocs.com/annotation/java/extract/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "https://products.groupdocs.com/annotation/java/extract/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/java/extract/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/java/extract/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/java/extract/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/extract/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/extract/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/java/extract/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/java/extract/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/extract/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/extract/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/java/extract/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/java/extract/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/extract/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/java/extract/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/extract/html/"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/java/extract/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/java/extract/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/java/extract/png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/java/extract/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/java/extract/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/extract/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/java/extract/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/java/extract/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/java/extract/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/java/extract/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/java/extract/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/java/extract/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/java/extract/wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/java/extract/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
