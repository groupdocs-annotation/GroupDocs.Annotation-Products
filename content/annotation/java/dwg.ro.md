---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java DWG Adnotare API Adnotare în C#"
head_description: "API Java pentru a crea și adnota tipuri populare de adnotări din DWG, imagini, desene și formate de fișiere de documente."

############################# Header ############################
title: "Adnotă DWG din Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Descarcare varianta scurta de prezentare gratuita"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Despre GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation pentru Java API este o bibliotecă care vă permite să adăugați adnotări la PDF, Word și alte documente pe Mac, Windows sau Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) este un API nativ Java pentru gestionarea adnotărilor cu suport complet pentru crearea, adăugarea, editarea, ștergerea, extragerea și exportul adnotărilor din imagini și diverse alte documente. Lista completă a formatelor de document acceptate pe care o puteți vedea pe această [pagină](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Această bibliotecă vă permite să lucrați nu numai cu documentul DWG, ci și cu multe alte tipuri de documente, cum ar fi Word, Excel, PowerPoint, e-mailuri Outlook, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad și multe altele.
        API-ul GroupDocs.Annotation pentru Java vă permite să creați și să adăugați note noi, să editați adnotări, să extrageți comentarii, adnotări și să le eliminați din documente. Biblioteca acceptă 13 tipuri diferite de adnotări, inclusiv text, polilinie, zonă, subliniere, punct, filigran, săgeată, elipsă, înlocuire text, distanță, câmp text, redactare resurse în documente PDF, HTML, Microsoft Word, foi de calcul, diagrame, prezentări, desene, imagini și multe alte formate de fișiere.
        Exemplul (vă rugăm să vedeți mai jos) demonstrează lucrul cu documentul DWG, în acest exemplu puteți vedea pașii principali ai modului de lucru cu GroupDocs. Adnotare: Configurați o licență, deschideți un document cu care doriți să lucrați, creând un adnotare, adăugând obiecte de date pentru a seta proprietățile de adnotare în funcție de cerințele dvs. și salvând rezultatul în locul necesar. De asemenea, puteți arunca o privire mai detaliată asupra funcțiilor acceptate pe [pagina] github (https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java) sau în [documentația] produsului nostru (https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Pași pentru a adăuga adnotări la DWG în Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilitează pentru dezvoltatorii Java adăugarea diferitelor tipuri de adnotări la fișierele DWG în cadrul oricărei aplicații bazate pe Java prin implementarea câțiva pași simpli.
        *   Creați obiecte Răspuns cu comentariu și dată.
        *   Creați obiect AreaAnnotation, setați opțiuni de zonă și adăugați răspunsuri.
        *   Creați un obiect Annotator și adăugați adnotare pentru zonă.
        *   Salvați fișierul de ieșire.
    title_right: "Cerințe de sistem"
    content_right: |
        API-urile GroupDocs.Annotation pentru Java sunt acceptate pe toate platformele și sistemele de operare majore. Înainte de a executa codul de mai jos, vă rugăm să vă asigurați că aveți următoarele cerințe preliminare instalate pe sistemul dumneavoastră.
        *   Sisteme de operare: Microsoft Windows, Linux, MacOS
        *   Mediu de dezvoltare: NetBeans, Intellij IDEA, Eclipse etc
        *   Mediu Java Runtime: Java 7 (1.7) și versiuni ulterioare
        *   Obțineți cea mai recentă versiune de GroupDocs.Annotation pentru Java de la [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Previzualizare adnotări și eșantion de cod
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
    title_left: "Pași pentru a elimina adnotările din DWG în Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilitează pentru dezvoltatorii Java eliminarea detaliilor adnotărilor din fișierele DWG din orice aplicație bazată pe Java prin implementarea câțiva pași simpli.
        *   Creați obiecte Răspuns cu comentariu și dată.
        *   Instanciați obiectul SaveOptions și setați AnnotationTypes = AnnotationType.None.
        *   Apelați metoda de salvare cu calea sau fluxul de document rezultat și obiectul SaveOptions.

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
    title_left: "Pași pentru editarea adnotărilor din DWG în Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) facilitează pentru dezvoltatorii Java actualizarea diferitelor proprietăți de adnotări din fișierele DWG din orice aplicație bazată pe Java prin implementarea câțiva pași simpli.
        *   Instanțiați obiectul Annotator cu calea documentului de intrare sau fluxul cu LoadOptions instanțiate cu ImportAnnotations = true.
        *   Creați o implementare AnnotationBase și setați ID-ul adnotărilor existente (dacă adnotarea cu acel ID nu este găsită, nimic nu va fi schimbat) sau lista de căi a adnotărilor (toate adnotările existente vor fi eliminate).
        *   Apelați metoda de actualizare a obiectului Annotator cu adnotări transmise.
        *   Apelați metoda de salvare cu calea sau fluxul de document rezultat și obiectul SaveOptions.

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
    title_left: "Pași pentru extragerea adnotărilor din DWG în Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) le permite dezvoltatorilor Java să adnoteze documente și să extragă informații despre adnotări din fișiere DWG din orice aplicație bazată pe Java, prin implementarea câțiva pași simpli.
        *   Creați obiecte Răspuns cu comentariu și dată.
        *   Instanțiați obiectul LoadOptions și apelați SetImportAnnotations cu argument adevărat.
        *   Definiți variabila cu tipul Listă.
        *   Apelați metoda get și returnați rezultatul la variabila de mai sus.

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
    title: "Demo live pentru a adăuga, elimina, edita și extrage adnotări la documente și imagini"
    content: |
        Adăugați, eliminați, editați și extrageți adnotări în fișierul DWG chiar acum, vizitând site-ul web [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family). Demo-ul live are următoarele beneficii

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-dwg"
          title: "Despre formatul de fișier DWG"
          content: |
            Fișierele cu extensia DWG reprezintă fișiere binare proprietare utilizate pentru a conține date de proiectare 2D și 3D. La fel ca DXF, care sunt fișiere ASCII, DWG reprezintă formatul de fișier binar pentru desenele CAD (Computer Aided Design). Conține imagini vectoriale și metadate pentru reprezentarea conținutului fișierelor CAD. Există vizualizatoare gratuite disponibile pentru vizualizarea fișierelor DWG pe sistemul de operare Windows, cum ar fi DWG TrueView gratuit de la Autodesk. Există și alte aplicații terțe care acceptă accesarea fișierelor DWG.

          link: "https://docs.fileformat.com/image/dwg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Lucrul cu alte formate de documente populare"
    content: |
        Actualizați proprietățile adnotărilor din unele dintre formatele de fișiere populare, așa cum este menționat mai jos.
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