---
layout: "auto-gen-annotation"
date: 2021-05-13T12:44:59+03:00
draft: false

head_title: "読む＆amp; C＃.NETアプリケーションでWMFファイルの注釈を編集する"
head_description: "一般的な注釈タイプをWMFファイル、画像、描画、およびドキュメントファイル形式に更新するC＃.NET注釈エディターAPI."

title: ".NETのWMFファイルの注釈を編集する"
description: ".画像、Microsoft Office、その他のドキュメントファイル形式用のNET注釈エディタ。次のような13種類の注釈を使用してドキュメントに注釈を付けます。エリア、テキスト、メモ、透かしなど."
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
        [GroupDocs.Annotation for .NET](/annotation/net/)は、ネイティブの.NET注釈管理およびエディターAPIであり、画像およびドキュメントファイル形式から注釈を読み取り、[追加](/annotation/net/add/wmf/)、更新、[削除](/annotation/net/remove/wmf/)、および[抽出](/annotation/net/extract/wmf/)します。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Word、Excel、Visioダイアグラム、プレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを簡単に更新できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、カスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "C＃でWMFから注釈を編集する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のWMFファイルから注釈の詳細を簡単に編集できます。

        *入力ドキュメントパスまたはストリームを使用してAnnotatorオブジェクトをインスタンス化します。
        * AnnotationBase実装を作成し、既存の注釈のID（そのIDを持つ注釈が見つからない場合、何も変更されない）または注釈のパスリスト（既存の注釈はすべて削除されます）を設定します。
        *渡されたアノテーションを使用してAnnotatorオブジェクトのUpdateメソッドを呼び出します。
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
        //注釈付きドキュメントを開きます
        using (Annotator annotator = new Annotator("result.wmf"))
        {
        	//既存のアノテーションのいくつかのプロパティを変更すると仮定します
                AreaAnnotation updated = new AreaAnnotation
                	{
                            //既存のアノテーションIDを設定することが重要です
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
                //アノテーションを更新します
                annotator.Update(updated);
                annotator.Save("result.wmf");
        }
        ```
        
demos:
    enable: true
    title: "注釈を更新するためのライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、WMFファイルの注釈を今すぐ編集してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-wmf"
          title: "WMFファイル形式について"
          content: |
            WMF拡張子の付いたファイルは、ベクターおよびビットマップ形式の画像データを格納するためのMicrosoft Windowsメタファイル（WMF）を表します。より正確に言うと、WMFは、デバイスに依存しないグラフィックスファイル形式のベクターファイル形式カテゴリに属しています。 Windowsグラフィックデバイスインターフェイス（GDI）は、WMFファイルに格納されている関数を使用して、画面に画像を表示します。拡張メタファイル（EMF）として知られるWMFのより拡張されたバージョンは、フォーマットをより豊富な機能にするために後で公開されました。実際には、WMFはSVGに似ています。

          link: "https://docs.fileformat.com/image/wmf/"

more_formats:
    enable: false
    title: "他のファイル形式での注釈の編集"
    content: |
        .NET用のマルチフォーマットドキュメントおよび画像注釈エディタAPI。以下に示すように、いくつかの一般的なファイル形式から注釈を更新します。
    format: 
          link: "https://products.groupdocs.com/annotation/net/edit/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/net/edit/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/net/edit/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/net/edit/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/net/edit/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/net/edit/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"

          link: "https://products.groupdocs.com/annotation/net/edit/dotm/"
          description: "MicrosoftWordマクロ対応テンプレート"

          link: "https://products.groupdocs.com/annotation/net/edit/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/net/edit/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/net/edit/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/net/edit/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/edit/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/edit/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/net/edit/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/net/edit/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/edit/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/edit/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/net/edit/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/net/edit/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/edit/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/net/edit/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/edit/html/"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/net/edit/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/net/edit/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/net/edit/png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/net/edit/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/net/edit/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/edit/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/edit/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/net/edit/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/net/edit/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/net/edit/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/net/edit/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/net/edit/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/net/edit/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/net/edit/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
