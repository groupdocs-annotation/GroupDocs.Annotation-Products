
---
############################# Static ############################
layout: "auto-gen-annotation"
date: 07/05/2022 12:44:18
draft: false

###_DIMA_### link rel="canonical" href="https://products.groupdocs.com/annotation/net/dot"/>

############################# Head ############################
head_title: "Retirer Annotations depuis DOT dans l'application Net"
head_description: "Net API pour créer et Retirer types d'annotations populaires depuis DOT, images, dessins et formats de fichiers de documents."

############################# Header ############################
title: "Annotez DOT depuis Net"
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
        img_alt: "GroupDocs.Annotation pour Net"
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
    title: "À propos de GroupDocs.Annotation pour l'API Net"
    content: |
        L'API GroupDocs.Annotation for Net est une bibliothèque qui vous permet d'ajouter des annotations aux documents PDF, Word et autres sur Mac, Windows ou Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) est une API native Net pour la gestion des annotations avec une prise en charge complète pour la création, l'ajout, la modification, la suppression, l'extraction et l'exportation d'annotations à partir de images et divers autres documents. La liste complète des formats de documents pris en charge que vous pouvez voir sur cette [page](https://docs.groupdocs.com/annotation/net/supported-document-formats/).

        Cette bibliothèque vous permet de travailler non seulement avec le document DOT mais également avec de nombreux autres types de documents tels que Word, Excel, PowerPoint, les e-mails Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad et bien d'autres.

        L'API GroupDocs.Annotation pour Net vous permet de créer et d'ajouter de nouvelles notes, edit annotations, extract commentaires, annotations et remove les des documents. La bibliothèque prend en charge 13 types d'annotations différents, notamment Texte, Polyligne, Zone, Souligné, Point, Filigrane, Flèche, Ellipse, Remplacement de texte, Distance, Champ de texte, Rédaction de ressources en PDF, HTML, documents Microsoft Word, feuilles de calcul, diagrammes, présentations, dessins, images et de nombreux autres formats de fichiers.

        L'exemple (voir ci-dessous) illustre l'utilisation du document DOT. Dans cet exemple, vous pouvez voir les principales étapes de l'utilisation de GroupDocs.Annotation : configurer une licence, ouvrir un document avec lequel vous souhaitez travailler, créer un annotation, en ajoutant des objets de données pour définir les propriétés d'annotation en fonction de vos besoins et en enregistrant le résultat à l'endroit nécessaire. Vous pouvez également consulter plus en détail les fonctionnalités prises en charge sur notre github [page](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.Net), ou dans notre produit [documentation ](https://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Étapes pour ajouter des annotations depuis DOT dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Net d'ajouter facilement divers types d'annotations aux fichiers DOT dans n'importe quelle application basée sur Net en mettant en œuvre quelques étapes simples.
        * Créer des objets de réponse avec commentaire et date.
        * Créez un objet AreaAnnotation, définissez les options de zone et ajoutez des réponses.
        * Créer un objet Annotator et ajouter une annotation de zone.
        * Enregistrer le fichier de sortie.
    title_right: "Configuration requise"
    content_right: |
        Les API GroupDocs.Annotation pour Net sont prises en charge sur toutes les principales plates-formes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.
        * Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        * Environnements de développement : Visual Studio, Xamarin, MonoDevelop
        * Frameworks : .NET Framework, .NET Standard, .NET Core, Mono
        * Téléchargez la dernière version de GroupDocs.Annotation pour .NET à partir de [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title : "Aperçu des annotations et exemple de code"
    content : |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
    code: |
        ```cs
        //Ajouter une annotation de champ de texte au document à partir du disque local
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
                Message = "Ceci est une annotation de champ de texte",
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
                        Comment = "Premier commentaire",
                        RepliedOn = DateTime.Now
                    },
                    new Reply
                    {
                        Comment = "Deuxième commentaire",
                        RepliedOn = DateTime.Now
                    }
                }
            } ;
            annotator.Add(textField);
            annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Remove:
steps_Remove:
    enable: true
    title_left: "Étapes pour supprimer les annotations depuis DOT dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Net de supprimer plus facilement les détails d'annotation des fichiers DOT dans n'importe quelle application basée sur Net en mettant en œuvre quelques étapes simples.
        * Créer des objets de réponse avec commentaire et date.
        * Instanciez l'objet SaveOptions et définissez AnnotationTypes = AnnotationType.None.
        * Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

############################# Preview ############################
preview_Remove:
    enable: true
    
    code: |
        ```cs
        // 1- Comment supprimer une annotation d'un document à l'aide de l'index d'annotation
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            annotator.Remove(0);
            annotator.Save("removed.bmp");
        }
        
        // 2- Comment supprimer une annotation d'un document à l'aide d'un objet d'annotation
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var tmp = annotator.Get();
            annotator.Remove(tmp[0]);
            annotator.Save("removed.bmp");
        }
        
        // 3- Comment supprimer certaines annotations du document en utilisant la liste des identifiants
        
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            var idList = new List{1, 2, 3};
            annotator.Remove(idList);
            annotator.Save("removed.bmp");
        }
        
        // 4- Comment supprimer certaines annotations du document en utilisant la liste des annotations
        
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
    title_left: "Étapes pour modifier les annotations depuis DOT dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Net de mettre à jour plus facilement diverses propriétés d'annotation à partir de fichiers DOT dans n'importe quelle application basée sur Net en mettant en œuvre quelques étapes simples.
        * Instanciez l'objet Annotator avec le chemin d'accès au document d'entrée ou le flux avec LoadOptions instancié avec ImportAnnotations = true.
        * Créez une implémentation AnnotationBase et définissez l'ID de l'annotation existante (si l'annotation avec cet ID n'est pas trouvée, rien ne sera changé) ou la liste des chemins d'annotations (toutes les annotations existantes seront supprimées).
        * Appelez la méthode de mise à jour de l'objet Annotator avec les annotations passées.
        * Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

