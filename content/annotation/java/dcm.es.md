---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DCM API de anotación Anotar en C#"
head_description: "API de Java para crear y anotar tipos de anotaciones populares de DCM, imágenes, dibujos y formatos de archivos de documentos."

############################# Header ############################
title: "Anotar DCM desde Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Descargue prueba gratis"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Annotation para la API de Java"
    content: |
        GroupDocs.Annotation for Java API es una biblioteca que le permite agregar anotaciones a PDF, Word y otros documentos en Mac, Windows o Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) es una API nativa de Java para administrar anotaciones con soporte integral para crear, agregar, editar, eliminar, extraer y exportar anotaciones de imágenes y otros documentos. La lista completa de formatos de documentos compatibles se puede ver en esta [página] (https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Esta biblioteca le permite trabajar no solo con documentos DCM sino también con muchos otros tipos de documentos como Word, Excel, PowerPoint, correos electrónicos de Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad y muchos otros.
        La API de GroupDocs.Annotation para Java le permite crear y agregar nuevas notas, editar anotaciones, extraer comentarios, anotaciones y eliminarlas de los documentos. La biblioteca admite 13 tipos de anotaciones diferentes, incluidos Texto, Polilínea, Área, Subrayado, Punto, Marca de agua, Flecha, Elipse, Reemplazo de texto, Distancia, Campo de texto, Redacción de recursos en PDF, HTML, documentos de Microsoft Word, hojas de cálculo, diagramas, presentaciones, dibujos, imágenes y muchos otros formatos de archivo.
        El ejemplo (consulte a continuación) demuestra cómo trabajar con el documento DCM, en este ejemplo puede ver los pasos principales de cómo trabajar con GroupDocs. anotación, agregando objetos de datos para establecer las propiedades de la anotación de acuerdo con sus requisitos y guardando el resultado en el lugar necesario. También puede echar un vistazo más detallado a las funciones admitidas en nuestra [página] de github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), o en nuestra [documentación] del producto (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Pasos para agregar anotaciones a DCM en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Java agregar varios tipos de anotaciones a los archivos DCM dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        *   Cree objetos de respuesta con comentario y fecha.
        *   Cree un objeto AreaAnnotation, establezca opciones de área y agregue respuestas.
        *   Cree un objeto Annotator y agregue una anotación de área.
        *   Guardar archivo de salida.
    title_right: "Requisitos del sistema"
    content_right: |
        Las API de GroupDocs.Annotation para Java son compatibles con todas las principales plataformas y sistemas operativos. Antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema.
        *   Sistemas operativos: Microsoft Windows, Linux, Mac OS
        *   Entorno de desarrollo: NetBeans, Intellij IDEA, Eclipse, etc.
        *   Entorno de tiempo de ejecución de Java: Java 7 (1.7) y superior
        *   Obtenga la última versión de GroupDocs.Annotation para Java desde [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Vista previa de anotaciones y ejemplo de código
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
    title_left: "Pasos para eliminar anotaciones de DCM en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) hace que sea más fácil para los desarrolladores de Java eliminar los detalles de las anotaciones de los archivos DCM dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        *   Cree objetos de respuesta con comentario y fecha.
        *   Crea una instancia del objeto SaveOptions y establece AnnotationTypes = AnnotationType.None.
        *   Llame al método save con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

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
    title_left: "Pasos para editar anotaciones de DCM en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Java la actualización de varias propiedades de anotación de los archivos DCM dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        *   Cree una instancia del objeto Annotator con la ruta del documento de entrada o flujo con LoadOptions instanciado con ImportAnnotations = true.
        *   Cree alguna implementación de AnnotationBase y establezca el Id. de la anotación existente (si no se encuentra la anotación con ese Id., no se cambiará nada) o la lista de rutas de las anotaciones (se eliminarán todas las anotaciones existentes).
        *   Llame al método de actualización del objeto Annotator con anotaciones pasadas.
        *   Llame al método save con la ruta del documento resultante o la secuencia y el objeto SaveOptions.

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
    title_left: "Pasos para extraer anotaciones de DCM en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita a los desarrolladores de Java anotar documentos y extraer información de anotaciones de archivos DCM dentro de cualquier aplicación basada en Java mediante la implementación de unos sencillos pasos.
        *   Cree objetos de respuesta con comentario y fecha.
        *   Cree una instancia del objeto LoadOptions y llame a SetImportAnnotations con un argumento verdadero.
        *   Definir variable con tipo Lista.
        *   Llame al método get y devuelva el resultado a la variable anterior.

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
    title: "Demostraciones en vivo para agregar, eliminar, editar y extraer anotaciones en documentos e imágenes"
    content: |
        Agregue, elimine, edite y extraiga anotaciones en el archivo DCM ahora mismo visitando el sitio web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
La demostración en vivo tiene los siguientes beneficios

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dcm"
          title: "Acerca del formato de archivo DCM"
          content: |
            Los archivos con extensión .DCM representan imágenes digitales que almacenan información médica de pacientes, como resonancias magnéticas, tomografías computarizadas e imágenes de ultrasonido. Fue desarrollado por la Asociación Nacional de Fabricantes Eléctricos (NEMA) y estaba destinado a estandarizar el formato de archivo de imágenes para la distribución y visualización de imágenes médicas. Es similar al formato de archivo DICOM y puede incluir información del paciente como referencia.

          link: "https://docs.fileformat.com/image/dcm/"

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