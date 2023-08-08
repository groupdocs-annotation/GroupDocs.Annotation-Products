---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DCM 注釈 API C# で注釈を付ける"
head_description: "DCM、画像、図面、ドキュメント ファイル形式から一般的な注釈タイプを作成して注釈を付けるための Java API。"

############################# Header ############################
title: "Java から DCM に注釈を付ける"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "無料トライアルをダウンロード"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Java API の GroupDocs.Annotation について"
    content: |
        GroupDocs.Annotation for Java API は、Mac、Windows、または Ubuntu 上の PDF、Word、およびその他のドキュメントに注釈を追加できるようにするライブラリです。 [GroupDocs.Annotation for Java](/annotation/java) は、画像やその他のさまざまなドキュメントからの注釈の作成、追加、編集、削除、抽出、エクスポートを包括的にサポートする注釈管理用のネイティブ Java API です。サポートされているドキュメント形式の完全なリストは、この [ページ](https://docs.groupdocs.com/annotation/java/supported-document-formats/) で確認できます。
        このライブラリを使用すると、DCM ドキュメントだけでなく、Word、Excel、PowerPoint、Outlook 電子メール、Visio、Adobe、OpenDocument、OpenOffice、Photoshop、AutoCad など、他の多くのタイプのドキュメントでも作業できます。
        GroupDocs.Annotation for Java API を使用すると、新しいメモの作成と追加、注釈の編集、コメントや注釈の抽出、ドキュメントからの削除を行うことができます。このライブラリは、テキスト、ポリライン、エリア、下線、点、透かし、矢印、楕円、テキスト置換、距離、テキスト フィールド、PDF、HTML、Microsoft Word ドキュメント、スプレッドシート、図、プレゼンテーション、図面、画像、その他多くのファイル形式。
        例 (以下を参照) は、DCM ドキュメントの操作を示しています。この例では、GroupDocs.Annotation を使用する方法の主な手順を確認できます。ライセンスを設定し、操作したいドキュメントを開き、注釈を追加し、要件に従って注釈プロパティを設定し、結果を必要な場所に保存します。また、サポートされている機能の詳細については、github [ページ](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) または製品 [ドキュメント](https://docs.groupdocs.com/annotation/java/getting-started/)。

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Java で DCM に注釈を追加する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の DCM ファイルにさまざまな注釈タイプを簡単に追加できます。
        *   コメントと日付を含む Reply オブジェクトを作成します。
        *   AreaAnnotation オブジェクトを作成し、エリア オプションを設定し、応答を追加します。
        *   Annotator オブジェクトを作成し、領域の注釈を追加します。
        *   出力ファイルを保存します。
    title_right: "システム要求"
    content_right: |
        GroupDocs.Annotation for Java API は、すべての主要なプラットフォームとオペレーティング システムでサポートされています。以下のコードを実行する前に、次の前提条件がシステムにインストールされていることを確認してください。
        *   オペレーティング システム: Microsoft Windows、Linux、MacOS
        *   開発環境: NetBeans、Intellij IDEA、Eclipse など
        *   Java ランタイム環境: Java 7 (1.7) 以降
        *   Java 用 GroupDocs.Annotation の最新バージョンを [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation) から入手します。

############################# Preview ############################
preview_Add:
    enable: true
    title: 注釈のプレビューとコードサンプル
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Create an instance of Reply class and add comments
        Reply firstReply = new Reply();
        firstReply.setComment("First comment");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Second comment");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("This is area annotation");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Add annotation
        annotator.add(area);
        
        // Save to file
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Java で DCM から注釈を削除する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の DCM ファイルから注釈の詳細を簡単に削除できます。
        *   コメントと日付を含む Reply オブジェクトを作成します。
        *   SaveOptions オブジェクトをインスタンス化し、AnnotationTypes = AnnotationType.None を設定します。
        *   結果のドキュメント パスまたはストリームと SaveOptions オブジェクトを使用して save メソッドを呼び出します。

############################# Preview ############################
preview_Remove:
    enable: true
    code: |
        ```java
        // Create an instance of Annotator class 
        Annotator annotator = new Annotator("C://input.bmp");

        // Remove annotation by set type None 
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Save annotation to output file
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Java で DCM から注釈を編集する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の DCM ファイルからさまざまな注釈プロパティを簡単に更新できるようになります。
        *   ImportAnnotations = true でインスタンス化された LoadOptions を使用して、入力ドキュメント パスまたはストリームを使用して Annotator オブジェクトをインスタンス化します。
        *   AnnotationBase 実装を作成し、存在するアノテーションの ID (その ID を持つアノテーションが見つからない場合は何も変更されません) またはアノテーションのパス リスト (存在するすべてのアノテーションが削除されます) を設定します。
        *   渡されたアノテーションを使用して Annotator オブジェクトの update メソッドを呼び出します。
        *   結果のドキュメント パスまたはストリームと SaveOptions オブジェクトを使用して save メソッドを呼び出します。

############################# Preview ############################
preview_Edit:
    enable: true
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp";

        // Create an instance of Annotator class
        Annotator annotator = new Annotator("input.bmp");
        
        // Create an instance of Reply class for first example and add comments
        Reply reply1 = new Reply();
        reply1.setComment("Original first comment");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Original second comment");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Create an instance of AreaAnnotation class and set options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(new Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("This is original annotation");
        original.setReplies(replies);
        
        // Add original annotation
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Open annotated document
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Create an instance of Reply class for update first example
        Reply reply3 = new Reply();
        reply3.setComment("Updated first comment");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Updated second comment");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggest we want change some properties of existed annotation
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("This is updated annotation");
        updated.setReplies(replies1);
        
        // Update and save annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Java で DCM から注釈を抽出する手順"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) Java 開発者は、いくつかの簡単な手順を実装することで、Java ベースのアプリケーション内の DCM ファイルからドキュメントに注釈を付けたり、注釈情報を抽出したりすることが簡単になります。
        *   コメントと日付を含む Reply オブジェクトを作成します。
        *   LoadOptions オブジェクトをインスタンス化し、true 引数を指定して SetImportAnnotations を呼び出します。
        *   List型の変数を定義します。
        *   get メソッドを呼び出し、結果を上記の変数に返します。

############################# Preview ############################
preview_Extract:
    enable: true
    code: |
        ```java
        // For using this example input file ("annotated.bmp") must be with annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Create an instance of Annotator class and get annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "ドキュメントや画像に注釈を追加、削除、編集、抽出するライブデモ"
    content: |
        [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family) Web サイトにアクセスして、今すぐ DCM ファイルに注釈を追加、削除、編集、抽出します。 ライブデモには次のようなメリットがあります

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dcm"
          title: "DCM ファイル形式について"
          content: |
            拡張子が .DCM のファイルは、MRI、CT スキャン、超音波画像などの患者の医療情報を保存するデジタル画像を表します。これは全米電気製造業者協会 (NEMA) によって開発され、医療画像の配布と表示のための画像ファイル形式を標準化することを目的としていました。 DICOM ファイル形式に似ており、参照用の患者情報を含めることができます。

          link: "https://docs.fileformat.com/image/dcm/"

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