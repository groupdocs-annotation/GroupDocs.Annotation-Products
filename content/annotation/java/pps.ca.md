---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API d'anotació de Java PPS Anotar en C#"
head_description: "API de Java per crear i anotar tipus d'anotacions populars a partir de PPS, imatges, dibuixos i formats de fitxers de documents."

############################# Header ############################
title: "Anoteu PPS des de Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Baixeu la prova gratuïta"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Quant a l'API de GroupDocs.Annotation per a Java"
    content: |
        L'API de GroupDocs.Annotation per a Java és una biblioteca que us permet afegir anotacions a PDF, Word i altres documents a Mac, Windows o Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) és una API de Java nativa per gestionar anotacions amb suport complet per crear, afegir, editar, suprimir, extreure i exportar anotacions d'imatges i altres documents. La llista completa dels formats de document compatibles que podeu veure en aquesta [pàgina](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Aquesta biblioteca us permet treballar no només amb el document PPS sinó també amb molts altres tipus de documents com ara Word, Excel, PowerPoint, correus electrònics d'Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad i molts altres.
        L'API de GroupDocs.Annotation per a Java us permet crear i afegir notes noves, editar anotacions, extreure comentaris i anotacions i eliminar-les dels documents. La biblioteca admet 13 tipus d'anotacions diferents, com ara text, polilínia, àrea, subratllat, punt, filigrana, fletxa, el·lipse, substitució de text, distància, camp de text, redacció de recursos en PDF, HTML, documents de Microsoft Word, fulls de càlcul, diagrames, presentacions, dibuixos, imatges i molts altres formats de fitxer.
        L'exemple (vegeu a continuació) mostra com es treballa amb el document PPS, en aquest exemple podeu veure els passos principals de com treballar amb GroupDocs. Anotació: configureu una llicència, obriu un document amb el qual voleu treballar i creeu un anotació, afegint objectes de dades per establir propietats d'anotació segons els vostres requisits i desant el resultat al lloc necessari. També podeu fer una ullada més detallada sobre les funcions admeses a la nostra [pàgina] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) o a la nostra [documentació] del producte (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Passos per afegir anotacions a PPS a Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita als desenvolupadors de Java afegir diversos tipus d'anotacions als fitxers PPS dins de qualsevol aplicació basada en Java implementant uns quants passos senzills.
        *   Creeu objectes de resposta amb comentari i data.
        *   Creeu un objecte AreaAnnotation, configureu opcions d'àrea i afegiu respostes.
        *   Creeu un objecte Annotator i afegiu una anotació d'àrea.
        *   Desa el fitxer de sortida.
    title_right: "Requisits del sistema"
    content_right: |
        Les API de GroupDocs.Annotation per a Java són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.
        *   Sistemes operatius: Microsoft Windows, Linux, MacOS
        *   Entorn de desenvolupament: NetBeans, Intellij IDEA, Eclipse, etc
        *   Entorn d'execució de Java: Java 7 (1.7) i posterior
        *   Obteniu la darrera versió de GroupDocs.Annotation per a Java de [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Vista prèvia de l'anotació i mostra de codi
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
    title_left: "Passos per eliminar les anotacions de PPS a Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita als desenvolupadors de Java eliminar els detalls de les anotacions dels fitxers PPS dins de qualsevol aplicació basada en Java implementant uns quants passos senzills.
        *   Creeu objectes de resposta amb comentari i data.
        *   Crea una instancia de l'objecte SaveOptions i estableix AnnotationTypes = AnnotationType.None.
        *   Truqueu al mètode de desar amb la ruta o flux del document resultant i l'objecte SaveOptions.

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
    title_left: "Passos per editar anotacions de PPS a Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita que els desenvolupadors de Java actualitzin diverses propietats d'anotació dels fitxers PPS dins de qualsevol aplicació basada en Java mitjançant la implementació d'uns quants passos senzills.
        *   Instancia l'objecte Annotator amb la ruta del document d'entrada o el flux amb LoadOptions instància amb ImportAnnotations = true.
        *   Creeu una implementació de AnnotationBase i configureu l'identificador de l'anotació existent (si no es troba l'anotació amb aquest identificador, no es canviarà res) o la llista de camins d'anotacions (s'eliminaran totes les anotacions existents).
        *   Truca el mètode d'actualització de l'objecte Annotator amb anotacions passades.
        *   Truqueu al mètode de desar amb la ruta o flux del document resultant i l'objecte SaveOptions.

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
    title_left: "Passos per extreure anotacions de PPS a Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilita als desenvolupadors de Java anotar documents i extreure informació d'anotacions dels fitxers PPS dins de qualsevol aplicació basada en Java implementant uns quants passos senzills.
        *   Creeu objectes de resposta amb comentari i data.
        *   Instancia l'objecte LoadOptions i crida a SetImportAnnotations amb un argument veritable.
        *   Definiu variable amb el tipus Llista.
        *   Truqueu al mètode get i retorneu el resultat a la variable anterior.

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
    title: "Demostracions en directe per afegir, eliminar, editar i extreure anotacions a documents i imatges"
    content: |
        Afegiu, suprimiu, editeu i extreu anotacions al fitxer PPS ara mateix visitant el lloc web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). La demostració en directe té els següents avantatges

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-pps"
          title: "Sobre el format de fitxer PPS"
          content: |
            PPS, Presentació de diapositives de PowerPoint, els fitxers es creen amb Microsoft PowerPoint per a la presentació de diapositives. Microsoft PowerPoint 97-2003 admet la lectura i creació de fitxers PPS. La versió més recent d'aquest format de fitxer és PPSX, que es basa en els estàndards Office OpenXML. Els fitxers PPS encara es poden llegir amb les últimes versions de Microsoft PowerPoint, però els fitxers de creació recent només es poden desar en format de fitxer PPSX. Quan un fitxer PPS es comparteix amb un altre usuari i s'obre, comença com a mostra de Powerpoint a diferència del fitxer PPT que s'obre en mode editable.

          link: "https://docs.fileformat.com/image/pps/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Treballar amb altres formats de documents populars"
    content: |
        Actualitzeu les propietats d'anotació d'alguns dels formats de fitxer populars, tal com s'indica a continuació.
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