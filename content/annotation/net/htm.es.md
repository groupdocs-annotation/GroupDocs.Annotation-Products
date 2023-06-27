
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/htm"/>

############################# Head ############################
head_title: "{{Acción}} Anotaciones {{acción.preposiciones}} {{FORMATO}} en {{Plataforma}} Aplicación"
head_description: "Net API para crear y Eliminar tipos de anotaciones populares de HTM, imágenes, dibujos y formatos de archivos de documentos."

############################# Header ############################
title: "Anotar HTM de Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Download Free Trial"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true

    left:
        img_alt: "GroupDocs.Anotación para Net"
        image: "https://cms.admin.containerize.com/templates/groupdocs/images/product-logos/90x90-noborder/groupdocs-annotation-net.png"
        product: "GroupDocs.Annotation"
        platform: "Net"

    middle:
        button:
            # button loop
            - link: "https://apireference.groupdocs.com/annotation/net"
              text: "API Reference"
            # button loop
            - link: "https://github.com/groupdocs-annotation"
              text: "Code Examples"
            # button loop
            - link: "https://products.groupdocs.app/annotation/family"
              text: "Live Demos"
            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net"
        link_buy: "https://purchase.groupdocs.com"

############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Annotation para Net API"
    content: |
        GroupDocs.Annotation for Net API es una biblioteca que le permite agregar anotaciones a PDF, Word y otros documentos en Mac, Windows o Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) es una API Net nativa para administrar anotaciones con soporte integral para crear, agregar, editar, eliminar, extraer y exportar anotaciones de imágenes y varios otros documentos. La lista completa de formatos de documentos compatibles se puede ver en esta [página](https://docs.groupdocs.com/annotation/net/supported-document-formats/).

        Esta biblioteca le permite trabajar no solo con documentos HTM, sino también con muchos otros tipos de documentos como Word, Excel, PowerPoint, correos electrónicos de Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad y muchos otros.

        La API de GroupDocs.Annotation para Net le permite crear y agregar nuevas notas, editar anotaciones, extract comentarios, anotaciones y eliminar de los documentos. La biblioteca admite 13 tipos de anotaciones diferentes, incluidos Texto, Polilínea, Área, Subrayado, Punto, Marca de agua, Flecha, Elipse, Reemplazo de texto, Distancia, Campo de texto, Redacción de recursos en PDF, HTML, documentos de Microsoft Word, hojas de cálculo, diagramas, presentaciones, dibujos, imágenes y muchos otros formatos de archivo.

        El ejemplo (consulte a continuación) demuestra cómo trabajar con el documento HTM, en este ejemplo puede ver los pasos principales de cómo trabajar con GroupDocs. anotación, agregando objetos de datos para establecer las propiedades de la anotación de acuerdo con sus requisitos y guardando el resultado en el lugar necesario. También puede echar un vistazo más detallado a las funciones admitidas en nuestra de github [página](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), o en nuestro producto [documentación](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Pasos para agregar anotaciones de HTM en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Net agregar varios tipos de anotaciones a los archivos HTM dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        * Crear objetos de respuesta con comentario y fecha.
        * Crear objeto AreaAnnotation, establecer opciones de área y agregar respuestas.
        * Crear objeto Annotator y agregar anotación de área.
        * Guardar archivo de salida.
    title_right: "Requisitos del sistema"
    content_right: |
        Las API de GroupDocs.Annotation para Net son compatibles con las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.
        * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
        * Entornos de desarrollo: Visual Studio, Xamarin, MonoDevelop
        * Marcos: .NET Framework, .NET Standard, .NET Core, Mono
        * Descargue la última versión de GroupDocs.Annotation para .NET desde [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: "Vista previa de la anotación y ejemplo de código"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Añadir anotación de campo de texto al documento desde el disco local
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
                Message = "Esta es una anotación de campo de texto",
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
                        Comment = "Primer comentario",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Segundo comentario",
                        RepliedOn = DateTime.Now
                    }
                }
            };
            annotator.Add(textField);
            annotator.Save("resultado.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Pasos para eliminar anotaciones de HTM en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) hace que sea más fácil para los desarrolladores de Net eliminar los detalles de las anotaciones de los archivos HTM dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        * Crear objetos de respuesta con comentario y fecha.
        * Crea una instancia del objeto SaveOptions y establece AnnotationTypes = AnnotationType.None.
        * Llame al método de guardar con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```cs
        // 1- Cómo eliminar la anotación del documento usando el índice de anotación
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- Cómo eliminar la anotación del documento usando el objeto de anotación
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- Cómo eliminar algunas anotaciones del documento usando una lista de ID
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- Cómo eliminar algunas anotaciones del documento usando la lista de anotaciones
        
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
    title_left: "Pasos para editar anotaciones de HTM en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) hace que sea más fácil para los desarrolladores de Net actualizar varias propiedades de anotación de archivos HTM dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        * Crear una instancia del objeto Annotator con la ruta del documento de entrada o la secuencia con LoadOptions instanciadas con ImportAnnotations = true.
        * Cree alguna implementación de AnnotationBase y establezca el Id. de la anotación existente (si no se encuentra la anotación con ese Id., no se cambiará nada) o la lista de rutas de las anotaciones (se eliminarán todas las anotaciones existentes).
        * Llamar al método de actualización del objeto Annotator con anotaciones pasadas.
        * Llame al método de guardar con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```cs
        // abrir documento anotado
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            //suponiendo que vamos a cambiar algunas propiedades de la anotación existente
                AreaAnnotation updated = nueva AreaAnnotation
                    {
                            // Es importante establecer el Id. de anotación existente
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "Esta es una anotación actualizada",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Primer comentario actualizado",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Segundo comentario actualizado",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        };
                // actualizar anotación
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Pasos para extraer anotaciones de HTM en Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Net anotar documentos y extraer información de anotaciones de archivos HTM dentro de cualquier aplicación basada en Net mediante la implementación de unos sencillos pasos.
        * Crear objetos de respuesta con comentario y fecha.
        * Crea una instancia del objeto LoadOptions y llama a SetImportAnnotations con un argumento verdadero.
        * Definir variable con tipo Lista.
        * Llame al método get y devuelva el resultado a la variable anterior.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```cs
        // para usar este archivo de entrada de ejemplo ("anotado.bmp") debe tener anotaciones
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
    title: "Demostraciones en vivo para extraer anotaciones"
    content: |
        Vea y elimine las anotaciones del archivo HTM ahora mismo visitando el sitio web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        La demostración en vivo tiene los siguientes beneficios

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-htm"
          title: "Acerca del formato de archivo HTM"
          content: |
            Los archivos con la extensión HTM representan el lenguaje de marcado de hipertexto para crear páginas web para mostrar en navegadores web como Google Chrome, Internet Explorer, Firefox y muchos otros. Define las marcas para crear páginas estáticas que se publicarán en la World Wide Web (WWW) para que otras personas accedan a ellas. Estas marcas le dicen a los navegadores cómo mostrar el contenido de una página web. Dichas páginas pueden contener texto sin formato, imágenes, hipervínculos a otras páginas, videos y otra información multimedia. Cuando se publica una página web, puede echar un vistazo al código de marcado detrás de ella al ver la fuente de la página. Los navegadores modernos permiten inspeccionar cada sección de una página web donde se elabora cada subdivisión o elemento de marcado en la fuente HTM.
          link: "https://docs.fileformat.com/image/htm/"

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