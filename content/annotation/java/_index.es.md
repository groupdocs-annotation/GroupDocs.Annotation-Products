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
head_title: "API de anotación de documentos de Java | Ver y anotar imágenes PDF Word Excel PPTX"
head_description: "API de anotación de documentos de Java. Ver, etiquetar, comentar y anotar PDF Word DOCX, Excel XLSX, PPTX, EML EMLX, VSS VSD, OTP, CAD y formatos de archivo de imagen."

############################# Header ############################
title: "Anotación de documentos a través de la API de Java"
description: "Cree aplicaciones Java con capacidades para ver y anotar PDF, HTML, MS Office y otros formatos de documentos sin instalar ningún software externo."
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Descargue prueba gratis"
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
              text: "Visión de conjunto"

            # button loop
            - link: "#features"
              text: "Características"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/annotation"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/annotation/java"
              text: "Precios"

    right:
        link_download: "https://downloads.groupdocs.com/annotation"
        link_learn: "https://docs.groupdocs.com/annotation/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Visión de conjunto ############################
overview:
    enable: true
    content: |
      GroupDocs.Annotation for Java API proporciona una funcionalidad de manipulación, gestión de anotaciones y documentos fácil de usar para usar en sus aplicaciones empresariales basadas en Java. Nuestra biblioteca de anotadores de Java le permite trabajar con muchos tipos de anotaciones, que incluyen texto, polilínea, área, subrayado, punto, marca de agua, flecha, elipse, reemplazo de texto, distancia, campo de texto, redacción de recursos, etc. También ofrece un conjunto completo de objetos de datos para personalizar las propiedades de anotación según sus requisitos dentro de todos los formatos de documentos admitidos, incluidos: PDF, HTML, oficina de Microsoft Word, hojas de cálculo de Excel, presentaciones de PowerPoint, Visio, correos electrónicos de Outlook, imágenes, metarchivos, dibujos CAD y varios otros formatos.
        
      La API brinda la capacidad de obtener miniaturas de páginas de documentos y admite la importación y exportación de anotaciones hacia y desde archivos PDF.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          A continuación se muestra una descripción general de GroupDocs.Annotation para Java:
      
        right:
          enable: true
          icon: "fab fa-html5"
          title: "Visión de conjunto"
          content: |
            * Agregar anotaciones
            * Exportar anotaciones
            * Importar anotaciones
            * Comentarios basados en respuestas
            * Compatibilidad de anotaciones
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Annotation para Java es compatible con todos los [formatos de archivo de documentos populares](https://docs.groupdocs.com/annotation/java/supported-document-formats/), incluidos: oficina de Microsoft, PDF, imágenes y muchos otros.

        left:
          enable: true
          table:
            # table loop
            - title: "Formatos de oficina de Microsoft"
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
            - title: "Otros formatos"
              content: |
                * **Portable**: PDF (PDF/A-1a, PDF/A-1b, PDF/A-2a)
                * **OpenDocument**: ODT, ODS, ODP
                * **Images**: BMP, JPG, TIFF, TIF, PNG
                * **AutoCAD**: DWG, DXF
                * **Other**: HTML

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Annotation para Java es compatible con los siguientes sistemas operativos, marcos y administradores de paquetes:
      
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Sistemas operativos"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Marcos compatibles"
              content: |
                * Java 7 (1.7) y superior

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entornos de desarrollo"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Herramienta de automatización de compilación"
              content: |
                * Maven

############################# Características ############################
features:
    enable: true
    title: "Funciones de GroupDocs.Annotation para Java"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        link: "https://docs.groupdocs.com/annotation/java/add-area-annotation/"
        content: "Agregar anotación de área en el documento y vincular comentarios simples y anidados"

      # feature loop
      - icon: "fas fa-eye"
        link: "https://docs.groupdocs.com/annotation/java/add-arrow-annotation/"
        content: "Apunte a un contenido en particular usando la anotación de flecha"

      # feature loop
      - icon: "fas fa-bolt"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: "Establezca marcas de agua de texto en PDF, diapositivas, hojas de cálculo de Excel, imágenes y diagramas en posición en ángulo"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Agregar comentarios emergentes a cualquier lugar del documento mediante la anotación de puntos"

      # feature loop
      - icon: "fas fa-code"
        link: "https://docs.groupdocs.com/annotation/java/add-polyline-annotation/"
        content: "Utilice la anotación de polilínea para conectar la secuencia de segmentos de línea, segmentos de arco o ambos"

      # feature loop
      - icon: "fas fa-cloud"
        link: "https://docs.groupdocs.com/annotation/java/add-ellipse-annotation/"
        content: "Agregue anotaciones de elipse a PDF, documentos de Word, hojas de cálculo, presentaciones, diagramas e imágenes"

      # feature loop
      - icon: "fas fa-remove-format"
        link: "https://docs.groupdocs.com/annotation/java/add-watermark-annotation/"
        content: "Agregue marcas de agua en ángulo para PDF, PowerPoint, Excel, imágenes y diagramas"

      # feature loop
      - icon: "fas fa-comment-slash"
        link: "https://docs.groupdocs.com/annotation/java/extract-annotations-from-document/"
        content: "Obtener coordenadas de anotación de texto en la representación de imagen de un documento"

      # feature loop
      - icon: "fas fa-location-arrow"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Subrayar, tachar o modificar texto específico en un documento"

      # feature loop
      - icon: "fas fa-border-all"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Agregar sello de texto o marca de agua y campo de texto en un documento"

      # feature loop
      - icon: "fas fa-wrench"
        link: "https://docs.groupdocs.com/annotation/net/advanced-usage/"
        content: "Import & Exportar anotaciones among Word Documents & PowerPoint Presentations"

      # feature loop
      - icon: "fas fa-columns"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Anotar hojas de cálculo de Excel con tipos de anotación de texto, reemplazo de texto, marca de agua y redacción de recursos"

      # feature loop
      - icon: "fas fa-file-word"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Agregue anotaciones de polilínea, tachado, subrayado o texto a presentaciones y diapositivas de PowerPoint"

      # feature loop
      - icon: "fas fa-envelope"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Anotación de punto de marca en presentaciones usando coordenadas X, Y"

      # feature loop
      - icon: "fas fa-print"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Agregue anotaciones de tachado, texto, subrayado o polilínea a las imágenes"

      # feature loop
      - icon: "fas fa-file-archive"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: "Obtener información e imágenes de documentos para diagramas de Visio, como VSS y VSD"

      # feature loop
      - icon: "fas fa-file-code"
        link: "https://docs.groupdocs.com/annotation/java/basic-usage/"
        content: "Obtenga miniaturas de las páginas del documento y trabaje con archivos TIFF de varias páginas"
      
      # feature loop
      - icon: "fas fa-file-excel"
        link: "https://docs.groupdocs.com/annotation/java/get-file-info/"
        content: "Obtener todas las anotaciones de un documento con una sola llamada de función"

      # feature loop
      - icon: "fas fa-heading"
        link: "https://docs.groupdocs.com/annotation/java/add-link-annotation/"
        content: "Agregar anotaciones de vínculos a presentaciones de PDF, Word y PowerPoint"

      # feature loop
      - icon: "fas fa-project-diagram"
        link: "https://docs.groupdocs.com/annotation/java/add-point-annotation/"
        content: "Compatibilidad con SVG Path Parsing para PDF, Word, diagramas, diapositivas y otros formatos de documentos importantes"

      # feature loop
      - icon: "fas fa-cube"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: "Soporte para agregar anotaciones de marca de agua a documentos de Word y limpieza para reemplazo de texto"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/technical-support/"
        content: "Compatibilidad con procesamiento de formas en diagramas para anotaciones de texto"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/advanced-usage/"
        content: "Ahorre tiempo almacenando en caché vistas previas de páginas de documentos para un procesamiento más rápido"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-annotation-to-the-document/"
        content: "Anote fácilmente documentos de Word, Excel y PowerPoint incluso con formatos más antiguos"

      # feature loop
      - icon: "fab fa-uncharted"
        link: "https://docs.groupdocs.com/annotation/java/add-distance-annotation/"
        content: "Mostrar leyendas de anotaciones de distancia para Excel, PowerPoint y diagramas"

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Annotation ofrece API de visualización de documentos para otros entornos de desarrollo populares"

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
