---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net GIF API de anotação anotar em C #"
head_description: "Net API para criar e anotar tipos de anotação populares de GIF, imagens, desenhos e formatos de arquivo de documento."

############################# Header ############################
title: "Anote GIF da rede"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Baixar Teste Gratuito"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API é uma biblioteca que permite adicionar anotações a PDF, Word e outros documentos no Mac, Windows ou Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) é uma API de rede nativa para gerenciar anotações com suporte abrangente para criar, adicionar, editar, excluir, extrair e exportar anotações de imagens e vários outros documentos. A lista completa de formatos de documentos suportados pode ser vista nesta [página](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Esta biblioteca permite que você trabalhe não apenas com documento GIF, mas também com muitos outros tipos de documentos, como Word, Excel, PowerPoint, e-mails do Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad e muitos outros.
        O GroupDocs.Annotation for Net API permite criar e adicionar novas notas, editar anotações, extrair comentários, anotações e removê-los de documentos. A biblioteca suporta 13 tipos diferentes de anotação, incluindo Texto, Polilinha, Área, Sublinhado, Ponto, Marca d'água, Seta, Elipse, Substituição de Texto, Distância, Campo de Texto, Redação de Recursos em PDF, HTML, documentos do Microsoft Word, planilhas, diagramas, apresentações, desenhos, imagens e muitos outros formatos de arquivo.
        O exemplo (veja abaixo) demonstra como trabalhar com o documento GIF, neste exemplo você pode ver as principais etapas de como trabalhar com GroupDocs.Annotation: Configurar uma licença, abrir um documento com o qual deseja trabalhar, criar um anotação, adicionando objetos de dados para definir as propriedades de anotação de acordo com seus requisitos e salvando o resultado no local necessário. Além disso, você pode dar uma olhada mais detalhada nos recursos suportados em nossa [página do github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) ou em nossa [documentação do produto](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Etapas para adicionar anotações a GIF na rede"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita para os desenvolvedores da rede adicionar vários tipos de anotação a arquivos GIF em qualquer aplicativo baseado na rede, implementando algumas etapas fáceis.
        *   Crie objetos Reply com comentário e data.
        *   Crie um objeto AreaAnnotation, defina opções de área e adicione respostas.
        *   Crie o objeto Anotador e adicione a anotação de área.
        *   Salve o arquivo de saída.
    title_right: "Requisitos de sistema"
    content_right: |
        GroupDocs.Annotation for Net APIs são suportados em todas as principais plataformas e sistemas operacionais. Antes de executar o código abaixo, certifique-se de ter os seguintes pré-requisitos instalados em seu sistema.
        *   Sistemas Operacionais: Microsoft Windows, Linux, MacOS
        *   Ambientes de desenvolvimento: Visual Studio, Xamarin, MonoDevelop
        *   Estruturas: .NET Framework, .NET Standard, .NET Core, Mono
        *   Baixe a versão mais recente do GroupDocs.Annotation para .NET de [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Visualização de anotação e amostra de código
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
    title_left: "Etapas para remover anotações de GIF na rede"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) torna mais fácil para os desenvolvedores da rede remover detalhes de anotação de arquivos GIF dentro de qualquer aplicativo baseado na rede, implementando algumas etapas fáceis.
        *   Crie objetos Reply com comentário e data.
        *   Instancie o objeto SaveOptions e defina AnnotationTypes = AnnotationType.None.
        *   Chame o método save com o caminho ou fluxo do documento resultante e o objeto SaveOptions.

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
    title_left: "Etapas para editar anotações de GIF na rede"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) torna mais fácil para os desenvolvedores da rede atualizar várias propriedades de anotação de arquivos GIF dentro de qualquer aplicativo baseado na rede, implementando algumas etapas fáceis.
        *   Instanciar objeto Anotador com caminho de documento de entrada ou fluxo com LoadOptions instanciado com ImportAnnotations = true.
        *   Crie alguma implementação AnnotationBase e defina o Id da anotação existente (se a anotação com esse Id não for encontrada, nada será alterado) ou a lista de caminhos das anotações (todas as anotações existentes serão removidas).
        *   Chame o método de atualização do objeto Anotador com as anotações passadas.
        *   Chame o método save com o caminho ou fluxo do documento resultante e o objeto SaveOptions.

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
    title_left: "Etapas para extrair anotações de GIF na rede"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) torna mais fácil para os desenvolvedores da rede anotar documentos e extrair informações de anotação de arquivos GIF em qualquer aplicativo baseado na rede, implementando algumas etapas fáceis.
        *   Crie objetos Reply com comentário e data.
        *   Instancie o objeto LoadOptions e chame SetImportAnnotations com o argumento true.
        *   Defina a variável com o tipo Lista.
        *   Chame o método get e retorne o resultado para a variável acima.

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
    title: "Demonstrações ao vivo para adicionar, remover, editar e extrair anotações em documentos e imagens"
    content: |
        Adicione, remova, edite e extraia anotações para o arquivo GIF agora mesmo visitando o site [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). A demonstração ao vivo tem os seguintes benefícios

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-gif"
          title: "Sobre o formato de arquivo GIF"
          content: |
            Um GIF ou Graphical Interchange Format é um tipo de imagem altamente compactada. De propriedade da Unisys, o GIF usa o algoritmo de compactação LZW que não degrada a qualidade da imagem. Para cada imagem, o GIF normalmente permite até 8 bits por pixel e até 256 cores são permitidas na imagem. Em contraste com uma imagem JPEG, que pode exibir até 16 milhões de cores e toca razoavelmente os limites do olho humano. Quando a internet surgiu, os GIFs continuaram sendo a melhor escolha porque exigiam baixa largura de banda e eram compatíveis com os gráficos que consumiam áreas sólidas de cor. Um GIF animado combina várias imagens ou quadros em um único arquivo e os exibe em uma sequência para gerar um clipe animado ou um pequeno vídeo. As limitações de cores são de até 256 para cada quadro e provavelmente são as menos adequadas para reproduzir outras imagens e fotografias com gradiente de cores.

          link: "https://docs.fileformat.com/image/gif/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Trabalhando com outros formatos de documento populares"
    content: |
        Atualize as propriedades de anotação de alguns dos formatos de arquivo populares, conforme indicado abaixo.
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