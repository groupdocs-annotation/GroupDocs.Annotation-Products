
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/java/xlsm"/>

############################# Head ############################
head_title: "Retirer Annotations depuis XLSM dans l'application Java"
head_description: "Java API pour créer et Retirer types d'annotations populaires depuis XLSM, images, dessins et formats de fichiers de documents."

############################# Header ############################
title: "Annotez XLSM depuis Java"
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
        img_alt: "GroupDocs.Annotation pour Java"
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
    title: "À propos de GroupDocs.Annotation pour l'API Java"
    content: |
        L'API GroupDocs.Annotation for Java est une bibliothèque qui vous permet d'ajouter des annotations aux documents PDF, Word et autres sur Mac, Windows ou Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) est une API native Java pour la gestion des annotations avec une prise en charge complète pour la création, l'ajout, la modification, la suppression, l'extraction et l'exportation d'annotations à partir de images et divers autres documents. La liste complète des formats de documents pris en charge que vous pouvez voir sur cette [page](https://docs.groupdocs.com/annotation/java/supported-document-formats/).

        Cette bibliothèque vous permet de travailler non seulement avec le document XLSM mais également avec de nombreux autres types de documents tels que Word, Excel, PowerPoint, les e-mails Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad et bien d'autres.

        L'API GroupDocs.Annotation pour Java vous permet de créer et d'ajouter de nouvelles notes, edit annotations, extract commentaires, annotations et remove les des documents. La bibliothèque prend en charge 13 types d'annotations différents, notamment Texte, Polyligne, Zone, Souligné, Point, Filigrane, Flèche, Ellipse, Remplacement de texte, Distance, Champ de texte, Rédaction de ressources en PDF, HTML, documents Microsoft Word, feuilles de calcul, diagrammes, présentations, dessins, images et de nombreux autres formats de fichiers.

        L'exemple (voir ci-dessous) illustre l'utilisation du document XLSM. Dans cet exemple, vous pouvez voir les principales étapes de l'utilisation de GroupDocs.Annotation : configurer une licence, ouvrir un document avec lequel vous souhaitez travailler, créer un annotation, en ajoutant des objets de données pour définir les propriétés d'annotation en fonction de vos besoins et en enregistrant le résultat à l'endroit nécessaire. Vous pouvez également consulter plus en détail les fonctionnalités prises en charge sur notre github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), ou dans notre produit [documentation ](https://docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Étapes pour ajouter des annotations depuis XLSM dans Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Java d'ajouter facilement divers types d'annotations aux fichiers XLSM dans n'importe quelle application basée sur Java en mettant en œuvre quelques étapes simples.
        * Créer des objets de réponse avec commentaire et date.
        * Créez un objet AreaAnnotation, définissez les options de zone et ajoutez des réponses.
        * Créer un objet Annotator et ajouter une annotation de zone.
        * Enregistrer le fichier de sortie.
    title_right: "Configuration requise"
    content_right: |
        Les API GroupDocs.Annotation pour Java sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.
        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnement de développement : NetBeans, Intellij IDEA, Eclipse, etc.
        * Environnement d'exécution Java : Java 7 (1.7) et supérieur
        * Obtenez la dernière version de GroupDocs.Annotation pour Java à partir de [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title : "Aperçu des annotations et exemple de code"
    content : |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-area-annotation.png)
    code: |
        ```java
        // Crée une instance de la classe Reply et ajoute des commentaires
        Reply firstReply = new Reply();
        firstReply.setComment("Premier commentaire");
        firstReply.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply secondReply = new Reply();
        secondReply.setComment("Deuxième commentaire");
        secondReply.setRepliedOn(Calendar.getInstance().getTime());
        
        List<Reply> replies = new ArrayList<Reply>();
        replies.add(firstReply);
        replies.add(secondReply);
        
        // Crée une instance de la classe AreaAnnotation et définit les options
        AreaAnnotation area = new AreaAnnotation();
        area.setBackgroundColor(65535);
        area.setBox(new Rectangle(100, 100, 100, 100));
        area.setCreatedOn(Calendar.getInstance().getTime());
        area.setMessage("Ceci est une annotation de area");
        area.setOpacity(0.7);
        area.setPageNumber(0);
        area.setPenColor(65535);
        area.setPenStyle(PenStyle.Dot);
        area.setPenWidth((byte) 3);
        area.setReplies(replies);
        
        // Crée une instance de la classe Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Ajouter une annotation
        annotator.add(area);
        
        // Enregistrer dans un fichier
        annotator.save("output.bmp");
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Étapes pour supprimer les annotations depuis XLSM dans Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Java de supprimer plus facilement les détails d'annotation des fichiers XLSM dans n'importe quelle application basée sur Java en mettant en œuvre quelques étapes simples.
        * Créer des objets de réponse avec commentaire et date.
        * Instanciez l'objet SaveOptions et définissez AnnotationTypes = AnnotationType.None.
        * Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```java
        // Crée une instance de la classe Annotator
        Annotator annotator = new Annotator("C://input.bmp");

        // Supprimer l'annotation par type d'ensemble Aucun
        SaveOptions saveOptions = new SaveOptions();
        saveOptions.setAnnotationTypes(AnnotationType.None);

        // Enregistrer l'annotation dans le fichier de sortie
        annotator.save("C://output.bmp", saveOptions);
        annotator.dispose();
        ```

############################# Steps ############################
howTo_Edit:
steps_Edit:
    enable: true
    title_left: "Étapes pour modifier les annotations depuis XLSM dans Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Java de mettre à jour plus facilement diverses propriétés d'annotation à partir de fichiers XLSM dans n'importe quelle application basée sur Java en mettant en œuvre quelques étapes simples.
        * Instanciez l'objet Annotator avec le chemin d'accès au document d'entrée ou le flux avec LoadOptions instancié avec ImportAnnotations = true.
        * Créez une implémentation AnnotationBase et définissez l'ID de l'annotation existante (si l'annotation avec cet ID n'est pas trouvée, rien ne sera changé) ou la liste des chemins d'annotations (toutes les annotations existantes seront supprimées).
        * Appelez la méthode de mise à jour de l'objet Annotator avec les annotations passées.
        * Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```java
        String outputPath = "UpdateAnnotation.bmp" ;

        // Crée une instance de la classe Annotator
        Annotator annotator = new Annotator("input.bmp");
        
        // Crée une instance de la classe Reply pour le premier exemple et ajoute des commentaires
        Reply reply1 = new Reply();
        reply1.setComment("Premier commentaire d'origine");
        reply1.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply2 = new Reply();
        reply2.setComment("Deuxième commentaire original");
        reply2.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies.add(reply1);
        replies.add(reply2);
        
        // Crée une instance de la classe AreaAnnotation et définit les options
        AreaAnnotation original = new AreaAnnotation();
        original.setId(1);
        original.setBackgroundColor(65535);
        original.setBox(nouveau Rectangle(100, 100, 100, 100));
        original.setCreatedOn(Calendar.getInstance().getTime());
        original.setMessage("Ceci est l'annotation originale");
        original.setReplies(replies1);
        
        // Ajouter l'annotation d'origine
        annotator.add(original);
        annotator.save(outputPath);
        annotator.dispose();
        
        LoadOptions loadOptions = new LoadOptions();
        
        // Ouvrir le document annoté
        Annotator annotator1 = new Annotator(outputPath, loadOptions);
        
        // Crée une instance de la classe Reply pour mettre à jour le premier exemple
        Reply reply3 = new Reply();
        reply3.setComment("Premier commentaire mis à jour");
        reply3.setRepliedOn(Calendar.getInstance().getTime());
        
        Reply reply4 = new Reply();
        reply4.setComment("Deuxième commentaire mis à jour");
        reply4.setRepliedOn(Calendar.getInstance().getTime());
        
        java.util.List replies1 = new ArrayList();
        replies1.add(reply3);
        replies1.add(reply4);

        // Suggère que nous voulons modifier certaines propriétés d'une annotation existante
        AreaAnnotation updated = new AreaAnnotation();
        updated.setId(1);
        updated.setBackgroundColor(255);
        updated.setBox(new Rectangle(0, 0, 50, 200));
        updated.setCreatedOn(Calendar.getInstance().getTime());
        updated.setMessage("Ceci est une annotation mise à jour");
        updated.setReplies(replies1);
        
        // Mettre à jour et enregistrer l'annotation
        annotator1.update(updated);
        annotator1.save(outputPath);
        annotator1.dispose();
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Étapes pour extraire les annotations depuis XLSM dans Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Java d'annoter facilement des documents et d'extraire des informations d'annotation à partir de fichiers XLSM dans n'importe quelle application basée sur Java en mettant en œuvre quelques étapes simples.
        * Créer des objets de réponse avec commentaire et date.
        * Instanciez l'objet LoadOptions et appelez SetImportAnnotations avec l'argument true.
        * Définir la variable avec le type Liste.
        * Appelez la méthode get et renvoyez le résultat à la variable ci-dessus.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```java
        // Pour utiliser cet exemple, le fichier d'entrée ("annotated.bmp") doit être avec des annotations
        LoadOptions loadOptions = new LoadOptions();
        
        // Crée une instance de la classe Annotator et récupère les annotations
        final Annotator annotator = new Annotator("annotated.bmp", loadOptions);
        List annotations = annotator.get();
        ```

############################# Demos ############################
demos:
    enable: true
    title: "Démos en direct pour extraire les annotations"
    content: |
        Affichez et supprimez les annotations du fichier XLSM dès maintenant en visitant le site Web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        La démo en direct présente les avantages suivants

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsm"
          title: "À propos du format de fichier XLSM"
          content: |
            Les fichiers avec l'extension XLSM sont un type de fichiers de feuille de calcul prenant en charge les macros. Du point de vue de l'application, une macro est un ensemble d'instructions utilisées pour automatiser les processus. Une macro est utilisée pour enregistrer les étapes qui sont exécutées à plusieurs reprises et facilite l'exécution des actions en exécutant à nouveau la macro. Les macros sont programmées avec Visual Basic pour Applications (VBA) de Microsoft à partir du classeur Excel à l'aide de Visual Basic Editor et peuvent être exécutées/déboguées directement à partir de là.
          link: "https://docs.fileformat.com/image/xlsm/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Travailler avec d'autres formats de documents populaires"
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