---
layout: "auto-gen-annotation"
date: 2021-05-13T12:45:05+03:00
draft: false

head_title: "抽出＆amp; C＃.NETのXLSMファイルから注釈をエクスポートする"
head_description: "XLSMファイル、画像、描画、およびドキュメントファイル形式から一般的な注釈タイプを抽出するためのC＃.NET注釈extractionAPI."

title: "C＃でXLSMから注釈を抽出する"
description: "あらゆるタイプのC＃.NETアプリケーションで、Microsoft Office、画像、HTML、図面、およびその他のドキュメントファイル形式から注釈を抽出します。"
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/annotation/net"

submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Annotation for .NET"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: ".NET"

    middle:
        button:

            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "APIリファレンス"

            - link: "https://github.com/groupdocs-annotation"
              text: "コード例"

            - link: "https://products.groupdocs.app/annotation/family"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"

about:
    enable: true
    title: "GroupDocs.Annotation for .NET APIについて"
    content: |
        [GroupDocs.Annotation for .NET](/annotation/net/)は、画像やドキュメントファイル形式から注釈を読み取り、[追加](/annotation/net/add/xlsm/)、[編集](/annotation/net/edit/xlsm/)、[削除](/annotation/net/remove/xlsm/)、抽出、エクスポートするためのネイティブの.NET注釈管理APIです。ユーザーは、コメント、メモ、コメント、およびテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを、PDF、HTML、Microsoft Word文書、Excelスプレッドシート、Visioダイアグラム、PowerPointプレゼンテーション、図面、画像、およびその他の多くのファイル形式から簡単に抽出できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、注釈のカスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "XLSMから注釈を抽出するための手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のXLSMファイルから注釈情報を簡単に抽出できます。

        *入力ドキュメントパスまたはストリームを使用してAnnotatorオブジェクトをインスタンス化します。
        * LoadOptionsオブジェクトをインスタンス化し、ImportAnnotation=trueに設定します。
        *タイプリストで変数を定義します。
        * Getメソッドを呼び出し、結果を上記の変数に返します。
        *タイプListでXmlSerializerオブジェクトをインスタンス化します。
        * FileStreamobjectを使用して、以下の例のようにファイルへの注釈をシリアル化します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：Visual Studio、Xamarin、MonoDevelop
        *フレームワーク：.NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.annotation)から最新バージョンのGroupDocs.Annotationfor.NETをダウンロードします。
        
    code: |
        ```cs
        //この例を使用するには、入力ファイル（ "annotated.xlsm"）に注釈を付ける必要があります
        using (Annotator annotator = new Annotator("annotated.xlsm"))
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
        
demos:
    enable: true
    title: "注釈を抽出するためのライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、XLSMファイルから注釈を今すぐ抽出します。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-xlsm"
          title: "XLSMファイル形式について"
          content: |
            XLSM拡張子の付いたファイルは、マクロをサポートするSpreasheetファイルの一種です。アプリケーションの観点からは、マクロはプロセスの自動化に使用される一連の命令です。マクロは、繰り返し実行されるステップを記録するために使用され、マクロを再度実行することによってアクションの実行を容易にします。マクロは、VisualBasicEditorを使用してExcelワークブック内からMicrosoftのVisualBasicfor Applications（VBA）でプログラムされ、そこから直接実行/デバッグできます。

          link: "https://docs.fileformat.com/spreadsheet/xlsm/"

more_formats:
    enable: false
    title: "サポートされている他のファイル形式からの注釈の抽出"
    content: |
        ドキュメントおよび画像用の.NET注釈抽出API。以下に示すように、いくつかの一般的なファイル形式から注釈をエクスポートします。
    format: 
          link: "https://products.groupdocs.com/annotation/net/extract/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/net/extract/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/net/extract/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/net/extract/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/net/extract/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/net/extract/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"


          link: "https://products.groupdocs.com/annotation/net/extract/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/net/extract/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/net/extract/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/net/extract/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/extract/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/net/extract/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/net/extract/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/extract/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/extract/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/net/extract/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/net/extract/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/extract/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/net/extract/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/extract/html/"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/net/extract/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/net/extract/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/net/extract/png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/net/extract/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/net/extract/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/extract/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/extract/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/net/extract/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/net/extract/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/net/extract/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/net/extract/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/net/extract/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/net/extract/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/net/extract/wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/net/extract/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