############################# Preview ############################
preview_Edit:
    enable: true
    
    code: |
        ```cs
        // ouvre le document annoté
        using (Annotator annotator = new Annotator("result.bmp"))
        {
            // en supposant que nous allons modifier certaines propriétés de l'annotation existante
                AreaAnnotation updated = new AreaAnnotation
                    {
                            // Il est important de définir l'identifiant de l'annotation existante
                            Id = 1,
                            BackgroundColor = 255,
                            Box = new Rectangle(0, 0, 50, 200),
                            CreatedOn = DateTime.Now,
                            Message = "Ceci est une annotation mise à jour",
                            Replies = new List
                            {
                                new Reply
                                {
                                    Comment = "Premier commentaire mis à jour",
                                    RepliedOn = DateTime.Now
                                },
                                new Reply
                                {
                                    Comment = "Mise à jour du deuxième commentaire",
                                    RepliedOn = DateTime.Now
                                }
                            }
                        } ;
                // mettre à jour l'annotation
                annotator.Update(updated);
                annotator.Save("result.bmp");
        }
        ```

############################# Steps ############################
howTo_Extract:
steps_Extract:
    enable: true
    title_left: "Étapes pour extraire les annotations depuis DOT dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) permet aux développeurs de Net d'annoter facilement des documents et d'extraire des informations d'annotation à partir de fichiers DOT dans n'importe quelle application basée sur Net en mettant en œuvre quelques étapes simples.
        * Créer des objets de réponse avec commentaire et date.
        * Instanciez l'objet LoadOptions et appelez SetImportAnnotations avec l'argument true.
        * Définir la variable avec le type Liste.
        * Appelez la méthode get et renvoyez le résultat à la variable ci-dessus.

############################# Preview ############################
preview_Extract:
    enable: true
    
    code: |
        ```cs
        // pour utiliser cet exemple, le fichier d'entrée ("annotated.bmp") doit être avec des annotations
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
    title: "Démos en direct pour extraire les annotations"
    content: |
        Affichez et supprimez les annotations du fichier DOT dès maintenant en visitant le site Web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
        La démo en direct présente les avantages suivants

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dot"
          title: "À propos du format de fichier DOT"
          content: |
            Les fichiers avec l'extension .DOT sont des fichiers modèles créés par Microsoft Word pour avoir des paramètres pré-formatés pour la génération d'autres fichiers DOC ou DOCX. Un fichier modèle est créé afin d'avoir des paramètres utilisateur spécifiques qui doivent être appliqués aux fichiers suivants créés à partir de ceux-ci. Ces paramètres incluent les marges de page, les bordures, les en-têtes, les pieds de page et d'autres paramètres de page. Ces modèles sont utilisés dans les documents officiels tels que les en-têtes d'entreprise et les formulaires standardisés. Le format de fichier DOT est spécifique à Microsoft Word 2003 et versions antérieures, mais est également pris en charge par les versions supérieures. Microsoft Word ouvre par défaut chaque nouveau document basé sur le fichier normal.dot. S'il est modifié, tous les nouveaux fichiers créés auront les mêmes paramètres que ceux du fichier modèle. Dans Microsoft Word 2007, le format de fichier DOT a été remplacé par le format de fichier DOTX basé sur Office OpenXML.
          link: "https://docs.fileformat.com/image/dot/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Travailler avec d'autres formats de documents populaires"
    content: |
        Mettez à jour les propriétés d'annotation de certains des formats de fichiers populaires, comme indiqué ci-dessous.
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