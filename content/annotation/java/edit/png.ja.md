---
layout: "auto-gen"
date: 2021-05-13T12:44:32+03:00
draft: false

head_title: "JavaアプリケーションでPNGファイルの注釈を編集する"
head_description: "PNG、画像、図面、ドキュメントファイル形式から一般的な注釈タイプを更新するJava注釈エディタAPI."

title: "JavaでPNGファイルの注釈を編集する"
description: "画像、Microsoft Office、その他のドキュメントファイル形式用のJava注釈エディタ。次のような13種類の注釈を使用してPNGファイルに注釈を付けます。エリア、テキスト、メモ、透かしなど."
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
        [GroupDocs.Annotation for Java](/annotation/java/)は、画像やドキュメントファイル形式から注釈を効率的に表示、追加、更新、削除、抽出するためのネイティブJava注釈操作ソリューションです。ユーザーは、コメント、メモ、コメント、およびPDF、HTML、Word、Excel、Visioダイアグラム、プレゼンテーション、図面、画像、およびその他の多くのファイル形式のテキスト、グラフィックス、透かしなどのさまざまな注釈タイプを簡単に編集できます。注釈処理機能は、インポートされたドキュメントから注釈を正確に読み取ることができ、カスタマイズを実装した後、元のファイル形式または目的のファイル形式にエクスポートして戻すことができます。

