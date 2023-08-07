---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "API d'annotation Net VSX Annoter en C#"
head_description: "Net API pour créer et annoter des types d'annotations populaires à partir de VSX, des images, des dessins et des formats de fichiers de documents."

############################# Header ############################
title: "Annoter VSX à partir du Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Télécharger la version d'essai gratuite"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "À propos de GroupDocs.Annotation pour l'API Net"
    content: |
        GroupDocs.Annotation for Net API est une bibliothèque qui vous permet d'ajouter des annotations aux documents PDF, Word et autres sur Mac, Windows ou Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) est une API Net native pour la gestion des annotations avec une prise en charge complète pour la création, l'ajout, la modification, la suppression, l'extraction et l'exportation d'annotations à partir d'images et de divers autres documents. La liste complète des formats de documents pris en charge que vous pouvez voir sur cette [page](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Cette bibliothèque vous permet de travailler non seulement avec le document VSX mais également avec de nombreux autres types de documents tels que Word, Excel, PowerPoint, les e-mails Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad et bien d'autres.
        L'API GroupDocs.Annotation for Net vous permet de créer et d'ajouter de nouvelles notes, de modifier des annotations, d'extraire des commentaires, des annotations et de les supprimer des documents. La bibliothèque prend en charge 13 types d'annotations différents, notamment Texte, Polyligne, Zone, Souligné, Point, Filigrane, Flèche, Ellipse, Remplacement de texte, Distance, Champ de texte, Rédaction de ressources en PDF, HTML, documents Microsoft Word, feuilles de calcul, diagrammes, présentations, dessins, images et de nombreux autres formats de fichiers.
        L'exemple (voir ci-dessous) montre comment travailler avec le document VSX, dans cet exemple, vous pouvez voir les principales étapes de la façon de travailler avec GroupDocs.Annotation : configurer une licence, ouvrir un document avec lequel vous souhaitez travailler, créer un annotation, en ajoutant des objets de données pour définir les propriétés d'annotation en fonction de vos besoins et en enregistrant le résultat à l'endroit requis. Vous pouvez également consulter plus en détail les fonctionnalités prises en charge sur notre [page] github(https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET), ou dans notre produit [documentation](https ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Étapes pour ajouter des annotations à VSX dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) permet aux développeurs Internet d'ajouter facilement divers types d'annotations aux fichiers VSX dans n'importe quelle application Internet en mettant en œuvre quelques étapes simples.
        *   Créez des objets de réponse avec un commentaire et une date.
        *   Créez un objet AreaAnnotation, définissez les options de zone et ajoutez des réponses.
        *   Créez un objet Annotator et ajoutez une annotation de zone.
        *   Enregistrez le fichier de sortie.
    title_right: "Configuration requise"
    content_right: |
        Les API GroupDocs.Annotation for Net sont prises en charge sur toutes les principales plateformes et systèmes d'exploitation. Avant d'exécuter le code ci-dessous, assurez-vous que les prérequis suivants sont installés sur votre système.
        *   Systèmes d'exploitation : Microsoft Windows, Linux, MacOS
        *   Environnements de développement : Visual Studio, Xamarin, MonoDevelop
        *   Frameworks : .NET Framework, .NET Standard, .NET Core, Mono
        *   Téléchargez la dernière version de GroupDocs.Annotation pour .NET à partir de [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Aperçu des annotations et exemple de code
    content: |
        ![Annotation preview image]https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png
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
    title_left: "Étapes pour supprimer les annotations de VSX dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) permet aux développeurs Internet de supprimer plus facilement les détails d'annotation des fichiers VSX dans n'importe quelle application Internet en mettant en œuvre quelques étapes simples.
        *   Créez des objets de réponse avec un commentaire et une date.
        *   Instanciez l'objet SaveOptions et définissez AnnotationTypes = AnnotationType.None.
        *   Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

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
    title_left: "Étapes pour modifier les annotations de VSX dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) permet aux développeurs Internet de mettre à jour plus facilement diverses propriétés d'annotation à partir de fichiers VSX dans n'importe quelle application Internet en mettant en œuvre quelques étapes simples.
        *   Instanciez l'objet Annotator avec le chemin d'accès au document d'entrée ou le flux avec LoadOptions instancié avec ImportAnnotations = true.
        *   Créez une implémentation AnnotationBase et définissez l'ID de l'annotation existante (si l'annotation avec cet ID n'est pas trouvée, rien ne sera modifié) ou la liste des chemins d'annotations (toutes les annotations existantes seront supprimées).
        *   Appelez la méthode de mise à jour de l'objet Annotator avec les annotations transmises.
        *   Appelez la méthode save avec le chemin ou le flux de document résultant et l'objet SaveOptions.

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
    title_left: "Étapes pour extraire les annotations de VSX dans Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) permet aux développeurs Internet d'annoter facilement des documents et d'extraire des informations d'annotation à partir de fichiers VSX dans n'importe quelle application Internet en mettant en œuvre quelques étapes simples.
        *   Créez des objets de réponse avec un commentaire et une date.
        *   Instanciez l'objet LoadOptions et appelez SetImportAnnotations avec l'argument true.
        *   Définissez une variable de type Liste.
        *   Appelez la méthode get et renvoyez le résultat à la variable ci-dessus.

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
    title: "Démonstrations en direct pour ajouter, supprimer, modifier, extraire des annotations sur des documents et des images"
    content: |
        Ajoutez, supprimez, modifiez et extrayez des annotations dans le fichier VSX dès maintenant en visitant le site Web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
La démo en direct présente les avantages suivants

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-vsx"
          title: "À propos du format de fichier VSX"
          content: |
            Les fichiers avec l'extension .VSX font référence à des gabarits constitués de dessins et de formes utilisés pour créer des diagrammes dans Microsoft Visio. Les fichiers VSX sont enregistrés au format de fichier XML et étaient pris en charge jusqu'à Visio 2013. Ils sont différents du format de fichier VSDX principal introduit avec Microsoft Visio 2013. Les fichiers VSX peuvent être ouverts dans n'importe quel éditeur de texte pour afficher le contenu.

          link: "https://docs.fileformat.com/image/vsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Travailler avec d'autres formats de documents courants"
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