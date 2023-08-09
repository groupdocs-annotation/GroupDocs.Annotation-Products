---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API d'annotation Java DXF Annoter en C#"
head_description: "API Java pour créer et annoter des types d'annotations populaires à partir de DXF, des images, des dessins et des formats de fichiers de documents."

############################# Header ############################
title: "Annoter DXF à partir de Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Télécharger la version d'essai gratuite"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "À propos de l'API GroupDocs.Annotation pour Java"
    content: |
        L'API GroupDocs.Annotation for Java est une bibliothèque qui vous permet d'ajouter des annotations aux documents PDF, Word et autres sur Mac, Windows ou Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) est une API Java native pour la gestion des annotations avec une prise en charge complète pour la création, l'ajout, la modification, la suppression, l'extraction et l'exportation d'annotations à partir d'images et de divers autres documents. La liste complète des formats de documents pris en charge que vous pouvez voir sur cette [page](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Cette bibliothèque vous permet de travailler non seulement avec le document DXF mais également avec de nombreux autres types de documents tels que Word, Excel, PowerPoint, les e-mails Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad et bien d'autres.
        L'API GroupDocs.Annotation pour Java vous permet de créer et d'ajouter de nouvelles notes, de modifier des annotations, d'extraire des commentaires, des annotations et de les supprimer des documents. La bibliothèque prend en charge 13 types d'annotations différents, notamment Texte, Polyligne, Zone, Souligné, Point, Filigrane, Flèche, Ellipse, Remplacement de texte, Distance, Champ de texte, Rédaction de ressources en PDF, HTML, documents Microsoft Word, feuilles de calcul, diagrammes, présentations, dessins, images et de nombreux autres formats de fichiers.
        L'exemple (voir ci-dessous) montre comment travailler avec le document DXF, dans cet exemple, vous pouvez voir les principales étapes de la façon de travailler avec GroupDocs.Annotation : configurer une licence, ouvrir un document avec lequel vous souhaitez travailler, créer un annotation, en ajoutant des objets de données pour définir les propriétés d'annotation en fonction de vos besoins et en enregistrant le résultat à l'endroit requis. Vous pouvez également consulter plus en détail les fonctionnalités prises en charge sur notre [page github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), ou dans notre produit [documentation](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Étapes pour ajouter des annotations à DXF en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs Java d'ajouter facilement divers types d'annotations aux fichiers DXF dans n'importe quelle application Java en implémentant quelques étapes simples.
        *   Créez des objets de réponse avec un commentaire et une date.
        *   Créez un objet AreaAnnotation, définissez les options de zone et ajoutez des réponses.
        *   Créez un objet Annotator et ajoutez une annotation de zone.
        *   Enregistrez le fichier de sortie.
    title_right: "Configuration requise"
    content_right: |
        Les API GroupDocs.Annotation pour Java sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.
        *   Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        *   Environnement de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        *   Environnement d'exécution Java : Java 7 (1.7) et supérieur
        *   Obtenez la dernière version de GroupDocs.Annotation pour Java à partir de [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Aperçu des annotations et exemple de code
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
    title_left: "Étapes pour supprimer les annotations de DXF en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs Java de supprimer plus facilement les détails d'annotation des fichiers DXF dans n'importe quelle application Java en implémentant quelques étapes simples.
        *   Créez des objets de réponse avec un commentaire et une date.
        *   Instanciez l'objet SaveOptions et définissez AnnotationTypes = AnnotationType.None.
        *   Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

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
    title_left: "Étapes pour modifier les annotations de DXF en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs Java de mettre à jour plus facilement diverses propriétés d'annotation à partir de fichiers DXF dans n'importe quelle application Java en implémentant quelques étapes simples.
        *   Instanciez l'objet Annotator avec le chemin d'accès au document d'entrée ou le flux avec LoadOptions instancié avec ImportAnnotations = true.
        *   Créez une implémentation AnnotationBase et définissez l'ID de l'annotation existante (si l'annotation avec cet ID n'est pas trouvée, rien ne sera modifié) ou la liste des chemins d'annotations (toutes les annotations existantes seront supprimées).
        *   Appelez la méthode de mise à jour de l'objet Annotator avec les annotations transmises.
        *   Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

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
    title_left: "Étapes pour extraire les annotations de DXF en Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs Java d'annoter facilement des documents et d'extraire des informations d'annotation à partir de fichiers DXF dans n'importe quelle application Java en implémentant quelques étapes simples.
        *   Créez des objets de réponse avec un commentaire et une date.
        *   Instanciez l'objet LoadOptions et appelez SetImportAnnotations avec l'argument true.
        *   Définissez une variable de type Liste.
        *   Appelez la méthode get et renvoyez le résultat à la variable ci-dessus.

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
    title: "Démonstrations en direct pour ajouter, supprimer, modifier, extraire des annotations sur des documents et des images"
    content: |
        Ajoutez, supprimez, modifiez et extrayez des annotations dans le fichier DXF dès maintenant en visitant le site Web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). La démo en direct présente les avantages suivants

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dxf"
          title: "À propos du format de fichier DXF"
          content: |
            DXF, Drawing Interchange Format ou Drawing Exchange Format, est une représentation de données étiquetées du fichier de dessin AutoCAD. Chaque élément du fichier a un nombre entier de préfixe appelé code de groupe. Ce code de groupe représente en fait l'élément qui suit et indique la signification d'un élément de données pour un type d'objet donné. DXF permet de représenter presque toutes les informations spécifiées par l'utilisateur dans un fichier de dessin. Le format de fichier DXF a été développé par Autodesk en tant que format de fichier de données CAO pour l'interopérabilité des données entre AutoCAD et d'autres applications. Ainsi, les données peuvent être importées d'autres formats vers DXF vers AutoCAD conformément aux spécifications d'interopérabilité du format de fichier DXF.

          link: "https://docs.fileformat.com/image/dxf/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Travailler avec d'autres formats de documents courants"
    content: |
        Mettez à jour les propriétés d'annotation de certains des formats de fichiers populaires, comme indiqué ci-dessous.
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