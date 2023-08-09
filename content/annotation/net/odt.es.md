---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net ODT API de anotación Anotar en C#"
head_description: "Net API para crear y anotar tipos de anotaciones populares de ODT, imágenes, dibujos y formatos de archivos de documentos."

############################# Header ############################
title: "Anotar ODT de Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Descargue prueba gratis"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Annotation para Net API"
    content: |
        GroupDocs.Annotation for Net API es una biblioteca que le permite agregar anotaciones a PDF, Word y otros documentos en Mac, Windows o Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) es una API de red nativa para administrar anotaciones con soporte completo para crear, agregar, editar, eliminar, extraer y exportar anotaciones de imágenes y otros documentos. La lista completa de formatos de documentos compatibles se puede ver en esta [página](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Esta biblioteca le permite trabajar no solo con documentos ODT sino también con muchos otros tipos de documentos como Word, Excel, PowerPoint, correos electrónicos de Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad y muchos otros.
        GroupDocs.Annotation for Net API le permite crear y agregar nuevas notas, editar anotaciones, extraer comentarios, anotaciones y eliminarlas de los documentos. La biblioteca admite 13 tipos de anotaciones diferentes, incluidos Texto, Polilínea, Área, Subrayado, Punto, Marca de agua, Flecha, Elipse, Reemplazo de texto, Distancia, Campo de texto, Redacción de recursos en PDF, HTML, documentos de Microsoft Word, hojas de cálculo, diagramas, presentaciones, dibujos, imágenes y muchos otros formatos de archivo.
        El ejemplo (consulte a continuación) demuestra cómo trabajar con el documento ODT, en este ejemplo puede ver los pasos principales de cómo trabajar con GroupDocs. anotación, agregando objetos de datos para establecer las propiedades de la anotación de acuerdo con sus requisitos y guardando el resultado en el lugar necesario. También puede echar un vistazo más detallado a las funciones admitidas en nuestra [página de github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), o en nuestra [documentación] del producto (https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Pasos para agregar anotaciones a ODT en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita a los desarrolladores de Net agregar varios tipos de anotaciones a los archivos ODT dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        *   Cree objetos de respuesta con comentario y fecha.
        *   Cree un objeto AreaAnnotation, establezca opciones de área y agregue respuestas.
        *   Cree un objeto Annotator y agregue una anotación de área.
        *   Guardar archivo de salida.
    title_right: "Requisitos del sistema"
    content_right: |
        Las API de GroupDocs.Annotation for Net son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema.
        *   Sistemas operativos: Microsoft Windows, Linux, Mac OS
        *   Entornos de desarrollo: Visual Studio, Xamarin, MonoDevelop
        *   Marcos: .NET Framework, .NET Standard, .NET Core, Mono
        *   Descargue la última versión de GroupDocs.Annotation para .NET desde [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Vista previa de anotaciones y ejemplo de código
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
    title_left: "Pasos para eliminar anotaciones de ODT en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) hace que sea más fácil para los desarrolladores de Net eliminar los detalles de las anotaciones de los archivos ODT dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        *   Cree objetos de respuesta con comentario y fecha.
        *   Crea una instancia del objeto SaveOptions y establece AnnotationTypes = AnnotationType.None.
        *   Llame al método save con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

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
    title_left: "Pasos para editar anotaciones de ODT en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) hace que sea más fácil para los desarrolladores de Net actualizar varias propiedades de anotación de los archivos ODT dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        *   Cree una instancia del objeto Annotator con la ruta del documento de entrada o flujo con LoadOptions instanciado con ImportAnnotations = true.
        *   Cree alguna implementación de AnnotationBase y establezca el Id. de la anotación existente (si no se encuentra la anotación con ese Id., no se cambiará nada) o la lista de rutas de las anotaciones (se eliminarán todas las anotaciones existentes).
        *   Llame al método de actualización del objeto Annotator con anotaciones pasadas.
        *   Llame al método save con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

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
    title_left: "Pasos para extraer anotaciones de ODT en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita a los desarrolladores de Net anotar documentos y extraer información de anotaciones de archivos ODT dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        *   Cree objetos de respuesta con comentario y fecha.
        *   Cree una instancia del objeto LoadOptions y llame a SetImportAnnotations con un argumento verdadero.
        *   Definir variable con tipo Lista.
        *   Llame al método get y devuelva el resultado a la variable anterior.

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
    title: "Demostraciones en vivo para agregar, eliminar, editar y extraer anotaciones en documentos e imágenes"
    content: |
        Agregue, elimine, edite y extraiga anotaciones en el archivo ODT ahora mismo visitando el sitio web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). La demostración en vivo tiene los siguientes beneficios

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-odt"
          title: "Acerca del formato de archivo ODT"
          content: |
            Los archivos ODT son un tipo de documentos creados con aplicaciones de procesamiento de texto que se basan en el formato de archivo de texto OpenDocument. Estos se crean con aplicaciones de procesador de texto, como OpenOffice Writer gratuito, y pueden contener contenido como texto, imágenes, objetos y estilos. El archivo ODT es para el procesador de texto Writer lo que DOCX es para Microsoft Word. Varias aplicaciones, incluidos Google Docs y el procesador de texto basado en la web de Google incluido con Google Drive, pueden abrir los archivos ODT para editarlos. Microsoft Word también puede abrir archivos ODT y guardarlos en otros formatos como DOC y DOCX.

          link: "https://docs.fileformat.com/image/odt/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Trabajar con otros formatos de documentos populares"
    content: |
        Actualice las propiedades de anotación de algunos de los formatos de archivo populares como se indica a continuación.
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