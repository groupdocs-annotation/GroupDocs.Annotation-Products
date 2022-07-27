---
############################# Static ############################
layout: "product"
date: 2022-07-05T12:44:18+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Net"
platform_tag: "net"

############################# Head ############################
head_title: "NetドキュメントアノテーションAPI| PDF WordExcelPPTX画像の表示と注釈"
head_description: "Netドキュメント注釈API。 PDF Word DOCX、Excel XLSX、PPTX、EML EMLX、VSS VSD、OTP、CAD、および画像ファイル形式の表示、タグ付け、コメント、および注釈付け."

############################# Header ############################
title: "NetAPIを介したドキュメント注釈"
description: "外部ソフトウェアをインストールせずに、PDF、HTML、MS Office、およびその他のドキュメント形式を表示および注釈付けする機能を備えたNetアプリケーションを構築します."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Net"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            - link: "#overview"
              text: "概要"

            - link: "#features"
              text: "特徴"

            - link: "#support"
              text: "サポート"

            - link: "https://products.groupdocs.app/annotation"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation Net APIは、Android、MacOS、Linux、Windowsなどのさまざまなプラットフォームやオペレーティングシステムでドキュメントの注釈を操作できるようにする製品です。 GroupDocs.Annotationは、多くの利点を提供するシンプルなAPIを備えたライブラリを提供します。たとえば、データの機密性を維持する必要がある場合、ライブラリを操作するために必要な電力を選択する必要がある場合、または注釈を使用して作業を部分的に変更する必要がある場合、ライブラリは非常に優れています。軽量で柔軟性があります。

        GroupDocs.Annotation for Net APIを使用すると、テキスト、ポリライン、エリア、アンダーライン、ポイント、透かし、矢印、楕円、テキスト置換、距離、テキストフィールド、リソース編集などのさまざまな種類の注釈を操作できます。 。また、PDF、HTML、Microsoft Office Word、Excelスプレッドシート、PowerPointプレゼンテーション、Visio、Outlook電子メール、画像、メタファイル、CAD描画、その他のさまざまな形式など、最も一般的なドキュメント形式をサポートしています。 APIは、ドキュメントページのサムネイルを取得する機能を提供し、PDFファイルとの間の注釈のインポートとエクスポートをサポートします。

        ライブラリを使用して、[追加]（/annotation/net/add/bmp/）、[編集]（/annotation/net/edit/bmp/）、[エキス]（/annotation/net/extract/bmp/） および[消去]（/annotation/net/remove/bmp/） ドキュメントからの注釈、ドキュメントのローテーション、サムネイルソリューションの変更、これはすべての可能性の完全なリストではありません。また、サポートされているすべてのドキュメント形式内の要件に従って注釈プロパティをカスタマイズするための包括的なデータオブジェクトのセットも提供します。

        Net APIのGroupDocs.Annotationの操作は非常に簡単で、いくつかの基本的な手順で構成されています。最初にライセンスを設定し、次に操作するファイルを選択し、ドキュメントの注釈（削除/編集/抽出/削除）を使用して何らかの方法で操作し、結果を保存する必要があります。詳細については、製品の[ドキュメント]（https://docs.groupdocs.com/annotation/net/getting-started/） または[例]（https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net） セット。

        GroupDocs.Annotationは定期的に更新され、お客様をサポ​​ートします。いつでも質問したり、アイデアを送信したり、新しいもののニーズについて教えてください。新しいバージョンで喜んで実装します。
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          以下は、Net用のGroupDocs.Annotationの概要です。
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "概要"
          content: |
            *注釈を追加
            *注釈のエクスポート
            *注釈のインポート
            *返信ベースのコメント
            *注釈の互換性
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation for Netは、Microsoft Office、PDF、画像など、一般的な[ドキュメントファイル形式]（https://docs.groupdocs.com/annotation/net/supported-document-formats/）をすべてサポートしています。
        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: [DOC](/annotation/net/add/doc/), [DOCX](/annotation/net/add/docx/), [DOCM](/annotation/net/add/docm/), [DOT](/annotation/net/add/dot/), [DOTX](/annotation/net/add/dotx/), [RTF](/annotation/net/add/rtf/)
                * **Excel**: [XLS](/annotation/net/add/xls/), [XLSX](/annotation/net/add/xlsx/), [XLSB](/annotation/net/add/xlsb/), [XLSM](/annotation/net/add/xlsm/)
                * **PowerPoint**: [PPT](/annotation/net/add/ppt/), [PPTX](/annotation/net/add/pptx/), [PPS](/annotation/net/add/pps/), [PPSX](/annotation/net/add/ppsx/), [POTM](/annotation/net/add/potm/), [POTX](/annotation/net/add/potx/), [PPSM](/annotation/net/add/ppsm/), [PPTM](/annotation/net/add/pptm/), [WMF](/annotation/net/add/wmf/), [EMF](/annotation/net/add/emf/)
                * **Outlook**: [EML](/annotation/net/add/eml/), [EMLX](/annotation/net/add/emlx/), [MSG](/annotation/net/add/msg/)
                * **Visio**: [VSS](/annotation/net/add/vss/), [VST](/annotation/net/add/vst/), [VSD](/annotation/net/add/vsd/), [VSDX](/annotation/net/add/vsdx/), [VSX](/annotation/net/add/vsx/)

        right:
          enable: true
          table:
            # table loop
            - title: "その他のフォーマット"
              content: |
                * **Portable**: [PDF](/annotation/net/add/pdf/) (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: [ODT](/annotation/net/add/odt/), [ODS](/annotation/net/add/ods/), [ODP](/annotation/net/add/odp/)
                * **Images**: [BMP](/annotation/net/add/bmp/), [JPG](/annotation/net/add/jpg/), [JPEG](/annotation/net/add/jpeg/), [TIFF](/annotation/net/add/tiff/), [TIF](/annotation/net/add/tif/), [PNG](/annotation/net/add/png/), [GIF](/annotation/net/add/gif/), [DCM](/annotation/net/add/dcm/), [DICOM](/annotation/net/add/dicom/)
                * **AutoCAD**: [DWG](/annotation/net/add/dwg/), [DXF](/annotation/net/add/dxf/), [CAD](/annotation/net/add/cad/)
                * **Other**: [HTM](/annotation/net/add/htm/), [HTML](/annotation/net/add/html/), [CSV](/annotation/net/add/csv/), [DJVU](/annotation/net/add/djvu/), [OTP](/annotation/net/add/otp/), [OTT](/annotation/net/add/ott/)

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Netは、次のオペレーティングシステム、フレームワーク、およびパッケージマネージャーをサポートしています。
      
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                * Windowsデスクトップ（x86およびx64）
                * Windows Server（x86およびx64）
                * Windows Azure
                * Linux
                * マックOS

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * .NET Standard 2.0
                * .NETFramework2.0以降
                * .NETCore2.0以降
                * MonoFramework1.2以降

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "パッケージマネージャー"
              content: |
                * NuGet
            
            - icon: "fas fa-tools"
              title: "開発環境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Annotation for Net Features"

    feature:
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: "注釈と返信の追加、編集、削除"

      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: "注釈をドキュメントにエクスポート"

      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/net/evaluation-limitations-and-licensing-of-groupdocs-annotation/"
        content: "従量制ライセンス–APIの使用状況に応じて支払うことで請求を管理"
      
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/net/extract-annotations-from-document/"
        content: "ドキュメントのすべての注釈を取得するための単一の関数呼び出し"

      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: "ポイント注釈に値を割り当てるか、既存のポイント値を移動します"

      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/net/add-link-annotation/"
        content: "PDF、Word、PowerPointのスライドにリンク注釈を追加する"

      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/net/basic-usage/"
        content: "注釈の背景色を設定するか、ドキュメントからすべての注釈を削除します"

      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: "正確にPDFファイルに注釈を付ける–PDFドキュメントの画像表現とキャッシュページプレビューを取得"

      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/import-annotations/"
        content: "ドキュメントの画像表現でテキスト注釈のテキスト座標を取得する"

      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: "ユーザーコメントをエリアアノテーションとネストされたコメントのサポートにリンクする"

      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/net/add-arrow-annotation/"
        content: "特定のコンテンツを指すために矢印注釈を使用する"

      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/net/add-distance-annotation/"
        content: "距離注釈を使用して、オブジェクト間の距離を表す線を描画します"

      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/net/add-point-annotation/"
        content: "クリックするとウィンドウがポップしてコメントが追加されるポイントベースの注釈"

      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/net/add-polyline-annotation/"
        content: "ポリライン注釈として作成された線分の接続シーケンスを作成します"

      - icon: "fas fa-lock"
        link: "https://docs.groupdocs.com/annotation/net/add-ellipse-annotation/"
        content: "直線セグメント、円弧セグメント、または両方の組み合わせを作成します"

      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/net/add-area-annotation/"
        content: "改訂の提案されたドキュメント領域にマークを付ける"
      
      - icon: "fas fa-fill-drip"
        link: "https://docs.groupdocs.com/annotation/net/add-image-annotation/"
        content: "PDF、図、Word、Excel、プレゼンテーション、画像に画像注釈を追加する"

      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: "ドキュメントにテキストフィールドとテキストベースのスタンプまたは透かしを追加する"

      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/net/add-annotation-to-the-document/"
        content: "ドキュメント内の特定のテキストを取り消し線、下線、または置換"

      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/net/update-annotations/"
        content: "新しい高さと幅のパラメータを割り当てて、注釈のサイズを変更します"

      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/net/generate-document-pages-preview/"
        content: "ドキュメントページのサムネイルを取得します。画像と図のさまざまな注釈付きドキュメントを管理する"

      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/export-annotations/"
        content: "複数ページのTIFFファイルに注釈をエクスポートして操作する"
  
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-watermark-annotation/"
        content: "透かし注釈の垂直方向と水平方向の配置を調整する"
  
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/add-text-field-annotation/"
        content: "テキストフィールドのテキストの水平方向の配置を追加する"

      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/net/document-text-info/"
        content: "ドキュメントのテキスト行（テキスト、幅、高さ、インデント）に関する情報を取得します"

    more_feature:
      - title: "複数のタイプの注釈のサポート"
        content: |
          GroupDocs.Annotation for .NETを使用すると、さまざまなタイプの注釈を操作できます。これにより、タスクでチームと協力しながら、コミュニケーションの自由と容易さが得られます。エリア注釈（エリアを長方形としてマークしてメモを追加）、ポイント注釈（ドキュメント内の任意のポイントにコメントを貼り付ける）、テキスト注釈（選択したテキストにコメントを追加）、取り消し線/下線注釈（段落に適用）、ポリライン注釈（図形とフリーハンドの線を描画）、矢印注釈（コメントが添付された矢印ポインター）、楕円注釈（楕円内にテキストを表示）、距離注釈（オブジェクト間の距離を表す線を描画）、リンク注釈（サポートされているドキュメント形式へのWebリンクを追加）、および注釈（テキストスタンプまたは透かしをドキュメントに追加できます）。

          ```cs
          //AnnotationInfoのリストを初期化します
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          //テキスト注釈を初期化します
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          //リストに注釈を追加します
          annotations.Add(textAnnotation);
          //入力ファイルストリームを取得します
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          //注釈をエクスポートし、出力ファイルを保存します
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotationは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Annotation for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-annotation-java.png"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---