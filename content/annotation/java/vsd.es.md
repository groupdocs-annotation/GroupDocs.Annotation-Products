
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/vsd"/>

############################# Head ############################
head_title: "{{Acción}} Anotaciones {{acción.preposiciones}} {{FORMATO}} en {{Plataforma}} Aplicación"
head_description: "Java API para crear y Eliminar tipos de anotaciones populares de VSD, imágenes, dibujos y formatos de archivos de documentos."

############################# Header ############################
title: "Anotar VSD de Java"
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
        img_alt: "GroupDocs.Anotación para Java"
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
    title: "Acerca de GroupDocs.Annotation para Java API"
    content: |
        GroupDocs.Annotation for Java API es una biblioteca que le permite agregar anotaciones a PDF, Word y otros documentos en Mac, Windows o Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) es una API Java nativa para administrar anotaciones con soporte integral para crear, agregar, editar, eliminar, extraer y exportar anotaciones de imágenes y varios otros documentos. La lista completa de formatos de documentos compatibles se puede ver en esta [página](https://docs.groupdocs.com/annotation/java/supported-document-formats/).

        Esta biblioteca le permite trabajar no solo con documentos VSD, sino también con muchos otros tipos de documentos como Word, Excel, PowerPoint, correos electrónicos de Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad y muchos otros.

        La API de GroupDocs.Annotation para Java le permite crear y agregar nuevas notas, editar anotaciones, extract comentarios, anotaciones y eliminar de los documentos. La biblioteca admite 13 tipos de anotaciones diferentes, incluidos Texto, Polilínea, Área, Subrayado, Punto, Marca de agua, Flecha, Elipse, Reemplazo de texto, Distancia, Campo de texto, Redacción de recursos en PDF, HTML, documentos de Microsoft Word, hojas de cálculo, diagramas, presentaciones, dibujos, imágenes y muchos otros formatos de archivo.

        El ejemplo (consulte a continuación) demuestra cómo trabajar con el documento VSD, en este ejemplo puede ver los pasos principales de cómo trabajar con GroupDocs. anotación, agregando objetos de datos para establecer las propiedades de la anotación de acuerdo con sus requisitos y guardando el resultado en el lugar necesario. También puede echar un vistazo más detallado a las funciones admitidas en nuestra de github [página](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), o en nuestro producto [documentación](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Pasos para agregar anotaciones de VSD en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Java agregar varios tipos de anotaciones a los archivos VSD dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        * Crear objetos de respuesta con comentario y fecha.
        * Crear objeto AreaAnnotation, establecer opciones de área y agregar respuestas.
        * Crear objeto Annotator y agregar anotación de área.
        * Guardar archivo de salida.
    title_right: "Requisitos del sistema"
    content_right: |
        Las API de GroupDocs.Annotation para Java son compatibles con las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener instalados los siguientes requisitos previos en su sistema.
        * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
        * Entorno de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        * Java Runtime Environment: Java 7 (1.7) y superior
        * Obtenga la última versión de GroupDocs.Annotation para Java de [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: "Vista previa de la anotación y ejemplo de código"
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Crear una instancia de la clase Responder y agregar comentarios
        Reply firstReply = new Reply();
        firstReply.setComment("Primer comentario");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Segundo comentario");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Crear una instancia de la clase AreaAnnotation y establecer opciones
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectángulo(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("Esta es una anotación de área");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Crear una instancia de la clase Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Añadir anotación
        annotator.add(area);
        
        // Guardar en archivo
        annotator.save("salida.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Pasos para eliminar anotaciones de VSD en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) hace que sea más fácil para los desarrolladores de Java eliminar los detalles de las anotaciones de los archivos VSD dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        * Crear objetos de respuesta con comentario y fecha.
        * Crea una instancia del objeto SaveOptions y establece AnnotationTypes = AnnotationType.None.
        * Llame al método de guardar con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```java
        // Crear una instancia de la clase Annotator
        Annotator annotator = new Annotator("C://input.bmp");

        // Eliminar anotación por tipo de conjunto Ninguno
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Guarda la anotación en el archivo de salida
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Pasos para editar anotaciones de VSD en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) hace que sea más fácil para los desarrolladores de Java actualizar varias propiedades de anotación de archivos VSD dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        * Crear una instancia del objeto Annotator con la ruta del documento de entrada o la secuencia con LoadOptions instanciadas con ImportAnnotations = true.
        * Cree alguna implementación de AnnotationBase y establezca el Id. de la anotación existente (si no se encuentra la anotación con ese Id., no se cambiará nada) o la lista de rutas de las anotaciones (se eliminarán todas las anotaciones existentes).
        * Llamar al método de actualización del objeto Annotator con anotaciones pasadas.
        * Llame al método de guardar con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```java
        String ruta de salida = "UpdateAnnotation.bmp";

        // Crear una instancia de la clase Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Crear una instancia de la clase Responder para el primer ejemplo y agregar comentarios
        Reply reply1 = new Reply();
        reply1.setComment("Primer comentario original");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Segundo comentario original");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Crear una instancia de la clase AreaAnnotation y establecer opciones
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(nuevo Rectángulo(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("Esta es la anotación original");
        original.setReplies(replies);
        
        // Añadir anotación original
        annotator.add(original);
        annotator.save (ruta de salida);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Abrir documento anotado
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Crear una instancia de clase de respuesta para actualizar el primer ejemplo
        Reply reply3 = new Reply();
        reply3.setComment("Primer comentario actualizado");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Segundo comentario actualizado");
        respuesta4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Sugerimos que queramos cambiar algunas propiedades de la anotación existente
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(nuevo Rectángulo(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("Esta es una anotación actualizada");
        updated.setReplies(respuestas1);
        
        // Actualizar y guardar anotación
        annotator1.update(updated);
        annotator1.save(outputPath);
        anotador1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Pasos para extraer anotaciones de VSD en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Java anotar documentos y extraer información de anotaciones de archivos VSD dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        * Crear objetos de respuesta con comentario y fecha.
        * Crea una instancia del objeto LoadOptions y llama a SetImportAnnotations con un argumento verdadero.
        * Definir variable con tipo Lista.
        * Llame al método get y devuelva el resultado a la variable anterior.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```java
        // Para usar este ejemplo, el archivo de entrada ("anotado.bmp") debe tener anotaciones
        LoadOptions loadOptions = new LoadOptions();
        
        // Crear una instancia de la clase Annotator y obtener anotaciones
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Demostraciones en vivo para extraer anotaciones"
    content: |
        Vea y elimine las anotaciones del archivo VSD ahora mismo visitando el sitio web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        La demostración en vivo tiene los siguientes beneficios

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsd"
          title: "Acerca del formato de archivo VSD"
          content: |
            Los archivos VSD son dibujos creados con la aplicación Microsoft Visio para representar una variedad de objetos gráficos y la interconexión entre estos. Dichos dibujos pueden contener objetos visuales como objetos visuales, diagramas de flujo, diagrama UML, flujo de información, organigramas, diagramas de software, diseño de red, modelos de bases de datos, mapeo de objetos y otra información similar. Microsoft Visio ofrece la capacidad de convertir archivos de Visio a varios formatos de archivo diferentes, incluidos PNG, BMP, PDF y otros.
          link: "https://docs.fileformat.com/image/vsd/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Trabajar con otros formatos de documentos populares"
    content: |
        Actualice las propiedades de anotación de algunos de los formatos de archivo populares como se indica a continuación.
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