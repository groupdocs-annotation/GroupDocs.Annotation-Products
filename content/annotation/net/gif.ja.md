---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net GIF 注釈 API C# で注釈を付ける"
head_description: "GIF、画像、図面、ドキュメント ファイル形式から一般的な注釈タイプを作成して注釈を付けるための Net API。"

############################# Header ############################
title: "ネットから GIF に注釈を付ける"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Net API の GroupDocs.Annotation について"
    content: |
        GroupDocs.Annotation for Net API は、Mac、Windows、または Ubuntu 上の PDF、Word、その他のドキュメントに注釈を追加できるライブラリです。 [GroupDocs.Annotation for Net](/annotation/net) は、画像やその他のさまざまなドキュメントからの注釈の作成、追加、編集、削除、抽出、エクスポートを包括的にサポートする注釈管理用のネイティブ Net API です。サポートされているドキュメント形式の完全なリストは、この[ページ](https://docs.groupdocs.com/annotation/net/supported-document-formats/)で確認できます。
        このライブラリを使用すると、GIF ドキュメントだけでなく、Word、Excel、PowerPoint、Outlook 電子メール、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad など、他の多くのタイプのドキュメントでも作業できます。
        GroupDocs.Annotation for Net API を使用すると、新しいメモの作成と追加、注釈の編集、コメントや注釈の抽出、ドキュメントからの削除が可能になります。このライブラリは、テキスト、ポリライン、エリア、下線、点、透かし、矢印、楕円、テキスト置換、距離、テキスト フィールド、PDF、HTML、Microsoft Word ドキュメント、スプレッドシート、図、プレゼンテーション、図面、画像、その他多くのファイル形式。
        例 (以下を参照) は、GIF ドキュメントの操作を示しています。この例では、GroupDocs.Annotation を使用する方法の主な手順を確認できます。ライセンスを設定し、操作したいドキュメントを開き、注釈を追加し、要件に従って注釈プロパティを設定し、結果を必要な場所に保存します。また、サポートされている機能の詳細については、github [ページ](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) または製品 [ドキュメント](https ://docs.groupdocs.com/annotation/net/getting-started/)。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Net で GIF に注釈を追加する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) これにより、ネット開発者は、いくつかの簡単な手順を実装するだけで、ネットベースのアプリケーション内の GIF ファイルにさまざまな注釈タイプを簡単に追加できます。
        *   コメントと日付を含む Reply オブジェクトを作成します。
        *   AreaAnnotation オブジェクトを作成し、エリア オプションを設定し、応答を追加します。
        *   Annotator オブジェクトを作成し、領域の注釈を追加します。
        *   出力ファイルを保存します。
    title_right: "システム要求"
    content_right: |
        Net API の GroupDocs.Annotation は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、次の前提条件がシステムにインストールされていることを確認してください。
        *   オペレーティング システム: Microsoft Windows、Linux、MacOS
        *   開発環境: Visual Studio、Xamarin、MonoDevelop
        *   フレームワーク: .NET Framework、.NET Standard、.NET Core、Mono
        *   [NuGet](https://www.nuget.org/packages/groupdocs.annotation) から .NET 用の GroupDocs.Annotation の最新バージョンをダウンロードします。

############################# Preview ############################
preview_Add:
    enable: true
    title: 注釈のプレビューとコードサンプル
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
    title_left: "Net の GIF から注釈を削除する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) これにより、ネット開発者は、いくつかの簡単な手順を実装することで、ネットベースのアプリケーション内の GIF ファイルから注釈の詳細を簡単に削除できるようになります。
        *   コメントと日付を含む Reply オブジェクトを作成します。
        *   SaveOptions オブジェクトをインスタンス化し、AnnotationTypes = AnnotationType.None を設定します。
        *   結果のドキュメント パスまたはストリームと SaveOptions オブジェクトを使用して save メソッドを呼び出します。

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
    title_left: "Net で GIF から注釈を編集する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) これにより、ネット開発者は、いくつかの簡単な手順を実装することで、ネットベースのアプリケーション内の GIF ファイルからさまざまな注釈プロパティを簡単に更新できるようになります。
        *   ImportAnnotations = true でインスタンス化された LoadOptions を使用して、入力ドキュメント パスまたはストリームを使用して Annotator オブジェクトをインスタンス化します。
        *   AnnotationBase 実装を作成し、存在するアノテーションの ID (その ID を持つアノテーションが見つからない場合は何も変更されません) またはアノテーションのパス リスト (存在するすべてのアノテーションが削除されます) を設定します。
        *   渡されたアノテーションを使用して Annotator オブジェクトの update メソッドを呼び出します。
        *   結果のドキュメント パスまたはストリームと SaveOptions オブジェクトを使用して save メソッドを呼び出します。

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
    title_left: "Net の GIF から注釈を抽出する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) これにより、ネット開発者は、いくつかの簡単な手順を実装することで、ネットベースのアプリケーション内のドキュメントに注釈を付けたり、GIF ファイルから注釈情報を抽出したりすることが簡単になります。
        *   コメントと日付を含む Reply オブジェクトを作成します。
        *   LoadOptions オブジェクトをインスタンス化し、true 引数を指定して SetImportAnnotations を呼び出します。
        *   List型の変数を定義します。
        *   get メソッドを呼び出し、結果を上記の変数に返します。

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
    title: "ドキュメントや画像に注釈を追加、削除、編集、抽出するライブデモ"
    content: |
        [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) Web サイトにアクセスして、今すぐ GIF ファイルに注釈を追加、削除、編集、抽出します。 ライブデモには次のようなメリットがあります

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-gif"
          title: "GIF ファイル形式について"
          content: |
            GIF または Graphical Interchange Format は、高度に圧縮された画像の一種です。 Unisys が所有する GIF は、画質を劣化させない LZW 圧縮アルゴリズムを使用しています。各画像について、GIF では通常、ピクセルあたり最大 8 ビットが許可され、画像全体で最大 256 色が許可されます。 JPEG 画像とは対照的に、JPEG 画像は最大 1,600 万色を表示でき、人間の目の限界にかなり近づいています。インターネットが出現した当時、GIF は低帯域幅を必要とし、色のベタ領域を消費するグラフィックスと互換性があったため、依然として最良の選択肢でした。アニメーション GIF は、多数の画像またはフレームを 1 つのファイルに結合し、それらをシーケンスで表示してアニメーション クリップまたは短いビデオを生成します。色の制限は各フレームで最大 256 であり、カラー グラデーションのある他の画像や写真を再現するのには最も適していないと考えられます。

          link: "https://docs.fileformat.com/image/gif/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "他の一般的なドキュメント形式の使用"
    content: |
        以下に示すように、いくつかの一般的なファイル形式から注釈プロパティを更新します。
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