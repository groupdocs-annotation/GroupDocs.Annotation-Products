---
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:45+03:00
draft: false

head_title: "JavaアプリケーションでPDFから注釈を削除する"
head_description: "PDF、画像、図面、ドキュメントファイル形式から一般的な注釈タイプを削除するJavaannotation API."

title: "JavaでPDFから注釈を削除する"
description: "あらゆるタイプのJavaアプリケーションで、Microsoft Office、画像、図面、HTML、およびその他のドキュメントファイル形式からすでに追加されている注釈を削除します."
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
        [GroupDocs.Annotation for Java](/annotation/java/)は、画像やドキュメントファイル形式から注釈を表示、[追加](/annotation/java/add/pdf/)、[更新](/annotation/java/edit/pdf/)、消去、[抽出](/annotation/java/extract/pdf/)、またはエクスポートするためのネイティブJava注釈管理ライブラリです。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Word、Excel、Visioダイアグラム、プレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを簡単に削除できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、カスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "JavaでPDFから注釈を削除する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、Javaベースのアプリケーション内のPDFファイルから注釈の詳細を簡単に削除できます。

        *コメントと日付を使用して返信オブジェクトを作成します。
        * SaveOptionsオブジェクトをインスタンス化し、AnnotationTypes=AnnotationType.Noneを設定します。
        *結果のドキュメントパスまたはストリームとSaveOptionsオブジェクトを使用してsaveメソッドを呼び出します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for Java APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：NetBeans、Intellij IDEA、Eclipseなど
        * Javaランタイム環境：Java 7（1.7）以降
        * [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)から最新バージョンのGroupDocs.AnnotationforJavaを入手してください。
        
    code: |
        ```java
        Annotator annotator = new Annotator("C://input.pdf");
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);
        annotator.save("C://output.pdf", saveOptions);
        annotator.dispose();
        ```
        
demos:
    enable: true
    title: "ドキュメントや画像から注釈を削除するライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、PDFファイルから注釈を表示および削除してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-pdf"
          title: "PDFファイル形式について"
          content: |
            Portable Document Format（PDF）は、1990年代にAdobeによって作成されたドキュメントの一種です。このファイル形式の目的は、アプリケーションソフトウェア、ハードウェア、およびオペレーティングシステムに依存しない形式で、ドキュメントやその他の参照資料を表現するための標準を導入することでした。 PDFファイルは、拡張機能/プラグインを介して、Adobe Acrobat Reader / Writerでも、Chrome、Safari、Firefoxなどの最新のブラウザーでも開くことができます。市販のソフトウェアスイートのほとんどは、追加のソフトウェアコンポーネントを必要とせずに、ドキュメントをPDFファイル形式に変換することもできます。したがって、PDFファイル形式には、テキスト、画像、ハイパーリンク、フォームフィールド、リッチメディア、デジタル署名、添付ファイル、メタデータ、地理空間機能、ソースドキュメントの一部として使用できる3Dオブジェクトなどの情報を含めることができます。

          link: "https://docs.fileformat.com/view/pdf/"

more_formats:
    enable: false
    title: "他の一般的なファイル形式からの注釈の編集"
    content: |
        ドキュメントおよび画像ファイル形式から注釈を削除するJavaAPI。以下に示すように、一般的なファイル形式のいくつかから注釈プロパティを消去します。
    format: 
          link: "https://products.groupdocs.com/annotation/java/remove/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/java/remove/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/java/remove/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/java/remove/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/java/remove/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"


          link: "https://products.groupdocs.com/annotation/java/remove/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/java/remove/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/java/remove/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/java/remove/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/remove/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/remove/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/java/remove/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/java/remove/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/remove/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/remove/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/java/remove/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/java/remove/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/remove/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/java/remove/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/remove/html/"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/java/remove/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/java/remove/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/java/remove/png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/java/remove/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/java/remove/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/remove/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/remove/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/java/remove/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/java/remove/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/java/remove/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/java/remove/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/java/remove/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/java/remove/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/java/remove/wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/java/remove/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
