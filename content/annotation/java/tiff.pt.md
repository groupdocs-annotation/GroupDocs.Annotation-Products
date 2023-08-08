---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API de anotação Java TIFF Anotação em C#"
head_description: "API Java para criar e anotar tipos de anotação populares de TIFF, imagens, desenhos e formatos de arquivo de documento."

############################# Header ############################
title: "Anote TIFF de Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Baixar Teste Gratuito"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Annotation para API Java"
    content: |
        GroupDocs.Annotation for Java API é uma biblioteca que permite adicionar anotações a PDF, Word e outros documentos no Mac, Windows ou Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) é uma API Java nativa para gerenciar anotações com suporte abrangente para criar, adicionar, editar, excluir, extrair e exportar anotações de imagens e vários outros documentos. A lista completa de formatos de documentos suportados pode ser vista nesta [página](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Esta biblioteca permite que você trabalhe não apenas com documento TIFF, mas também com muitos outros tipos de documentos, como Word, Excel, PowerPoint, e-mails do Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad e muitos outros.
        A API GroupDocs.Annotation for Java permite criar e adicionar novas notas, editar anotações, extrair comentários, anotações e removê-los de documentos. A biblioteca suporta 13 tipos diferentes de anotação, incluindo Texto, Polilinha, Área, Sublinhado, Ponto, Marca d'água, Seta, Elipse, Substituição de Texto, Distância, Campo de Texto, Redação de Recursos em PDF, HTML, documentos do Microsoft Word, planilhas, diagramas, apresentações, desenhos, imagens e muitos outros formatos de arquivo.
        O exemplo (veja abaixo) demonstra como trabalhar com o documento TIFF, neste exemplo você pode ver as principais etapas de como trabalhar com GroupDocs.Annotation: Configurar uma licença, abrir um documento com o qual deseja trabalhar, criar um anotação, adicionando objetos de dados para definir as propriedades de anotação de acordo com seus requisitos e salvando o resultado no local necessário. Além disso, você pode dar uma olhada mais detalhada nos recursos suportados em nossa [página] do github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) ou em nossa [documentação] do produto (https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Etapas para adicionar anotações a TIFF em Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita para os desenvolvedores Java adicionar vários tipos de anotação a arquivos TIFF em qualquer aplicativo baseado em Java, implementando algumas etapas fáceis.
        *   Crie objetos Reply com comentário e data.
        *   Crie um objeto AreaAnnotation, defina opções de área e adicione respostas.
        *   Crie o objeto Anotador e adicione a anotação de área.
        *   Salve o arquivo de saída.
    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Annotation para APIs Java são suportados em todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.
        *   Sistemas Operacionais: Microsoft Windows, Linux, MacOS
        *   Ambiente de Desenvolvimento: NetBeans, Intellij IDEA, Eclipse etc.
        *   Java Runtime Environment: Java 7 (1.7) e superior
        *   Obtenha a versão mais recente do GroupDocs.Annotation for Java no [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Visualização de anotação e amostra de código
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
    title_left: "Etapas para remover anotações de TIFF em Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) torna mais fácil para os desenvolvedores Java remover detalhes de anotação de arquivos TIFF em qualquer aplicativo baseado em Java implementando algumas etapas fáceis.
        *   Crie objetos Reply com comentário e data.
        *   Instancie o objeto SaveOptions e defina AnnotationTypes = AnnotationType.None.
        *   Chame o método save com o caminho ou fluxo do documento resultante e o objeto SaveOptions.

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
    title_left: "Etapas para editar anotações de TIFF em Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) torna mais fácil para os desenvolvedores Java atualizar várias propriedades de anotação de arquivos TIFF em qualquer aplicativo baseado em Java implementando algumas etapas fáceis.
        *   Instanciar objeto Anotador com caminho de documento de entrada ou fluxo com LoadOptions instanciado com ImportAnnotations = true.
        *   Crie alguma implementação AnnotationBase e defina o Id da anotação existente (se a anotação com esse Id não for encontrada, nada será alterado) ou a lista de caminhos das anotações (todas as anotações existentes serão removidas).
        *   Chame o método de atualização do objeto Anotador com as anotações passadas.
        *   Chame o método save com o caminho ou fluxo do documento resultante e o objeto SaveOptions.

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
    title_left: "Etapas para extrair anotações de TIFF em Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) torna mais fácil para os desenvolvedores Java anotar documentos e extrair informações de anotação de arquivos TIFF em qualquer aplicativo baseado em Java implementando algumas etapas fáceis.
        *   Crie objetos Reply com comentário e data.
        *   Instancie o objeto LoadOptions e chame SetImportAnnotations com o argumento true.
        *   Defina a variável com o tipo Lista.
        *   Chame o método get e retorne o resultado para a variável acima.

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
    title: "Demonstrações ao vivo para adicionar, remover, editar e extrair anotações em documentos e imagens"
    content: |
        Adicione, remova, edite e extraia anotações para o arquivo TIFF agora mesmo visitando o site [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). A demonstração ao vivo tem os seguintes benefícios

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-tiff"
          title: "Sobre o formato de arquivo TIFF"
          content: |
            TIFF ou TIF, Tagged Image File Format, representa imagens raster que se destinam ao uso em uma variedade de dispositivos que atendem a esse padrão de formato de arquivo. Ele é capaz de descrever dados de imagem de dois níveis, tons de cinza, paleta de cores e cores em vários espaços de cores. Ele oferece suporte a esquemas de compactação com perdas e sem perdas para escolher entre espaço e tempo para aplicativos que usam o formato. O formato é extensível e passou por diversas revisões que permitem a inclusão de uma quantidade ilimitada de informações particulares ou para fins especiais. O formato não depende da máquina e está livre de limites como processador, sistema operacional ou sistemas de arquivos.

          link: "https://docs.fileformat.com/image/tiff/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Trabalhando com outros formatos de documento populares"
    content: |
        Atualize as propriedades de anotação de alguns dos formatos de arquivo populares, conforme indicado abaixo.
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