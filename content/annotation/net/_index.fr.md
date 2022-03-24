---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "API d'annotation de documents C# .NET | Annoter les fichiers image PDF Word Excel PPTX"
head_description: "API d'annotation de documents C# .NET. Affichez, étiquetez, commentez et annotez des fichiers PDF Word DOC DOCX, Excel XLS XLSX, PPT PPTX, OTP, CAD, EMF WMF et image."

############################# Header ############################
title: "Annoter du texte ou des images dans des documents"
description: "Donnez à vos applications .NET les moyens d'ajouter, de modifier et de supprimer tous les types d'annotations populaires de plus de 50 formats de documents pour une collaboration plus simple et efficace."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Télécharger la version d'essai gratuite"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for .NET"
        image: "/border/groupdocs-annotation-net.svg"
        product: "GroupDocs.Annotation"
        platform: ".NET"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Aperçu"

            # button loop
            - link: "#features"
              text: "Caractéristiques"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation pour .NET est un ensemble complet d'API qui vous aide à créer des applications de gestion d'annotations de documents en C#, ASP.NET et d'autres technologies .NET associées. Vous pouvez créer et travailler avec tous les types d'annotations populaires, tels que zone, point, texte, ellipse, lien, soulignement, polyligne, flèche, distance, filigrane, image, etc. pour PDF, HTML, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, Visio, images, dessin CAO et divers autres formats. La bibliothèque d'annotateurs de documents vous permet d'exporter des documents après avoir ajouté des annotations, des commentaires ou des notes en surbrillance à leur format d'origine. Il vous donne également un ensemble pratique d'objets de données grâce auxquels vous pouvez personnaliser les annotations selon vos besoins.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Annotation pour .NET :

        right:
          enable: true
          icon: "fab fa-html5"
          title: "Aperçu"
          content: |
            * Ajouter des annotations
            * Exporter les annotations
            * Importer des annotations            
            * Commentaires basés sur les réponses
            * Compatibilité des annotations
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation pour .NET prend en charge tous les [formats de fichiers de documents](https://docs.groupdocs.com/annotation/net/supported-document-formats/) courants, y compris : Microsoft Office, PDF, images et bien d'autres.

        left:
          enable: true
          table:
            # table loop
            - title: "Formats Microsoft Office"
              content: |
                * **Microsoft Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF 
                * **Microsoft Excel**: XLS, XLSX, XLSM, XLSB, CSV
                * **Microsoft PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Microsoft Visio**: VSD, VSS, VSDX, VST, VSDM, VSSX, VSTM

        right:
          enable: true
          table:
            # table loop
            - title: "Autres formats"
              content: |
                * **Portable** : PDF (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **Document ouvert** : ODT, ODS, ODP
                * **Images** : BMP, JPEG, PNG, TIFF
                * **AutoCAD** : DWG, DXF
                * **Métafichiers** : EMF, WMF
                * **Courriel** : EML, EMLX
                * **Web** : HTM, HTML

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for .NET prend en charge la suite Systèmes d'exploitation, Frameworks & Directeur chargé d'emballages:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Windows (x86 et x64)
                * Serveur Windows (x86 et x64)
                * windows Azure
                * Linux
                * Mac OS

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * Norme .NET 2.0
                * .NET Framework 2.0 ou supérieur
                * .NET Core 2.0 ou supérieur
                * Mono Framework 1.2 ou supérieur

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Directeur chargé d'emballage"
              content: |
                * NuGet
            
            # table loop
            - icon: "fas fa-tools"
              title: "Environnements de développement"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Annotation pour les fonctionnalités .NET"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Ajouter, modifier et supprimer des annotations et des réponses"

      # feature loop
      - icon: "fas fa-eye"
        content: "Exporter les annotations vers le document"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Licence mesurée - Facturation contrôlée en payant en fonction de l'utilisation de l'API"
      
      # feature loop
      - icon: "fas fa-code"
        content: "Appel de fonction unique pour récupérer toutes les annotations d'un document"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Affecter une valeur à une annotation de point ou déplacer une valeur de point existante"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Ajouter une annotation de lien aux diapositives PDF, Word et PowerPoint"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Définir la couleur d'arrière-plan d'une annotation ou supprimer toutes les annotations du document"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Annotez les fichiers PDF avec précision - Obtenez une représentation d'image du document PDF et des aperçus de page de cache"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Obtenir les coordonnées textuelles de l'annotation textuelle dans la représentation d'image du document"

      # feature loop
      - icon: "fas fa-columns"
        content: "Lier les commentaires des utilisateurs à l'annotation de zone et à la prise en charge des commentaires imbriqués"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Utiliser l'annotation fléchée pour pointer vers un contenu particulier"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Utiliser l'annotation de distance pour tracer une ligne qui représente la distance entre les objets"

      # feature loop
      - icon: "fas fa-print"
        content: "Annotation basée sur des points qui, lorsqu'on clique dessus, fait apparaître la fenêtre pour ajouter des commentaires"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Créer une séquence connectée de segments de ligne créés en tant qu'annotation de polyligne"

      # feature loop
      - icon: "fas fa-lock"
        content: "Créer des segments de ligne droite, des segments d'arc ou une combinaison des deux"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Marquer les zones de document proposées pour la rédaction"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Ajouter des annotations d'image aux PDF, diagrammes, Word, Excel, présentations et images"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Ajouter un champ de texte et un tampon ou un filigrane basé sur du texte dans le document"

      # feature loop
      - icon: "fas fa-heading"
        content: "Barré, souligné ou remplacé un texte particulier dans un document"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Redimensionner l'annotation en attribuant de nouveaux paramètres de hauteur et de largeur"

      # feature loop
      - icon: "fas fa-cube"
        content: "Obtenir des vignettes de pages de document. Gérer une variété de documents annotés pour les images et les diagrammes"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Exporter des annotations vers et travailler avec des fichiers TIFF multipages"
  
      # feature loop
      - icon: "fab fa-uncharted"
        content: "Ajuster l'alignement vertical et horizontal pour l'annotation de filigrane"
  
      # feature loop
      - icon: "fab fa-uncharted"
        content: "Ajouter un alignement horizontal du texte pour le champ de texte"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Obtenir des informations sur les lignes de texte du document (texte, largeur, hauteur, retraits)"

    more_feature :
      # more_feature_loop
      - title: "Prise en charge de plusieurs types d'annotations"
        content: |
          GroupDocs.Annotation pour .NET vous permet de travailler avec différents types d'annotations. Cela donne la liberté et la facilité de communication tout en collaborant avec votre équipe sur des tâches. Vous pouvez utiliser des annotations, telles que l'annotation de zone (marquer une zone en tant que rectangle et y ajouter des notes), l'annotation de points (coller des commentaires à n'importe quel endroit du document), l'annotation de texte (ajouter un commentaire au texte sélectionné), l'annotation barrée/soulignée ( appliqué à un paragraphe), annotation de polyligne (dessiner des formes et des lignes à main levée), annotation de flèche (pointeur fléché avec commentaires attachés), annotation d'ellipse (afficher le texte à l'intérieur de l'ellipse), annotation de distance (dessiner une ligne qui représente la distance entre les objets), lien annotation (ajouter des liens Web aux formats de document pris en charge) et annotation en filigrane (un tampon de texte ou un filigrane peut être ajouté au document).

          ```cs
          // Initialiser la liste des AnnotationInfo
          List<AnnotationInfo> annotations = new List<AnnotationInfo>();
          // Initialiser l'annotation de texte
          AnnotationInfo textAnnotation = new AnnotationInfo
          {
            Box = new Rectangle((float)265.44, (float)153.86, 206, 36), Type = AnnotationType.Text 
          };
          // Ajouter une annotation à la liste
          annotations.Add(textAnnotation);
          // Obtenir le flux du fichier d'entrée
          Stream inputFile = new FileStream("D:/input.pdf", FileMode.Open, File
          .ReadWrite);
          // Exporter l'annotation et enregistrer le fichier de sortie
          CommonUtilities.SaveOutputDocument(inputFile, annotations, DocumentType.Pdf);
          ```

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for Java"
          image: "/border/groupdocs-annotation-java.svg"
          product: "GroupDocs.Annotation"
          platform: "Java"
          link: "/annotation/java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
