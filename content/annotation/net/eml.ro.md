---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Net EML Adnotare API Adnotare în C#"
head_description: "Net API pentru a crea și adnota tipuri populare de adnotări din EML, imagini, desene și formate de fișiere de document."

############################# Header ############################
title: "Adnotă EML din Net"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Descarcare varianta scurta de prezentare gratuita"
    link: "https://downloads.groupdocs.com/annotation/net"

############################# About ############################
about:
    enable: true
    title: "Despre GroupDocs.Adnotation for Net API"
    content: |
        GroupDocs.Annotation pentru Net API este o bibliotecă care vă permite să adăugați adnotări la PDF, Word și alte documente pe Mac, Windows sau Ubuntu. [GroupDocs.Annotation for Net](/annotation/net) este un API net nativ pentru gestionarea adnotărilor cu suport complet pentru crearea, adăugarea, editarea, ștergerea, extragerea și exportul adnotărilor din imagini și din diverse alte documente. Lista completă a formatelor de document acceptate pe care o puteți vedea pe această [pagină](https://docs.groupdocs.com/annotation/net/supported-document-formats/).
        Această bibliotecă vă permite să lucrați nu numai cu documentul EML, ci și cu multe alte tipuri de documente, cum ar fi Word, Excel, PowerPoint, e-mailuri Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad și multe altele.
        API-ul GroupDocs.Annotation pentru Net vă permite să creați și să adăugați note noi, să editați adnotări, să extrageți comentarii, adnotări și să le eliminați din documente. Biblioteca acceptă 13 tipuri diferite de adnotări, inclusiv text, polilinie, zonă, subliniere, punct, filigran, săgeată, elipsă, înlocuire text, distanță, câmp text, redactare resurse în documente PDF, HTML, Microsoft Word, foi de calcul, diagrame, prezentări, desene, imagini și multe alte formate de fișiere.
        Exemplul (vă rugăm să vedeți mai jos) demonstrează lucrul cu documentul EML, în acest exemplu puteți vedea pașii principali ai modului de lucru cu GroupDocs. Adnotare: Configurați o licență, deschideți un document cu care doriți să lucrați, creând un adnotare, adăugând obiecte de date pentru a seta proprietățile de adnotare în funcție de cerințele dvs. și salvând rezultatul în locul necesar. De asemenea, puteți arunca o privire mai detaliată asupra funcțiilor acceptate pe [pagina] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) sau în [documentația] produsului nostru (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-.NET) ://docs.groupdocs.com/annotation/net/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Pași pentru a adăuga adnotări la EML în Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilitează pentru dezvoltatorii Net să adauge diferite tipuri de adnotări la fișierele EML în cadrul oricărei aplicații bazate pe net prin implementarea câțiva pași simpli.
        *   Creați obiecte Răspuns cu comentariu și dată.
        *   Creați obiect AreaAnnotation, setați opțiuni de zonă și adăugați răspunsuri.
        *   Creați un obiect Annotator și adăugați adnotare pentru zonă.
        *   Salvați fișierul de ieșire.
    title_right: "Cerințe de sistem"
    content_right: |
        GroupDocs.Annotation pentru API-urile Net sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.
        *   Sisteme de operare: Microsoft Windows, Linux, MacOS
        *   Medii de dezvoltare: Visual Studio, Xamarin, MonoDevelop
        *   Framework: .NET Framework, .NET Standard, .NET Core, Mono
        *   Descărcați cea mai recentă versiune de GroupDocs.Annotation pentru .NET de la [NuGet](https://www.nuget.org/packages/groupdocs.annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Previzualizare adnotări și eșantion de cod
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
    title_left: "Pași pentru a elimina adnotările din EML din Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilitează pentru dezvoltatorii Net să elimine detaliile adnotărilor din fișierele EML din orice aplicație bazată pe net prin implementarea câțiva pași simpli.
        *   Creați obiecte Răspuns cu comentariu și dată.
        *   Instanciați obiectul SaveOptions și setați AnnotationTypes = AnnotationType.None.
        *   Apelați metoda de salvare cu calea sau fluxul de document rezultat și obiectul SaveOptions.

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
    title_left: "Pași pentru editarea adnotărilor din EML în Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) facilitează pentru dezvoltatorii Net să actualizeze diferite proprietăți de adnotare din fișiere EML în cadrul oricărei aplicații bazate pe net prin implementarea câțiva pași simpli.
        *   Instanțiați obiectul Annotator cu calea documentului de intrare sau fluxul cu LoadOptions instanțiate cu ImportAnnotations = true.
        *   Creați o implementare AnnotationBase și setați ID-ul adnotărilor existente (dacă adnotarea cu acel ID nu este găsită, nimic nu va fi schimbat) sau lista de căi a adnotărilor (toate adnotările existente vor fi eliminate).
        *   Apelați metoda de actualizare a obiectului Annotator cu adnotări transmise.
        *   Apelați metoda de salvare cu calea sau fluxul de document rezultat și obiectul SaveOptions.

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
    title_left: "Pași pentru extragerea adnotărilor din EML în Net"
    content_left: |
        [GroupDocs.Annotation](/annotation/net/) permite dezvoltatorilor Net să adnoteze documente și să extragă informații despre adnotări din fișiere EML în cadrul oricărei aplicații bazate pe Net prin implementarea câțiva pași simpli.
        *   Creați obiecte Răspuns cu comentariu și dată.
        *   Instanțiați obiectul LoadOptions și apelați SetImportAnnotations cu argument adevărat.
        *   Definiți variabila cu tipul Listă.
        *   Apelați metoda get și returnați rezultatul la variabila de mai sus.

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
    title: "Demo live pentru a adăuga, elimina, edita și extrage adnotări la documente și imagini"
    content: |
        Adăugați, eliminați, editați și extrageți adnotări în fișierul EML chiar acum, vizitând site-ul web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
Demo-ul live are următoarele beneficii

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-eml"
          title: "Despre formatul de fișier EML"
          content: |
            Formatul de fișier EML reprezintă mesajele de e-mail salvate folosind Outlook și alte aplicații relevante. Aproape toți clienții de e-mail acceptă acest format de fișier pentru conformitatea cu standardul RFC-822 Internet Message Format. Microsoft Outlook este software-ul implicit pentru deschiderea tipurilor de mesaje EML. Fișierele EML pot fi folosite pentru salvarea pe disc, precum și pentru trimiterea către destinatari folosind protocoale de comunicare.

          link: "https://docs.fileformat.com/image/eml/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Lucrul cu alte formate de documente populare"
    content: |
        Actualizați proprietățile adnotărilor din unele dintre formatele de fișiere populare, așa cum este menționat mai jos.
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