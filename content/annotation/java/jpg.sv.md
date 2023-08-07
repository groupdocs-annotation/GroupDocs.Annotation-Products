---
############################# Static ############################
layout: "auto-gen-annotation"

############################# Head ############################
head_title: "Java JPG Annotation API Annotate i C#"
head_description: "Java API för att skapa och kommentera populära anteckningstyper från JPG, bilder, ritningar och dokumentfilformat."

############################# Header ############################
title: "Annotera JPG från Java"
description: ""
bg_image: "https://cms.admin.containerize.com/templates/aspose/App_Themes/V3/images/bg/header1.png"
bg_overlay: false
button:
    enable: true
    icon: "fas fa-arrow-down"
    label: "Ladda ner gratis provversion"
    link: "https://downloads.groupdocs.com/annotation/java"

############################# About ############################
about:
    enable: true
    title: "Om GroupDocs.Annotation for Java API"
    content: |
        GroupDocs.Annotation for Java API är ett bibliotek som låter dig lägga till kommentarer till PDF, Word och andra dokument på Mac, Windows eller Ubuntu. [GroupDocs.Annotation for Java](/annotation/java) är ett inbyggt Java API för att hantera kommentarer med omfattande stöd för att skapa, lägga till, redigera, ta bort, extrahera och exportera kommentarer från bilder och olika andra dokument. Den fullständiga listan över dokumentformat som stöds kan du se på denna [sida](https://docs.groupdocs.com/annotation/java/supported-document-formats/).
        Detta bibliotek låter dig arbeta inte bara med JPG dokument utan också med många andra typer av dokument som Word, Excel, PowerPoint, Outlook e-post, Visio, Adobe, OpenDocument, OpenOffice, Photoshop, AutoCad och många andra.
        GroupDocs.Annotation for Java API låter dig skapa och lägga till nya anteckningar, redigera kommentarer, extrahera kommentarer, anteckningar och ta bort dem från dokument. Biblioteket stöder 13 olika anteckningstyper, inklusive text, polylinje, område, understrykning, punkt, vattenstämpel, pil, ellips, textersättning, avstånd, textfält, resursredigering i PDF, HTML, Microsoft Word-dokument, kalkylblad, diagram, presentationer, ritningar, bilder och många andra filformat.
        Exemplet (se nedan) visar hur du arbetar med JPG-dokument, i det här exemplet kan du se huvudstegen för hur du arbetar med GroupDocs. Annotation: Konfigurera en licens, öppna ett dokument du vill arbeta med, skapa en annotering, lägga till dataobjekt för att ställa in anteckningsegenskaper enligt dina krav och spara resultatet på önskad plats. Du kan också titta mer detaljerat på de funktioner som stöds på vår github [sida](https://github.com/groupdocs-annotation/GroupDocs.Annotation-for-Java), eller i vår produkt [dokumentation](https: //docs.groupdocs.com/annotation/java/getting-started/).

############################# Steps ############################
howTo_Add:
steps_Add:
    enable: true
    title_left: "Steg för att lägga till kommentarer till JPG i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gör det enkelt för Java-utvecklare att lägga till olika annoteringstyper till JPG-filer i valfri Java-baserad applikation genom att implementera några enkla steg.
        *   Skapa svarsobjekt med kommentar och datum.
        *   Skapa AreaAnnotation-objekt, ställ in områdesalternativ och lägg till svar.
        *   Skapa Annotator-objekt och lägg till områdesanteckning.
        *   Spara utdatafil.
    title_right: "Systemkrav"
    content_right: |
        GroupDocs.Annotation för Java API:er stöds på alla större plattformar och operativsystem. Innan du kör koden nedan, se till att du har följande förutsättningar installerade på ditt system.
        *   Operativsystem: Microsoft Windows, Linux, MacOS
        *   Utvecklingsmiljö: NetBeans, Intellij IDEA, Eclipse etc
        *   Java Runtime Environment: Java 7 (1.7) och högre
        *   Hämta den senaste versionen av GroupDocs.Annotation for Java från [GroupDocs Artifact Repository](https://repository.groupdocs.com/webapp/#/artifacts/browse/tree/General/repo/com/groupdocs/groupdocs-annotation)

############################# Preview ############################
preview_Add:
    enable: true
    title: Förhandsgranskning av anteckningar och kodexempel
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
    title_left: "Steg för att ta bort anteckningar från JPG i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gör det enklare för Java-utvecklare att ta bort anteckningsdetaljer från JPG-filer i valfri Java-baserad applikation genom att implementera några enkla steg.
        *   Skapa svarsobjekt med kommentar och datum.
        *   Instantiera SaveOptions-objektet och ställ in AnnotationTypes = AnnotationType.None.
        *   Anropa sparmetoden med resulterande dokumentsökväg eller ström och SaveOptions-objekt.

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
    title_left: "Steg för att redigera kommentarer från JPG i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gör det enklare för Java-utvecklare att uppdatera olika annoteringsegenskaper från JPG-filer i valfri Java-baserad applikation genom att implementera några enkla steg.
        *   Instantiera Annotator-objekt med indatadokumentsökväg eller -ström med instansierade LoadOptions med ImportAnnotations = true.
        *   Skapa en AnnotationBase-implementering och ange Id för existerande anteckning (om anteckning med det Id inte hittas, kommer ingenting att ändras) eller sökvägslista med anteckningar (alla existerande anteckningar kommer att tas bort).
        *   Anrop uppdateringsmetod för Annotator-objekt med godkända anteckningar.
        *   Anropa sparmetoden med resulterande dokumentsökväg eller ström och SaveOptions-objekt.

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
    title_left: "Steg för att extrahera kommentarer från JPG i Java"
    content_left: |
        [GroupDocs.Annotation](/annotation/java/) gör det enkelt för Java-utvecklare att kommentera dokument och extrahera anteckningsinformation från JPG-filer i alla Java-baserade program genom att implementera några enkla steg.
        *   Skapa svarsobjekt med kommentar och datum.
        *   Instantiera LoadOptions-objektet och anrop SetImportAnnotations med sant argument.
        *   Definiera variabel med typen List.
        *   Anrop get-metoden och returnera resultatet till variabeln ovan.

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
    title: "Live-demos att lägga till, ta bort, redigera, extrahera kommentarer till dokument och bilder"
    content: |
        Lägg till, ta bort, redigera och extrahera kommentarer till filen JPG just nu genom att besöka webbplatsen [GroupDocs.Annotation Live Demos](https://products.groupdocs.app/annotation/family).
Livedemon har följande fördelar

############################# About Formats ############################
about_formats:
    enable: true
    format:
        # format loop
        - icon: "far fa-file-jpg"
          title: "Om filformatet JPG"
          content: |
            En JPG är en typ av bildformat som sparas med metoden för förlustkomprimering. Utdatabilden, som ett resultat av komprimering, är en kompromiss mellan lagringsstorlek och bildkvalitet. Användare kan justera komprimeringsnivån för att uppnå önskad kvalitetsnivå samtidigt som lagringsstorleken minskas. Bildkvaliteten påverkas försumbart om 10:1-komprimering tillämpas på bilden. Ju högre komprimeringsvärde, desto högre försämring i bildkvalitet.

          link: "https://docs.fileformat.com/image/jpg/"

############################# More Formats ############################
more_formats:
    enable: true
    title: "Arbeta med andra populära dokumentformat"
    content: |
        Uppdatera annoteringsegenskaper från några av de populära filformaten enligt nedan.
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