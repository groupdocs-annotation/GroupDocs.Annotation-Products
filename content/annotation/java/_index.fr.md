---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Annotation"
product_tag: "annotation"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "API d'annotation de documents Java | Afficher et annoter des images PDF Word Excel PPTX"
head_description: "API d'annotation de documents Java. Affichez, étiquetez, commentez et annotez des PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAO et formats de fichiers image."

############################# Header ############################
title: "Annotation de documents via l'API Java"
description: "Créez des applications Java avec des capacités pour afficher et annoter des formats PDF, HTML, MS Office et d'autres formats de documents sans installer de logiciel externe."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Télécharger la version d'essai gratuite"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Annotation for Java"
        image: "/border/groupdocs-annotation-java.svg"
        product: "GroupDocs.Annotation"
        platform: "Java"

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
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Aperçu ############################
overview:
    enable: true
    content: |
      L'API GroupDocs.Annotation pour Java fournit des fonctionnalités de gestion de documents, d'annotations et de manipulation faciles à utiliser dans vos applications métier basées sur Java. Notre bibliothèque d'annotateurs Java vous permet de travailler avec de nombreux types d'annotations, notamment du texte, une polyligne, une zone, un soulignement, un point, un filigrane, une flèche, une ellipse, un remplacement de texte, une distance, un champ de texte, une rédaction de ressources, etc. Il offre également un ensemble complet d'objets de données pour personnaliser les propriétés d'annotation selon vos besoins dans tous les formats de document pris en charge, notamment : PDF, HTML, Microsoft Office Word, feuilles de calcul Excel, présentations PowerPoint, Visio, e-mails Outlook, images, métafichiers, dessin CAO et divers autres formats.
        
      L'API offre la possibilité d'obtenir des vignettes de pages de document et prend en charge l'importation et l'exportation d'annotations vers et depuis des fichiers PDF.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Voici un aperçu de GroupDocs.Annotation pour Java :
      
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
          GroupDocs.Annotation pour Java prend en charge tous les [formats de fichiers de documents](https://docs.groupdocs.com/annotation/java/supported-document-formats/) courants, y compris : Microsoft Office, PDF, images et bien d'autres.

        left:
          enable: true
          table:
            # table loop
            - title: "Formats Microsoft Office"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM, RTF
                * **Excel**: XLS, XLSX, XLSB, XLSM
                * **PowerPoint**: PPT, PPTX, PPS, PPSX
                * **Outlook**: EML, EMLX
                * **Visio**: VSS, VST, VSD, VSDX

        right:
          enable: true
          table:
            # table loop
            - title: "Autres formats"
              content: |
                * **Portable** : PDF (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **Document ouvert** : ODT, ODS, ODP
                * **Images** : BMP, JPG, TIFF, TIF, PNG
                * **AutoCAD** : DWG, DXF
                * **Autre** : HTML

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation for Java prend en charge la suite Systèmes d'exploitation, Frameworks & Directeur chargé d'emballages:
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Systèmes d'exploitation"
              content: |
                * Bureau Microsoft Windows
                * Serveur Microsoft Windows
                * Linux
                * Mac OS

            # table loop
            - icon: "fas fa-code"
              title: "Cadres pris en charge"
              content: |
                * Java 7 (1.7) et supérieur

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Environnements de développement"
              content: |
                * NetBeans
                * IDÉE IntelliJ
                * Éclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Outil d'automatisation de construction"
              content: |
                * Maven

############################# Caractéristiques ############################
features:
    enable: true
    title: "GroupDocs.Annotation pour les fonctionnalités Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Ajouter une annotation de zone dans le document et lier des commentaires simples et imbriqués"

      # feature loop
      - icon: "fas fa-eye"
        content: "Pointez vers un contenu particulier à l'aide d'une annotation fléchée"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Définir des filigranes de texte sur PDF, des diapositives, des feuilles de calcul Excel, des images et des diagrammes en position inclinée"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Ajoutez des commentaires contextuels à n'importe quel endroit du document à l'aide de l'annotation de points"

      # feature loop
      - icon: "fas fa-code"
        content: "Utiliser l'annotation polyligne pour connecter une séquence de segments de ligne, des segments d'arc ou les deux"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Ajouter une annotation Ellipse aux PDF, documents Word, feuilles de calcul, présentations, diagrammes et images"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Ajouter des filigranes angulaires pour PDF, PowerPoint, Excel, images et diagrammes"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Récupérer les coordonnées de l'annotation de texte dans la représentation d'image d'un document"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Souligner, barrer ou modifier un texte spécifique dans un document"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Ajouter un tampon de texte ou un filigrane et un champ de texte dans un document"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Importer et exporter des annotations parmi des documents Word et des présentations PowerPoint"

      # feature loop
      - icon: "fas fa-columns"
        content: "Annoter des feuilles de calcul Excel avec des types d'annotation de texte, de remplacement de texte, de filigrane et de rédaction de ressources"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Ajouter des annotations polylignes, barrées, soulignées ou textuelles aux présentations et diapositives PowerPoint"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Marquer l'annotation de points dans les présentations à l'aide des coordonnées X, Y"

      # feature loop
      - icon: "fas fa-print"
        content: "Ajouter des annotations barrées, textuelles, soulignées ou polylignes aux images"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Récupérer des informations sur les documents et des images pour les diagrammes Visio, tels que VSS et VSD"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Obtenez des vignettes des pages de document et travaillez avec des fichiers TIFF multipages"
      
      # feature loop
      - icon: "fas fa-file-excel"
        content: "Récupérer toutes les annotations d'un document avec un seul appel de fonction"

      # feature loop
      - icon: "fas fa-heading"
        content: "Ajouter des annotations de lien aux présentations PDF, Word et PowerPoint"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Prise en charge de l'analyse de chemin SVG pour PDF, Word, diagrammes, diapositives et autres principaux formats de documents"

      # feature loop
      - icon: "fas fa-cube"
        content: "Prise en charge de l'ajout d'annotations de filigrane aux documents Word et du nettoyage pour le remplacement de texte"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Prise en charge du traitement de forme dans les diagrammes pour les annotations de texte"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Gagnez du temps en mettant en cache les aperçus de page des documents pour un traitement plus rapide"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Annotez facilement des documents Word, Excel et PowerPoint, même avec des formats plus anciens"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Afficher les légendes d'annotation de distance pour Excel, PowerPoint et les diagrammes"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation propose des API de visualisation de documents pour d'autres environnements de développement populaires"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Annotation for .NET"
          image: "/border/groupdocs-annotation-net.svg"
          product: "GroupDocs.Annotation"
          platform: ".NET"
          link: "/annotation/net/"

############################# Back to top ###############################
back_to_top:
  enable: true
---
