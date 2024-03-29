---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net XLSX Annotation API Annotate en C#"
head_description: "Net API per crear i anotar tipus d'anotacions populars a partir de XLSX, imatges, dibuixos i formats de fitxers de documents."

############################# Header ############################
title: "Anoteu XLSX de Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Baixeu la prova gratuïta"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Quant a GroupDocs.Annotation for Net API"
    content: |
        GroupDocs.Annotation for Net API és una biblioteca que us permet afegir anotacions a PDF, Word i altres documents a Mac, Windows o Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) és una API de xarxa nativa per gestionar anotacions amb suport complet per crear, afegir, editar, suprimir, extreure i exportar anotacions d'imatges i altres documents. La llista completa dels formats de document compatibles que podeu veure en aquesta [pàgina](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Aquesta biblioteca us permet treballar no només amb el document XLSX sinó també amb molts altres tipus de documents com ara Word, Excel, PowerPoint, correus electrònics d'Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad i molts altres.
        L'API de GroupDocs.Annotation per a Net us permet crear i afegir notes noves, editar anotacions, extreure comentaris i anotacions i eliminar-los dels documents. La biblioteca admet 13 tipus d'anotacions diferents, com ara text, polilínia, àrea, subratllat, punt, filigrana, fletxa, el·lipse, substitució de text, distància, camp de text, redacció de recursos en PDF, HTML, documents de Microsoft Word, fulls de càlcul, diagrames, presentacions, dibuixos, imatges i molts altres formats de fitxer.
        L'exemple (vegeu a continuació) mostra com es treballa amb el document XLSX, en aquest exemple podeu veure els passos principals de com treballar amb GroupDocs. Anotació: configureu una llicència, obriu un document amb el qual voleu treballar i creeu un anotació, afegint objectes de dades per establir propietats d'anotació segons els vostres requisits i desant el resultat al lloc necessari. També podeu veure més detalladament les funcions admeses a la nostra [pàgina github](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) o a la nostra [documentació del producte](https://docs.groupdocs.com/annotation/net/getting-started/)

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Passos per afegir anotacions a XLSX a Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita que els desenvolupadors de Net puguin afegir diversos tipus d'anotacions als fitxers XLSX dins de qualsevol aplicació basada en Net mitjançant la implementació d'uns quants passos senzills.
        *   Creeu objectes de resposta amb comentari i data.
        *   Creeu un objecte AreaAnnotation, configureu opcions d'àrea i afegiu respostes.
        *   Creeu un objecte Annotator i afegiu una anotació d'àrea.
        *   Desa el fitxer de sortida.
    title_right: "Requisits del sistema"
    content_right: |
        GroupDocs.Annotation per a les API de xarxa són compatibles amb totes les plataformes i sistemes operatius principals. Abans d'executar el codi següent, assegureu-vos que teniu els següents requisits previs instal·lats al vostre sistema.
        *   Sistemes operatius: Microsoft Windows, Linux, MacOS
        *   Entorns de desenvolupament: Visual Studio, Xamarin, MonoDevelop
        *   Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
        *   Baixeu la darrera versió de GroupDocs.Annotation per a .NET des de [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Vista prèvia de l'anotació i mostra de codi
    content: |
        ![Annotation preview image](https://docs.groupdocs.com/annotation/java/images/add-text-field-annotation.png)
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
    title_left: "Passos per eliminar les anotacions de XLSX a Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita als desenvolupadors de Net eliminar els detalls de les anotacions dels fitxers XLSX dins de qualsevol aplicació basada en Net mitjançant la implementació d'uns quants passos senzills.
        *   Creeu objectes de resposta amb comentari i data.
        *   Crea una instancia de l'objecte SaveOptions i estableix AnnotationTypes = AnnotationType.None.
        *   Truqueu al mètode de desar amb la ruta o flux del document resultant i l'objecte SaveOptions.

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
    title_left: "Passos per editar les anotacions de XLSX a Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita que els desenvolupadors de Net actualitzin diverses propietats d'anotació dels fitxers XLSX dins de qualsevol aplicació basada en Net mitjançant la implementació d'uns quants passos senzills.
        *   Instancia l'objecte Annotator amb la ruta del document d'entrada o el flux amb LoadOptions instància amb ImportAnnotations = true.
        *   Creeu una implementació de AnnotationBase i configureu l'identificador de l'anotació existent (si no es troba l'anotació amb aquest identificador, no es canviarà res) o la llista de camins d'anotacions (s'eliminaran totes les anotacions existents).
        *   Truca el mètode d'actualització de l'objecte Annotator amb anotacions passades.
        *   Truqueu al mètode de desar amb la ruta o flux del document resultant i l'objecte SaveOptions.

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
    title_left: "Passos per extreure anotacions de XLSX a Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilita als desenvolupadors de Net anotar documents i extreure informació d'anotacions dels fitxers XLSX dins de qualsevol aplicació basada en Net mitjançant la implementació d'uns quants passos senzills.
        *   Creeu objectes de resposta amb comentari i data.
        *   Instancia l'objecte LoadOptions i crida a SetImportAnnotations amb un argument veritable.
        *   Definiu variable amb el tipus Llista.
        *   Truqueu al mètode get i retorneu el resultat a la variable anterior.

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
    title: "Demostracions en directe per afegir, eliminar, editar i extreure anotacions a documents i imatges"
    content: |
        Afegiu, suprimiu, editeu i extreu anotacions al fitxer XLSX ara mateix visitant el lloc web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). La demostració en directe té els següents avantatges

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-xlsx"
          title: "Sobre el format de fitxer XLSX"
          content: |
            XLSX és un format conegut per als documents de Microsoft Excel que va ser introduït per Microsoft amb el llançament de Microsoft Office 2007. Basat en l'estructura organitzada segons les convencions d'embalatge obert tal com es descriu a la part 2 de l'estàndard OOXML ECMA-376, el nou format és un paquet zip que conté una sèrie de fitxers XML. L'estructura i els fitxers subjacents es poden examinar simplement descomprimint el fitxer .xlsx.

          link: "https://docs.fileformat.com/image/xlsx/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Treballar amb altres formats de documents populars"
    content: |
        Actualitzeu les propietats d'anotació d'alguns dels formats de fitxer populars, tal com s'indica a continuació.
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