steps:
    enable: true
    title_left: "JavaでPNGから注釈を編集する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/)を使用すると、Java開発者は、いくつかの簡単な手順を実装することで、Javaベースのアプリケーション内のPNGファイルからさまざまな注釈プロパティを簡単に更新できます。

        *入力ドキュメントパスでAnnotatorオブジェクトをインスタンス化するか、ImportAnnotations=trueでインスタンス化されたLoadOptionsでストリームをインスタンス化します。
        * AnnotationBase実装を作成し、既存の注釈のID（そのIDを持つ注釈が見つからない場合、何も変更されない）または注釈のパスリスト（既存の注釈はすべて削除されます）を設定します。
        *渡されたアノテーションを使用してAnnotatorオブジェクトのupdateメソッドを呼び出します。
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
        String outputPath = "UpdateAnnotation.png";
        Annotator annotator = new Annotator("input.png");
        
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        //元の注釈を追加します
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        loadOptions.setImportAnnotations(true);
        
        //注釈付きドキュメントを開きます
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);
        
        //既存のアノテーションのいくつかのプロパティを変更したいことを提案します
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        //アノテーションを更新します
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```
        
demos:
    enable: true
    title: "ドキュメントや画像から注釈を変更するためのライブデモ"
    content: |
        [GroupDocs.Annotationライブデモ](https://products.groupdocs.app/annotation/family)サイトにアクセスして、PNGファイルから注釈を今すぐ読んで編集してください。  
        ライブデモには次の利点があります
        
about_formats:
    enable: true
    format:
        - icon: "far fa-file-png"
          title: "PNGファイル形式について"
          content: |
            PNG（Portable Network Graphics）は、ロスレス圧縮を使用するラスターイメージファイル形式の一種を指します。このファイル形式は、Graphics Interchange Format（GIF）の代わりとして作成されたものであり、著作権の制限はありません。ただし、PNGファイル形式はアニメーションをサポートしていません。 PNGファイル形式は、ユーザーの間で人気のあるロスレス画像圧縮をサポートしています。時間の経過とともに、PNGは最もよく使用される画像ファイル形式の1つとして進化してきました。ほとんどすべてのオペレーティングシステムは、PNGファイルを開くことをサポートしています。たとえば、Microsoft Windowsビューアには、OSがデフォルトでインストールの一部として利用可能なサポートを備えているため、PNGファイルを開く機能があります。

          link: "https://docs.fileformat.com/image/png/"

more_formats:
    enable: false
    title: "他の一般的なファイル形式からの注釈の編集"
    content: |
        ドキュメントおよび画像形式用のJava注釈エディタAPI。以下に示すように、一般的なファイル形式のいくつかから注釈プロパティを更新します。
    format: 
          link: "https://products.groupdocs.com/annotation/java/edit/pdf/"
          description: "AdobePortableドキュメント形式"

          link: "https://products.groupdocs.com/annotation/java/edit/doc/"
          description: "MicrosoftWordドキュメント"

          link: "https://products.groupdocs.com/annotation/java/edit/docm/"
          description: "MicrosoftWordマクロ対応ドキュメント"

          link: "https://products.groupdocs.com/annotation/java/edit/docx/"
          description: "Microsoft WordOpenXMLドキュメント"

          link: "https://products.groupdocs.com/annotation/java/edit/dot/"
          description: "MicrosoftWord文書テンプレート"

          link: "https://products.groupdocs.com/annotation/java/edit/dotx/"
          description: "WordOpenXMLドキュメントテンプレート"


          link: "https://products.groupdocs.com/annotation/java/edit/rtf/"
          description: "リッチテキストドキュメント"

          link: "https://products.groupdocs.com/annotation/java/edit/odt/"
          description: "ドキュメントテキストを開く"

          link: "https://products.groupdocs.com/annotation/java/edit/xls/"
          description: "MicrosoftExcelバイナリファイル形式"

          link: "https://products.groupdocs.com/annotation/java/edit/xlsx/"
          description: "Microsoft ExcelOpenXMLスプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/edit/xlsm/"
          description: "MicrosoftExcelマクロ対応スプレッドシート"

          link: "https://products.groupdocs.com/annotation/java/edit/xlsb/"
          description: "MicrosoftExcelバイナリワークシート"

          link: "https://products.groupdocs.com/annotation/java/edit/ods/"
          description: "ドキュメントスプレッドシートを開く"

          link: "https://products.groupdocs.com/annotation/java/edit/ppt/"
          description: "PowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/edit/pptx/"
          description: "PowerPointOpenXMLプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/edit/ppsx/"
          description: "PowerPointOpenXMLスライドショー"

          link: "https://products.groupdocs.com/annotation/java/edit/potm/"
          description: "MicrosoftPowerPointテンプレート"

          link: "https://products.groupdocs.com/annotation/java/edit/pptm/"
          description: "MicrosoftPowerPointプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/edit/pps/"
          description: "MicrosoftPowerPoint97-2003スライドショー"

          link: "https://products.groupdocs.com/annotation/java/edit/odp/"
          description: "OpenDocumentプレゼンテーション"

          link: "https://products.groupdocs.com/annotation/java/edit/html/"
          description: "ハイパーテキストマークアップ言語"

          link: "https://products.groupdocs.com/annotation/java/edit/tiff/"
          description: "タグ付き画像ファイル形式"

          link: "https://products.groupdocs.com/annotation/java/edit/jpeg/"
          description: "JPEG画像"

          link: "https://products.groupdocs.com/annotation/java/edit/bmp/"
          description: "ビットマップファイル形式"

          link: "https://products.groupdocs.com/annotation/java/edit/eml/"
          description: "電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/edit/msg/"
          description: "MicrosoftOutlookの電子メールメッセージ"

          link: "https://products.groupdocs.com/annotation/java/edit/vsd/"
          description: "MicrosoftVisio2003-2010図面"

          link: "https://products.groupdocs.com/annotation/java/edit/vsdx/"
          description: "MicrosoftVisio図面"

          link: "https://products.groupdocs.com/annotation/java/edit/vss/"
          description: "MicrosoftVisio2003-2010ステンシル"

          link: "https://products.groupdocs.com/annotation/java/edit/vst/"
          description: "MicrosoftVisio2013ステンシル"

          link: "https://products.groupdocs.com/annotation/java/edit/dwg/"
          description: "Autodesk Design Data Formats"

          link: "https://products.groupdocs.com/annotation/java/edit/dxf/"
          description: "AutoCAD Drawing Interchange"

          link: "https://products.groupdocs.com/annotation/java/edit/dcm/"
          description: "医学におけるデジタルイメージングと通信"

          link: "https://products.groupdocs.com/annotation/java/edit/wmf/"
          description: "Windowsメタファイル"

          link: "https://products.groupdocs.com/annotation/java/edit/emf/"
          description: "強化されたメタファイル形式"


back_to_top:
    enable: true
---
