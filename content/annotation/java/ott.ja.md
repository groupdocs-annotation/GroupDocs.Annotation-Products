
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/ott"/>

############################# Head ############################
head_title: "Java アプリケーションの 削除 注釈 から OTT"
head_description: "Java API と 削除 の一般的な注釈タイプ から OTT、画像、図面、ドキュメント ファイル形式を作成します。"

############################# Header ############################
title: "注釈を付ける OTT から Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "Java の GroupDocs.Annotation"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-java.png"
        product: "GroupDocs.Annotation"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/java"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Java API の GroupDocs.Annotation について"
    content: |
        GroupDocs.Annotation for Java API は、Mac、Windows、または Ubuntu 上の PDF、Word、その他のドキュメントに注釈を追加できるライブラリです。 [GroupDocs.Annotation for Java](/annotation/java) は、注釈を管理するためのネイティブ Java API であり、注釈の作成、追加、編集、削除、抽出、エクスポートを包括的にサポートしています。画像やその他のさまざまなドキュメント。サポートされているドキュメント形式の完全なリストは、この [ページ](https://docs.groupdocs.com/annotation/java/supported-document-formats/) で確認できます。

        このライブラリを使用すると、OTT ドキュメントだけでなく、Word、Excel、PowerPoint、Outlook 電子メール、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad など、他の多くのタイプのドキュメントでも作業できます。

        GroupDocs.Annotation for Java API を使用すると、新しいメモ、エディット 注釈、抜粋 を作成および追加できます。コメント、注釈をドキュメントから 削除 します。このライブラリは、テキスト、ポリライン、エリア、下線、点、透かし、矢印、楕円、テキスト置換、距離、テキスト フィールド、PDF、HTML、Microsoft Word ドキュメント、スプレッドシート、図、プレゼンテーション、図面、画像、その他多くのファイル形式。

        例 (下記を参照) は、OTT ドキュメントの操作を示しています。この例では、GroupDocs.Annotation を使用する方法の主な手順を確認できます。ライセンスを設定し、操作したいドキュメントを開き、注釈を追加し、要件に従って注釈プロパティを設定し、結果を必要な場所に保存します。また、サポートされている機能の詳細については、github [ページ](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) または製品  で確認できます。 [ドキュメント](https://docs.groupdocs.com/annotation/java/getting-started/)。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java に注釈 から OTT を追加する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) これにより、Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の OTT ファイルにさまざまな注釈タイプを簡単に追加できます。
        * コメントと日付を含む Reply オブジェクトを作成します。
        * AreaAnnotation オブジェクトを作成し、エリア オプションを設定し、応答を追加します。
        * Annotator オブジェクトを作成し、エリア アノテーションを追加します。
        * 出力ファイルを保存します。
    title_right: "システム要求"
    content_right: |
        Java API の GroupDocs.Annotation は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、次の前提条件がシステムにインストールされていることを確認してください。
        * オペレーティング システム: Microsoft Windows、Linux、MacOS
        * 開発環境: NetBeans、Intellij IDEA、Eclipse など
        * Java 実行環境: Java 7 (1.7) 以降
        * Java 用 GroupDocs.Annotation の最新バージョンを [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) から入手します。

############################# Preview ############################
preview_Add:
    enable: true
    タイトル: 「アノテーションのプレビューとコードサンプル」
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // クラスのインスタンスを作成し、コメントを追加します
        Reply firstReply = new Reply();
        firstReply.setComment("最初のコメント");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply SecondReply = new Reply();
        SecondReply.setComment("2 番目のコメント");
        SecondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(2番目の返信);
        
        // AreaAnnotation クラスのインスタンスを作成し、オプションを設定します
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("これはエリアの注釈です");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Annotator クラスのインスタンスを作成する
        Annotator annotator = new Annotator("input.bmp");
        
        // アノテーションを追加します
        annotator.add(area);
        
        // ファイルに保存
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Java の注釈 から OTT を削除する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) これにより、Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の OTT ファイルから注釈の詳細を簡単に削除できるようになります。
        * コメントと日付を含む Reply オブジェクトを作成します。
        * SaveOptions オブジェクトをインスタンス化し、AnnotationTypes = AnnotationType.None を設定します。
        * 結果のドキュメント パスまたはストリームと SaveOptions オブジェクトを使用して save メソッドを呼び出します。

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```ジャバ
        // Annotator クラスのインスタンスを作成する
        Annotator annotator = new Annotator("C://input.bmp");

        // セットタイプによるアノテーションの削除 None
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // アノテーションを出力ファイルに保存
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();;
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "{{プラットフォーム}} で注釈 から OTT を編集する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) これにより、Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の OTT ファイルからさまざまな注釈プロパティを簡単に更新できるようになります。
        * ImportAnnotations = true でインスタンス化された LoadOptions を使用して、入力ドキュメント パスまたはストリームを使用して Annotator オブジェクトをインスタンス化します。
        * AnnotationBase 実装を作成し、存在するアノテーションの ID (その ID を持つアノテーションが見つからない場合は何も変更されません) またはアノテーションのパス リスト (存在するすべてのアノテーションが削除されます) を設定します。
        * 渡されたアノテーションを使用して Annotator オブジェクトの update メソッドを呼び出します。
        * 結果のドキュメント パスまたはストリームと SaveOptions オブジェクトを使用して save メソッドを呼び出します。

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```ジャバ
        String outputPath = "UpdateAnnotation.bmp";

        // Annotator クラスのインスタンスを作成する
        Annotator annotator = new Annotator("input.bmp");
        
        // 最初の例として Reply クラスのインスタンスを作成し、コメントを追加します
        Reply reply1 = new Reply();
        Reply1.setComment("元の最初のコメント");
        Reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply Reply2 = new Reply();;
        Reply2.setComment("元の 2 番目のコメント");
        Reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(Reply2);
        
        // AreaAnnotation クラスのインスタンスを作成し、オプションを設定します
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        Original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("これはオリジナルのアノテーションです");
        original.setReplies(replies);
        
        // オリジナルのアノテーションを追加します
        annotator.add(オリジナル);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptionsloadOptions = new LoadOptions();
        
        // 注釈付きドキュメントを開く
         Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // 最初の例の更新用に Reply クラスのインスタンスを作成します
        Reply Reply3 = new Reply();
        Reply3.setComment("最初のコメントを更新しました");
        Reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply Reply4 = new Reply();
        Reply4.setComment("2 番目のコメントを更新しました");
        Reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(Reply3);
        replies1.add(Reply4);

        // 既存のアノテーションのいくつかのプロパティを変更することを提案します
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("これは更新されたアノテーションです");
        updated.setReplies(replies1);
        
        // アノテーションを更新して保存します
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Java で注釈 から OTT を抽出する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) これにより、Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の OTT ファイルからドキュメントに注釈を付けたり、注釈情報を抽出したりすることが簡単になります。
        * コメントと日付を含む Reply オブジェクトを作成します。
        * LoadOptions オブジェクトをインスタンス化し、true 引数を指定して SetImportAnnotations を呼び出します。
        * リスト型の変数を定義します。
        * get メソッドを呼び出し、結果を上記の変数に返します。

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```ジャバ
        // このサンプルを使用するには、入力ファイル ("annotated.bmp") に注釈が必要です
        LoadOptionsloadOptions = new LoadOptions();
        
        // Annotator クラスのインスタンスを作成し、アノテーションを取得します
        Final Annotator annotator = new Annotator("annotated.bmp",loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "注釈を抽出するライブデモ"
    content: |
        [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) Web サイトにアクセスして、今すぐ OTT ファイルから注釈を表示して削除します。
        ライブデモには次のようなメリットがあります

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-ott"
          title: "OTT ファイル形式について"
          content: |
            OTT 拡張子の付いたファイルは、OASIS の OpenDocument 標準形式に準拠してアプリケーションによって生成されたテンプレート ドキュメントを表します。これらは、無料の OpenOffice Writer などのワード プロセッサ アプリケーションで作成され、これらのテンプレート ファイルから新しいドキュメントを生成するために使用できる設定を保持できます。これらの設定には、ページ余白、枠線、ヘッダー、フッター、その他のページ設定が含まれます。このようなテンプレートは、会社のレターヘッドや標準化されたフォームなどの公式文書で使用されます。
          link: "https://docs.fileformat.com/image/ott/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "他の一般的なドキュメント形式の使用"
    content: |
        以下に示すように、いくつかの一般的なファイル形式から注釈プロパティを更新します。
    format:
        # format loop
        - name: "Annotate PDF document"
          link: "https://products.groupdocs.com/annotation/java/pdf/"
          description: "Adobe Portable Document Format"

        # format loop
        - name: "Annotate DOC document"
          link: "https://products.groupdocs.com/annotation/java/doc/"
          description: "Microsoft Word Document"

        # format loop
        - name: "Annotate DOCM document"
          link: "https://products.groupdocs.com/annotation/java/docm/"
          description: "Microsoft Word Macro-Enabled Document"

        # format loop
        - name: "Annotate DOCX document"
          link: "https://products.groupdocs.com/annotation/java/docx/"
          description: "Microsoft Word Open XML Document"

        # format loop
        - name: "Annotate DOT document"
          link: "https://products.groupdocs.com/annotation/java/dot/"
          description: "Microsoft Word Document Template"

        # format loop
        - name: "Annotate DOTX document"
          link: "https://products.groupdocs.com/annotation/java/dotx/"
          description: "Word Open XML Document Template"

        # format loop
        - name: "Annotate RTF document"
          link: "https://products.groupdocs.com/annotation/java/rtf/"
          description: "Rich Text Document"

        # format loop
        - name: "Annotate ODT document"
          link: "https://products.groupdocs.com/annotation/java/odt/"
          description: "Open Document Text"

        # format loop
        - name: "Annotate XLS document"
          link: "https://products.groupdocs.com/annotation/java/xls/"
          description: "Microsoft Excel Binary File Format"

        # format loop
        - name: "Annotate XLSX document"
          link: "https://products.groupdocs.com/annotation/java/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"

        # format loop
        - name: "Annotate XLSM document"
          link: "https://products.groupdocs.com/annotation/java/xlsm/"
          description: "Microsoft Excel Macro-Enabled Spreadsheet"

        # format loop
        - name: "Annotate XLSB document"
          link: "https://products.groupdocs.com/annotation/java/xlsb/"
          description: "Microsoft Excel Binary Worksheet"

        # format loop
        - name: "Annotate ODS document"
          link: "https://products.groupdocs.com/annotation/java/ods/"
          description: "Open Document Spreadsheet"

        # format loop
        - name: "Annotate PPT document"
          link: "https://products.groupdocs.com/annotation/java/ppt/"
          description: "PowerPoint Presentation"

        # format loop
        - name: "Annotate PPTX document"
          link: "https://products.groupdocs.com/annotation/java/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop
        - name: "Annotate PPSX document"
          link: "https://products.groupdocs.com/annotation/java/ppsx/"
          description: "PowerPoint Open XML Slide Show"

        # format loop
        - name: "Annotate POTM document"
          link: "https://products.groupdocs.com/annotation/java/potm/"
          description: "Microsoft PowerPoint Template"

        # format loop
        - name: "Annotate PPTM document"
          link: "https://products.groupdocs.com/annotation/java/pptm/"
          description: "Microsoft PowerPoint Presentation"

        # format loop
        - name: "Annotate PPS document"
          link: "https://products.groupdocs.com/annotation/java/pps/"
          description: "Microsoft PowerPoint 97-2003 Slide Show"

        # format loop
        - name: "Annotate ODP document"
          link: "https://products.groupdocs.com/annotation/java/odp/"
          description: "OpenDocument Presentation"

        # format loop
        - name: "Annotate HTML document"
          link: "https://products.groupdocs.com/annotation/java/html/"
          description: "HyperText Markup Language"

        # format loop
        - name: "Annotate TIFF document"
          link: "https://products.groupdocs.com/annotation/java/tiff/"
          description: "Tagged Image File Format"

        # format loop
        - name: "Annotate JPEG document"
          link: "https://products.groupdocs.com/annotation/java/jpeg/"
          description: "JPEG Image"

        # format loop
        - name: "Annotate PNG document"
          link: "https://products.groupdocs.com/annotation/java/png/"
          description: "Portable Network Graphic"

        # format loop
        - name: "Annotate EML document"
          link: "https://products.groupdocs.com/annotation/java/eml/"
          description: "E-mail Message"

        # format loop
        - name: "Annotate MSG document"
          link: "https://products.groupdocs.com/annotation/java/msg/"
          description: "Microsoft Outlook E-mail Message"

        # format loop
        - name: "Annotate VSD document"
          link: "https://products.groupdocs.com/annotation/java/vsd/"
          description: "Microsoft Visio 2003-2010 Drawing"

        # format loop
        - name: "Annotate VSDX document"
          link: "https://products.groupdocs.com/annotation/java/vsdx/"
          description: "Microsoft Visio Drawing"

        # format loop
        - name: "Annotate VSS document"
          link: "https://products.groupdocs.com/annotation/java/vss/"
          description: "Microsoft Visio 2003-2010 Stencil"

        # format loop
        - name: "Annotate VST document"
          link: "https://products.groupdocs.com/annotation/java/vst/"
          description: "Microsoft Visio 2013 Stencil"

        # format loop
        - name: "Annotate DWG document"
          link: "https://products.groupdocs.com/annotation/java/dwg/"
          description: "Autodesk Design Data Formats"

        # format loop
        - name: "Annotate DXF document"
          link: "https://products.groupdocs.com/annotation/java/dxf/"
          description: "AutoCAD Drawing Interchange"

        # format loop
        - name: "Annotate DCM document"
          link: "https://products.groupdocs.com/annotation/java/dcm/"
          description: "Digital Imaging and Communications in Medicine"

        # format loop
        - name: "Annotate WMF document"
          link: "https://products.groupdocs.com/annotation/java/wmf/"
          description: "Windows Metafile"

        # format loop
        - name: "Annotate EMF document"
          link: "https://products.groupdocs.com/annotation/java/emf/"
          description: "Enhanced Metafile Format"


############################# Back to top ###############################
back_to_top:
    enable: true
---