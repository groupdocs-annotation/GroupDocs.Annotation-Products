---
layout: "auto-gen-annotation"
date: 2021-05-13T12:45:05+03:00
draft: false

head_title: "C＃.NETアプリケーションのBMPファイルから注釈を削除する"
head_description: "C＃.NET注釈APIを使用して、一般的な注釈タイプをBMPファイル、画像、図面、およびドキュメントファイル形式に削除します."

title: "C＃でBMPから注釈を削除する"
description: "以前に追加したすべての注釈を、Microsoft Office、画像、Web、図面、およびその他のあらゆる種類の.NETアプリケーションのドキュメントファイル形式から削除します。"
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
        [GroupDocs.Annotation for .NET](/annotation/net/)は、画像やドキュメントファイル形式から注釈を表示、[追加](/annotation/net/add/bmp/)、[変更](/annotation/net/edit/bmp/)、削除、[抽出](/annotation/net/extract/bmp/)するためのネイティブの.NET注釈処理APIです。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Word、Excel、Visioダイアグラム、プレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを簡単に削除できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、カスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "BMPから注釈を削除する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のBMPファイルから注釈の詳細を簡単に削除できます。

        *入力ドキュメントパスまたはストリームを使用してAnnotatorオブジェクトをインスタンス化します。
        * SaveOptionsオブジェクトをインスタンス化し、AnnotationTypes=AnnotationType.Noneを設定します。
        *結果のドキュメントパスまたはストリームとSaveOptionsオブジェクトを使用してSaveメソッドを呼び出します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：Visual Studio、Xamarin、MonoDevelop
        *フレームワーク：.NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.annotation)から最新バージョンのGroupDocs.Annotationfor.NETをダウンロードします。
        
    code: |
        ```cs
        //1-注釈インデックスを使用してドキュメントから注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
        	annotator.Remove(0);
        	annotator.Save("removed.bmp");
        }
        
        //2-注釈オブジェクトを使用してドキュメントから注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp[0]);
        	annotator.Save("removed.bmp");
        }
        
        //3-IDのリストを使用してドキュメントから一部の注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
        	var idList = new List{1, 2, 3};
        	annotator.Remove(idList);
        	annotator.Save("removed.bmp");
        }
        
        //4-注釈のリストを使用してドキュメントからいくつかの注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp);
        	annotator.Save("removed.bmp");
        }
        ```
        
demos:
    enable: true
    title: "アノテーションを削除するライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、今すぐBMPファイルから注釈を削除してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-bmp"
          title: "BMPファイル形式について"
          content: |
            拡張子が.BMPのファイルは、ビットマップデジタル画像の保存に使用されるビットマップ画像ファイルを表します。これらの画像はグラフィックアダプタから独立しており、デバイスに依存しないビットマップ（DIB）ファイル形式とも呼ばれます。この独立性は、MicrosoftWindowsやMacなどの複数のプラットフォームでファイルを開くという目的を果たします。 BMPファイル形式では、データを2次元デジタル画像として、モノクロとさまざまな色深度のカラー形式の両方で保存できます。

          link: "https://docs.fileformat.com/image/bmp/"

more_formats:
    enable: false
    title: "サポートされている他のファイル形式からの注釈の消去"
    content: |
        .NET用のAPIを削除するマルチフォーマットのドキュメントと画像の注釈。以下に示すように、一般的なファイル形式のいくつかから注釈を削除します。
    format: 
          link: "https://products.groupdocs.com/annotation/net/remove/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/net/remove/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/net/remove/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"


          link: "https://products.groupdocs.com/annotation/net/remove/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/net/remove/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/net/remove/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/remove/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/remove/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/net/remove/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/net/remove/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/net/remove/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/net/remove/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/net/remove/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/html/"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/net/remove/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/net/remove/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/net/remove/png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/net/remove/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/remove/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/remove/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/net/remove/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/net/remove/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/net/remove/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/net/remove/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/net/remove/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/net/remove/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/net/remove/wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/net/remove/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
