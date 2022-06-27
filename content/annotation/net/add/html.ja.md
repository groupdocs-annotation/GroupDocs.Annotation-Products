---
layout: "auto-gen"
date: 2021-05-13T12:44:50+03:00
draft: false

head_title: "C＃.NETアプリケーションのHTMLファイルに注釈を追加する"
head_description: "C＃.NETアノテーション処理とHTMLファイル、画像、図面、ドキュメントファイル形式に一般的な注釈タイプを追加するための管理API."

title: ".NETのHTMLに注釈を追加する"
description: "テキスト、コメント、メモなど、13種類の注釈を使用して、画像、Microsoft Office、およびその他のドキュメントファイル形式に注釈を付けます。"
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
        [GroupDocs.Annotation for .NET](/annotation/net/)は、ユーザーが画像やドキュメントファイル形式に注釈を追加、編集、削除できるようにするネイティブ.NETAPIです。コメント、メモ、コメント、およびテキスト、グラフィックス、透かしを含むさまざまな注釈タイプをPDF、HTML、Word、Excel、Visioダイアグラム、プレゼンテーション、図面、画像、およびその他の多くのファイル形式に簡単に使用できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、カスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "C＃でHTMLに注釈を追加する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/)を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内からHTMLファイルに注釈プロパティを簡単に追加できます。

        *入力ドキュメントパスまたはストリームを使用してAnnotatorオブジェクトをインスタンス化します。
        *必要なプロパティ（位置、ページ番号など）を使用してTextFieldAnnotationオブジェクトをインスタンス化します。
        * Addメソッドを呼び出し、TextFieldAnnotationオブジェクトを渡します。
        *結果のドキュメントパスまたはストリームを使用してSaveメソッドを呼び出します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：Visual Studio、Xamarin、MonoDevelop
        *フレームワーク：.NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.annotation)から最新バージョンのGroupDocs.Annotationfor.NETをダウンロードします。
        
############################# Preview ############################
preview:
    enable: true
    title: "Annotation preview and code sample"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //ローカルディスクからドキュメントにテキストフィールドの注釈を追加します
        using (Annotator annotator = new Annotator("input.html"))
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
            annotator.Save("result.html");
        }
        ```
        
demos:
    enable: true
    title: "注釈を追加するためのライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、今すぐHTMLファイルに注釈を追加してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-html"
          title: "HTMLファイル形式について"
          content: |
            HTML（ハイパーテキストマークアップ言語）は、ブラウザで表示するために作成されたWebページの拡張機能です。 Webの言語として知られるHTMLは、Webページの一部として表示される新しい情報要件の要件とともに進化してきました。最新のバリアントはHTML5として知られており、言語を操作するための多くの柔軟性を提供します。 HTMLページは、ホストされているサーバーから受信するか、ローカルシステムからロードすることもできます。各HTMLページは、フォーム、テキスト、画像、アニメーション、リンクなどのHTML要素で構成されています。これらの要素は、img、a、pなどのタグで表され、各タグには開始と終了があります。また、JavaScriptやスタイルシート（CSS）などのスクリプト言語で記述されたアプリケーションを埋め込んで、全体的なレイアウトを表現することもできます。

          link: "https://docs.fileformat.com/web/html/"

more_formats:
    enable: false
    title: "他のファイル形式への注釈の追加"
    content: |
        .NET用のマルチフォーマットドキュメントおよび画像注釈処理API。以下に説明するように、一般的なファイル形式のいくつかに注釈を追加します。
    format: 
          link: "https://products.groupdocs.com/annotation/net/add/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/net/add/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/net/add/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/net/add/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/net/add/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/net/add/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"


          link: "https://products.groupdocs.com/annotation/net/add/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/net/add/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/net/add/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/net/add/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/add/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/add/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/net/add/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/net/add/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/add/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/add/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/net/add/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/net/add/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/add/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/net/add/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/add/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/net/add/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/net/add/png/"
          description: "ポータブルネットワークグラフィック"

          link: "https://products.groupdocs.com/annotation/net/add/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/net/add/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/add/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/add/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/net/add/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/net/add/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/net/add/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/net/add/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/net/add/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/net/add/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/net/add/wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/net/add/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
