---
layout: "auto-gen-child"
date: 2021-05-13T12:45:09+03:00
draft: false

head_title: "C＃.NETアプリケーションのPPSXファイルから注釈を削除する"
head_description: "一般的な注釈タイプをPPSXファイル、画像、描画、およびドキュメントファイル形式に削除するC＃.NET注釈API."

title: "C＃でPPSXから注釈を削除する"
description: "以前に追加したすべての注釈を、Microsoft Office、画像、Web、図面、およびその他のあらゆる種類の.NETアプリケーションのドキュメントファイル形式から削除します。."
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
        [GroupDocs.Annotation for .NET](/annotation/net/）は、画像やドキュメントファイル形式から注釈を表示、追加、変更、削除、抽出するためのネイティブの.NET注釈処理APIです。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Word、Excel、Visioダイアグラム、プレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを簡単に削除できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、カスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "PPSXから注釈を削除する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/）を使用すると、.NET開発者は、いくつかの簡単な手順を実装することで、アプリケーション内のPPSXファイルから注釈の詳細を簡単に削除できます。

        *入力ドキュメントパスまたはストリームを使用してAnnotatorオブジェクトをインスタンス化します。
        * SaveOptionsオブジェクトをインスタンス化し、AnnotationTypes=AnnotationType.Noneを設定します。
        *結果のドキュメントパスまたはストリームとSaveOptionsオブジェクトを使用してSaveメソッドを呼び出します。
        
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for .NET APIは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。以下のコードを実行する前に、システムに次の前提条件がインストールされていることを確認してください。

        *オペレーティングシステム：Microsoft Windows、Linux、MacOS
        *開発環境：Visual Studio、Xamarin、MonoDevelop
        *フレームワーク：.NET Framework、.NET Standard、.NET Core、Mono
        * [NuGet](https://www.nuget.org/packages/groupdocs.annotation）から最新バージョンのGroupDocs.Annotationfor.NETをダウンロードします。
        
    code: |
        ```cs
        //1-注釈インデックスを使用してドキュメントから注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.ppsx"))
        {
        	annotator.Remove(0);
        	annotator.Save("removed.ppsx");
        }
        
        //2-注釈オブジェクトを使用してドキュメントから注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.ppsx"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp[0]);
        	annotator.Save("removed.ppsx");
        }
        
        //3-IDのリストを使用してドキュメントから一部の注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.ppsx"))
        {
        	var idList = new List{1, 2, 3};
        	annotator.Remove(idList);
        	annotator.Save("removed.ppsx");
        }
        
        //4-注釈のリストを使用してドキュメントからいくつかの注釈を削除する方法
        
        using (Annotator annotator = new Annotator("result.ppsx"))
        {
        	var tmp = annotator.Get();
        	annotator.Remove(tmp);
        	annotator.Save("removed.ppsx");
        }
        ```
        
demos:
    enable: true
    title: "アノテーションを削除するライブデモ"
    content: |
        [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family）Webサイトにアクセスして、今すぐPPSXファイルから注釈を削除してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-ppsx"
          title: "PPSXファイル形式について"
          content: |
            PPSX、パワーポイントスライドショー、ファイルは、スライドショーの目的でMicrosoft PowerPoint2007以降を使用して作成されます。これは、Microsoft PowerPoint97-2003バージョンでサポートされていたPPSファイル形式の更新です。 PPSXファイルを別のユーザーと共有して開くと、編集可能モードで開くPPTXファイルとは異なり、PowerPointの表示として起動します。スライドショーの順序は、元のプレゼンテーションと同じです。スライドショー中のPPSXへのプレゼンテーションスライドには、すべてのスライドに画像、音声、その他の埋め込みメディアが付属しています。

          link: "https://docs.fileformat.com/presentation/ppsx/"

more_formats:
    enable: true
    title: "サポートされている他のファイル形式からの注釈の消去"
    content: |
        .NET用のAPIを削除するマルチフォーマットのドキュメントと画像の注釈。以下に示すように、一般的なファイル形式のいくつかから注釈を削除します。
    format: 
          link: "https://products.groupdocs.com/annotation/net/remove/pdf/"
          description: "Adobe Portableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/net/remove/doc/"
          description: "Microsoft Wordドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/docm/"
          description: "Microsoft Wordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/docx/"
          description: "Microsoft Word OpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/dot/"
          description: "Microsoft Word文書テンプレート"

          link: "https://products.groupdocs.com/annotation/net/remove/dotx/"
          description: "Word OpenXMLドキュメントテンプレート"

          link: "https://products.groupdocs.com/annotation/net/remove/dotm/"
          description: "Microsoft Wordマクロ対応テンプレート"

          link: "https://products.groupdocs.com/annotation/net/remove/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/net/remove/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/net/remove/xls/"
          description: "Microsoft Excelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/net/remove/xlsx/"
          description: "Microsoft Excel OpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/remove/xlsm/"
          description: "Microsoft Excelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/net/remove/xlsb/"
          description: "Microsoft Excelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/net/remove/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/net/remove/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/pptx/"
          description: "PowerPoint OpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/potm/"
          description: "Microsoft PowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/net/remove/pptm/"
          description: "Microsoft PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/net/remove/pps/"
          description: "Microsoft PowerPoint97-2003スライドショー"

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

          link: "https://products.groupdocs.com/annotation/net/remove/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/net/remove/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/remove/msg/"
          description: "Microsoft Outlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/net/remove/vsd/"
          description: "Microsoft Visio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/net/remove/vsdx/"
          description: "Microsoft Visio図面"

          link: "https://products.groupdocs.com/annotation/net/remove/vss/"
          description: "Microsoft Visio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/net/remove/vst/"
          description: "Microsoft Visio2013ステンシル"

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
